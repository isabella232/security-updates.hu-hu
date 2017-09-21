---
TOCTitle: '4. lépés: Frissítések és szinkronizálás konfigurálása'
Title: '4. lépés: Frissítések és szinkronizálás konfigurálása'
ms:assetid: 'deeaa7e1-9b50-45cb-9537-d75f70de3405'
ms:contentKeyID: 21741818
ms:mtpsurl: 'https://technet.microsoft.com/hu-hu/library/Dd939924(v=WS.10)'
---

4. lépés: Frissítések és szinkronizálás konfigurálása
=====================================================

Ez a rész azt ismerteti, hogy miként konfigurálhatók a letölteni kívánt frissítések a Windows Server Update Services 3.0 Service Pack 2 (WSUS 3.0 SP2) szolgáltatással.

Az 4. lépés műveletei
---------------------

Az itt leírt eljárásokat a WSUS konfigurációs varázslója vagy a WSUS felügyeleti konzol segítségével hajthatja végre.

1.  A felsőbb rétegbeli kiszolgáló és a proxykiszolgáló adatainak mentése és letöltése
2.  A frissítések nyelvének kiválasztása
3.  Azoknak a termékeknek a kiválasztása, amelyekhez frissítéseket szeretne letölteni
4.  A frissítések besorolásának kiválasztása
5.  A kiszolgáló szinkronizálási ütemezésének meghatározása

A hálózati kapcsolat beállítását követően letölthetők a szükséges frissítések a WSUS-kiszolgáló szinkronizálásával. A szinkronizálás akkor kezdődik, amikor a WSUS-kiszolgáló kapcsolatot létesít a Microsoft Update webhellyel, majd megállapítja, hogy közzétettek-e új frissítéseket a legutóbbi szinkronizálás óta. Amikor első alkalommal szinkronizálja a WSUS-kiszolgálót, az összes frissítés rendelkezésre áll, és készen áll arra, hogy jóváhagyja azok telepítését. Az első szinkronizálás hosszú ideig is tarthat.

A jelen részben leírt eljárások az alapértelmezett beállításokkal történő szinkronizálást ismertetett. A WSUS 3.0 SP2 olyan beállításokat is tartalmaz, melyek lehetővé teszik a sávszélesség minimalizálását a szinkronizálás során.

A Windows Server Update Services konfigurációs varázslójának használata esetén
------------------------------------------------------------------------------

A 3. lépésben végrehajtotta a felsőbb rétegbeli kiszolgáló és a proxykiszolgáló konfigurációját. A következő műveleteket a konfigurációs varázsló **Kapcsolódás felsőbb rétegbeli kiszolgálóhoz** lapján kell elvégezni.

**A felsőbb rétegbeli kiszolgáló és a proxykiszolgáló adatainak mentése és letöltése**
1.  A konfigurációs varázsló Kapcsolódás felsőbb rétegbeli kiszolgálóhoz lapján kattintson a **Kapcsolódás indítása** gombra. Ezzel menti és feltölti a beállításokat, valamint összegyűjti a rendelkezésre álló frissítésekkel kapcsolatos adatokat.

2.  A kapcsolódás alatt elérhető a **Kapcsolódás leállítása** gomb. Ha probléma merülne fel a kapcsolódással, kattintson a **Kapcsolódás leállítása** gombra, végezze el a szükséges javítást, majd indítsa újra a kapcsolódást.

3.  Ha a letöltés sikeresen befejeződött, kattintson a **Tovább** gombra.

**A frissítések nyelvének kiválasztása**
1.  A Nyelvek kiválasztása lapon beállíthatja, hogy minden nyelven vagy csak bizonyos nyelveken kívánja-e letölteni a frissítéseket. Ha csak a nyelvek egy részét jelöli ki, azzal lemezterületet takaríthat meg; fontos azonban, hogy minden olyan nyelvet kijelöljön, amelyre az adott WSUS-kiszolgáló bármelyik ügyfelének szüksége lehet.

    Ha csak bizonyos nyelvű frissítéseket szeretne letölteni, válassza a **Csak az ilyen nyelvű frissítések letöltése** lehetőséget, és jelölje ki azokat a nyelveket, amelyeken le kívánja tölteni a frissítéseket.

2.  Kattintson a **Tovább** gombra.

**A frissítendő termékek kiválasztása**
1.  A Termékek kiválasztása lapon kiválaszthatja azokat a termékeket, amelyekhez frissítéseket szeretne letölteni Bejelölheti a kívánt termékkategóriákat (például Windows) vagy konkrét termékeket (például Windows Server 2008). Ha kiválaszt egy termékkategóriát, az minden, a kategóriába tartozó termék kijelölését eredményezi.

2.  Kattintson a **Tovább** gombra.

**A frissítésbesorolások kiválasztása**
1.  A Besorolások kiválasztása lapon kiválaszthatja, hogy milyen besorolású frissítéseket kíván letölteni. Kiválaszthatja az összes besorolást vagy a besorolások egy részhalmazát.

2.  Kattintson a **Tovább** gombra.

**A szinkronizálás ütemezésének beállítása**
1.  A Szinkronizálási ütemezés beállítása lapon megadhatja, hogy a szinkronizálást manuálisan vagy automatikusan kívánja-e végrehajtani.

    Ha a **Manuális szinkronizálás** lehetőséget választja, a szinkronizálási eljárást a WSUS felügyeleti konzolból kell elindítania.

    Az **Automatikus szinkronizálás** lehetőség választása esetén a WSUS-kiszolgáló megadott időközönként elvégzi a szinkronizálást. Adjon meg egy időpontot az **Első szinkronizálás** beállításhoz, a **Szinkronizálás naponta** beállításnál pedig adja meg, hogy hányszor végezzen a kiszolgáló naponta szinkronizálást. Ha például azt állítja be, hogy naponta négy szinkronizálás történjen, és az első 3:00 órakor kezdődjön, a következő időpontokban történik szinkronizálás: 3:00, 9:00, 15:00 és 21:00.

2.  Kattintson a **Tovább** gombra.

3.  Ha a Befejezve lapon nem törli a jelölést **A Windows Server Update Services felügyeleti beépülő moduljának elindítása** jelölőnégyzetből, elindíthatja a WSUS felügyeleti konzolt, továbbá elindíthatja az első szinkronizálást, ha bejelölve hagyja az **Első szinkronizálás elindítása** jelölőnégyzetet.

4.  Kattintson a **Befejezés** gombra.

<p> </p>
    <table style="border:1px solid black;">
    <colgroup>
    <col width="100%" />
    </colgroup>
    <thead>
    <tr class="header">
    <th><img src="images/Dd939924.Important(WS.10).gif" />Fontos</th>
    </tr>
    </thead>
    <tbody>
    <tr class="odd">
    <td style="border:1px solid black;">Miközben a kiszolgáló szinkronizálást végez, nem lehet konfigurációs módosításokat végezni. Várjon, amíg a szinkronizálás befejeződik, és csak utána módosítsa a beállításokat.
    <p></p></td>
    </tr>
    </tbody>
    </table>
<p> </p>

A WSUS felügyeleti konzol használata esetén
-------------------------------------------

A következőkben annak ismertetését olvashatja, hogy miként végezhetők el a konfiguráció lépései a WSUS felügyeleti konzol segítségével.

**Termékek és frissítésbesorolások kiválasztása**
1.  Kattintson a **Beállítások** lapon a **Termékek és besorolások** elemre. Ekkor megjelenik egy, a **Termékek** és a **Besorolások** lapot tartalmazó párbeszédpanel.

2.  A **Termékek** lapon jelölje be azt a termékcsaládot vagy adott termékeket, amelyekhez frissítéseket kíván letölteni, vagy válassza a **Minden termék** lehetőséget.

3.  Jelölje be a kívánt frissítésbesorolásokat a **Besorolások** lapon, vagy válassza a **Minden besorolás** lehetőséget.

4.  A beállítások mentéséhez kattintson az **OK** gombra.

**Frissítésfájlok és nyelvek kiválasztása**
1.  Kattintson a **Beállítások** lapon a **Frissítésfájlok és nyelvek** elemre. Ekkor megjelenik egy, a **Frissítésfájlok** és a **Frissítések nyelve** lapot tartalmazó párbeszédpanel.

2.  A **Frissítésfájlok** lapon a **Frissítésfájlok tárolása helyileg ezen a kiszolgálón** beállítással kiválaszthatja, hogy a frissítésfájlok tárolása helyben történjen, vagy megadhatja, hogy minden ügyfélszámítógép frissítése közvetlenül a Microsoft Update webhelyről menjen végbe. Ha úgy dönt, hogy a kiszolgálón tárolja a frissítésfájlokat, azt is megadhatja, hogy csak a jóváhagyott frissítéseket tölti le, illetve hogy letölti-e a gyorstelepítő fájlokat.

3.  A **Frissítések nyelve** lapon, ha a frissítésfájlokat helyben tárolja, választhat a **Frissítések letöltése minden nyelvhez** (alapértelmezett beállítás) és a **Csak a választott nyelvű frissítések letöltése** lehetőség közül. Ha vannak alsóbb rétegbeli kiszolgálói a WSUS-kiszolgálónak, azok csak a felsőbb rétegbeli kiszolgálón megadott nyelveken fognak frissítéseket kapni.

4.  A beállítások mentéséhez kattintson az **OK** gombra.

**A WSUS-kiszolgáló szinkronizálása**
1.  Kattintson a **Beállítások** lapon a **Szinkronizálás ütemezése** parancsra.

2.  A **Szinkronizálási ütemezése** lapon megadhatja, hogy a szinkronizálást manuálisan vagy automatikusan kívánja-e végrehajtani.

    Ha a **Manuális szinkronizálás** lehetőséget választja, a szinkronizálási eljárást a WSUS felügyeleti konzolból kell elindítania.

    Az **Automatikus szinkronizálás** lehetőség választása esetén a WSUS-kiszolgáló megadott időközönként elvégzi a szinkronizálást. Adjon meg egy időpontot az **Első szinkronizálás** beállításhoz, a **Szinkronizálás naponta** beállításnál pedig adja meg, hogy hányszor végezzen a kiszolgáló naponta szinkronizálást. Ha például azt állítja be, hogy naponta négy szinkronizálás történjen, és az első 3:00 órakor kezdődjön, a következő időpontokban történik szinkronizálás: 3:00, 9:00, 15:00 és 21:00.

3.  A beállítások mentéséhez kattintson az **OK** gombra.

4.  A WSUS felügyeleti konzol navigációs ablaktáblájában kattintson a **Szinkronizálások** elemre.

5.  Kattintson a jobb gombbal, vagy navigáljon a jobb oldalon lévő **Műveletek** ablaktáblába, és kattintson a **Szinkronizálás most** elemre.

    Ha nem látható a **Műveletek** ablaktábla a konzol jobb oldalán, kattintson az eszköztáron a **Nézet** menüre, majd a **Testreszabás** parancsra, és ellenőrizze, hogy be van-e jelölve a **Munkaablak** jelölőnégyzet.

6.  A szinkronizálás befejezését követően a frissítések listájának megtekintéséhez kattintson a bal oldali ablaktábla **Frissítések** elemére.

Következő lépés
---------------

[5. lépés: Ügyfélfrissítések konfigurálása](https://technet.microsoft.com/5ae60ead-3e94-456c-a692-c0f193ea5d5a)

További források
----------------

[Részletes útmutató a Windows Server Update Services 3.0 SP2 telepítéséhez](https://technet.microsoft.com/4b504edc-93b3-45b0-a7e8-d0107f1a4442)
