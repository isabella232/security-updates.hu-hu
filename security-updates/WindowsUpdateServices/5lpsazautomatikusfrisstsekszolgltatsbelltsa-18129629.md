---
TOCTitle: '5. lépés: Az Automatikus frissítések szolgáltatás beállítása'
Title: '5. lépés: Az Automatikus frissítések szolgáltatás beállítása'
ms:assetid: '5da6d10a-6ff1-4de8-b53a-4893bf8bd9fa'
ms:contentKeyID: 18129629
ms:mtpsurl: 'https://technet.microsoft.com/hu-hu/library/Cc720532(v=WS.10)'
---

5. lépés: Az Automatikus frissítések szolgáltatás beállítása
============================================================

A Windows Server Update Services (WSUS) szolgáltatáshoz csatlakozó ügyfélszámítógépek megfelelő működéséhez az Automatikus frissítések segédprogram kompatibilis verziója szükséges. A WSUS telepítője az IIS szolgáltatás automatikus beállításával gondoskodik arról, hogy a WSUS-kiszolgálóhoz csatlakozó valamennyi ügyfélszámítógépre az Automatikus frissítések segédprogram legújabb verziója kerüljön.

A hálózati környezettől függ, hogy melyik módszerrel lehet a leghatékonyabban konfigurálni az Automatikus frissítések szolgáltatást: Active Directory-környezetben tartományi csoportházirend-objektummal (GPO), nem Active Directory környezetben pedig a Helyi csoportházirend objektummal célszerű végrehajtani a beállítást. Akár a Helyi csoportházirend objektummal, akár egy tartományi csoportházirend-objektummal végzi a beállítást, az ügyfélszámítógépeket mindenképpen be kell állítani a WSUS-kiszolgálóval létesítendő kapcsolatra, majd meg kell adni az Automatikus frissítések szolgáltatás beállításait.

A következőkben olvasható útmutatás azt feltételezi, hogy a hálózaton Active Directory környezet működik, illetve hogy tisztában van a Csoportházirend beépülő modul használatának és a hálózat vele történő felügyeletének módjával. A WSUS szolgáltatás beállításai számára új csoportházirend-objektumot kell létrehozni, majd hozzá kell rendelni a tartományhoz.

A Csoportházirend beépülő modulról a weben elérhető technikai támogatási központ nyújt további felvilágosítást, a [csoportházirendet](http://go.microsoft.com/fwlink/?linkid=47375) ismertető webhelyen (lehet, hogy a hivatkozás angol nyelvű anyagra mutat).

**Az 5. lépésben a következő műveleteket kell végrehajtani**:

-   A WSUS felügyeleti sablonjának hozzáadása
-   Az Automatikus frissítések szolgáltatás beállítása
-   Az ügyfélszámítógép beállítása a WSUS-kiszolgálóval létesítendő kapcsolat használatára
-   A frissítések WSUS-kiszolgálón történő keresésének manuális elindítása

Hajtsa végre az első három műveletet a használni kívánt, tartományi csoportházirend-objektumon. Létre kell hoznia egy új csoportházirend-objektumot, vagy egy meglévőt kell használnia. Ha a Csoportházirend-kezelő konzolt használja a csoportházirend-objektumok kezelésére, keresse meg a módosítani kívánt csoportházirend-objektumot, majd kattintson a **Szerkesztés** parancsra.

Ahhoz, hogy a WSUS kezelése során megtekinthesse a házirend-beállításokat, gondoskodnia kell arról, hogy a WSUS felügyeleti sablonfájl, a wuau.adm, fel legyen véve a Csoportházirendobjektum-szerkesztőbe. Mivel alapértelmezés szerint a wuau.adm része az operációs rendszernek, már benne kell lennie a Csoportházirendobjektum-szerkesztőben.

**A WSUS felügyeleti sablonjának hozzáadása**
1.  A Csoportházirendobjektum-szerkesztő segédprogram konzolján kattintson az egyik **Felügyeleti sablonok** csomópontra.

2.  Kattintson a **Művelet** menü **Sablon hozzáadása/eltávolítása** pontjára, majd a **Hozzáadás** parancsra.

3.  A **Házirendsablonok** párbeszédpanelen jelölje ki a **wuau.adm** sablont, majd kattintson a **Megnyitás** gombra.

4.  A **Sablon hozzáadása/eltávolítása** párbeszédpanelen kattintson a **Bezárás** gombra.

**Az Automatikus frissítések szolgáltatás beállítása**
1.  Bontsa ki a Csoportházirendobjektum-szerkesztő modul konzoljának **Számítógép konfigurációja**, **Felügyeleti sablonok**, majd **Windows-összetevők** csomópontját, és kattintson a **Windows Update** mappára.

2.  A jobb oldali ablaktáblában kattintson duplán **Az automatikus frissítés konfigurálása** beállításra.

3.  Jelölje be az **Engedélyezve** választógombot, majd válasszon az alábbi lehetőségek közül.

    -   **Értesítés letöltés és telepítés előtt egyaránt**: Ha ezt a listaelemet választja, a rendszer értesíti a bejelentkezett és rendszergazdát a frissítések letöltése és telepítése előtt.
    -   **Automatikus letöltés és értesítés a telepítés előtt**: Ha ezt a beállítást választja, a program automatikusan megkezdi a frissítések letöltését, majd értesíti a bejelentkezett rendszergazdát a frissítések telepítése előtt.
    -   **Automatikus letöltés és ütemezés szerinti telepítés**: Amennyiben az Automatikus frissítések szolgáltatás ütemezés szerinti telepítésre van beállítva, meg kell adni az ismétlődő ütemezett telepítés napját és idejét is.
    -   **A helyi rendszergazda adja meg a beállítást**: Ezzel a beállítással a helyi rendszergazdák a Vezérlőpultról megnyitható Automatikus frissítések segédprogramban kiválaszthatják a használni kívánt beállításokat (megadhatják például a saját igényeiknek megfelelő telepítési ütemezést). A helyi rendszergazdák nem tilthatják le az Automatikus frissítések szolgáltatást.

4.  Kattintson az **OK** gombra.

| ![](images/Cc720532.note(WS.10).gif)Megjegyzés:                                                                                                                                  |
|---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| **A helyi rendszergazda adja meg a beállítást** lehetőség csak abban az esetben jelenik meg, ha az Automatikus frissítések szolgáltatás a WSUS szolgáltatással kompatibilis verzióra frissítette saját magát. |

**Az ügyfélszámítógép beállítása a WSUS-kiszolgálóval létesítendő kapcsolat használatára**
1.  Bontsa ki a Csoportházirendobjektum-szerkesztő modul konzoljának **Számítógép konfigurációja**, **Felügyeleti sablonok**, majd **Windows-összetevők** csomópontját, és kattintson a **Windows Update** mappára.

2.  A jobb oldali ablaktáblában kattintson duplán az **Adja meg az intraneten található Microsoft frissítési szolgáltatás helyét** beállításra.

3.  Jelölje be az **Engedélyezve** választógombot, majd írja be ugyanazon WSUS-kiszolgáló HTTP alapú URL-címét az **Adja meg a frissítések keresését végző intranetes frissítési szolgáltatást** és az **Adja meg a statisztikát tároló intranetkiszolgálót** mezőbe (például *http://kiszolgálónév*), végül kattintson az **OK** gombra.

| ![](images/Cc720532.note(WS.10).gif)Megjegyzés:                                                                                                                                                                                                                                                             |
|------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| Amennyiben a Helyi csoportházirend objektumot használja a számítógép WSUS-kiszolgálóval létesítendő kapcsolatának definiálására, a beállítás azonnal érvénybe lép, és a számítógép rövid időn belül megjelenik a WSUS szolgáltatás felügyeleti konzolján. Felgyorsíthatja a folyamatot, ha manuálisan elindítja a frissítések keresését. |

Az adott ügyfélszámítógép beállítását követően a rendszer néhány perc elteltével megjeleníti a számítógépet a WSUS-konzol **Számítógépek** lapján. Tartományi csoportházirenddel beállított ügyfélszámítógépek esetén körülbelül húsz percre van szükség a Csoportházirend modulbeli beállítások frissítéséhez (tehát ennyi idő elteltével alkalmazza a rendszer az új házirend-beállításokat az ügyfélszámítógépen). A Csoportházirend modul alapértelmezés szerint kilencven percenként frissül a háttérben, a véletlenszerű eltolási érték pedig 0–30 perc. Ha rövidebb frissítési időközt szeretne beállítani, nyisson meg egy parancsablakot az ügyfélszámítógépen, és írja be a parancssorba a következőt: **gpupdate /force**.

A Helyi csoportházirend objektummal beállított ügyfélszámítógépek esetében a Csoportházirend modul beállításait azonnal alkalmazza a rendszer, noha a frissítés körülbelül húsz percet vesz igénybe.

A beállítások alkalmazását követően a frissítések keresése saját kezűleg is elindítható. Ha ezt teszi, nem kell megvárnia azt a húsz percet, amíg az ügyfélszámítógép kapcsolatot létesít a WSUS-kiszolgálóval.

**Frissítések WSUS-kiszolgálón történő keresésének saját kezű indítása**
1.  Kattintson az ügyfélszámítógép **Start** menüjének **Futtatás** parancsára.

2.  Írja be a **cmd** parancsot a **Megnyitás** mezőbe, majd kattintson az **OK** gombra.

3.  Írja be a parancssorba a **wuauclt.exe /detectnow** parancsot. Ezzel a művelettel a rendszer arra utasítja az Automatikus frissítések szolgáltatást, hogy azonnal létesítsen kapcsolatot a WSUS-kiszolgálóval.
