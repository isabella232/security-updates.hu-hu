---
TOCTitle: '5. lépés: Ügyfélfrissítések konfigurálása'
Title: '5. lépés: Ügyfélfrissítések konfigurálása'
ms:assetid: '5ae60ead-3e94-456c-a692-c0f193ea5d5a'
ms:contentKeyID: 21741735
ms:mtpsurl: 'https://technet.microsoft.com/hu-hu/library/Dd939830(v=WS.10)'
---


5.lépés: Ügyfélfrissítések konfigurálása
===============================================

A Windows Server Update Services 3.0 (WSUS 3.0 SP2) szolgáltatásban a WSUS telepítője az IIS szolgáltatás automatikus beállításával gondoskodik arról, hogy a WSUS-kiszolgálóhoz csatlakozó valamennyi ügyfélszámítógépre az automatikus frissítési szolgáltatás legújabb verziója kerüljön.

A hálózati környezettől függ, hogy melyik módszerrel lehet a leghatékonyabban konfigurálni az automatikus frissítési szolgáltatást: Az Active Directory® címtárszolgáltatást használó környezetekben használhat egy meglévő tartományalapú csoportházirend-objektumot (GPO), vagy létrehozhat egy új objektumot, nem Active Directory-alapú környezetekben pedig a Helyi csoportházirend objektummal célszerű végrehajtani a beállítást. Ebben a lépésben konfigurálja az automatikus frissítési szolgáltatást, majd az ügyfélszámítógépeket a WSUS szolgáltatást futtató kiszolgálóhoz irányítja.

A következő eljárások azt feltételezik, hogy a hálózaton Active Directory címtárszolgáltatás fut, illetve hogy tisztában van a Csoportházirend beépülő modul használatának és a hálózat vele történő felügyeletének módjával.

A Csoportházirend beépülő modulról a weben elérhető technikai támogatási központ nyújt további felvilágosítást, a csoportházirendet ismertető webhelyen [http://go.microsoft.com/fwlink/?LinkID=47375](http://go.microsoft.com/fwlink/?linkid=47375) (előfordulhat, hogy a hivatkozás angol nyelvű tartalomra mutat).


Az 5. lépés műveletei
---------------------

A 4. lépésben konfigurálta a letölteni kívánt frissítéseket. A jelen eljárásokkal konfigurálhatja az ügyfélszámítógépeken az automatikus frissítéseket.

1.  Az automatikus frissítési szolgáltatás konfigurálása a Csoportházirend beépülő modulban
2.  Az ügyfélszámítógép beállítása a WSUS-kiszolgálóval létesítendő kapcsolat használatára
3.  A frissítések WSUS-kiszolgálón történő keresésének manuális elindítása

Az első két eljárást egy tetszés szerinti tartományalapú csoportházirend-objektumon, a harmadik eljárást pedig az ügyfélszámítógépen a parancssorban fogja végrehajtani.

**Az Automatikus frissítések szolgáltatás beállítása**
1.  A Csoportházirend-kezelő konzolban tallózással keresse meg azt a csoportházirend-objektumot, amelyen a WSUS szolgáltatást konfigurálni szeretné, majd kattintson a **Szerkesztés** elemre.

2.  Bontsa ki a Csoportházirend-kezelő konzol **Számítógép konfigurációja**, **Felügyeleti sablonok**, majd **Windows-összetevők** csomópontját, és kattintson a **Windows Update** mappára.

3.  A jobb oldali ablaktáblában kattintson duplán **Az automatikus frissítés konfigurálása** beállításra.

4.  Jelölje be az **Engedélyezve** választógombot, majd válasszon az alábbi lehetőségek közül.

    -   **Értesítés letöltés és telepítés előtt egyaránt:** Ha ezt a lehetőséget választja, a rendszer értesíti a bejelentkezett rendszergazdát a frissítések letöltése és telepítése előtt.
    -   **Automatikus letöltés és értesítés a telepítés előtt:** Ha ezt a beállítást választja, a program automatikusan megkezdi a frissítések letöltését, majd értesíti a bejelentkezett rendszergazdát a frissítések telepítése előtt.
    -   **Automatikus letöltés és ütemezés szerinti telepítés:** Ha ezt a beállítást választja, a program automatikusan megkezdi a frissítések letöltését, és a felhasználó által megadott napon és időpontban telepíti azokat.
    -   **A helyi rendszergazda adja meg a beállítást:** Ezzel a beállítással a helyi rendszergazdák a Vezérlőpult Automatikus frissítések segédprogramjában kiválaszthatják a használni kívánt beállításokat (megadhatják például a saját igényeiknek megfelelő telepítési ütemezést). A helyi rendszergazdák nem tilthatják le az automatikus frissítési szolgáltatást.

5.  Kattintson az **OK** gombra.

**Az ügyfélszámítógépek WSUS-kiszolgálóhoz való irányítása**
1.  A **Windows Update** részleteit megjelenítő ablaktáblában kattintson duplán az **Adja meg az intraneten található Microsoft frissítési szolgáltatás helyét** elemre.

2.  Jelölje be az **Engedélyezve** választógombot, majd írja be ugyanazon WSUS-kiszolgáló HTTP-alapú URL-címét az **Adja meg a frissítések keresését végző intranetes frissítési szolgáltatást** és az **Adja meg a statisztikát tároló intranetkiszolgálót** mezőbe (például *http://kiszolgálónév*), végül kattintson az **OK** gombra.

 
> [!NOTE]  
> Ha a helyi csoportházirend-objektumot használja a számítógép WSUS-kiszolgálóval létesítendő kapcsolatának definiálására, a beállítás azonnal érvénybe lép, és a számítógép megjelenik a WSUS szolgáltatás felügyeleti konzolján. Felgyorsíthatja a folyamatot, ha manuálisan elindítja a frissítések keresését.

Az adott ügyfélszámítógép beállítását követően a rendszer néhány perc elteltével megjeleníti a számítógépet a WSUS felügyeleti konzoljának **Számítógépek** lapján. Tartományi csoportházirenddel beállított ügyfélszámítógépek esetén körülbelül húsz percre van szükség a Csoportházirend modulbeli beállítások frissítéséhez (tehát ennyi idő elteltével alkalmazza a rendszer az új házirend-beállításokat az ügyfélszámítógépen). A Csoportházirend modul alapértelmezés szerint kilencven percenként frissül a háttérben, a véletlenszerű eltolási érték pedig 0–30 perc. Ha rövidebb frissítési időközt szeretne beállítani, nyisson meg egy parancsablakot az ügyfélszámítógépen, és írja be a parancssorba a **gpupdate /force** parancsot.

A helyi csoportházirend-objektummal beállított ügyfélszámítógépek eseten a Csoportházirend modul beállításait azonnal alkalmazza a rendszer, noha a frissítés körülbelül húsz percet vesz igénybe.

Ha ezt teszi, nem kell megvárnia azt a húsz percet, amíg az ügyfélszámítógép kapcsolatot létesít a WSUS-kiszolgálóval.

**Frissítések WSUS-kiszolgálón történő keresésének saját kezű indítása**
1.  Kattintson az ügyfélszámítógép **Start** menüjének **Futtatás** parancsára.

2.  Írja be a **cmd** parancsot a **Megnyitás** mezőbe, majd kattintson az **OK** gombra.

3.  Írja be a parancssorba a **wuauclt.exe /detectnow** parancsot. Ezzel a művelettel a rendszer arra utasítja az Automatikus frissítések szolgáltatást, hogy azonnal létesítsen kapcsolatot a WSUS-kiszolgálóval.

Következő lépés
---------------

[6. lépés: Számítógépcsoportok konfigurálása](https://technet.microsoft.com/70518732-2179-4e41-9609-7f9999867f41)

További források
----------------

[Részletes útmutató a Windows Server Update Services 3.0 SP2 telepítéséhez](https://technet.microsoft.com/4b504edc-93b3-45b0-a7e8-d0107f1a4442)
