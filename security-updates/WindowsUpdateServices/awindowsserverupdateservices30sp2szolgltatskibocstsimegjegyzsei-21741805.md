---
TOCTitle: 'A Windows Server Update Services 3.0 SP2 szolgáltatás kibocsátási megjegyzései'
Title: 'A Windows Server Update Services 3.0 SP2 szolgáltatás kibocsátási megjegyzései'
ms:assetid: 'b3723422-489d-47b7-abfa-663353647da0'
ms:contentKeyID: 21741805
ms:mtpsurl: 'https://technet.microsoft.com/hu-hu/library/Dd939886(v=WS.10)'
---

A Windows Server Update Services 3.0 SP2 szolgáltatás kibocsátási megjegyzései
==============================================================================

A kibocsátási megjegyzések a Windows Server Update Services 3.0 Service Pack 2 (WSUS 3.0 SP2) szolgáltatást tárgyalják. Ez a dokumentum a következő szakaszokat tartalmazza:

1.  Újdonságok ebben a kiadásban
2.  Rendszerkövetelmények a WSUS 3.0 SP2 kiszolgáló telepítéséhez
3.  Előfeltételek és gyakorlati tanácsok a WSUS-kiszolgáló telepítéséhez
4.  Előfeltételek a Windows Small Business Server rendszeren történő telepítéshez
5.  Rendszerkövetelmények a WSUS 3.0 SP2 távoli konzolról való telepítéséhez
6.  Rendszerkövetelmények ügyféltelepítéshez
7.  Frissítési követelmények és ajánlások
8.  A WSUS 3.0 SP2 telepítése
9.  A telepítő parancssori paraméterei a WSUS 3.0 SP2 felügyelet nélküli telepítéséhez
10. Ismert problémák

Újdonságok ebben a kiadásban
----------------------------

-   Integráció a Windows Server 2008 R2 rendszerrel.
-   A Windows Server 2008 R2 rendszer BranchCache szolgáltatásának támogatása.
-   Windows 7 operációs rendszerű ügyfelek támogatása.
-   Továbbfejlesztett Windows Update Agent ügyfél (WUA ügyfél). Az új WUA ügyfél teljesítménynövelő, illetve a felhasználói élményt fokozó fejlesztések mellett a vásárlói visszajelzések során feltárt különböző hibák javítását is tartalmazza.
    -   Az ügyfelek vizsgálata gyorsabb a korábbi verzióknál.
    -   A WSUS-kiszolgálókkal kezelt számítógépek a teljes vizsgálat helyett kiválasztott WSUS-kiszolgálókon is elvégezhetik az ellenőrzéseket. Ez egy nagyságrenddel gyorsabb ellenőrzést tesz lehetővé a Microsoft frissítési alkalmazásprogramozási felületét (Microsoft Update API) használó alkalmazások, például a Windows Defender számára.
    -   A Windows Update Agent (WUA) felhasználói élményt fokozó fejlesztéseinek köszönhetően a felhasználók logikusabban rendszerezhetik a frissítéseket, és jobban átláthatják az egyes frissítések szükségességét és viselkedését.
    -   A lemezképekből telepített számítógépek egyértelműbben azonosíthatók a WSUS-konzolban. További részleteket olvashat [A Windows 2000- vagy Windows XP-lemezképpel telepített Windows 2000- és Windows XP-alapú számítógépek nem láthatók a Windows Server Update Services (WSUS) konzolján](http://go.microsoft.com/fwlink/?linkid=159749) című cikkben.
-   Újdonságok:
    -   Az automatikus jóváhagyási szabályok segítségével meghatározhatja a jóváhagyási határidő dátumát és időpontját minden számítógépre vagy adott számítógép-csoportokra vonatkozóan.
    -   A nyelv alsóbb rétegbeli kiszolgálókon való kiválasztásának javítása révén új figyelmeztető párbeszédpanel jelenik meg, amikor a frissítéseket csak meghatározott nyelvekhez tölti le.
    -   Az új frissítési és számítógépállapot-jelentések lehetővé teszik a telepítésre jóváhagyott frissítések szűrését. A jelentések a WSUS konzoljáról futtathatók, illetve a hozzájuk kapcsolódó programozási felület révén beépíthetők saját jelentésekbe.
-   A WSUS 3.0 Service Pack 1 ügyfél- és kiszolgálóoldali felhasználói felülete kompatibilis a Service Pack 2 verzióéval.
-   Szoftverfrissítések.
-   A Windows Update Agent ebben a kiadásban javított ismert problémái:
    1.  A WSUS 3.0 SP2 és a Windows 7 tartalmazza a Windows Update Agent – Windows XP, Windows Vista, Windows Server 2000, Windows Server 2003 és Windows Server 2008 rendszerhez készült – új változatát. A kiadásban a következő probléma került javításra: A nem helyi rendszerek nem interaktív munkamenetből történő API-hívásai sikertelenek.
    2.  A Windows Update Agent 7.2.6001.788-as verziójában javított probléma. A frissítésben a következő probléma került javításra: Ha a Windows Update vagy a Microsoft Update webhelyről egyidejűleg 80-nál több frissítést próbál telepíteni, a 0x80070057 hibakód jelenik meg.
    3.  A Windows Update Agent 7.2.6001.784-es verziója által tartalmazott fejlesztések és hibajavítások. A frissítés a következőket tartalmazza: A keresés és az aláírás-frissítések küldésének gyorsítása a Windows Update szolgáltatásban, a Windows Installer újratelepítési szolgáltatásának támogatása, részletesebb hibaüzenetek.

<span id="BKMK_SysReqWSUS30SP2"></span>
Rendszerkövetelmények a WSUS 3.0 SP2 kiszolgáló telepítéséhez
-------------------------------------------------------------

A szakasz a WSUS 3.0 SP2 telepítésének szoftver- és hardverkövetelményeit ismerteti.

### Szoftveres előfeltételek a WSUS kiszolgáló telepítéséhez

-   A telepítéshez az alábbi operációs rendszerek valamelyike szükséges:
    -   Windows Server 2008 R2
    -   Windows Server 2008 SP1 vagy újabb verzió
 
        <table style="border:1px solid black;">
        <colgroup>
        <col width="100%" />
        </colgroup>
        <thead>
        <tr class="header">
        <th style="border:1px solid black;" ><img src="images/Dd939886.Warning(WS.10).gif" />Figyelmeztetés</th>
        </tr>
        </thead>
        <tbody>
        <tr class="odd">
        <td style="border:1px solid black;">Ha a WSUS 3.0 SP2 kiszolgálót Windows Server 2008 rendszerre telepíti Windows Server 2008 R2 helyett, a Windows Server 2008 R2 rendszerre való frissítés sikertelen lesz. További információt talál az <a href="#bkmk_knownissues">Ismert problémák</a> szakaszban.
        </td>
        </tr>
        </tbody>
        </table>
 

    -   Windows Server 2003 SP1 vagy újabb verzió
    -   Windows Small Business Server 2008
    -   Windows Small Business Server 2003

    Ne feledje, hogy a további feltételek a Windows Small Business Server rendszerre vonatkoznak. További információt az „Előfeltételek a Windows Small Business Server rendszeren történő telepítéshez” című részben talál.
-   Internet Information Services (IIS) 6.0 vagy újabb verzió
-   A Microsoft .NET Framework 2.0-s vagy újabb verziója
-   A telepítéshez az alábbi adatbázis-kezelők valamelyike szükséges:
    -   Microsoft SQL Server 2008 Standard Edition vagy Enterprise Edition
    -   Microsoft SQL Server 2005 SP3 vagy újabb verzió
    -   Belső Windows-adatbázis

    Ha nincs telepítve az SQL Server valamelyik támogatott verziója, a WSUS 3.0 SP2 telepítővarázslója telepíti a Belső Windows-adatbázis összetevőt.
-   Microsoft Management Console 3.0
-   A Microsoft Report Viewer 2008 terjeszthető változata

 
<table style="border:1px solid black;">
<colgroup>
<col width="100%" />
</colgroup>
<thead>
<tr class="header">
<th style="border:1px solid black;" ><img src="images/Dd939886.Important(WS.10).gif" />Fontos</th>
</tr>
</thead>
<tbody>
<tr class="odd">
<td style="border:1px solid black;">A Windows Server 2008 R2 rendszerhez a WSUS 3.0 SP2 szükséges. Windows Server 2008 R2 rendszer telepítése esetén a WSUS 3.0 SP2 verziót ajánlott telepítenie. A WSUS 3.0 SP1 verzióját ne telepítse Windows Server 2008 R2 rendszeren.

A WSUS 3.0 SP2 távoli SQL-konfigurációban nem támogatja az előtér-kiszolgálón futó terminálszolgáltatáson keresztüli használatot.
</td>
</tr>
</tbody>
</table>
 

### A WSUS felügyeleti konzol használatának szoftveres előfeltételei

-   A következő operációs rendszerek valamelyike: Windows Server 2008 R2, Windows Server 2008, Windows Server 2003 SP2 vagy újabb verzió, Windows Small Business Server 2008 vagy Windows Small Business Server 2003, Windows Vista vagy Windows XP SP2
-   Microsoft .NET Framework 2.0 vagy újabb verzió
-   Microsoft Management Console 3.0
-   A Microsoft Report Viewer 2008 terjeszthető változata

### Hardverkövetelmények a WSUS kiszolgáló telepítéséhez

Az alábbi lista a kiszolgáló alapszintű telepítéséhez szükséges minimális hardverkövetelményeket tartalmazza. A támogatott hardverkonfigurációk részletes listáját a WSUS 3.0 SP2 üzembehelyezési útmutatójában találja, a [http://go.microsoft.com/fwlink/?LinkId=139832](http://go.microsoft.com/fwlink/?linkid=139832) címen.

-   Mind a rendszerpartíciónak, mind pedig a WSUS 3.0 SP2 rendszert tároló partíciónak NTFS fájlrendszerűnek kell lennie.
-   Legalább 1 GB szabad lemezterület a rendszerpartíción
-   Legalább 2 GB szabad lemezterület az adatbázisfájlok tárolására használandó köteten
-   Legalább 20 GB (lehetőség szerint 30 GB) szabad lemezterület a tartalom tárolására szolgáló köteten

 
<table style="border:1px solid black;">
<colgroup>
<col width="100%" />
</colgroup>
<thead>
<tr class="header">
<th style="border:1px solid black;" ><img src="images/Dd939886.Important(WS.10).gif" />Fontos</th>
</tr>
</thead>
<tbody>
<tr class="odd">
<td style="border:1px solid black;">A WSUS 3.0 SP2 nem telepíthető tömörített meghajtókra.
</td>
</tr>
</tbody>
</table>
 

Előfeltételek és gyakorlati tanácsok a WSUS-kiszolgáló telepítéséhez
--------------------------------------------------------------------

Győződjön meg arról, hogy elvégezte az ebben a szakaszban szereplő megfelelő lépéseket, mielőtt telepíti a WSUS 3.0 SP2 szolgáltatást.

### IIS

-   A Kiszolgálókezelő Webkiszolgáló (IIS) szerepkör-szolgáltatáshoz tartozó szerepkör-szolgáltatási lapján telepítsen minden szükséges szolgáltatást, az IIS összes alapértelmezett szerepkör-szolgáltatását, valamint az **ASP.NET**, a **Windows-hitelesítés**, a **Dinamikus tartalomtömörítés** és a **Kompatibilitás az IIS 6 kezelésével** összetevőt.
-   Ha az IIS az IIS 5.0 elkülönítési üzemmódjában fut, a telepítés sikertelen lesz. A WSUS 3.0 SP2 telepítése előtt tiltsa le az IIS 5.0 elkülönítési üzemmódját.
-   Ha bármely IIS-összetevő 32 bites kompatibilitási üzemmódban van telepítve egy 64 bites platformon, az a WSUS 3.0 SP2 telepítésének sikertelenségét okozhatja. Minden IIS-összetevőt natív módban kell telepíteni a 64 bites platformokon.

### Proxykiszolgálók

A WSUS 3.0 SP2 csak olyan proxykiszolgálókat támogat, melyek kizárólag a HTTP protokollt támogatják. Gyakorlati tanácsként célszerű egy második, HTTPS protokollt támogató proxykiszolgálót beállítani a **wsusutil configuresslproxy** parancssori paranccsal, mielőtt a konfigurációs varázslóval vagy a felügyeleti konzolban hozzákezd a WSUS kiszolgáló konfigurálásához.

### A 80-as porton keresztül elérhető webhelyek

Ha legalább két, a 80-as porton keresztül elérhető webhellyel (például Windows SharePoint Services-webhelyekkel) rendelkezik, a WSUS telepítését megelőzően egy kivételével törölje az összeset. Ha elmulasztja ezt a lépést, előfordulhat, hogy a kiszolgáló ügyfelei nem tudják önmagukat frissíteni.

### Víruskereső programok

Előfordulhat, hogy a WSUS 3.0 SP2 telepítésekor le kell tiltani a víruskereső programokat, és csak ezt követően lehet végrehajtani a telepítést. Miután letiltotta a víruskereső szoftvert, indítsa újra a számítógépet, mielőtt telepíti a WSUS szolgáltatást. A számítógép újraindításával megakadályozható, hogy a fájlok zárolva legyenek, amikor a telepítő hozzájuk szeretne férni. A telepítés befejezését követően ismét kapcsolja be a víruskereső szoftvert. A víruskereső szoftver letiltásának és visszakapcsolásának pontos lépéseiről a víruskereső szoftver forgalmazójának webhelyén találhat tájékoztatást.

 
<table style="border:1px solid black;">
<colgroup>
<col width="100%" />
</colgroup>
<thead>
<tr class="header">
<th style="border:1px solid black;" ><img src="images/Dd939886.Caution(WS.10).gif" />Vigyázat!</th>
</tr>
</thead>
<tbody>
<tr class="odd">
<td style="border:1px solid black;">Ez a megkerülő megoldás sérülékenyebbé teheti a számítógépet vagy a hálózatot a rosszindulatú felhasználók és a kártevő szoftverek, például vírusok támadásával szemben. Nem javasoljuk ezt a megoldást, de tájékoztatásul közöljük, hogy saját belátása szerint szükség esetén alkalmazni tudja, ezt azonban csak saját felelősségére teheti.

A víruskereső szoftverek abban segítenek, hogy megvédhesse számítógépét a vírusoktól. Amíg a víruskereső program le van tiltva, ne töltsön le és ne nyisson meg fájlokat nem megbízhatónak vélt forrásból, ne látogasson nem megbízható webhelyekre, és ne nyisson meg e-mail mellékleteket.
</td>
</tr>
</tbody>
</table>
 

### Beágyazott eseményindítók az SQL Server alkalmazásban

Ha a Windows Server Update Services adattárolójaként egy SQL Server-alapú adatbázist szeretne használni, az SQL Server rendszergazdájának ellenőriznie kell, hogy a beágyazott eseményindítók engedélyezve vannak-e a kiszolgálón, mielőtt a WSUS rendszergazdája telepíti a WSUS 3.0 SP2 rendszert. A beágyazott eseményindítók használata alapértelmezés szerint be van ugyan kapcsolva, de az SQL Server rendszergazdái kikapcsolhatják. A WSUS 3.0 SP2 telepítője engedélyezi a rekurzív eseményindítást szabályozó, adatbázisszintű RECURSIVE\_TRIGGERS beállítást. A telepítő azonban külön nem engedélyezi a beágyazott eseményindítást, mivel ez kiszolgálószintű, azaz globális beállítás.

### A távoli SQL-kiszolgálóval kapcsolatos korlátozások és követelmények

A WSUS 3.0 SP2 a más számítógépeken futó SQL Server kiszolgálókat is támogatja, amennyiben azok verziója és kiadása megfelel a követelményeknek. A távoli SQL-kiszolgálók telepítésére az alábbi követelmények vonatkoznak.

-   Tartományvezérlőnek konfigurált kiszolgáló nem használható a távoli SQL-pár háttérkiszolgálójaként.
-   A távoli SQL-adatbázis előtér-kiszolgálójaként üzemelő számítógépen nem futtatható a Terminálszolgáltatások összetevő.
-   Az előtér-számítógépet és a háttérszámítógépet is csatlakoztatnia kell egy Active Directory-tartományhoz. Ha a két számítógép eltérő tartományban található, hozzon létre tartományok közötti bizalmi kapcsolatot, mielőtt telepíti a WSUS szolgáltatást.
-   Ha a WSUS 2.0 távoli SQL-konfigurációban van telepítve, és frissíteni szeretné a WSUS 3.0 SP2 verzióra, előbb tegye a következőket:
    1.  Távolítsa el a WSUS 2.0 verziót a számítógépről (a Vezérlőpult **Programok telepítése és törlése** segédprogramjával), és gondoskodjon arról, hogy a meglévő adatbázis ne módosuljon.
    2.  Telepítse az SQL Server 2005 SP2 vagy az SQL Server 2008 adatbázis-kezelőt, és frissítse a meglévő adatbázist.

### Az IIS újraindul a WSUS 3.0 SP2 telepítése folyamán

A WSUS 3.0 SP2 telepítő figyelmeztetés nélkül újraindítja az IIS kiszolgálót, ami hatással lehet a szervezeten belül működő webhelyekre. Ajánlott a telepítés előtt erről tájékoztatni az érintett feleket. Ne feledje, hogy amennyiben nem fut az IIS szolgáltatás, a WSUS 3.0 SP2 telepítője el fogja indítani azt.

Előfeltételek a Windows Small Business Server rendszeren történő telepítéshez
-----------------------------------------------------------------------------

A WSUS 3.0 SP2 szolgáltatás az alábbi feltételek teljesülése esetén telepíthető a Windows Small Business Server rendszerre.

### Ha az IIS virtuális gyökér korlátozva van bizonyos IP-címekre vagy tartománynevekre

Előfordulhat, hogy a Windows Small Business Server telepített példányán az alapértelmezett IIS webhelyre vonatkozóan be van állítva az **IP-cím és tartománynév korlátozása**. Ebben az esetben előfordulhat, hogy a kiszolgálón futó Windows Update ügyfél nem tudja frissíteni magát. A WSUS 3.0 SP2 telepítése előtt távolítsa el ezt a korlátozást.

### ISA proxykiszolgáló használata esetén

-   Ha a Windows Small Business Server ISA-proxykiszolgálón keresztül éri el az internetet, a **Beállítások** párbeszédpanelen meg kell adni a **proxykiszolgáló beállításai, proxykiszolgáló neve, portszám** információkat.
-   Ha az ISA Windows-hitelesítést igényel, a proxykiszolgáló hitelesítő adatait a *TARTOMÁNY*\\*felhasználó* formátumban kell megadni. A felhasználónak az Internetfelhasználók csoportba kell tartoznia.

### Ha a Windows Small Business Server varázslói nélkül adott alhálózatot a hálózathoz

A WSUS-kiszolgáló telepítője két IIS virtuális gyökeret telepít a kiszolgálóra: a SelfUpdate és a ClientWebService nevűt. Ezenfelül néhány fájlt elhelyez a 80-as porton figyelő alapértelmezett webhely gyökérkönyvtárába. Az ügyfélszámítógépek az alapértelmezett webhelyen keresztül ezeket használva frissíthetik önmagukat. Alapértelmezés szerint az alapértelmezett webhely úgy van beállítva, hogy a localhost címen és a kiszolgálóhoz kapcsolódó megadott alhálózatokon kívül minden IP-címhez megtagadja a hozzáférést. Ennek következtében a nem a helyi állomáshoz vagy a megadott alhálózatokhoz tartozó ügyfélszámítógépek nem tudják önmagukat frissíteni. Ha a Microsoft Windows Small Business Server varázslói nélkül alakított ki alhálózatot a hálózati szegmensben, végre kell hajtani az alábbi műveleteket:

1.  Bontsa ki a Kiszolgálókezelés eszközben a **Speciális kezelés**, az **Internet Information Services**, a **Webhelyek**, majd az **Alapértelmezett webhely** elemet, kattintson a jobb gombbal a **Selfupdate** virtuális könyvtárra, végül kattintson a **Tulajdonságok** elemre.
2.  Kattintson a **Könyvtárbiztonság** elemre.
3.  Kattintson az **IP-cím és tartománynév korlátozása** csoportban a **Szerkesztés** gombra, majd a **hozzáférése engedélyezve** lehetőségre.
4.  Kattintson az **OK** gombra, kattintson a jobb gombbal a **ClientWebService** virtuális könyvtárra, majd kattintson a **Tulajdonságok** pontra.
5.  Kattintson a **Könyvtárbiztonság** elemre.
6.  Kattintson az **IP-cím és tartománynév korlátozása** csoportban a **Szerkesztés** gombra, majd a **hozzáférése engedélyezve** lehetőségre.

Rendszerkövetelmények a WSUS 3.0 SP2 távoli konzolról való telepítéséhez
------------------------------------------------------------------------

A WSUS 3.0 SP2 a következő operációs rendszereken telepíthető:

-   Windows Server 2008 R2, Windows Server 2008 SP1 vagy újabb verzió, Windows Server 2003 SP2 vagy újabb verzió, Windows Small Business Server 2003, Windows Small Business Server 2005 vagy Windows Small Business Server 2008, Windows Vista, valamint Windows XP Professional SP3 vagy újabb verzió.

Rendszerkövetelmények a WSUS-ügyfél telepítéséhez
-------------------------------------------------

A WSUS-ügyfélszoftver, az Automatikus frissítések szolgáltatás a következő operációs rendszerek bármelyikére telepíthető:

-   Windows Server 2008 R2, Windows Server 2008 SP1 vagy újabb verzió, Windows Server 2003 SP2 vagy újabb verzió, Windows Small Business Server 2003, Windows Small Business Server 2005, Windows Small Business Server 2008, Windows Vista, Windows XP Professional RTM, Windows XP Professional SP1, Windows XP Professional SP2, Windows XP Professional SP3 vagy újabb verzió, Windows 2000 SP4, illetve Windows 7 (ügyfél).

Frissítési követelmények és ajánlások
-------------------------------------

A következő WSUS-verziók eltávolítás nélkül is frissíthetők a WSUS 3.0 SP2 rendszerre:

-   WSUS 2.0, 2.0 SP1, 3.0 és 3.0 SP1.

A WSUS 1.0 nem frissíthető a 3.0 SP2 verzióra. A WSUS 3.0 SP2 telepítése előtt távolítsa el a SUS 1.0 szolgáltatást.

A Windows Server 2008 R2 rendszerhez a WSUS 3.0 SP2 szükséges. Windows Server 2008 R2 rendszer telepítése esetén a WSUS 3.0 SP2 verziót telepítse; a WSUS 3.0 SP1 verziót ne telepítse ezen az operációs rendszeren.

#### Teendők a WSUS 3.0 SP2 verzióra való frissítés előtt

1.  Ellenőrizze az eseménynaplókat, hogy nincsenek-e a felsőbb és alsóbb rétegbeli kiszolgálók közötti szinkronizációval kapcsolatos problémák, illetve az ügyfelek által jelentett problémák. Ha vannak, frissítés előtt szüntesse meg ezeket.

2.  A DBCC CHECKDB eljárással ellenőrizheti, hogy a WSUS-adatbázis megfelelően van-e indexelve. Erről bővebben a [DBCC CHECKDB](http://go.microsoft.com/fwlink/?linkid=86948) című részben olvashat.

3.  Készítsen biztonsági másolatot a WSUS adatbázisáról A WSUS 3.0 SP2 telepítője az alapértelmezett *meghajtó*\\WSUS mappába helyezi az adatbázist (ahol *meghajtó* a legtöbb szabad lemezterülettel rendelkező helyi NTFS-meghajtó). Ha a könyvtár már tartalmaz biztonsági másolatot, előfordulhat, hogy felül lesz írva. A WSUS aktuális verziójának adatbázisáról készült biztonsági másolatokat ajánlott áthelyezni egy másik mappába, mielőtt a WSUS 3.0 SP2 verzióra frissítene.

4.  Ha manuálisan (nem a Wsusutil segédprogrammal) módosította a WSUS által használt portot, és jelenleg a Software Update Services 1.0-s vagy WSUS 2.0-s verzióját használja, indítsa el az alapértelmezett webhelyet a SUS 1.0, illetve a WSUS 2.0 64 bites verziójának eltávolítása előtt.

5.  Élő WSUS-adatbáziskapcsolatok esetén (például ha az SQL Server Management Studio meg van nyitva) előfordulhat, hogy a telepítés sikertelen lesz. A WSUS 3.0 SP2 telepítése előtt zárja be az összes kapcsolatot.

### Sikertelen frissítés javítása

Ha a WSUS egy korábbi verziójáról frissít a WSUS 3.0 SP2 szolgáltatásra, és a frissítés bármilyen okból kifolyólag sikertelen (de nem azért, mert a SUS 1.0-ról próbál frissíteni, ami nem támogatott), tegye a következőket.

1.  Telepítse újra a WSUS korábbi verzióját.
2.  Állítsa helyre az adatbázist a frissítés előtt készített biztonsági másolatból. A frissítés nem fejezhető be sikeresen, ha van korábbi telepítésből származó, meglévő WSUS 3.0 SP2 adatbázis. A legtöbb esetben a WSUS szolgáltatás automatikusan biztonsági másolatot is készít. Ennek helye a WSUSSetup.log fájlból deríthető ki.
3.  Tekintse meg a naplófájlokat a hiba okának kiderítése érdekében, és oldja meg a problémát.
4.  Telepítse a WSUS 3.0 SP2 szolgáltatást

### A számítógép nevének a WSUS 3.0 SP2 verziójára való frissítés előtti módosítása azt eredményezi, hogy sikertelen lesz a frissítés

Ha módosítja a számítógép nevét a WSUS 2.0 telepítése és a WSUS 3.0 SP2 verzióra történő frissítés között, az a frissítés sikertelenségéhez vezethet.

Távolítsa el, majd adja újra hozzá az ASPNET és a WSUS-rendszergazdák csoportot. Ezután futtassa a frissítést.

        ```

### Ha az MSDE adatbázis-kezelőről áttért az SQL Server 2008 vagy az SQL Server 2005 használatára a WSUS 2.0-s verziójában, módosítania kell egy beállításazonosító értékét

Ha telepített WSUS 2.0 szolgáltatással rendelkezik, és az SQL Server 2008 vagy az SQL Server 2005 használatára tért át, 1-ről 0-ra kell módosítania a **HKLM\\SOFTWARE\\Microsoft\\Update Services\\Server\\Setup\\WmsdeInstalled** beállításazonosító értékét. Ha nem teszi meg ezt, mielőtt frissítene a WSUS 3.0 SP2 verziójára, a frissítés sikertelen lesz.

### Ha eltávolítja a WSUS 3.0 SP2 szolgáltatást, de meghagyja a naplófájlokat, lehet, hogy helytelenek lesznek az engedélyeik az esetleges újratelepítés után

A WSUS 3.0 SP2 eltávolítása során megőrizheti a telepítési naplófájlokat. A WSUS 3.0 SP2 újratelepítésekor elveszhetnek a régi naplófájlokra vonatkozó engedélyek (általában csak a WSUS-rendszergazdák engedélyei). Ajánlott a naplófájlok engedélyeit a telepítést követően ellenőrizni.

### A WSUS 2.0 rendszerű ügyfelek „Nem vonatkozik rá” állapotú frissítései a WSUS 3.0 SP2 verzióra való frissítést követően rövid ideig „Ismeretlen” állapotúként jelennek meg

A WSUS 2.0 rendszerű ügyfelek **Nem vonatkozik rá** állapotú frissítései a WSUS 3.0 SP2 verzióra való frissítést követően rövid ideig **Ismeretlen** állapotúként jelenhetnek meg. A legközelebbi keresést követően a frissítés állapota ismét **Nem vonatkozik rá** lesz.

A WSUS 3.0 SP2 telepítése
-------------------------

A WSUS 3.0 SP2 rendszer Windows Kiszolgálókezelővel vagy WUSSetup.exe programmal végzett telepítésének menetét részletesen ismerteti a WSUS lépésenkénti telepítési útmutatója a [http://go.microsoft.com/fwlink/?LinkId=139836](http://go.microsoft.com/fwlink/?linkid=139836) című weblapon.

A WSUS 3.0 szolgáltatás telepítéséről és használatáról a következő forrásokból tájékozódhat bővebben:

A WSUS központi telepítési útmutatója a [http://go.microsoft.com/fwlink/?LinkId=139832](http://go.microsoft.com/fwlink/?linkid=139832) webhelyen

A WSUS használati útmutatója a [http://go.microsoft.com/fwlink/?LinkId=139838](http://go.microsoft.com/fwlink/?linkid=139838) webhelyen

A telepítő parancssori paraméterei a WSUS 3.0 SP2 felügyelet nélküli telepítéséhez
----------------------------------------------------------------------------------

A WSUS 3.0 SP2 telepítését felügyelet nélküli üzemmódban is elvégezheti a WSUS parancssori telepítőprogramjával. A táblázat a WSUS 3.0 SP2 parancssori telepítőjének paramétereit tartalmazza.

###  

 
<table style="border:1px solid black;">
<colgroup>
<col width="50%" />
<col width="50%" />
</colgroup>
<thead>
<tr class="header">
<th style="border:1px solid black;" >Kapcsoló</th>
<th style="border:1px solid black;" >Leírás</th>
</tr>
</thead>
<tbody>
<tr class="odd">
<td style="border:1px solid black;"><strong>/q</strong></td>
<td style="border:1px solid black;">Csendes telepítés.</td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><strong>/u</strong></td>
<td style="border:1px solid black;">Eltávolítás.</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><strong>/p</strong></td>
<td style="border:1px solid black;">Előfeltételek ellenőrzése. A rendszer vizsgálata és a hiányzó előfeltételek jelentése.</td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><strong>/?, /h</strong></td>
<td style="border:1px solid black;">A parancssori paraméterek és leírások megjelenítése.</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><strong>/g</strong></td>
<td style="border:1px solid black;">Frissítés a WSUS korábbi verziójáról. (Az SUS 1.0 frissítése nem támogatott.) Ezzel a kapcsolóval csak a /q (csendes telepítés) kapcsoló használható együtt. A kapcsoló egyetlen érvényes tulajdonsága a DEFAULT_WEBSITE.</td>
</tr>
</tbody>
</table>
  
A táblázat a WSUS 3.0 SP2 parancssori tulajdonságait tartalmazza.
  
###  

 
<table style="border:1px solid black;">
<colgroup>
<col width="50%" />
<col width="50%" />
</colgroup>
<thead>
<tr class="header">
<th style="border:1px solid black;" >Tulajdonság</th>
<th style="border:1px solid black;" >Leírás</th>
</tr>
</thead>
<tbody>
<tr class="odd">
<td style="border:1px solid black;">CONTENT_LOCAL</td>
<td style="border:1px solid black;">0=a tartalom helyben van tárolva, 1=tárolás a Microsoft Update webhelyen</td>
</tr>
<tr class="even">
<td style="border:1px solid black;">CONTENT_DIR</td>
<td style="border:1px solid black;">A tartalomkönyvtár elérési útja. Az alapértelmezett érték a <em>WSUS_telepítési_meghajtó\WSUS\WSUSContent</em>, ahol a <em>WSUS_telepítési_meghajtó</em> a legtöbb szabad lemezterülettel rendelkező helyi meghajtó.</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;">WYUKON_DATA_DIR</td>
<td style="border:1px solid black;">A belső Windows-adatbázis adatkönyvtárának elérési útja.</td>
</tr>
<tr class="even">
<td style="border:1px solid black;">SQLINSTANCE_NAME</td>
<td style="border:1px solid black;">A nevet a <em>Kiszolgálónév</em>\<em>SQL_példány_neve</em> formátumban kell megadni. Ha az adatbázispéldány a helyi gépen található, használja a %COMPUTERNAME% környezeti változót. Ha nincs jelen egy már létező példány, akkor a %COMPUTERNAME%\WSUS az alapértelmezés.</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;">DEFAULT_WEBSITE</td>
<td style="border:1px solid black;">1=80-as port, 0=8530-as port</td>
</tr>
<tr class="even">
<td style="border:1px solid black;">PREREQ_CHECK_LOG</td>
<td style="border:1px solid black;">A naplófájl elérési útja és neve</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;">CONSOLE_INSTALL</td>
<td style="border:1px solid black;">0=a WSUS-kiszolgáló telepítése, 1=csak a konzol telepítése</td>
</tr>
<tr class="even">
<td style="border:1px solid black;">ENABLE_INVENTORY</td>
<td style="border:1px solid black;">0=nem telepíti a leltárszolgáltatásokat, 1=telepíti a leltárszolgáltatásokat</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;">DELETE_DATABASE</td>
<td style="border:1px solid black;">0=az adatbázis megőrzése, 1=az adatbázis eltávolítása</td>
</tr>
<tr class="even">
<td style="border:1px solid black;">DELETE_CONTENT</td>
<td style="border:1px solid black;">0=a tartalomfájlok megőrzése, 1=a tartalomfájlok eltávolítása</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;">DELETE_LOGS</td>
<td style="border:1px solid black;">0=naplófájlok megőrzése, 1=naplófájlok eltávolítása (a /u kapcsolóval használva)</td>
</tr>
<tr class="even">
<td style="border:1px solid black;">CREATE_DATABASE</td>
<td style="border:1px solid black;">0=a jelenlegi adatbázis használata, 1=adatbázis létrehozása</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;">PROGRESS_WINDOW_HANDLE</td>
<td style="border:1px solid black;">A Windows Installer állapotüzeneteinek visszaadására szolgáló ablakleíró</td>
</tr>
<tr class="even">
<td style="border:1px solid black;">MU_ROLLUP</td>
<td style="border:1px solid black;">1=részvétel a Microsoft Update szolgáltatásainak javítását célzó programban, 0=a a Microsoft Update szolgáltatásainak javítását célzó programban való részvétel mellőzése</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;">FRONTEND_SETUP</td>
<td style="border:1px solid black;">1=ne írja a tartalom helyét az adatbázisba, 0=írja be a tartalom helyét az adatbázisba (hálózati terheléselosztáshoz)</td>
</tr>
</tbody>
</table>
  
### Példa
  
```  
WSUSSetup.exe /q DEFAULT\_WEBSITE=0 (telepítés csendes üzemmódban a 8530-as porton) WSUSSetup.exe /q /u (a WSUS eltávolítása)  
```
 
<table style="border:1px solid black;">
<colgroup>
<col width="100%" />
</colgroup>
<thead>
<tr class="header">
<th style="border:1px solid black;" ><img src="images/Dd939886.Important(WS.10).gif" />Fontos</th>
</tr>
</thead>
<tbody>
<tr class="odd">
<td style="border:1px solid black;">Ha csendes üzemmódban (/q) telepíti a WSUS 3.0 SP2 szolgáltatást, és a gépre nincs telepítve minden előfeltétel, a telepítő létrehoz egy WSUSPreReqCheck.xml nevű fájlt, amelyet a %TEMP% könyvtárban helyez el.
</td>
</tr>
</tbody>
</table>
 

<span id="BKMK_KnownIssues"></span>
Ismert problémák
----------------

-   A WSUS telepítésének sikeres befejezését követően a telepítő megkéri a felhasználót, hogy kattintson a **Befejezés** gombra. Ritkán, de megjelenhet egy üzenet a következő szöveggel: **Hiba történt a kiszolgálóval való kommunikáció közben, ezért a varázslót be kell zárni. A WSUS 3.0 konzoljának Beállítások lapjáról indíthatja újra a WSUS-kiszolgáló konfigurálása varázslót.** Ha szeretne meggyőződni róla, hogy a telepítés során megadott beállítások megőrződtek, nyissa meg a WSUS felügyeleti konzoljának **Beállítások** lapját, és ellenőrizze őket.
-   **A Windows Update Agent (WUA) honosított ügyfelei a WSUS 3.0 SP2 megjelenésénél később jelennek meg.** Ezt a Windows 7 honosítási ütemterve indokolja. A WSUS 3.0 SP2 és a honosított WUA ügyfelek megjelenése közötti időszakban a WUA ügyfél csak öt nyelvet támogat (angol, német, francia, spanyol és japán).
-   **Az SP2 kiadásban megjelenő frissítési és számítógépállapot-jelentések nem működnek olyan környezetekben, melyekben a WSUS 3.0 SP2 kiszolgálók alsóbb rétegbeli WSUS 3.0 SP1 kiszolgálókat kezelnek.** Ha egy SP1 rendszerű kiszolgálón próbálkozik a jelentéskészítéssel, a következő hibaüzenet jelenik meg: „Hiba történt a jelentés generálása közben. Próbálja meg újra futtatni a jelentést, vagy ha tartós a probléma, forduljon a hálózati rendszergazdához.” A jelentés ismételt futtatásával nem oldódik meg a probléma, és az nem is hálózati jellegű. Az új jelentések által használt alkalmazásprogramozási felület az SP1 verziónak nem része, azonban az SP2 felügyeleti konzolja nem akadályozza meg az új jelentési funkciók használatát az SP1 verziójú kiszolgálók kezelése során.
-   **Ha tanúsítványnév nélkül van beállítva az SSL protokoll, a WSUS 3.0 SP2 verzióra való frissítés sikertelen lesz.** Az SSL konfigurálása során meg kell határozni egy tanúsítványnevet.
-   **Ha a WSUS 3.0 SP2 Belső Windows-adatbázis használatára van beállítva egy Windows Server 2008 rendszeren, az operációs rendszer nem frissíthető Windows Server 2008 R2 rendszerre.** A Windows Server 2008 R2 rendszerre való frissítés előtt a kompatibilitást taglaló jelentés hibaüzenetet tartalmazhat, mely a Belső Windows-adatbázis kikapcsolására kéri. A Belső Windows-adatbázis frissítése nem hagyható ki a Windows Server 2008 R2 rendszerre való frissítés előtt. A Belső Windows-adatbázis frissítésével kapcsolatban további információt és útmutatást talál a Tudásbázis [A Belső Windows-adatbázis legújabb szervizcsomagjának beszerzése](http://go.microsoft.com/fwlink/?linkid=162104) (http://go.microsoft.com/fwlink/?LinkId=162104) című cikkében.

Szerzői jogi információk
------------------------

A jelen dokumentumban található adatok, az URL-címeket és más internetes weblapokra mutató hivatkozásokat is beleértve, előzetes bejelentés nélkül megváltozhatnak. A dokumentum példáiban szereplő vállalatok, szervezetek, termékek, tartománynevek, e-mail címek, emblémák, személyek, helyek és események a képzelet szüleményei. Az ettől eltérő eseteket külön jelezzük. A valódi vállalatokkal, szervezetekkel, termékekkel, tartományokkal, e-mail címekkel, emblémákkal, személyekkel, helyekkel vagy eseményekkel fennálló hasonlóság a véletlen műve. Az összes vonatkozó szerzői jogi rendelkezés és törvény betartása a felhasználó felelőssége. A bejegyzett szerzői jogok korlátozásait figyelembe véve a Microsoft Corporation kifejezett írásbeli engedélye nélkül a dokumentum egyetlen része sem másolható, nem rögzíthető és nem tárolható visszakereshető rendszerben. Továbbítása semmiféle formában és semmilyen módon (elektronikus, mechanikai, fénymásolás, hangrögzítési vagy más eljárással) vagy célból nem engedélyezett.

A Microsoft olyan szabadalmakkal, szabadalmaztatott alkalmazásokkal, védjegyekkel, szerzői jogokkal vagy egyéb szellemi tulajdonjogokkal rendelkezhet, amelyek benne foglaltatnak e dokumentumban. Hacsak a Microsoft valamelyik írásos licencszerződése másként nem rendelkezik, a jelen dokumentum rendelkezésre bocsátása nem jogosítja fel a felhasználót ezen szabadalmak, védjegyek, szerzői jogok vagy egyéb szellemi tulajdon használatára.

© 2009 Microsoft Corporation. Minden jog fenntartva.

A Microsoft, az Active Directory, az ActiveX, az Authenticode, az Excel, az InfoPath, az Internet Explorer, az MSDN, az Outlook, a Visual Studio, a Win32, a Windows, a Windows Server és a Windows Vista a Microsoft cégcsoport védjegye.

Minden egyéb kereskedelmi védjegy a tulajdonosa védjegye.
