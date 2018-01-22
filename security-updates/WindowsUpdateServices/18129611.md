---
TOCTitle: '5. lépés: Az Automatikus frissítések szolgáltatás frissítése és beállítása'
Title: '5. lépés: Az Automatikus frissítések szolgáltatás frissítése és beállítása'
ms:assetid: '4ac8d574-f48e-4d9d-86c9-9aeb0f57e750'
ms:contentKeyID: 18129611
ms:mtpsurl: 'https://technet.microsoft.com/hu-hu/library/Cc720533(v=WS.10)'
---

5. lépés: Az Automatikus frissítések szolgáltatás frissítése és beállítása
==========================================================================

A Windows Server Update Services (WSUS) szolgáltatáshoz csatlakozó ügyfélszámítógépek megfelelő működéséhez az Automatikus frissítések segédprogram kompatibilis verziója szükséges. A WSUS telepítője az IIS szolgáltatás automatikus beállításával biztosítja, hogy a WSUS-kiszolgálóhoz csatlakozó valamennyi ügyfélszámítógépre az Automatikus frissítések segédprogram legújabb verziója kerüljön.

> [!NOTE]  
> Noha az Automatikus frissítések szolgáltatás legtöbb verziója beállítható úgy, hogy a WSUS-kiszolgálóval kapcsolatot létesítve automatikusan megtörténjen a WSUS rendszerrel kompatibilis verzióra történő önálló frissítés, a szolgáltatás Windows XP rendszerbeli, szervizcsomaggal nem frissített verziója nem képes saját magát automatikusan frissíteni. Amennyiben számítógépein a Windows XP rendszer szervizcsomag nélküli verziója működik, és a Software Update Services (SUS) szolgáltatást sem használta még az adott számítógépes környezetben, a szükséges útmutatásokat a „Deploying Microsoft Windows Server Update Services” (A Microsoft Windows Server Update Services szolgáltatás központi telepítése) című (angol nyelvű) szakmai dokumentációban találja meg. 

Az Automatikus frissítések szolgáltatás beállításának leghatékonyabb módja a hálózati környezet függvénye: Active Directory környezetben Active Directory alapú csoportházirend-objektummal (GPO), nem Active Directory környezetben pedig a Helyi csoportházirend objektummal célszerű végrehajtani a beállítást. Akár a Helyi csoportházirend objektummal, akár egy tartományvezérlőn tárolt csoportházirend-objektummal végzi a beállítást, az ügyfélszámítógépeket mindenképpen be kell állítani a WSUS-kiszolgálóval létesítendő kapcsolatra, majd meg kell adni az Automatikus frissítések szolgáltatás beállításait.

A következőkben olvasható útmutatás azt feltételezi, hogy a hálózaton Active Directory környezet működik, illetve hogy a Csoportházirend beépülő modul beállítása már megtörtént, így ön tisztában van a modul használatának és a hálózat vele történő felügyeletének mikéntjével. A WSUS szolgáltatás beállításaihoz új csoportházirend-objektumot kell létrehozni, majd annak hozzárendelését a tartományi szinten végre kell hajtani.

A Csoportházirend beépülő modulról a [Group Policy](http://go.microsoft.com/fwlink/?linkid=47375) (Csoportházirend) című (angol nyelvű) oldal nyújt további felvilágosítást (http://go.microsoft.com/fwlink/?LinkID=47375).

Az 5. lépésben a következő műveleteket kell végrehajtani:

-   A WSUS felügyeleti sablonjának betöltése
-   Az Automatikus frissítések szolgáltatás beállítása
-   Ügyfélszámítógépek beállítása a WSUS-kiszolgálóval létesítendő kapcsolat használatára
-   Frissítések keresésének saját kezű beállítása az ügyfélszámítógépeken

Hajtsa végre az alábbi három műveletet a használni kívánt, Active Directory alapú csoportházirend-objektumon.

**A WSUS felügyeleti sablonjának hozzáadása**
1.  A Csoportházirendobjektum-szerkesztő segédprogram konzolján kattintson az egyik **Felügyeleti sablonok** csomópontra.

2.  Kattintson a **Művelet** menü **Sablon hozzáadása/eltávolítása** parancsára.

3.  Kattintson a **Hozzáadás** gombra.

4.  A **Házirendsablonok** párbeszédpanelen jelölje ki a **wuau.adm** sablont, majd kattintson a **Megnyitás** gombra.

5.  A **Sablon hozzáadása/eltávolítása** párbeszédpanelen kattintson a **Bezárás** gombra.

**Az Automatikus frissítések szolgáltatás működésének beállítása**
1.  Bontsa ki a Csoportházirendobjektum-szerkesztő modul konzoljának **Számítógép konfigurációja**, **Felügyeleti sablonok**, majd **Windows-összetevők** csomópontját, és kattintson a **Windows Update** mappára.

2.  A jobb oldali ablaktáblában kattintson duplán **Az automatikus frissítés konfigurálása** beállításra.

3.  Jelölje be az **Engedélyezve** választógombot, majd válasszon az alábbi lehetőségek közül.

    -   **Értesítés letöltés és telepítés előtt egyaránt:** Ezt a listaelemet választva a rendszer értesíti a bejelentkezett és rendszergazdai jogosultságokkal rendelkező felhasználót a frissítések letöltése és telepítése előtt.
    -   **Automatikus letöltés és értesítés a telepítés előtt:** Ha ezt a beállítást választja, a program automatikusan megkezdi a frissítések letöltését, majd értesíti a bejelentkezett és rendszergazdai jogosultságokkal rendelkező felhasználót a frissítések telepítése előtt.
    -   **Automatikus letöltés és ütemezés szerinti telepítés:** Amennyiben az Automatikus frissítések szolgáltatás ütemezés szerinti telepítésre van beállítva, meg kell adni az ismétlődő ütemezett telepítés napját és idejét is.
    -   **A helyi rendszergazda adja meg a beállítást:** Ezt a beállítást választva a helyi rendszergazdák a Vezérlőpultról megnyitható Automatikus frissítések segédprogramban kiválaszthatják a használni kívánt beállításokat (megadhatják például a saját igényeiknek megfelelő telepítési ütemezést). A helyi rendszergazdák nem tilthatják le az Automatikus frissítések szolgáltatást.

4.  Kattintson az **OK** gombra.

> [!NOTE]  
> **A helyi rendszergazda adja meg a beállítást** lehetőség csak abban az esetben jelenik meg, ha az Automatikus frissítések szolgáltatás a WSUS szolgáltatással kompatibilis verzióra frissítette saját magát. 

**Az ügyfélszámítógép beállítása a WSUS-kiszolgálóval létesítendő kapcsolat használatára**
1.  Bontsa ki a Csoportházirendobjektum-szerkesztő modul konzoljának **Számítógép konfigurációja**, **Felügyeleti sablonok**, majd **Windows-összetevők** csomópontját, és kattintson a **Windows Update** mappára.

2.  A jobb oldali ablaktáblában kattintson duplán az **Adja meg az intraneten található Microsoft frissítési szolgáltatás helyét** beállításra.

3.  Jelölje be az **Engedélyezve** választógombot, majd írja be ugyanazon WSUS-kiszolgáló HTTP alapú URL-címét az **Adja meg a frissítések keresését végző intranetes frissítési szolgáltatást** és az **Adja meg a statisztikát tároló intranetkiszolgálót** mezőbe (például **http://***kiszolgálónév*).

4.  Kattintson az **OK** gombra.

> [!NOTE]  
> Amennyiben a Helyi csoportházirend objektumot használja a számítógép WSUS-kiszolgálóval létesítendő kapcsolatának definiáláshoz, a beállítás azonnal érvénybe lép, és a számítógép hozzávetőlegesen húsz percen belül megjelenik a WSUS szolgáltatás felügyeleti konzolján. A folyamat gyorsítása érdekében kezdeményezze a frissítések keresését saját kezűleg. 

Az adott ügyfélszámítógép beállítását követően a rendszer néhány perc elteltével megjeleníti a számítógépet a WSUS-konzol **Számítógépek** lapján. Active Directory alapú csoportházirend-objektummal beállított ügyfélszámítógépek esetén körülbelül húsz percre van szükség a Csoportházirend modulbeli beállítások frissítéséhez (tehát ennyi idő elteltével alkalmazza a rendszer az új beállításokat az ügyfélszámítógépen). A Csoportházirend modul alapértelmezés szerint kilencven percenként frissül a háttérben, a véletlenszerű eltolási érték pedig 0–30 perc. Ha rövidebb frissítési időközt szeretne beállítani, nyisson meg egy parancsablakot az ügyfélszámítógépen, és írja be a parancssorba a **gpupdate /force** parancsot.

A Helyi csoportházirend objektummal beállított ügyfélszámítógépek esetén a Csoportházirend modul beállításait azonnal alkalmazza a rendszer, noha a frissítés körülbelül húsz percet vesz igénybe.

A beállítások alkalmazását követően a frissítések keresése saját kezűleg is elindítható – ha ezt teszi, nem kell megvárnia azt a húsz percet, amíg az ügyfélszámítógép kapcsolatot létesít a WSUS-kiszolgálóval.

**Frissítések WSUS-kiszolgálón történő keresésének saját kezű indítása**
1.  Kattintson az ügyfélszámítógép **Start** menüjének **Futtatás** parancsára.

2.  Írja be a Megnyitás mezőbe a **cmd** parancsot, majd kattintson az **OK** gombra.

3.  Írja be a parancssorba a **wuauclt.exe /detectnow** parancsot. Ezzel a művelettel a rendszer arra utasítja az Automatikus frissítések szolgáltatást, hogy azonnal létesítsen kapcsolatot a WSUS-kiszolgálóval.
