---
TOCTitle: '1. lépés: A WSUS 3.0 SP2 telepítési követelményeinek megerősítése'
Title: '1. lépés: A WSUS 3.0 SP2 telepítési követelményeinek megerősítése'
ms:assetid: 'ec01bd75-5def-4899-8cee-ddab827bbd83'
ms:contentKeyID: 21741829
ms:mtpsurl: 'https://technet.microsoft.com/hu-hu/library/Dd939916(v=WS.10)'
---

1. lépés: A WSUS 3.0 SP2 telepítési követelményeinek megerősítése
=================================================================

Mielőtt telepítené a Windows Server Update Services 3.0 Service Pack 2 (WSUS 3.0 SP2) szolgáltatást, illetve arra frissítene, meg kell győződnie arról, hogy a kiszolgáló és az ügyfélszámítógépek egyaránt megfelelnek a WSUS 3.0 SP2 rendszerkövetelményeinek, valamint hogy rendelkezik a telepítés végrehajtásához szükséges engedélyekkel.

A kiszolgáló hardver- és szoftverkövetelményei a WSUS 3.0 SP2 telepítéséhez
---------------------------------------------------------------------------

1.  Győződjön meg arról, hogy a kiszolgáló megfelel a WSUS 3.0 SP2 rendszerkövetelményeinek mind a hardvereszközök, mind pedig az operációs rendszer és más szükséges szoftverek tekintetében. A rendszerkövetelmények listáját a WSUS 3.0 SP2 kibocsátási megjegyzései között, a [http://go.microsoft.com/fwlink/?LinkId=139840](http://go.microsoft.com/fwlink/?linkid=139840) webhelyen találja. Ha a WSUS 3.0 SP2 telepítéséhez a Kiszolgálókezelőt használja, a szoftverkövetelményeknek való megfelelést a „Felkészülés a WSUS 3.0 SP2 telepítésére” című részben található lépésekkel ellenőrizheti.
2.  Ha olyan szerepköröket vagy szoftverfrissítéseket telepít, amelyekhez újra kell indítani a kiszolgálót a telepítés végeztével, akkor a kiszolgálót még a WSUS 3.0 SP2 telepítése előtt indítsa újra.

Ügyfélszámítógépek szoftverkövetelményei
----------------------------------------

Az Automatikus frissítések segédprogram a WSUS 3.0 szolgáltatás ügyféloldali összetevője. Erre vonatkozóan mindössze annyi a hardverkövetelmény, hogy legyen működő hálózati kapcsolat.

1.  Győződjön meg arról, hogy az a számítógép, amelyen telepíti az automatikus frissítési szolgáltatást, megfelel a WSUS 3.0 SP2 ügyfélszámítógépekre vonatkozó rendszerkövetelményeinek. A rendszerkövetelmények listáját a WSUS 3.0 SP2 kibocsátási megjegyzései között, a [http://go.microsoft.com/fwlink/?LinkId=139840](http://go.microsoft.com/fwlink/?linkid=139840) webhelyen találja.
2.  Ha olyan szoftverfrissítéseket telepít, amelyekhez újra kell indítani a számítógépet, az újraindítást még a WSUS 3.0 SP2 telepítése előtt hajtsa végre.

Engedélyek
----------

A következő engedélyekre van szükségük a megadott felhasználóknak és könyvtáraknak:

1.  Az NT Authority\\Hálózati szolgáltatás fióknak teljes hozzáférést kell adni a következő mappákhoz, hogy a WSUS felügyeleti beépülő modul helyesen jelenjen meg:
    -   %windir%\\Microsoft .NET\\Framework\\v2.0.50727\\Temporary ASP.NET Files
    -   %windir%\\Temp
2.  Ellenőrizze, hogy a WSUS 3.0 SP2 telepítéséhez használni kívánt fiók tagja-e a Helyi rendszergazdák csoportnak.

Felkészülés a WSUS 3.0 SP2 telepítésére
---------------------------------------

Windows 7 vagy Windows Server 2008 SP2 rendszer esetén a WSUS 3.0 SP2 a Kiszolgálókezelőből telepíthető. Ha másik támogatott operációs rendszert használ, vagy ha csak a WSUS felügyeleti konzolt telepíti, ugorjon a jelen útmutató következő részére a WSUS 3.0 SP2 szolgáltatásnak a WUSSetup.exe fájl segítségével történő telepítéséhez.

**Felkészülés a WSUS 3.0 SP2 telepítésére a Kiszolgálókezelő használata esetén**
1.  Egy, a helyi Rendszergazdák csoportba tartozó felhasználói fiókkal jelentkezzen be arra a kiszolgálóra, amelyen a WSUS 3.0 SP2 szolgáltatást telepíteni szeretné.

2.  Mutasson a **Start** menü **Felügyeleti eszközök** pontjára, majd kattintson a **Kiszolgálókezelő** parancsra.

3.  A Kiszolgálókezelő ablakának jobb oldali ablaktáblájában, a Szerepkörök összegzése csoportban kattintson a **Szerepkör hozzáadása** hivatkozásra.

4.  Ha megjelenik az alapismereteket ismertető lap, kattintson a **Tovább** gombra.

5.  A Kiszolgálói szerepkörök kiválasztása lapon győződjön meg arról, hogy be van jelölve az **Alkalmazáskiszolgáló** és a **Webkiszolgáló (IIS)** jelölőnégyzet. Ha be vannak jelölve, akkor a jelen lépés fennmaradó műveleteit végrehajtva ellenőrizze, hogy ki vannak-e jelölve a szükséges szerepkör-szolgáltatások. Ellenkező esetben az alábbiak szerint telepítse az Alkalmazáskiszolgáló és a Webkiszolgáló (IIS) szerepkört.

    1.  A Kiszolgálói szerepkörök kiválasztása lapon jelölje be az **Alkalmazáskiszolgáló** és a **Webkiszolgáló (IIS)** jelölőnégyzetet. Kattintson a **Tovább** gombra.
    2.  Az Alkalmazáskiszolgáló szerepkör-szolgáltatás telepítése esetén kattintson az Alkalmazáskiszolgáló lapon a **Tovább** gombra. Az Alkalmazáskiszolgáló szerepkörhöz tartozó Szerepkör-szolgáltatások lapon fogadja el az alapértelmezett beállításokat, majd kattintson a **Tovább** gombra.
    3.  A Webkiszolgáló (IIS) szerepkör-szolgáltatás telepítése esetén kattintson a Webkiszolgáló (IIS) lapon a **Tovább** gombra. A Webkiszolgáló (IIS) szerepkör-szolgáltatáshoz tartozó Szerepkör-szolgáltatások lapon őrizze meg az alapértelmezett beállításokat, valamint jelölje be az **ASP.NET**, a **Windows-hitelesítés**, **Dinamikus tartalomtömörítés** és a **Kompatibilitás az IIS 6 kezelésével** jelölőnégyzetet. Ha megjelenik a Szerepkörök hozzáadása varázsló ablaka, kattintson a **Szükséges szerepkör-szolgáltatások hozzáadása** gombra. Kattintson a **Tovább** gombra.
    4.  A Telepítendők megerősítése lapon kattintson a **Telepítés** gombra.
    5.  A Telepítés eredménye lapon győződjön meg arról, hogy a jelen lépésben telepített szerepkör-szolgáltatások telepítése sikeres volt, majd kattintson a **Bezárás** gombra.

Következő lépés
---------------

[2. lépés: A WSUS Server vagy felügyeleti konzol telepítése](https://technet.microsoft.com/6db6fcb0-c55d-43b9-9b07-4040c6267759)

További források
----------------

[Részletes útmutató a Windows Server Update Services 3.0 SP2 telepítéséhez](https://technet.microsoft.com/4b504edc-93b3-45b0-a7e8-d0107f1a4442)
