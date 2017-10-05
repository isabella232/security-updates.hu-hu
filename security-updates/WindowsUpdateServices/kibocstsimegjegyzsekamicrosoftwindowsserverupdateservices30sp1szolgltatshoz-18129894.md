---
TOCTitle: 'Kibocsátási megjegyzések a Microsoft Windows Server Update Services 3.0 SP1 szolgáltatáshoz'
Title: 'Kibocsátási megjegyzések a Microsoft Windows Server Update Services 3.0 SP1 szolgáltatáshoz'
ms:assetid: 'a5aa93bf-842b-4ad4-ab0f-fe867843cb02'
ms:contentKeyID: 18129894
ms:mtpsurl: 'https://technet.microsoft.com/hu-hu/library/Cc708525(v=WS.10)'
---

Kibocsátási megjegyzések a Microsoft Windows Server Update Services 3.0 SP1 szolgáltatáshoz
===========================================================================================

Jelen kibocsátási megjegyzések a Microsoft® Windows® Server Update Services (WSUS) 3.0 Service Pack 1 szolgáltatással kapcsolatos ismert problémákat, valamint a szolgáltatás telepítésére vonatkozó javaslatokat, illetve követelményeket tartalmaznak. A dokumentum a következő részekből áll:

-   A WSUS 3.0 SP1 kiszolgálótelepítésének rendszerkövetelményei
-   A WSUS 3.0 SP1 kiszolgálótelepítésének konfigurációs követelményei
-   A WSUS 3.0 SP1-alapú távoli konzolok telepítésének rendszerkövetelményei
-   Az ügyféltelepítés rendszerkövetelményei
-   A WSUS SP1 kiszolgálótelepítésének szoftverkövetelményei
-   A WSUS 3.0 SP1 kiszolgálótelepítésének minimális lemezterület-igénye
-   A WSUS 3.0 SP1 frissítési követelményei
-   A telepítés parancssori paraméterei
-   Telepítési problémák
-   Frissítési problémák
-   Ismert problémák
-   A WSUS 3.0 SP1 szolgáltatás Windows Server® 2008 rendszeren
-   A WSUS 3.0 SP1 szolgáltatás Windows Small Business Server 2003 rendszeren

A WSUS 3.0 SP1 kiszolgálótelepítésének rendszerkövetelményei
------------------------------------------------------------

#### A WSUS 3.0 SP1 kiszolgálószolgáltatás Windows Server 2008 és Windows Server 2003 Service Pack 1 rendszereken támogatott

A WSUS 3.0 SP1 kiszolgálószolgáltatás Windows Server 2008 és Windows Server 2003 Service Pack 1 rendszereken támogatott.

#### A Windows 2000 Server rendszert a WSUS 3.0 SP1 kiszolgálószolgáltatás nem támogatja

WSUS 3.0 SP1 kiszolgálókon a Microsoft Windows® 2000 operációs rendszer nem támogatott.

#### A WSUS 3.0 SP1 használata terminálszolgáltatásokat futtató kiszolgálókon nem támogatott

Bár a WSUS 3.0 SP1 szolgáltatás megfelelően működhet terminálszolgáltatásokat futtató kiszolgálókon is, ez nem támogatott vagy javasolt. A WSUS 3.0 SP1 nem működik terminálszolgáltatásokat futtató, távoli SQL-kiszolgálókat használó konfigurációkban. Mivel a terminálszolgáltatások licenckiszolgálóján minden egyedi művelet (köztük a telepítés is) a rendszerfiókban történik, és előfordulhat, hogy a rendszerfiók nem rendelkezik megfelelő engedélyekkel a távoli SQL-kiszolgálóhoz, a telepítés sikertelen lehet.

A WSUS 3.0 SP1 kiszolgálótelepítésének konfigurációs követelményei
------------------------------------------------------------------

#### Telepíteni kell az IIS szolgáltatást

A WSUS 3.0 SP1 használatához telepíteni kell az Internet Information Services (IIS) szolgáltatást, amely a Windows Server 2008 és a Microsoft Windows Server 2003 operációs rendszeren nem található meg alapértelmezés szerint. Ha a WSUS 3.0 SP1 szolgáltatást IIS nélkül telepíti, a Windows Server Update Services telepítője az IIS telepítésének hiányára figyelmeztető hibaüzenetet jelenít meg.

#### Az IIS szolgáltatásnak az IIS 5.0 elkülönítési üzemmódjában történő futtatásakor a telepítés meghiúsul

Ha a kiszolgálót Windows 2000 Server operációs rendszerről frissíti Windows Server 2003 rendszerre, előfordulhat, hogy az ISS szolgáltatás az IIS 5.0 elkülönítési üzemmódjában fut. Az IIS 5.0 elkülönítési módja az IIS-kezelőben is engedélyezhető. Az IIS 5.0 elkülönítési módjában azonban a telepítés meghiúsul, ezért a WSUS 3.0 SP1 telepítése előtt le kell ezt a módot tiltania.

#### Az IIS-összetevők 32 bites kompatibilitási módban történő telepítésekor a 64 bites platformokon a WSUS 3.0 SP1 telepítése meghiúsulhat

64 bites platformokon minden IIS-összetevőt natív módban kell telepítenie. Ha bármelyik IIS-összetevő 32 bites kompatibilitási módban van, a telepítés meghiúsulhat.

#### A proxykiszolgálók támogathatják kizárólag a HTTP protokollt, vagy a HTTP és a HTTPS protokollt együttesen is

A WSUS 3.0 SP1 szolgáltatásban lehetőség van arra, hogy a proxykiszolgálók csak a HTTP protokollt támogassák. A WSUS-kiszolgáló konfigurációs varázslóból vagy felügyeleti konzolból történő telepítése előtt a parancssorból (a **wsusutil configuresslproxy** parancs használatával) konfigurálnia kell egy HTTPS protokollt használó második proxykiszolgálót.

#### Ha a 80-as portot kettőnél több webhely használja, a WSUS telepítése előtt egy kivételével az összes webhelyet törölni kell

Ha a 80-as proton keresztül kettőnél több webhely kommunikál (például a Windows® SharePoint® Services), egy kivételével az összeset törölnie kell a WSUS telepítése előtt. Ha ezt nem teszi meg, a kiszolgáló ügyfeleinél sikeretlen lehet az önfrissítés.

#### A WSUS 3.0 SP1 telepítése előtt előfordulhat, hogy le kell tiltani a víruskereső programokat

A WSUS 3.0 SP1 megfelelő telepítése érdekében előfordulhat, hogy előtte le kell tiltania a víruskereső programokat. Miután letiltotta a programokat, a WSUS telepítése előtt indítsa újra a számítógépet. Ezzel megakadályozhatja, hogy a programok zárolják a fájlokat, amikor a telepítő hozzájuk szeretne férni. Telepítés után ne felejtse el újra engedélyezni a víruskereső programokat. A víruskereső programok engedélyezésének és letiltásának pontos lépéseiről az adott program gyártójának webhelyén tájékozódhat.

| ![](images/Cc708525.Caution(WS.10).gif)Figyelmeztetés:                                                                                                                                                                                                                                                             |
|-------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| Ez a kerülő megoldás a számítógépet vagy a hálózatot sebezhetőbbé teheti a támadó szándékú felhasználókkal és szoftverekkel – például vírusokkal – szemben. Az eljárás végrehajtása ugyan nem javasolt, de az információt rendelkezésére bocsátjuk, hogy belátása szerint dönthessen. A kerülő megoldást csak saját felelősségére használhatja. |

| ![](images/Cc708525.note(WS.10).gif)Megjegyzés:                                                                                                                                                                                                             |
|------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| A víruskereső programok feladata a számítógép vírusok elleni védelme. Ha a víruskereső program le van tiltva, akkor nem szabad letölteni vagy megnyitni nem biztonságos forrásból származó fájlokat, felkeresni nem biztonságos webhelyeket, illetve megnyitni az e-mailek mellékleteit. |

#### A WSUS 3.0 SP1 futtatásához az SQL Server alkalmazásban engedélyezni kell a beágyazott triggerek használatát

A beágyazott triggerek használatának engedélyezése alapértelmezés szerint be van ugyan kapcsolva, de az SQL Server rendszergazdája kikapcsolhatja.

Ha a Windows Server Update Services adattárolójaként egy SQL Server-alapú adatbázist szeretne használni, az SQL Server rendszergazdájának ellenőriznie kell, hogy a beágyazott triggerek engedélyezettek-e a kiszolgálón. A WSUS 3.0 SP1 rendszergazdája csak ezután telepítheti a WSUS 3.0 SP1 szolgáltatást, és adhatja meg a telepítés folyamán a használni kívánt adatbázist.

A WSUS 3.0 SP1 telepítő engedélyezi a RECURSIVE\_TRIGGERS adatbázis-specifikus beállítást, az egész kiszolgálóra érvényes, beágyazott triggerekre vonatkozó beállítást azonban nem kapcsolja be.

Annak ellenőrzésére, hogy a beágyazott triggerek engedélyezettek-e, futtassa az alábbi parancsot:

**sp\_configure 'nested triggers'**

A beágyazott triggerekre vonatkozó beállítás engedélyezéséhez kötegfájlból futtassa az alábbi parancsokat az SQL Server alkalmazást működtető számítógépen:

**sp\_configure 'nested triggers', 1**

**GO**

**RECONFIGURE**

**GO**

Ha a kiszolgálón nincs telepítve az SQL Server Management Studio, az SQL-parancsokat parancssorból is futtathatja. A Microsoft SQL Server 2005 parancssori lekérdezőeszköze a [Microsoft letöltőközpontjából](http://go.microsoft.com/fwlink/?linkid=70728), a http://go.microsoft.com/fwlink/?LinkId=70728 címen szerezhető be. (Előfordulhat, hogy a lap angol nyelven jelenik meg.) A kezdéshez futtassa az **sqlcmd parancsot**.

Ha az SQL-parancsfájlokat a Belső Windows-adatbázis lekérdezésével szeretné futtatni, a fenti webhelyről le kell töltenie az SQL Server Native Client alkalmazást is.

#### A távoli SQL korlátozásai és követelményei

A WSUS 3.0 SP1 támogatja azon adatbázisszoftverek használatát, amelyek nem a WSUS 3.0 SP1 szolgáltatás többi részét futtató számítógépeken működnek. A távoli SQL-telepítés néhány konfigurációs követelménye:

-   Távoli SQL használata esetén a tartományvezérlőként beállított kiszolgálók nem alkalmazhatók háttérszámítógépként.
-   Távoli SQL használata esetén az előtér-kiszolgáló nem lehet terminálkiszolgáló.
-   Ha a háttérkiszolgálón Windows Server 2003 rendszer fut, adatbázis-kezelőként legalább a Microsoft SQL Server 2005 Service Pack 1 alkalmazást kell használni, amely a [Microsoft letöltőközpontjából](http://go.microsoft.com/fwlink/?linkid=66143), a http://go.microsoft.com/fwlink/?LinkId=66143 címen szerezhető be. (Előfordulhat, hogy a lap angol nyelven jelenik meg.). Ha a háttérkiszolgálón Windows Server® 2008 rendszer található, akkor az SQL Server 2005 Service Pack 2 alkalmazást kell használni.
-   Az előtér- és a háttérkiszolgálónak is Active Directory-tartományhoz kell csatlakoznia, mert ha a kiszolgálók különböző tartományokban találhatók, a WSUS telepítése előtt a tartományok között megbízhatósági kapcsolatot kell létrehoznia.
-   Ha a távoli SQL-konfigurációban már telepítve van a WSUS 2.0-s változata, és frissíteni szeretne a WSUS 3.0 SP1 változatra, a Vezérlőpult **Programok telepítése és törlése** funkciójával a háttérszámítógépről előbb el kell távolítania a 2.0-s változatot a meglévő adatbázis érintetlenül hagyásával. Ezután telepítenie kell az SQL Server 2005 SP1 vagy SP2 alkalmazást, majd frissítenie kell a meglévő adatbázist. Végül az előtér-számítógépre telepítenie kell a WSUS 3.0 SP1 szolgáltatást.

A WSUS 3.0 SP1-alapú távoli konzolok telepítésének rendszerkövetelményei
------------------------------------------------------------------------

A WSUS 3.0 SP1 távoli konzol a következő platformokon telepíthető:

-   Windows Server 2008
-   Windows Vista® vagy egy későbbi változat
-   Windows Server 2003 SP1 vagy egy későbbi változat
-   Windows XP SP2 vagy egy későbbi változat

Az ügyféltelepítés rendszerkövetelményei
----------------------------------------

Az automatikus frissítési szolgáltatás a WSUS ügyfélszoftvere. A WSUS szolgáltatással együtt a következő operációs rendszerek bármelyikén használható:

-   Windows Vista vagy egy későbbi változat
-   Windows Server 2008 vagy egy későbbi változat
-   Microsoft® Windows Server 2003, bármelyik kiadás
-   Microsoft Windows XP Professional SP2 vagy egy későbbi változat
-   Microsoft Windows 2000 Professional SP4, Windows 2000 Server SP4 vagy Windows 2000 Advanced Server SP4

A WSUS 3.0 SP1 kiszolgálótelepítésének szoftverkövetelményei
------------------------------------------------------------

Az alábbi táblázat a Windows Server 2003 SP1-platformok szoftverkövetelményeit tartalmazza. A Windows Server 2008 szoftverkövetelményeiről a Windows Server 2008 rendszeren futtatott WSUS 3.0 SP1 szolgáltatással foglalkozó részben tájékozódhat.

A WSUS 3.0 SP1 telepítő futtatása előtt ellenőrizze, hogy a rendszer megfelel-e ezen szoftverkövetelményeknek. Ha az itt említett frissítések bármelyike a számítógép újraindítását kéri a telepítés befejezését követően, akkor az újraindítást a WSUS 3.0 SP1 szolgáltatás telepítése előtt kell végrehajtani.

###  

 
<table style="border:1px solid black;">
<colgroup>
<col width="50%" />
<col width="50%" />
</colgroup>
<thead>
<tr class="header">
<th style="border:1px solid black;" >Követelmény</th>
<th style="border:1px solid black;" >Ismertetés</th>
</tr>
</thead>
<tbody>
<tr class="odd">
<td style="border:1px solid black;">Microsoft Internet Information Services (IIS)</td>
<td style="border:1px solid black;">Az operációs rendszerből telepíthető.</td>
</tr>
<tr class="even">
<td style="border:1px solid black;">Újraterjeszthető csomag a Microsoft® .NET-keretrendszer 2.0-s verziójához</td>
<td style="border:1px solid black;">Erről bővebben a Microsoft® .NET-keretrendszer 2.0-s verziójának x68 típusú újraterjeszhető csomagjával foglalkozó dokumentumban, a <a href="http://go.microsoft.com/fwlink/?linkid=68935">Microsoft letöltőközpontjában</a>, a http://go.microsoft.com/fwlink/?LinkId=68935 címen tájékozódhat. 64 bites platform esetén olvassa el a Microsoft® .NET-keretrendszer 2.0-s verziójának x64 típusú újraterjeszhető csomagjával foglalkozó dokumentumot, a <a href="http://go.microsoft.com/fwlink/?linkid=70637">Microsoft letöltőközpontjában</a>, a http://go.microsoft.com/fwlink/?LinkId=70637 címen. (Előfordulhat, hogy a lap angol nyelven jelenik meg.)</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;">Microsoft Management Console 3.0 Windows Server 2003 rendszerhez</td>
<td style="border:1px solid black;">A WSUS 3.0 SP1 felhasználói felület használatához ez előfeltétel. Erről bővebben a Windows Server 2003 rendszerhez készült Microsoft Management Console 3.0 alkalmazással (KB907265) foglalkozó dokumentumban, a <a href="http://go.microsoft.com/fwlink/?linkid=70412">Microsoft letöltőközpontjában</a>, a http://go.microsoft.com/fwlink/?LinkId=70412 címen tájékozódhat. 64 bites platform esetén olvassa el a Windows Server 2003 x64 kiadásához készült Microsoft Management Console 3.0 alkalmazással (KB907265) foglalkozó dokumentumot a <a href="http://go.microsoft.com/fwlink/?linkid=70638">Microsoft letöltőközpontjában</a>, a http://go.microsoft.com/fwlink/?LinkId=70638 címen. (Előfordulhat, hogy a lap angol nyelven jelenik meg.)</td>
</tr>
<tr class="even">
<td style="border:1px solid black;">Microsoft jelentésmegtekintő</td>
<td style="border:1px solid black;">A WSUS 3.0 SP1 felhasználói felület használatához ez előfeltétel. Erről bővebben a Microsoft jelentésmegtekintő újraterjeszhető csomagjának 2005-ös verziójával foglalkozó dokumentumban, a <a href="http://go.microsoft.com/fwlink/?linkid=70410">Microsoft letöltőközpontjában</a>, a http://go.microsoft.com/fwlink/?LinkId=70410 címen tájékozódhat. (Előfordulhat, hogy a lap angol nyelven jelenik meg.)</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;">SQL Server 2005 (választható)</td>
<td style="border:1px solid black;">A WSUS 3.0 SP1 csomaggal együtt a Belső Windows-adatbázis is települni fog, hacsak az SQL Server egy kompatibilis példánya nincs már telepítve. Ha egy teljes SQL Server adatbázist szeretne használni, akkor Windows Server 2003 rendszer esetén (legalább) SQL Server 2005 SP1 csomagra lesz szüksége, amely a <a href="http://go.microsoft.com/fwlink/?linkid=66143">Microsoft letöltőközpontjából</a>, a http://go.microsoft.com/fwlink/?LinkId=66143 címről tölthető le. (Előfordulhat, hogy a lap angol nyelven jelenik meg.) Választhatja az Windows Server 2008 SQL Server 2005 SP2 csomagot is, amely szintén a <a href="http://go.microsoft.com/fwlink/?linkid=84823">Microsoft letöltőközpontjából</a>, a http://go.microsoft.com/fwlink/?LinkId=84823 címről tölthető le. (Előfordulhat, hogy a lap angol nyelven jelenik meg.)</td>
</tr>
</tbody>
</table>
  
| ![](images/Cc708525.note(WS.10).gif)Megjegyzés:                                                                                                                                                                                                                                                                                                                       |  
|----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|  
| Ha a WSUS 2.0 szolgáltatást már korábban telepítette, és SQL Server 2000, SQL Server Desktop Engine 2000 vagy bármilyen, az SQL Server 2005 SP1 szolgáltatásnál (illetve Windows Server 2008 rendszeren az SQL Server 2005 SP2 szolgáltatásnál) régebbi SQL Server-adatbázist használ, a WSUS 3.0 SP1 telepítésekor a Windows® Internal Database is települ, és a meglévő adatbázis is abba kerül. |
  
A WSUS 3.0 SP1 kiszolgálótelepítésének minimális lemezterület-igénye  
--------------------------------------------------------------------
  
A Windows Server Update Services telepítéséhez legalább az alábbi nagyságú szabad lemezterületre van szükség:
  
-   1 GB a rendszerpartíción  
-   2 GB az adatbázisfájlok majdani tárolására szolgáló köteten  
-   20 GB a tartalom tárolására szolgáló köteten
  
| ![](images/Cc708525.Important(WS.10).gif)Fontos:                                          |  
|------------------------------------------------------------------------------------------------------------------------|  
| A WSUS 3.0 SP1 nem telepíthető tömörített meghajtókra. Győződjön meg arról, hogy a választott meghajtó nem tömörített. |
  
A WSUS 3.0 SP1 frissítési követelményei  
---------------------------------------
  
#### Meg kell győződni arról, hogy a telepített WSUS megfelelően működik, és frissítés előtt biztonsági másolatot kell készíteni a WSUS-adatbázisról
  
Ha egy korábbi verzióról frissít a WSUS 3.0 SP1 szolgáltatásra, győződjön meg arról, hogy az aktuálisan telepített verzió megfelelően működik, és frissítés előtt készítsen biztonsági másolatot a WSUS-adatbázisról.
  
1.  Ellenőrizze az eseménynaplókban a legutóbbi hibákat, az alsóbb és a felsőbb szintű kiszolgálók közötti esetleges szinkronizálási problémákat vagy a jelentést nem készítő ügyfelekkel kapcsolatos esetleges hibákat. Folytatás előtt hárítson el minden hibát.  
2.  Előfordulhat, hogy szüksége lesz a DBCC CHECKDB futtatására a WSUS-adatbázis megfelelő indexeléséhez. A DBCC CHECKDB eszközről a [Microsoft Windows Update webhelyen](http://go.microsoft.com/fwlink/?linkid=86948), a http://go.microsoft.com/fwlink/?LinkId=86948 címen tájékozódhat. (Előfordulhat, hogy a lap angol nyelven jelenik meg.)  
3.  A WSUS-adatbázisról készítsen biztonsági másolatot.
  
#### Ha a WSUS által használt port kézzel lett módosítva, a frissítés előtt el kell távolítani
  
A WSUS portjának módosításkor a port kézzel történő megváltoztatása helyett használja mindig a wsusutil eszközt. Ha kézzel módosította a portot, és korábban frissített a Software Update Services 1.0 szolgáltatásról a WSUS 2.0 szolgáltatásra, tegye a következőket:
  
1.  Ha még nem telepítette a WSUS 3.0 szolgáltatást, távolítsa el a WSUS 2.0-s változatát az adatbázis és a tartalom megőrzése mellett. (Ha már telepítette a WSUS 3.0 szolgáltatást, távolítsa el azt az adatbázis és a tartalom megőrzése mellett.)  
2.  Indítsa el az alapértelmezett webhelyet, ideiglenesen engedélyezze újra az SUS 1.0 szolgáltatást, és ne engedje, hogy az eltávolítóprogram hozzáférjen.  
3.  Távolítsa el az SUS 1.0 szolgáltatást.  
4.  Telepítse a WSUS 3.0 szolgáltatást.
  
#### El kell távolítani a Software Update Services 1.0 szolgáltatást
  
A WSUS 3.0 SP1 telepítése meghiúsul, ha ugyanazon a számítógépen a Software Update Services 1.0 is telepítve van. A WSUS 3.0 SP1 telepítése előtt el kell távolítania a Software Update Services 1.0 szolgáltatást.
  
#### A WSUS 2.0 szolgáltatást 64 bites operációs rendszereken nem lehet a WSUS 3.0 SP1 szolgáltatásra frissíteni
  
A WSUS 2.0 64 bites operációs rendszereken nem támogatott, ezért az ilyen rendszereken a WSUS 2.0 szolgáltatást nem lehet a WSUS 3.0 SP1 szolgáltatásra frissíteni.
  
A telepítés parancssori paraméterei  
-----------------------------------
  
A WSUS parancssori telepítőprogramja segítségével a WSUS 3.0 SP1 szolgáltatást felügyelet nélkül is telepítheti. Az alábbi táblázat a WSUS 3.0 SP1 telepítésének parancssori paramétereit tartalmazza.
  
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
<td style="border:1px solid black;">Beavatkozás nélküli telepítés futtatása.</td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><strong>/u</strong></td>
<td style="border:1px solid black;">A termék eltávolítása. Ha telepítve van, ez a paraméter a Belső Windows-adatbázis példányát is eltávolítja.</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><strong>/p</strong></td>
<td style="border:1px solid black;">Csak az előfeltételek ellenőrzésének végrehajtása. Nem telepíti a terméket, de megvizsgálja a rendszert, és jelenti a hiányzó előfeltételeket.</td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><strong>/?, /h</strong></td>
<td style="border:1px solid black;">A parancssori paraméterek és leírásuk megjelenítése.</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><strong>/g</strong></td>
<td style="border:1px solid black;">Frissítés a WSUS korábbi verzióiról. (Ne frissítsen az SUS 1.0 szolgáltatásról.) Ehhez a kapcsolóhoz egyedül a /q paraméter (csendes telepítés) használható. A kapcsoló egyetlen érvényes tulajdonsága a DEFAULT_WEBSITE.</td>
</tr>
</tbody>
</table>
  
Az alábbi táblázat a WSUS 3.0 SP1 telepítésének parancssori tulajdonságait tartalmazza.
  
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
<td style="border:1px solid black;">0=a tartalom a helyi számítógépen található, 1=a tartalom a Microsoft Update webhelyen található</td>
</tr>
<tr class="even">
<td style="border:1px solid black;">CONTENT_DIR</td>
<td style="border:1px solid black;">A tartalom könyvtárának elérési útja. Az alapértelmezett elérési út a <em>WSUSTelepítésiMeghajtó</em><strong>\WSUS\WSUSContent</strong>, ahol a<em>WSUSTelepítésiMeghajtó</em> a legnagyobb szabad lemezterülettel rendelkező helyi meghajtó.</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;">WYUKON_DATA_DIR</td>
<td style="border:1px solid black;">A Belső Windows-adatbázis adatkönyvtárának elérési útja.</td>
</tr>
<tr class="even">
<td style="border:1px solid black;">SQLINSTANCE_NAME</td>
<td style="border:1px solid black;">A névnek a következő formátumúnak kell lennie: <em>Kiszolgálónév</em>\<em>SQL-példányNeve</em>. Ha az adatbázispéldány a helyi számítógépen található, használja a %COMPUTERNAME% környezeti változót. Ha a meglévő példány ott nem található, az alapértelmezett név a %COMPUTERNAME%\WSUS.</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;">DEFAULT_WEBSITE</td>
<td style="border:1px solid black;">0=8530-as port, 1=80-as port</td>
</tr>
<tr class="even">
<td style="border:1px solid black;">PREREQ_CHECK_LOG</td>
<td style="border:1px solid black;">A naplófájl elérési útja és neve.</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;">CONSOLE_INSTALL</td>
<td style="border:1px solid black;">0=a WSUS-kiszolgáló telepítése, 1=csak a konzol telepítése</td>
</tr>
<tr class="even">
<td style="border:1px solid black;">ENABLE_INVENTORY</td>
<td style="border:1px solid black;">0=a leltárszolgáltatások telepítésének mellőzése, 1=a leltárszolgáltatások telepítése</td>
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
<td style="border:1px solid black;">0=a naplófájlok megőrzése, 1=a naplófájlok eltávolítása (a /u telepítési kapcsolóval együtt használva)</td>
</tr>
<tr class="even">
<td style="border:1px solid black;">CREATE_DATABASE</td>
<td style="border:1px solid black;">0=az aktuális adatbázis használata, 1=új adatbázis létrehozása</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;">PROGRESS_WINDOW_HANDLE</td>
<td style="border:1px solid black;">Az MSI-folyamatot jelző üzenetek ablakának leírója.</td>
</tr>
<tr class="even">
<td style="border:1px solid black;">MU_ROLLUP</td>
<td style="border:1px solid black;">1=csatlakozás a Microsoft Update Improvement Program programhoz, 0=a Microsoft Update Improvement Program programhoz való csatlakozás mellőzése</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;">FRONTEND_SETUP</td>
<td style="border:1px solid black;">1=a tartalom helyének kihagyása az adatbázisból, 0=a tartalom helyének beírása az adatbázisba (hálózati terheléselosztás esetén)</td>
</tr>
</tbody>
</table>
  
#### Példa a kapcsolók használatára
  
```  
WSUSSetup.exe /q DEFAULT\_WEBSITE=0 (install in quiet mode using port 8530) WSUSSetup.exe /q /u (uninstall WSUS)  
```  
| ![](images/Cc708525.Important(WS.10).gif)Fontos:                                                                                                                                                  |  
|--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|  
| Ha a WSUS 3.0 SP1 szolgáltatást csendes módban (/q) telepíti, és a számítógépen nincsen meg a telepítéshez szükséges összes előfeltétel, a telepítő létrehoz egy WSUSPreReqCheck.xml nevű fájlt, és menti a %TEMP% könyvtárba. |
  
Telepítési problémák  
--------------------
  
#### Az ISS szolgáltatást a WSUS 3.0 SP1 telepítése közben a telepítő újraindítja
  
A WSUS 3.0 SP1 telepítője az ISS szolgáltatást értesítés nélkül újraindítja, ami befolyásolhatja a szervezeten belüli meglévő webhelyeket. Ha az IIS szolgáltatás nem fut, a WSUS 3.0 SP1 telepítője elindítja.
  
#### Ha kapcsolatok állnak fenn egy meglévő WSUS-adatbázissal, a telepítés sikertelen lehet
  
Ha egy meglévő telepítésről frissít a WSUS 3.0 SP1 szolgáltatásra, és kapcsolatok állnak fenn egy meglévő WSUS-adatbázissal (például ha az SQL Server Management Studio meg van nyitva), a telepítés meghiúsulhat. Ebben az esetben bontson minden kapcsolatot, és telepítse újra a WSUS 3.0 SP1 szolgáltatást.
  
#### A WSUS telepítője rossz könyvtárat jelez az adatbázisfájlokhoz
  
A WSUS telepítőjében, a telepítésre való készen állást jelző képernyőn helytelenül az jelenik meg, hogy az adatbázis helye az adatbázis helyének szülőkönyvtára. Azaz, ha például az alapértelmezett hely a %systemdrive%\\WSUS\\UpdateServicesDbFiles könyvtár, a képernyőn helytelenül az jelenik meg, hogy ez a hely a %systemdrive%\\WSUS könyvtár.
  
#### Ha a WSUS szolgáltatás MUI nyelvi csomagot tartalmazó olyan számítógépen fut, amelyen nem az angol az alapértelmezett nyelv, a súgó nem angolul, hanem az alapértelmezett nyelven jelenik meg
  
Az angoltól eltérő alapértelmezett nyelvű, MUI csomagot tartalmazó számítógépeken telepíthető a WSUS szolgáltatás, ha az aktuális területi beállítás angol. A felhasználói felület angolul fog megjelenni, de a súgó angol nyelven történő megjelentéséhez kerülő megoldást kell alkalmaznia. Másolja az angol nyelvű súgó .chm fájlját (*WSUSInstallDir*\\documentation\\mui\\0409\\WSUS30Help.chm) a fő dokumentációs könyvtárba (*WSUSInstallDir*\\documentation\\WSUS30Help.chm). Ekkor a súgónak minden nyelv esetén helyesen kell megjelennie.
  
Frissítési problémák  
--------------------
  
#### Helyreállítás sikertelen frissítés után
  
Ha a WSUS valamely korábbi verziójáról (WSUS 3.0, WSUS 2.0 SP1 vagy WSUS 2.0) frissít a WSUS 3.0 SP1 szolgáltatásra, és a frissítés valamilyen oknál fogva meghiúsul, tegye a következőket::
  
1.  Telepítse újra a WSUS korábbi verzióját.  
2.  Állítsa vissza az adatbázist a frissítés megkezdése előtt készített biztonsági másolatból. (A legtöbb esetben a WSUS is automatikusan készít egy biztonsági másolatot. Ennek helyéről a WSUSSetup.log fájlban tájékozódhat.)  
3.  Nézze át a naplókat a hiba okának felderítéséhez, majd szüntesse meg a problémát.  
4.  Próbálja meg újra frissíteni a WSUS szolgáltatást.
  
#### A WSUS 2.0 addig nem frissíthető a WSUS 3.0 SP1 szolgáltatásra, amíg a WSUS 3.0 SP1 korábbi telepítésből származó adatbázisa a számítógépen van
  
Ha korábban már telepítette a WSUS 3.0 SP1 szolgáltatást, majd újratelepítette a WSUS 2.0 szolgáltatást, a WSUS 3.0 SP1 újratelepítése előtt törölnie kell annak adatbázisát a számítógépről.
  
#### A számítógép nevének a WSUS 3.0 SP1 telepítése előtt történő módosítása meghiúsíthatja a frissítést
  
Ha a WSUS 2.0 telepítése után, a WSUS 3.0 SP1 szolgáltatásra való frissítés előtt módosítja a számítógép nevét , a frissítés meghiúsulhat.
  
Az alábbi parancsfájl használatával törölje és adja újra hozzá az ASPNET és a WSUS felügyeleti csoportot, majd ismételje meg a frissítést.
  
A parancsfájlban helyettesítse a *&lt;DBLocation&gt;* változót az adatbázis telepítési helyével, a *&lt;ContentDirectory&gt;* változót pedig a helyi tárolómappával.
  
```  
sqlcmd.exe -S *&lt;DBLocation&gt;* -E -Q "USE SUSDB DECLARE @asplogin varchar(200) SELECT @asplogin=name from sysusers WHERE name like '%ASPNET' EXEC sp\_revokedbaccess @asplogin" sqlcmd.exe -S *&lt;DBLocation&gt;* -E -Q "USE SUSDB DECLARE @wsusadminslogin varchar(200) SELECT @wsusadminslogin=name from sysusers WHERE name like '%WSUS Administrators' EXEC sp\_revokedbaccess @wsusadminslogin"   sqlcmd.exe -S *&lt;DBLocation&gt;* -E -Q "USE SUSDB DECLARE @asplogin varchar(200) SELECT @asplogin=HOST\_NAME()+'\\ASPNET' EXEC sp\_grantlogin @asplogin EXEC sp\_grantdbaccess @asplogin EXEC sp\_addrolemember webService,@asplogin" sqlcmd.exe -S *&lt;DBLocation&gt;* -E -Q "USE SUSDB DECLARE @wsusadminslogin varchar(200) SELECT @wsusadminslogin=HOST\_NAME()+'\\WSUS Administrators' EXEC sp\_grantlogin @wsusadminslogin EXEC sp\_grantdbaccess @wsusadminslogin EXEC sp\_addrolemember webService,@wsusadminslogin"   sqlcmd.exe -S *&lt;DBLocation&gt;* -E -Q "backup database SUSDB to disk=N'*&lt;ContentDirectory&gt;*\\SUSDB.Dat' with init"  
```
  
#### A telepítő felülírja a korábbi adatbázis biztonsági másolatát
  
A WSUS 3.0 SP1 telepítője az adatbázist az alapértelmezett *meghajtó*\\WSUS könyvtárba másolja (ahol a *meghajtó* a legnagyobb szabad lemezterülettel rendelkező helyi NTFS-meghajtó). Ha ebben a könyvtárban található az adatbázis biztonsági másolata, a telepítő azt felülírhatja. A WSUS 3.0 SP1 szolgáltatásra való frissítés előtt a rendszergazdáknak célszerű az aktuális verzió adatbázisáról készített biztonsági másolatot egy másik helyre menteni.
  
#### WSUS 2.0 szolgáltatást futtató számítógépeken az MSDE alkalmazásról az SQL Server 2000 vagy az SQL Server 2005 alkalmazásra való áttérés esetén módosítani kell egy beállításazonosítót
  
Ha a számítógépen WSUS 2.0 szolgáltatás fut, és SQL Server 2000 vagy SQL Server 2005 alkalmazásra tért át, módosítania kell a **HKLM\\SOFTWARE\\Microsoft\\Update Services\\Server\\Setup\\WmsdeInstalled** beállításazonosító értékét 1-ről 0-ra. Ha ezt nem teszi meg a WSUS 3.0 SP1 frissítése előtt, a frissítés meghiúsulhat.
  
#### A WSUS 2.0 telepítőjének elindítása majd leállítása után a telepítő törli a WSUS beállításkulcsot
  
Ha elindítja, majd később megszakítja a WSUS 2.0 telepítését, a telepítő törli a WSUS beállításkulcsot. Ez akkor okozhat problémát, ha már telepítve van a WSUS 3.0 SP1 szolgáltatás. Ugyanez a probléma jelentkezik akkor is, ha elindítja, majd megszakítja a WSUS 2.0 eltávolítását, és a WSUS 2.0 szolgáltatásról megpróbál frissíteni a WSUS 3.0 SP1 szolgáltatásra.
  
#### A WSUS 3.0 SP1 eltávolításakor a számítógépen maradó naplófájlok az újratelepítést követően elvesztik a megfelelő jogosultságokat
  
Amikor eltávolítja a WSUS 3.0 SP1 szolgáltatást, lehetősége van megtartani a telepítési naplófájlokat. Ha újratelepíti a WSUS 3.0 SP1 szolgáltatást, a régi naplófájlok elvesztik a jogosultságaikat (általában csak a WSUS rendszergazdák esetén). Ezeken a naplófájlokon vissza kell állítani a jogosultságokat.
  
#### Ha a WSUS 2.0-ügyfelek „Nem alkalmazható” állapotú frissítésekkel rendelkeznek, a WSUS 3.0 SP1 szolgáltatásra való frissítést követően ezek a frissítések egy rövid idő múlva „Ismeretlen” állapotúként jelennek meg
  
Ha a WSUS 2.0-kiszolgálóknak **Nem alkalmazható** állapotú frissítést tartalmazó ügyfeleik vannak, a kiszolgáló WSUS 3.0 SP1 szolgáltatásra való frissítését követően ezek a frissítések egy rövid idő múlva **Ismeretlen** állapotúként jelennek meg. A frissítések az ügyfél által végrehajtott következő keresés után ismét **Nem alkalmazható** állapotúként fognak megjelenni.
  
Ismert problémák  
----------------
  
#### A többszörös letöltési hibák, illetve az ismétlődő ügyfélszinkronizációs hibák elhárítása
  
Ha a WSUS 3.0 SP1-ügyfelek többszörös letöltési hibát jeleznek, illetve ha a WSUS 3.0 SP1-kiszolgálóval való szinkronizációjuk hosszabb ideig sikertelen, valószínűleg megsérült az ügyfél letöltési gyorsítótára. A helyzet megoldásához próbálja meg törölni az ügyfél letöltési gyorsítótárát a fájlrendszerből.
  
Az ügyfél letöltési gyorsítótárának törlése:
  
1.  Töröljön minden fájlt és alkönyvtárat az ügyfélszámítógép következő könyvtárából: **%windir%\\SoftwareDistribution\\Download**  
2.  Próbálja meg telepíteni a frissítést az ügyfélszámítógép WSUS 3.0 SP1 szolgáltatással való ismételt szinkronizálásával. A telepítésnek meg kell hiúsulnia a következő hibával: **WU\_E\_DM\_NOTDOWNLOADED, "Nem töltötték le a frissítést."**  
3.  A hibajelzés után az ügyfélszámítógép automatikusan újraindítja a letöltést, és a telepítés sikeresen megtörténik.
  
#### Szinkronizálási hiba esetén meg kell ismételni a szinkronizálást
  
Ha a szinkronizálás nem sikerül, első megoldásként próbálja meg ismét a kiszolgálóval való szinkronizálást. Ha a további szinkronizálási kísérletek sem vezetnek eredményre, olvassa el a [Windows Server Update Services 3.0 üzemltetési útmutatóját](http://go.microsoft.com/fwlink/?linkid=81072) a http://go.microsoft.com/fwlink/?LinkId=81072 címen. (Előfordulhat, hogy a lap angol nyelven jelenik meg.)
  
#### A WSUS 3.0 SP1 konfigurációjának közvetlenül az adatbázisban történő módosítása nem támogatott
  
A Windows Server Update Services szolgáltatás konfigurációs adatait egy SQL Server-alapú adatbázis tárolja. A konfigurációs adatoknak közvetlenül az adatbázisban való módosítása azonban nem támogatott. Ne módosítsa a WSUS 3.0 SP1 konfigurációs adatait közvetlenül az adatbázisban, hanem használja a WSUS 3.0 SP1 konzolját, vagy hívja meg a WSUS 3.0 SP1 alkalmazásfejlesztési felületeit.
  
#### A letöltési hibákat a rendszer nem jelzi azonnal, ha a lemezkvóta be van kapcsolva
  
Ha a lemezkvóta be van kapcsolva, és a rendszer túllépi azt, a WSUS-kiszolgálón történt frissítésletöltési hibákat csak későn jelzi a rendszer. Ennek elkerülése érdekében tiltsa le a lemezkvótát vagy növelje meg azt.
  
#### A WSUS 3.0 SP1 szolgáltatás SSL titkosítással történő központi telepítésekor az ügyfélszámítógépek 0x8024400a jelű hibakóddal leállnak
  
Az ügyfélszámítógépek frissítése az SSL titkosítást használó WSUS 3.0 SP1-kiszolgálóval való kommunikáció során 0x8024400a jelű hibakóddal meghiúsulhat. A hibát megszüntető frissítésről a [905422. számú Tudásbázis-cikkben](http://go.microsoft.com/fwlink/?linkid=70593), a http://go.microsoft.com/fwlink/?LinkId=70593 címen tájékozódhat. (Előfordulhat, hogy a lap angol nyelven jelenik meg.)
  
#### A WSUS rendszergazdák tartományi fiókot a WSUS eltávolításakor a rendszer nem törli
  
A WSUS rendszergazdák csoportot a rendszer tartományi fiókként (nem pedig helyi fiókként) hozza létre a tartományvezérlőkön, ezért, ha a WSUS eltávolításakor a rendszer törölné ezt a tartományi fiókot, az ezt használó összes telepítés letiltott állapotba kerülne. Emiatt a WSUS telepítésekor a rendszer nem törli ezt a fiókot.
  
#### Az alsóbb szintű kiszolgálók felsőbb szintű kiszolgálóvá történő konvertálásakor újra kell importálni a katalógushely-frissítéseket
  
Ha egy alsóbb szintű kiszolgálót felsőbb szintű kiszolgálóvá léptet elő, minden katalógushely-frissítést újra kell importálnia, különben a hely nem fogja tudni szinkronizálni az új katalógushely-frissítéseket a kiszolgálóra.
  
#### Az ISS szolgáltatás SSL titkosítással való használatakor a titkosítatlan hozzáférés továbbra is lehetséges, ha a „Biztonságos csatorna szükséges (SSL)” beállítás nincs bejelölve
  
Ha az IIS szolgáltatást tanúsítvány telepítésével állítja be az SSL titkosítás használatára, a hely továbbra is elérhető titkosítatlan HTTP-n keresztül, ha a **Biztonságos csatorna szükséges (SSL)** beállítás nincs bejelölve. Erről bővebben az [IIS](http://go.microsoft.com/fwlink/?linkid=98084) szolgáltatással foglalkozó dokumentumban, a http://go.microsoft.com/fwlink/?LinkID=98084 címen tájékozódhat. (Előfordulhat, hogy a lap angol nyelven jelenik meg.)
  
#### A katalógushely importálása meghiúsulhat a %windir%\\TEMP mappához való írási/olvasási jogosultság nélkül
  
Ha egy katalógushely importálásakor a hálózati szolgáltatásfióknak nincs írási/olvasási jogosultsága a %windir%\\TEMP mappához, az importálás a következőhöz hasonló hibaüzenettel meghiúsulhat: A kiszolgáló nem tudta feldolgozni a kérelmet. ---&gt; A fájl nem található: "C:\\WINDOWS\\TEMP\\*tempFileName*.dll".
  
#### A teljesítmény lecsökkenhet a WSUS 3.0 SP1 szolgáltatást futtató és a WSUS 2.0 szolgáltatást futtató alsóbb szintű replikakiszolgáló közötti szinkronizálás során
  
Ha a WSUS 3.0 SP1 szolgáltatást felsőbb szintű kiszolgálóra telepíti, és egy, a WSUS 2.0 szolgáltatást futtató, alsóbb szintű replikakiszolgálóval hajt végre szinkronizálást, teljesítményproblémák jelentkezhetnek. A hibát megszüntető frissítésről a [910847. számú Tudásbázis-cikkben](http://go.microsoft.com/fwlink/?linkid=70669), a http://go.microsoft.com/fwlink/?LinkId=70669 címen tájékozódhat. (Előfordulhat, hogy a lap angol nyelven jelenik meg.)
  
#### Ha az e-mail kiszolgáló nem működik vagy elérhetetlen, az e-mail értesítések küldése jelzés nélkül megszűnik
  
Ha a hálózati e-mail kiszolgáló offline állapotban van, a WSUS 3.0 SP1 jelzés nélkül mellőzi az e-mail értesítések küldését. Az eseménynaplóba azonban bejegyzi az 10052. számú eseményt (HealthCoreEmailNotificationRed).
  
#### A felsőbb szintű kiszolgálók módosított beállításai nem kerülnek át azonnal az alsóbb szintű kiszolgálókra
  
A felsőbb szintű kiszolgáló beállításainak módosításakor hosszabb idő is eltelhet, amíg a változások ténylegesen érvénybe lépnek. Ha például új nyelvet ad meg a felsőbb szintű kiszolgálón, majd azonnal szinkronizálást kezdeményez az alsóbb szintű kiszolgálóval, a módosítás ekkor még nem jelenik meg, csak a következő ütemezett szinkronizáláskor. A várakozási idő a felsőbb szintű kiszolgálón lévő frissítések számával arányosan növekszik.
  
#### A WSUS 3.0 SP1 eltávolításakor a rendszer nem törli az adatbázis példányát
  
A WSUS 3.0 SP1 szolgáltatás eltávolításakor az adatbázis példányát a rendszer nem törli, mert azt több alkalmazás is használhatja, amelyek működése az adatbázis eltávolításakor leállhat.
  
Ha szükség van a Belső Windows-adatbázis eltávolítására, használja az alábbi parancsokat:
  
(32 bites platformokon)
  
```  
msiexec /x {CEB5780F-1A70-44A9-850F-DE6C4F6AA8FB} callerid=ocsetup.exe  
```  
(64 bites platformokon)
  
```  
msiexec /x {BDD79957-5801-4A2D-B09E-852E7FA64D01} callerid=ocsetup.exe  
```  
Ha Windows Server 2008 rendszerről szeretné eltávolítani a Belső Windows-adatbázis SP2 szervizcsomaggal bővített változatát, használja a Kiszolgálókezelő alkalmazást.
  
Az eltávolítás során előfordulhat, hogy a rendszer nem törli az alapértelmezett .mdf és .ldf fájlokat, ami a WSUS 3.0 SP1 későbbiekben végrehajtott telepítésének meghiúsulásához vezet. Ezek a fájlok a %windir%\\SYSMSI\\SSEE könyvtárból törölhetők.
  
#### Ha egy alsóbb szintű kiszolgáló módosítja a hozzá tartozó felsőbb szintű kiszolgálót, az „Ismeretlen” állapotú frissítéseket a rendszer „Nem alkalmazható” állapotúként jelenti
  
Ha egy alsóbb szintű kiszolgáló egy másik felsőbb szintű kiszolgálóról hajt végre szinkronizálást, az **Ismeretlen** állapotú frissítéseket a rendszer az új felsőbb szintű kiszolgálón **Nem alkalmazható** állapotúként jelenti. Ez egy átmeneti állapot, amelyet a rendszer az alsóbb szintű kiszolgáló következő – a saját ügyfeleivel végrehajtott szinkronizálást követő – állapotjelentésekor a megfelelő állapotra javít.
  
#### A távoli konzolról, több kiszolgálón futtatott kiszolgáló-karbantartó varázsló egyik kiszolgálón történő időtúllépése esetén az összes kiszolgálóval való kapcsolat elveszik
  
Lehetőség van a kiszolgáló-karbantartó varázsló egyetlen távoli konzolról, több kiszolgálón való futtatására, de ha a karbantartási folyamat során az egyik kiszolgálón időtúllépés történik, a konzol az összes kiszolgálóval elveszti a kapcsolatot. Egyetlen adat sem veszik el, de a rendszergazdának minden kiszolgálóval újra fel kell vennie a távoli kapcsolatot.
  
#### A kapcsolat gyors egymásutánban történő elindítása majd leállítása után a konfiguráló varázslóban a „Nem történt szinkronizálási hiba” hibaüzenet jelenik meg
  
A WSUS konfigurálása során a kiszolgáló alapinformációinak továbbítása érdekében csatlakozni kell a felsőbb szintű kiszolgálóhoz (amely lehet Microsoft Update- vagy intranetes felsőbb szintű kiszolgáló). Ha a **Kapcsolat kezdeményezése**, majd azonnal a **Kapcsolat leállítása** elemre kattint, a következő helytelen hibaüzenet jelenik meg: „Nem történt szinkronizálási hiba”.
  
A WSUS 3.0 SP1 szolgáltatás Windows Server 2008 rendszeren  
----------------------------------------------------------
  
#### Támogatott verziók
  
A WSUS 3.0 SP1 a Windows Server 2008 32 bites és 64 bites változatait is támogatja.
  
#### Előfeltételek
  
###  

 
<table style="border:1px solid black;">
<colgroup>
<col width="50%" />
<col width="50%" />
</colgroup>
<thead>
<tr class="header">
<th style="border:1px solid black;" >Követelmény</th>
<th style="border:1px solid black;" >Ismertetés</th>
</tr>
</thead>
<tbody>
<tr class="odd">
<td style="border:1px solid black;">Microsoft Internet Information Services (IIS)</td>
<td style="border:1px solid black;">Az operációs rendszerből telepíthető. Győződjön meg arról, hogy az alábbi összetevők engedélyezve vannak:
<ul>
<li>Windows-hitelesítés<br />
<br />
</li>
<li>Statikus tartalom<br />
<br />
</li>
<li>ASP.NET<br />
<br />
</li>
<li>Kompatibilitás az IIS 6 kezelésével<br />
<br />
</li>
<li>Kompatibilitás az IIS 6 metabázisával<br />
<br />
</li>
</ul></td>
</tr>
<tr class="even">
<td style="border:1px solid black;">Újraterjeszthető csomag a Microsoft® .NET-keretrendszer 2.0-s verziójához (x86)</td>
<td style="border:1px solid black;">A Windows Server 2008 rendszeren nem szükséges, az operációs rendszer része.</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;">Microsoft Management Console 3.0</td>
<td style="border:1px solid black;">A Windows Server 2008 rendszeren nem szükséges, az operációs rendszer része.</td>
</tr>
<tr class="even">
<td style="border:1px solid black;">Microsoft jelentésmegtekintő</td>
<td style="border:1px solid black;">A WSUS felhasználói felület használatához ez előfeltétel. Erről bővebben a Microsoft jelentésmegtekintő újraterjeszhető csomagjának 2005-ös verziójával foglalkozó dokumentumban, a <a href="http://go.microsoft.com/fwlink/?linkid=70410">Microsoft letöltőközpontjában</a>, a http://go.microsoft.com/fwlink/?LinkId=70410 címen tájékozódhat. (Előfordulhat, hogy a lap angol nyelven jelenik meg.)</td>
</tr>
</tbody>
</table>
  
#### A Biztonság beállítása varázsló használata
  
Windows Server 2008 rendszerben a Biztonság beállítása varázsló (SCW) futtatásakor kijelölheti a WSUS szerepkört, és engedélyezheti a hozzá kapcsolódó függőségeket. A Biztonság beállítása varázsló futtatásához kattintson a **Start** gombra, mutasson a **Felügyeleti eszközök** pontra, majd kattintson a **Biztonság beállítása varázsló** parancsra.
  
A Biztonság beállítása varázsló és a WSUS szerepkör együttes használata során felmerülő ismert problémák:
  
-   **A Belső Windows-adatbázis szolgáltatás engedélyezve van, még akkor is, ha azt a WSUS szolgáltatás nem használja.** A WSUS szolgáltatást ön beállítja egy adatbázis – vagy a belső Windows-adatbázis vagy az SQL Server-adatbázis – használatára. Ha a WSUS az SQL Server alkalmazással együtt van telepítve, és a Biztonság beállítása varázslóban a WSUS szerepkört választja, a számítógépen meglévő Belső Windows-adatbázis szolgáltatást a rendszer engedélyezi, bár a WSUS szolgáltatás nem használja. Ha a belső Windows-adatbázis helyett SQL Server- adatbázist használ, tiltsa le a Belső Windows-adatbázis szolgáltatást.  
-   **A WSUS tűzfalszabályai egyedi webhelyeken nincsenek alapértelmezés szerint engedélyezve.** Ha a WSUS szolgáltatást egyedi webhelyen telepíti (8530-es vagy 8531-es port), a szükséges tűzfalszabályokat a rendszer nem engedélyezi alapértelmezés szerint, még akkor sem, ha a Biztonság beállítása varázslóban a WSUS szerepkört választja. Attól függően, hogy az SSL titkosítás be van-e állítva a WSUS-kiszolgálón, engedélyeznie kell a WSUS megfelelő tűzfalszabályait.
  
A WSUS 3.0 SP1 szolgáltatás Windows Small Business Server 2003 rendszeren  
-------------------------------------------------------------------------
  
#### Ha a virtuális IIS-gyökér adott IP-címek vagy tartománynevek számára le van tiltva, a WSUS 3.0 SP1-kiszolgáló nem tudja magát frissíteni
  
Előfordulhat, hogy a Windows Small Business Server néhány példányának alapértelmezett IIS-webhelye **IP-cím és tartománynév korlátozása** beállítással van konfigurálva. Ebben az esetben előfordulhat, hogy a kiszolgálón lévő Windows Update-ügyfél nem tudja frissíteni magát.
  
#### A WSUS 3.0 SP1 telepítése Small Business Server rendszerre – integrálási problémák
  
-   Ha a Windows Small Business Server 2003 rendszer ISA-proxykiszolgálót használ az internet-hozzáféréshez, a következő adatokat kézzel kell megadnia a **Beállítások** párbeszédpanelen: **a proxykiszolgáló beállításai, a proxykiszolgáló neve, port**.  
-   Ha az ISA szolgáltatás Windows-hitelesítést használ, a proxykiszolgáló hitelesítő adatait a *TARTOMÁNY*\\*felhasználó* formában kell megadni, és a felhasználónak az Internet-felhasználók csoport tagjának kell lennie.
  
#### Ha a Windows SBS varázslóinak használata nélkül adott hozzá alhálózatot a hálózathoz, végre kell hajtania az alábbi eljárást
  
A WSUS-kiszolgáló telepítője két IIS-gyökeret telepít a kiszolgálóra: a SelfUpdate és a ClientWebService mappát. Ezenkívül néhány fájlt az alapértelmezett webhely (80-as port) kezdőkönyvtárában is elhelyez, amely lehetővé teszi az ügyfélszámítógépek számára, hogy az alapértelmezett webhelyen keresztül frissítsék magukat. Alapértelmezés szerint az alapértelmezett webhely úgy van beállítva, hogy letiltsa a helyi állomáson kívül található IP-címekhez, illetve a kiszolgálóhoz csatlakozó adott alhálózatokhoz való hozzáférést. Emiatt a helyi állomáson kívül, illetve az adott alhálózatokon található ügyfélszámítógépek nem tudnak önfrissítést végrehajtani. Ha a Microsoft Windows Small Business Server 2003 (Windows SBS) varázslóinak használata nélkül adott hozzá alhálózatot a hálózathoz, végre kell hajtania az alábbi eljárást:
  
1.  A Kiszolgálókezelőben bontsa ki a **Speciális kezelés**, az **Internet Information Services**, a **Webhelyek**, majd az **Alapértelmezett webhely** csomópontot, kattintson a jobb gombbal a **Selfupdate** virtuális könyvtárra, majd válassza a **Tulajdonságok** parancsot.  
2.  Kattintson a **Könyvtárbiztonság** elemre.  
3.  Az **IP-cím és tartománynév korlátozása** beállításcsoportban kattintson a **Szerkesztés** gombra, majd jelölje ki a **Hozzáférés engedélyezve** elemet.  
4.  Kattintson az **OK** gombra, a jobb gombbal kattintson a **ClientWebService** virtuális könyvtárra, majd válassza a **Tulajdonságok** parancsot.  
5.  Kattintson a **Könyvtárbiztonság** elemre.  
6.  A **IP-cím és tartománynév korlátozása** beállításcsoportban kattintson a **Szerkesztés** gombra, majd jelölje ki a **Hozzáférés engedélyezve** elemet.
  
Szerzői jogi nyilatkozat  
------------------------
  
A dokumentumban szereplő információk – köztük az URL-címek és egyéb internetes webhelyhivatkozások – értesítés nélkül változhatnak. Ellenkező utalás hiányában a dokumentumban példaként említett cégek, szervezetek, termékek, tartománynevek, e-mail címek, emblémák, személyek, helyek és események kitaláltak, így bármely létező céggel, szervezettel, termékkel, tartománynévvel, e-mail címmel, emblémával, személlyel, hellyel vagy eseménnyel való egyezés kizárólag a véletlen műve. Az összes vonatkozó szerzői jogi törvény betartása a felhasználó felelőssége. A Microsoft Corporation kifejezett írásos engedélye nélkül sem a dokumentum egésze, sem annak tetszőleges része nem reprodukálható, nem tárolható visszakereshető rendszerben, semmilyen formában és módon (elektronikus, mechanikai, fénymásolásos, hangrögzítési vagy más eljárással), továbbá semmilyen célból nem továbbítható. Minden ilyen cselekmény a szerzői jogok megsértését jelenti.
  
A dokumentumban foglaltak a Microsoft szabadalmainak, szabadalmi oltalmainak, védjegyeinek, szerzői jogainak és egyéb szellemi tulajdonjogainak tárgyát képezhetik. Hacsak a Microsoft valamelyik írásos licencszerződése másként nem rendelkezik, a jelen dokumentum rendelkezésre bocsátása nem jogosítja fel a felhasználót ezen szabadalmak, védjegyek, szerzői jogok vagy egyéb szellemi tulajdon használatára.
  
©2007 Microsoft Corporation. Minden jog fenntartva.
  
A Microsoft SQL Server, a Windows, és a Windows Server a Microsoft Corporation védjegyei vagy bejegyzett védjegyei az Amerikai Egyesült Államokban, illetve más országokban.
  
Az egyéb márkanevek jogtulajdonosaik védjegyei.
