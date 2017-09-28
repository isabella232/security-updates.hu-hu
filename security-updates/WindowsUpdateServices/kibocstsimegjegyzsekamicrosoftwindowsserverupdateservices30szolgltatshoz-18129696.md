---
TOCTitle: 'Kibocsátási megjegyzések a Microsoft Windows Server Update Services 3.0 szolgáltatáshoz'
Title: 'Kibocsátási megjegyzések a Microsoft Windows Server Update Services 3.0 szolgáltatáshoz'
ms:assetid: '94d1385f-4872-4c29-8822-3a4ec5e45ae4'
ms:contentKeyID: 18129696
ms:mtpsurl: 'https://technet.microsoft.com/hu-hu/library/Cc708491(v=WS.10)'
---

Kibocsátási megjegyzések a Microsoft Windows Server Update Services 3.0 szolgáltatáshoz
=======================================================================================

A kibocsátási megjegyzések dokumentuma a Microsoft® Windows® Server Update Services (WSUS) 3.0 szolgáltatást érintő ismert problémákat tárgyalja, közli továbbá az alkalmazás telepítésének ajánlott és megkövetelt előfeltételeit. A dokumentum a következő részekből áll:

-   Rendszerkövetelmények a WSUS 3.0 kiszolgáló telepítéséhez
-   Konfigurációs követelmények a WSUS 3.0 kiszolgáló telepítéséhez
-   Rendszerkövetelmények a WSUS 3.0 távoli konzol telepítéséhez
-   Konfigurációs követelmények a WSUS 3.0 távoli konzol telepítéséhez
-   Rendszerkövetelmények az ügyfél telepítéséhez
-   Szoftverkövetelmények a WSUS 3.0 kiszolgáló telepítéséhez
-   Lemezterületre vonatkozó követelmények a WSUS 3.0 kiszolgáló telepítéséhez
-   A WSUS 3.0 frissítési követelményei
-   A telepítő parancssori paraméterei
-   Telepítési és frissítési problémák
-   Ismert problémák
-   A WSUS 3.0 Windows Server® 2008 rendszeren
-   A WSUS 3.0 szolgáltatás a Windows Small Business Server 2003 rendszeren

| ![](images/Cc708491.note(WS.10).gif)Megjegyzés:                                                                                                                             |
|----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| Ez a dokumentum letölthető a [Microsoft letöltőközpontból](http://go.microsoft.com/fwlink/?linkid=71220) ([http://go.microsoft.com/fwlink/?LinkId=71220](http://go.microsoft.com/fwlink/?linkid=71220)). |

Fontos konfigurációs kérdés: Felül kell írnia a proxykiszolgáló jelszavát a konfigurációs varázslóban
-----------------------------------------------------------------------------------------------------

Ha olyan proxykiszolgálót használ, amely felhasználónév/jelszó típusú hitelesítést igényel, a WSUS-kiszolgálón sikertelen lehet a frissítések szinkronizálása, ha nem írja felül a proxykiszolgáló jelszavát a WSUS-kiszolgáló konfigurációs varázslójának futtatásakor. Mivel a konfigurációs varázsló automatikusan elindul a telepítés végén, a probléma szinkronizálási hibákat okozhat egy korábbiról a WSUS 3.0-s verzióra frissítéskor.

A probléma úgy kerülhető el, hogy a frissítés után megszakítja a konfigurációs varázslót, vagy a konfigurációs varázsló futásakor újból beírja a megfelelő proxyjelszót. Előfordulása után a hiba javításához nyissa meg a **Frissítés forrása és a Proxykiszolgáló** lapot tartalmazó párbeszédpanelt a **Beállítások** lapon, írja be újra a proxyjelszót, majd mentse a beállítást.

Rendszerkövetelmények a WSUS 3.0 kiszolgáló telepítéséhez
---------------------------------------------------------

#### A WSUS 3.0 kiszolgáló Windows Server 2003 Service Pack 1 és Windows Server 2008 rendszeren használható

A WSUS 3.0 kiszolgáló Windows Server 2003 Service Pack 1 és Windows Server 2008 rendszeren használható.

#### A Windows 2000 Server nem használható a WSUS 3.0 kiszolgálókhoz

A Microsoft Windows® 2000 Server nem használható operációs rendszer a WSUS 3.0 kiszolgálókhoz.

#### A WSUS 3.0-s verziójának a Terminálszolgáltatásokat futtató kiszolgálókon való használatát nem támogatjuk.

Bár előfordulhat, hogy a WSUS 3.0 kiszolgáló működik a Terminálszolgáltatásokat futtató kiszolgálókon, de ez nem támogatott és nem ajánlott. A WSUS 3.0 nem fog futni olyan kiszolgálón, amelyen a Terminálszolgáltatások távoli SQL Server kiszolgálók használatára van beállítva. Mivel minden távoli, a Terminálszolgáltatásokat futtató licenckiszolgálón végzett egyéni művelet (beleértve a telepítést is) rendszerfiókként fog futni, és lehet, hogy a kiszolgáló rendszerfiókjának nincs hozzáférési joga a távoli SQL Server kiszolgálóhoz, előfordulhat, hogy a telepítés sikertelen lesz.

Konfigurációs követelmények a WSUS 3.0 kiszolgáló telepítéséhez
---------------------------------------------------------------

#### Futnia kell az IIS szolgáltatásnak

A Microsoft Windows Server Update Services 3.0 működéséhez a számítógépen futnia kell az Internet Information Services (IIS) szolgáltatásnak, amely alapértelmezés szerint nem települ sem a Microsoft Windows Server 2003, sem a Windows Server 2008 rendszerrel. Ha az IIS nélkül próbálja meg telepíteni a WSUS 3.0 összetevőt, a Windows Server Update Services telepítője egy hibaüzenetet jelenít meg, amely közli, hogy az IIS nincs telepítve

#### Ha az IIS az IIS 5.0-s verzió elkülönítési üzemmódjában fut, sikertelen lesz a telepítés

Ha a kiszolgálót a Windows 2000 Server rendszerről a Windows Server 2003 rendszerre frissítette, az IIS az IIS 5.0-s verzió kompatibilitási üzemmódjában futhat. Az IIS 5.0-s verzió elkülönítési üzemmódja az IIS-kezelőben is engedélyezhető. Ez telepítési hibát fog okozni. A WSUS 3.0 telepítése előtt tiltania kell az IIS 5.0-s verzió elkülönítési üzemmódját.

#### Ha bármely IIS-összetevő 32 bites kompatibilitási üzemmódban van telepítve egy 64 bites platformra, lehet, hogy a WSUS 3.0 telepítése sikertelen lesz

Minden IIS-összetevőt natív módban kell telepíteni a 64 bites platformokon. Ha bármely IIS-összetevő 32 bites kompatibilitási üzemmódban van telepítve, lehet, hogy a telepítés sikertelen lesz.

#### A proxykiszolgálóknak támogatniuk kell mind a HTTP, mind a HTTPs protokollt

Ha konfigurálja a gyökér WSUS kiszolgálót (azt a kiszolgálót, amely közvetlenül a Microsoft Update webhelyről kapja a frissítéseket), és proxykiszolgáló található a WSUS kiszolgáló és az internet között, a proxykiszolgálónak támogatnia kell mind a HTTP, mind a HTTPS protokollt.

#### Ha két vagy több webhely már fut a 80-as porton, egy kivételével törölje ezeket a WSUS telepítése előtt

Ha két vagy több webhely már fut a 80-as porton (például Windows® SharePoint® Services), ezeket egy kivételével törölnie kell a WSUS telepítése előtt. Ennek elmulasztásakor a kiszolgálóhoz tartozó ügyfelek nem tudják önmagukat frissíteni.

#### Előfordulhat, hogy a WSUS 3.0 telepítésekor le kell tiltani a víruskereső programokat

Előfordulhat, hogy a WSUS 3.0 telepítésekor le kell tiltani a víruskereső programokat, és csak ezt követően lehet végrehajtani a telepítést. Miután letiltotta a víruskereső programot, a WSUS telepítésének megkezdése előtt indítsa újra a számítógépet. A számítógép újraindításával megakadályozható, hogy a fájlok zárolva legyenek, amikor a telepítő hozzájuk szeretne férni. A telepítés befejezését követően ismét kapcsolja be a víruskereső programot. A víruskereső program letiltásának és visszakapcsolásának pontos lépéseiről a víruskereső program forgalmazójának webhelyén találhat tájékoztatást.

| ![](images/Cc708491.Caution(WS.10).gif)Figyelmeztetés:                                                                                                                                                                                                                                                            |
|------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| Ez a megkerülő megoldás sérülékenyebbé teheti a számítógépet vagy a hálózatot a rosszindulatú felhasználók és a kártevő szoftverek, például vírusok támadásával szemben. Nem javasoljuk ezt a megoldást, de tájékoztatásul közöljük, hogy saját belátása szerint szükség esetén alkalmazni tudja, ezt azonban csak saját felelősségére teheti. |

| ![](images/Cc708491.note(WS.10).gif)Megjegyzés:                                                                                                                                                                                                                |
|---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| A víruskereső programok arra szolgálnak, hogy megvédjék a számítógépet a vírusoktól. Amíg a víruskereső program le van tiltva, ne töltsön le és ne nyisson meg fájlokat nem megbízhatónak vélt forrásból, ne látogasson nem megbízható webhelyekre, és ne nyisson meg e-mail mellékleteket. |

#### A WSUS futtatásához az SQL Server alkalmazásban engedélyezni kell a beágyazott triggerek használatát

A beágyazott eseményindítók beállítás alapértelmezés szerint be van ugyan kapcsolva, de az SQL Server rendszergazdája kikapcsolhatja.

Ha a Windows Server Update Services adattárolójaként egy SQL Server-alapú adatbázist szeretne használni, az SQL Server rendszergazdájának ellenőriznie kell, hogy a beágyazott eseményindítók engedélyezve vannak-e a kiszolgálón; a WSUS 3.0 rendszergazdája csak ezután telepítheti a WSUS 3.0 szolgáltatást, és adhatja meg a telepítés folyamán a használni kívánt adatbázist.

A WSUS 3.0 telepítő engedélyezi a RECURSIVE\_TRIGGERS adatbázis-specifikus beállítást, az egész kiszolgálóra érvényes, beágyazott eseményindítókra vonatkozó beállítást azonban nem kapcsolja be.

Annak ellenőrzésére, hogy be van-e kapcsolva a beágyazott eseményindítók beállítás, futtassa az alábbi parancsot:

**sp\_configure 'nested triggers'**

A beágyazott eseményindítókra vonatkozó beállítás engedélyezéséhez kötegfájlból futtassa az alábbi parancsokat az SQL Server alkalmazást működtető számítógépen:

**sp\_configure 'nested triggers', 1**

**GO**

**RECONFIGURE**

**GO**

Ha nincs telepítve a kiszolgálóra az SQL Server Management Studio, az SQL-parancsfájlokat futtathatja a parancssorból. A Microsoft SQL Server 2005 Command Line Query segédprogram elérhető a [Microsoft letöltőközpontjában](http://go.microsoft.com/fwlink/?linkid=70728) (http://go.microsoft.com/fwlink/?LinkId=70728 – lehet, hogy a hivatkozás angol nyelvű anyagra mutat). Első lépésként futtassa az **sqlcmd** parancsot.

Ha SQL-parancsfájlokat kíván futtatni Belső Windows-adatbázis rendszeren, le kell töltenie az SQL Native Client ügyfélprogramot is ugyanarról a letöltési oldalról.

#### A távoli SQL-kiszolgálóval kapcsolatos korlátozások és követelmények

A WSUS 3.0 támogatja olyan adatbázisszoftverek használatát, amelyek nem a WSUS 3.0 szolgáltatást futtató számítógépen működnek. A távoli SQL-telepítéshez tartozik néhány konfigurációs követelmény

-   Tartományvezérlőnek konfigurált kiszolgáló nem használható a távoli SQL-pár háttérgépeként.
-   Nem szabad futtatnia a Terminálkiszolgáló szolgáltatást azon a számítógépen, amely a távoli SQL-telepítés előtér-kiszolgálója lesz.
-   Legalább a Microsoft SQL Server 2005 Service Pack 1 (elérhető a [Microsoft letöltőközpontban](http://go.microsoft.com/fwlink/?linkid=66143) (http://go.microsoft.com/fwlink/?LinkId=66143) használata szükséges adatbázisszoftverként a háttérszámítógépen, ha az Windows Server 2003 rendszerrel működik, és az SQL Server 2005 Service Pack 2 szükséges, ha az operációs rendszer a Windows Server® 2008.
-   Az előtér- és a háttérszámítógépnek azonos Active Directory-tartományhoz kell tartoznia, eltérő tartományoknál bizalmi kapcsolatot kell létesítenie ezek között a WSUS telepítésének elindítása előtt.
-   Ha a WSUS 2.0 már telepítve van egy távoli SQL-konfiguráción, és frissíteni szeretné ezt a WSUS 3.0-s verzióra, el kell távolítania a WSUS 2.0-s verziót a háttérszámítógépről (a Vezérlőpult **Programok telepítése és törlése** segédprogramjával), és gondoskodnia kell arról, hogy a meglévő adatbázis ne módosuljon. Ezután telepítenie kell az SQL Server 2005 SP1 vagy SP2 szervizcsomaggal bővített verzióját, és frissítenie kell a meglévő adatbázist. Végül telepítenie kell a WSUS 3.0 szolgáltatást az előtér-számítógépen.

#### A WSUS nem telepíthető, ha a gépre már telepítve van az Internet Explorer 7 egyes előzetes verzióinak és a Terminálszolgáltatásoknak a kombinációja

A WSUS telepítése sikertelen, ha az Internet Explorer 7 egyes „Release Candidate” változatai egyszerre vannak jelen a Terminálszolgáltatásokkal.

Rendszerkövetelmények a WSUS 3.0 távoli konzol telepítéséhez
------------------------------------------------------------

A WSUS 3.0 távoli konzol a következő platformokon telepíthető:

-   Windows Server 2008
-   Windows Vista®
-   Windows Server 2003 SP1
-   Windows XP SP2

Konfigurációs követelmények a WSUS 3.0 távoli konzol telepítéséhez
------------------------------------------------------------------

#### Széles sávú kapcsolat szükséges a távoli felügyeleti konzol és a WSUS 3.0 kiszolgáló között

Teljesítményproblémák jelentkezhetnek, ha keskeny sávú hálózati kapcsolaton keresztül csatlakoztatja a távoli felügyeleti konzolt a WSUS 3.0 kiszolgálóhoz. Szűréssel korlátozhatja ugyan a látható frissítések és számítógépek számát, de mindenképpen javasolt, hogy széles sávú kapcsolatot használjon a távoli felügyeleti konzol és a WSUS 3.0 kiszolgáló között. Ha teljesítményproblémák jelentkeznek a távoli konzolnál, a távoli felügyelet végrehajtásához célszerű a Terminálkiszolgáló szolgáltatást használni a kiszolgálóhoz való csatlakozásban.

Rendszerkövetelmények az ügyfél telepítéséhez
---------------------------------------------

A WSUS ügyfélszoftvere az Automatikus frissítések segédprogram. A következő operációs rendszerek bármelyikén használható:

-   Windows Vista
-   Windows Server 2008
-   Microsoft Windows Server 2003, bármely kiadás
-   Microsoft Windows XP Professional SP2
-   Microsoft Windows 2000 Professional SP4, Windows 2000 Server SP4 vagy Windows 2000 Advanced Server SP4

Szoftverkövetelmények a WSUS 3.0 kiszolgáló telepítéséhez
---------------------------------------------------------

A következő táblázat a Windows Server 2003 SP1 platformokon szükséges szoftverelemeket mutatja be. A Windows Server 2008 rendszer esetében megkövetelt szoftverekről a Windows Server 2008 rendszeren futó WSUS 3.0 szolgáltatásról szóló szakasz nyújt tájékoztatást.

A WSUS 3.0 telepítésének futtatása előtt ellenőrizze, hogy a rendszer megfelel-e ezeknek a szoftverkövetelményeknek. Ha az itt említett frissítések bármelyike a számítógép újraindítását kéri a telepítés végeztével, akkor az újraindítást a WSUS 3.0 alkalmazás telepítése előtt kell végrehajtani.

###  

<p> </p>
<table style="border:1px solid black;">
<colgroup>
<col width="50%" />
<col width="50%" />
</colgroup>
<thead>
<tr class="header">
<th>Követelmény</th>
<th>Részletek</th>
</tr>
</thead>
<tbody>
<tr class="odd">
<td style="border:1px solid black;"><p>Microsoft Internet Information Services (IIS)</p></td>
<td style="border:1px solid black;"><p>Az operációs rendszerből telepíthető.</p>
<p>Lásd 1. probléma: Futnia kell az IIS szolgáltatásnak.</p></td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><p>A Microsoft® .NET-keretrendszer 2.0-s verziójának terjeszthető csomagja (x86)</p></td>
<td style="border:1px solid black;"><p>A Microsoft® .NET-keretrendszer 2.0-s (x86) verziójának terjeszthető csomagja elérhető a <a href="http://go.microsoft.com/fwlink/?linkid=68935">Microsoft letöltőközpontjában</a> (http://go.microsoft.com/fwlink/?LinkId=68935 – lehet, hogy a hivatkozás angol nyelvű anyagra mutat). A 64 bites platformokhoz a Microsoft® .NET-keretrendszer 2.0-s (x64) verziója érhető el <a href="http://go.microsoft.com/fwlink/?linkid=70637">Microsoft letöltőközpontjában</a> (http://go.microsoft.com/fwlink/?LinkId=70637 – lehet, hogy a hivatkozás angol nyelvű anyagra mutat).</p></td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><p>A Windows Server 2003 rendszer Microsoft Management Console 3.0 összetevője</p></td>
<td style="border:1px solid black;"><p>Ez előfeltétele a WSUS 3.0 kezelőfelülete használatának. A Windows Server 2003 rendszer Microsoft Management Console 3.0 összetevője elérhető a <a href="http://go.microsoft.com/fwlink/?linkid=70412">Microsoft letöltőközpontjában</a> (http://go.microsoft.com/fwlink/?LinkId=70638 – lehet, hogy a hivatkozás angol nyelvű anyagra mutat). A 64 bites platformokhoz a Windows Server 2003 x64 Edition Microsoft Management Console 3.0 (KB907265) letölthető <a href="http://go.microsoft.com/fwlink/?linkid=70638">Microsoft letöltőközpontjából</a> (http://go.microsoft.com/fwlink/?LinkId=70638 – lehet, hogy a hivatkozás angol nyelvű anyagra mutat).</p></td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><p>Microsoft Report Viewer</p></td>
<td style="border:1px solid black;"><p>Ez előfeltétele a WSUS 3.0 kezelőfelülete használatának. A Microsoft Report Viewer 2005 terjeszthető csomagja letölthető <a href="http://go.microsoft.com/fwlink/?linkid=70410">Microsoft letöltőközpontjából</a> (http://go.microsoft.com/fwlink/?LinkId=70410 – lehet, hogy a hivatkozás angol nyelvű anyagra mutat).</p></td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><p>SQL Server 2005 (választható)</p></td>
<td style="border:1px solid black;"><p>A WSUS 3.0 telepíti az Belső Windows-adatbázis kiszolgálót, ha az SQL Server kompatibilis verziója még nincs telepítve. Ha SQL Server alapú adatbázist kíván használni, legalább az SQL Server 2005 SP1 (elérhető a <a href="http://go.microsoft.com/fwlink/?linkid=66143">Microsoft letöltőközpontban</a> (http://go.microsoft.com/fwlink/?LinkId=66143) szükséges Windows Server 2003 rendszeren, illetve az SQL Server 2005 SP2 (elérhető a <a href="http://go.microsoft.com/fwlink/?linkid=84823">Microsoft letöltőközpontban</a> a következő címen: http://go.microsoft.com/fwlink/?LinkId=84823) szükséges Windows Server 2008 rendszeren.</p></td>
</tr>
</tbody>
</table>
  
| ![](images/Cc708491.note(WS.10).gif)Megjegyzés:                                                                                                                                                                                                                                                                                                                    |  
|-------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|  
| Ha korábban telepítve lett a számítógépre a WSUS 2.0 szolgáltatás, és az az SQL Server 2000, SQL Server Desktop Engine 2000 vagy más, az SQL Server 2005 SP1 (vagy Windows Server 2008 rendszeren SQL Server 2005 SP2) verziónál korábbi SQL Server alapú adatbázist használ, a WSUS 3.0 telepítőprogramja telepíti a Windows® Internal Database kiszolgálót, és áttelepíti erre az adatbázist. |
  
Lemezterületre vonatkozó követelmények a WSUS 3.0 kiszolgáló telepítéséhez  
--------------------------------------------------------------------------
  
A Windows Server Update Services telepítéséhez legalább az alábbi mennyiségű szabad lemezterületre van szükség:
  
-   1 GB a rendszerpartíción  
-   2 GB az adatbázisfájlok majdani tárolására szolgáló köteten  
-   20 GB a tartalom tárolására használt köteten
  
| ![](images/Cc708491.Important(WS.10).gif)Fontos:                                                  |  
|--------------------------------------------------------------------------------------------------------------------------------|  
| A WSUS 3.0 nem telepíthető tömörített meghajtókra. Mielőtt kiválasztaná a meghajtót, győződjön meg róla, hogy nincs tömörítve. |
  
A WSUS 3.0 frissítési követelményei  
-----------------------------------
  
#### A frissítés előtt ellenőrizze a WSUS meglévő telepítésének megfelelő működését, és készítsen biztonsági másolatot a WSUS adatbázisáról
  
Ha egy korábbi verzióról frissít a WSUS 3.0-s verziójára, a művelet végrehajtása előtt ellenőrizze a meglévő telepítés megfelelő működését, és készítsen biztonsági másolatot a WSUS adatbázisáról.
  
1.  Keresse meg a legutóbbi hibákat az eseménynaplókban, az alsóbb és a felsőbb rétegbeli kiszolgálók közötti szinkronizálási problémákat, illetve a nem jelentő ügyfelekkel kapcsolatos problémákat. A folytatás előtt ügyeljen ezeknek a problémáknak a megoldására.  
2.  A WSUS adatbázisában a megfelelő indexelés ellenőrzéséhez célszerű futtatni a DBCC CHECKDB parancsot. Erről a további tudnivalókat lásd: [DBCC CHECKDB](http://go.microsoft.com/fwlink/?linkid=86948) (http://go.microsoft.com/fwlink/?LinkId=86948).  
3.  Készítsen biztonsági másolatot a WSUS adatbázisáról.
  
#### El kell távolítani a Software Update Services 1.0 szolgáltatást
  
A WSUS 3.0 telepítése nem hajtható végre, ha a számítógépre telepítve van a Software Update Services 1.0 szolgáltatás, ezért a WSUS 3.0 telepítése előtt el kell távolítani a Software Update Services 1.0 szolgáltatást.
  
#### Nem támogatott a WSUS 3.0 bétaváltozatáról a WSUS 3.0 végleges RTM változatára való frissítés, megengedett azonban az RC változatáról az RTM változatra történő frissítés
  
Ha már telepítve van a WSUS 3.0 valamelyik bétaváltozata, a WSUS 3.0 RTM verziójának telepítése előtt el kell távolítani, és törölni kell az adatbázist. Csak az RC verzióról lehet frissíteni az RTM verzióra.
  
#### 64 bites operációs rendszeren nem lehet a WSUS 2.0 verzióról a WSUS 3.0 verzióra frissíteni
  
64 bites operációs rendszeren nem támogatott a WSUS 2.0 használata. 64 bites rendszeren nem lehet a WSUS 2.0 verzióról a WSUS 3.0 verzióra frissíteni
  
A telepítő parancssori paraméterei  
----------------------------------
  
A WSUS 3.0 telepítését felügyelet nélküli üzemmódban is elvégezheti a WSUS parancssori paraméterei segítségével. A táblázat a WSUS 3.0 parancssori paramétereit tartalmazza.
  
###  

<p> </p>
<table style="border:1px solid black;">
<colgroup>
<col width="50%" />
<col width="50%" />
</colgroup>
<thead>
<tr class="header">
<th>Kapcsoló</th>
<th>Leírás</th>
</tr>
</thead>
<tbody>
<tr class="odd">
<td style="border:1px solid black;"><p><strong>/q</strong></p></td>
<td style="border:1px solid black;"><p>Csendes telepítés végrehajtása.</p></td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><p><strong>/u</strong></p></td>
<td style="border:1px solid black;"><p>A termék eltávolítása. Eltávolítja a Belső Windows-adatbázis példányát is, ha az telepítve van.</p></td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><p><strong>/p</strong></p></td>
<td style="border:1px solid black;"><p>Csak az előfeltételek ellenőrzése. Nem telepíti a terméket, csak megvizsgálja a rendszert, és jelenti azokat az elemeket, ahol az előfeltételek nem teljesülnek.</p></td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><p><strong>/?, /h</strong></p></td>
<td style="border:1px solid black;"><p>A parancssori paramétereket és ezek leírását jeleníti meg.</p></td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><p><strong>/g</strong></p></td>
<td style="border:1px solid black;"><p>Frissítés a WSUS 2.0-s verziójáról. Ennél a beállításnál az egyetlen érvényes paraméter a /q (csendes telepítés). Ennél a beállításnál az egyetlen érvényes tulajdonság a DEFAULT_WEBSITE.</p></td>
</tr>
</tbody>
</table>
  
A táblázat a WSUS 3.0 parancssori tulajdonságait tartalmazza.
  
###  

<p> </p>
<table style="border:1px solid black;">
<colgroup>
<col width="50%" />
<col width="50%" />
</colgroup>
<thead>
<tr class="header">
<th>Tulajdonság</th>
<th>Leírás</th>
</tr>
</thead>
<tbody>
<tr class="odd">
<td style="border:1px solid black;"><p>CONTENT_LOCAL</p></td>
<td style="border:1px solid black;"><p>0=a tartalom helyben van tárolva, 1=tárolás a Microsoft Update webhelyen</p></td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><p>CONTENT_DIR</p></td>
<td style="border:1px solid black;"><p>A tartalomkönyvtár elérési útvonala. Az alapértelmezés szerinti érték a <em>WSUS_telepítési_meghajtó</em><strong>\WSUS\WSUSContent</strong>, ahol <em>WSUS_telepítési_meghajtó</em> a legnagyobb szabad területtel rendelkező helyi meghajtó.</p></td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><p>WYUKON_DATA_DIR</p></td>
<td style="border:1px solid black;"><p>A Belső Windows-adatbázis adatkönyvtárának elérési útvonala.</p></td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><p>SQLINSTANCE_NAME</p></td>
<td style="border:1px solid black;"><p>A nevet a <em>Kiszolgálónév</em>\<em>SQL_példány_neve</em> formátumban kell megadni. Ha az adatbázispéldány a helyi gépen található, használja a %COMPUTERNAME% környezeti változót. Ha nincs jelen egy már létező példány, akkor a %COMPUTERNAME%\WSUS az alapértelmezés.</p></td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><p>DEFAULT_WEBSITE</p></td>
<td style="border:1px solid black;"><p>0=8530-as port, 1=80-as port</p></td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><p>PREREQ_CHECK_LOG</p></td>
<td style="border:1px solid black;"><p>A naplófájl elérési útja és neve</p></td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><p>CONSOLE_INSTALL</p></td>
<td style="border:1px solid black;"><p>0=WSUS-kiszolgáló telepítése, 1=csak a konzol telepítése</p></td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><p>ENABLE_INVENTORY</p></td>
<td style="border:1px solid black;"><p>0=nem telepíti a leltárszolgáltatásokat, 1=telepíti a leltárszolgáltatásokat</p></td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><p>DELETE_DATABASE</p></td>
<td style="border:1px solid black;"><p>0=az adatbázis megőrzése, 1=az adatbázis eltávolítása</p></td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><p>DELETE_CONTENT</p></td>
<td style="border:1px solid black;"><p>0=a tartalomfájlok megőrzése, 1=a tartalomfájlok eltávolítása</p></td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><p>DELETE_LOGS</p></td>
<td style="border:1px solid black;"><p>0=naplófájlok megőrzése, 1=naplófájlok eltávolítása (az /u telepítési kapcsolóval használható).</p></td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><p>CREATE_DATABASE</p></td>
<td style="border:1px solid black;"><p>0=a jelenlegi adatbázis használata, 1=adatbázis létrehozása</p></td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><p>PROGRESS_WINDOW_HANDLE</p></td>
<td style="border:1px solid black;"><p>Az MSI folyamatjelző üzeneteinek visszaadására szolgáló ablakleíró</p></td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><p>MU_ROLLUP</p></td>
<td style="border:1px solid black;"><p>1=csatlakozás a Microsoft Update szolgáltatásainak javítását célzó programhoz, 0=a csatlakozás mellőzése</p></td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><p>FRONTEND_SETUP</p></td>
<td style="border:1px solid black;"><p>1=ne írja a tartalom helyét az adatbázisba, 0=írja be a tartalom helyét az adatbázisba (hálózati terheléselosztáshoz)</p></td>
</tr>
</tbody>
</table>
  
#### Példa
  
```  
WSUSSetup.exe /q DEFAULT\_WEBSITE=0 (install in quiet mode using port 8530) WSUSSetup.exe /q /u (uninstall WSUS)  
```  
| ![](images/Cc708491.Important(WS.10).gif)Fontos:                                                                                                                                |  
|--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|  
| Ha csendes üzemmódban (/q) telepíti a WSUS 3.0 szolgáltatást, és a gépre nincs telepítve minden előfeltétel, a telepítő létrehoz egy WSUSPreReqCheck.xml nevű fájlt, amelyet a %TEMP% könyvtárban helyez el. |
  
Telepítési problémák  
--------------------
  
#### Az IIS újraindul a WSUS 3.0 telepítése folyamán
  
A WSUS 3.0 telepítő figyelmeztetés nélkül újraindítja az IIS-t, és ez hatással lehet a szervezetben működő webhelyekre Ha nem fut az IIS, a WSUS 3.0 telepítője elindítja.
  
#### Ha a kapcsolatok nyitva vannak egy meglévő WSUS-adatbázis felé, lehet, hogy a telepítés sikertelen lesz
  
Ha egy meglévő verzióról frissít a WSUS 3.0 szolgáltatásra, és a kapcsolatok nyitva vannak egy létező WSUS-adatbázis felé (ha például az SQL Server Management Studio meg van nyitva), lehet, hogy a telepítés sikertelen lesz. Zárjon be minden kapcsolatot, és telepítse újra a WSUS 3.0 szolgáltatást.
  
#### A WSUS telepítője helytelenül jelzi ki az adatbázisfájlok könyvtárát
  
A WSUS telepítőjének **Kezdődhet a telepítés** képernyője tévesen arról számol be, hogy az adatbázis helye az adatbázis helyének szülőkönyvtára. Például %systemdrive%\\WSUS\\UpdateServicesDbFiles az alapértelmezett hely, de ez helytelenül így jelenik meg: %systemdrive%\\WSUS.
  
#### Ha a WSUS olyan számítógépen van telepítve, amelyen megtalálhatók a többnyelvű kezelőfelület nyelvi csomagjai, és az alapértelmezés szerinti nyelv nem az angol, a Súgó az angol helyett az alapértelmezett nyelven fog megjelenni
  
Olyan számítógépen, amelyen megtalálhatók a többnyelvű kezelőfelület nyelvi csomagjai, és az alapértelmezés szerinti nyelv nem az angol, a WSUS továbbra is telepíthető, ha az aktuális felhasználó nyelvi beállítása angol. A felhasználói felület angolul fog megjelenni, de a Súgó angol nyelvű megjelenítéséhez további lépések szükségesek. Másolja az angol nyelvű súgófájlt (*WSUS\_telepítési\_könyvtár*\\documentation\\mui\\0409\\WSUS30Help.chm) a központi dokumentációs könyvtárba (*WSUS\_telepítési\_könyvtár*\\documentation\\WSUS30Help.chm). Ekkor a súgónak minden nyelven megfelelően kell megjelennie.
  
Frissítési problémák  
--------------------
  
#### Amikor a WSUS 3.0 RC verziójáról frissít a WSUS 3.0 RTM verziójára, az SSL-tanúsítvány nem lesz hozzárendelve a WSUS webhelyéhez
  
A WSUS 3.0 RC verzióról a WSUS 3.0 RTM verzióra való frissítés törli, majd újból létrehozza a WSUS webhelyét. Ennélfogva az SSL-tanúsítvány már nem lesz hozzárendelve a WSUS webhelyéhez. A frissítés után újból végre kell hajtania a tanúsítvány hozzárendelését.
  
#### Sikertelen frissítés javítása
  
Ha WSUS 2.0 verzióról frissít a WSUS 3.0 szolgáltatásra, és a frissítés bármilyen okból kifolyólag sikertelen, újra kell telepíteni a WSUS 2.0 szolgáltatást, és vissza kell állítani az adatbázist a biztonsági másolatból.
  
#### Nem lehet a WSUS 2.0 verzióról WSUS 3.0 verzióra frissíteni, ha létezik a korábbi telepítésből származó WSUS 3.0-adatbázis
  
Ha korábban telepítette a WSUS 3.0 szolgáltatást, majd újratelepítette a WSUS 2.0 verziót, a WSUS 3.0 újratelepítése előtt törölni kell a WSUS 3.0-adatbázist a gépről.
  
#### A számítógép nevének a WSUS 3.0-s verziójára való frissítés előtti módosítása azt eredményezi, hogy sikertelen lesz a frissítés
  
Ha módosítja a számítógép nevét a WSUS 2.0 telepítése és a WSUS 3.0 verzióra történő frissítés között, az a frissítés sikertelenségéhez vezethet.
  
Távolítsa el, majd adja újra hozzá az ASPNET és a WSUS-rendszergazdák csoportot. Ezután futtassa a frissítést.
  
Az *&lt;adatbázis\_helye&gt;* változó helyére azt a mappát kell beírnia, amelybe az adatbázis telepítve van, a *&lt;tartalmi\_könyvtár&gt;* helyére pedig a helyi tárolómappát.
  
```  
sqlcmd.exe -S *&lt;DBLocation&gt;* -E -Q "USE SUSDB DECLARE @asplogin varchar(200) SELECT @asplogin=name from sysusers WHERE name like '%ASPNET' EXEC sp\_revokedbaccess @asplogin" sqlcmd.exe -S *&lt;DBLocation&gt;* -E -Q "USE SUSDB DECLARE @wsusadminslogin varchar(200) SELECT @wsusadminslogin=name from sysusers WHERE name like '%WSUS Administrators' EXEC sp\_revokedbaccess @wsusadminslogin"   sqlcmd.exe -S *&lt;DBLocation&gt;* -E -Q "USE SUSDB DECLARE @asplogin varchar(200) SELECT @asplogin=HOST\_NAME()+'\\ASPNET' EXEC sp\_grantlogin @asplogin EXEC sp\_grantdbaccess @asplogin EXEC sp\_addrolemember webService,@asplogin" sqlcmd.exe -S *&lt;DBLocation&gt;* -E -Q "USE SUSDB DECLARE @wsusadminslogin varchar(200) SELECT @wsusadminslogin=HOST\_NAME()+'\\WSUS Administrators' EXEC sp\_grantlogin @wsusadminslogin EXEC sp\_grantdbaccess @wsusadminslogin EXEC sp\_addrolemember webService,@wsusadminslogin"   sqlcmd.exe -S *&lt;DBLocation&gt;* -E -Q "backup database SUSDB to disk=N'*&lt;ContentDirectory&gt;*\\SUSDB.Dat' with init"  
```
  
#### A telepítő felülírhatja az adatbázis egy korábbi biztonsági másolatát
  
A WSUS 3.0 a telepítés során megadott könyvtárban helyezi el az adatbázist. Ez alapértelmezés szerint a *%systemdrive%*\\WSUS\\UpdateServicesDbFiles könyvtár. Ha ebben a könyvtárban megtalálható az adatbázis egy korábbi biztonsági másolata, akkor azt az új adatbázis felülírja. A rendszergazdáknak biztonsági másolatot tanácsos készíteniük az adatbázisról, mielőtt alkalmaznák a frissítéseket arra a számítógépre, amelyen az adatbázis található.
  
#### MSDE áttelepítésekor SQL Server 2000 vagy SQL Server 2005 kiszolgálóra WSUS 2.0-s rendszeren módosítania kell egy beállításértéket
  
Ha a WSUS 2.0 telepítve van, és SQL Server 2000 vagy SQL Server 2005 rendszerről történt az áttelepítés, a **HKLM\\SOFTWARE\\Microsoft\\Update Services\\Server\\Setup\\WmsdeInstalled** beállítás értékét 1-ről 0-ra kell módosítani. Ha ezt elmulasztja a WSUS 3.0 rendszerre frissítés előtt, a frissítés sikertelen lesz.
  
#### A WSUS 2.0 telepítésének elindítása és megszakítása törli a WSUS rendszerleíró kulcsát
  
He elindítja, majd megszakítja WSUS 2.0 telepítését, az törli a WSUS rendszerleíró kulcsát. Ez problémákat okozhat, ha már telepítve van a WSUS 3.0-s verziója. Ugyanez a probléma jelentkezik, ha elkezdi eltávolítani a WSUS 2.0-s verzióját, megszakítja ezt a folyamatot, majd megpróbál frissíteni a WSUS 2.0-s verziójáról a WSUS 3.0-s verziójára.
  
#### Ha eltávolítja a WSUS 3.0 szolgáltatást, de meghagyja a naplófájlokat, lehet, hogy helytelenek lesznek az engedélyeik az esetleges újratelepítés után
  
Amikor eltávolítja a WSUS 3.0 szolgáltatást, választhatja azt, hogy megtartja a telepítés naplófájljait. Amikor újratelepíti a WSUS 3.0 szolgáltatást, a régi naplófájlok elveszítik az engedélyeiket (általában csak a WSUS-rendszergazdák esetében). Vissza kell állítani a naplófájlokra vonatkozó engedélyeket.
  
#### Ha a Windows SharePoint Services szolgáltatást a WSUS 3.0 RC változata után telepítették, csak egy megkerülő megoldással végezhető el sikeresen a WSUS 3.0 RTM változatára való frissítés
  
Ha telepítette a WSUS 3.0 RC változatát, majd ugyanarra a számítógépre telepítette a Windows SharePoint Services szolgáltatást, csak akkor tud frissíteni a WSUS 3.0 RTM változatára, ha az egyéni portra (a 8530-as portra) való telepítést választja. Ha a parancssorból szeretné elvégezni az ilyen telepítést, nyisson meg egy parancssorablakot, majd adja ki a következő parancsot: **WSUSSetup /q / g/ DEFAULT\_WEBSITE=0**. (Ha a kezelőfelületről szeretné elvégezni az ilyen telepítést, adja ki a **WSUSSetup /g DEFAULT\_WEBSITE=0** parancsot.)
  
Ha a WSUS olyan számítógépen van telepítve, amelyen megtalálhatók a többnyelvű kezelőfelület nyelvi csomagjai, a Súgó a felhasználó aktuális nyelve helyett az alapértelmezés szerinti nyelven fog megjelenni
  
#### Ha a WSUS 2.0 ügyfelek „Nem vonatkozik rá” állapotú frissítéseket tartalmaznak, ezek állapota rövid időre „Ismeretlen” lesz a WSUS 3.0 rendszerre frissítés után
  
Ha egy WSUS 2.0 kiszolgálóhoz „Nem vonatkozik rá” állapotú frissítéseket tartalmazó ügyfelek tartoznak, ezek a frissítések rövid időre „Ismeretlen” állapotúvá válnak a kiszolgáló WSUS 3.0 rendszerre frissítése után. A „Nem vonatkozik rá” állapot tér vissza, miután az ügyfél legközebb ellenőrzést hajt végre.
  
Ismert problémák  
----------------
  
#### Többszörös letöltési hiba vagy az ügyfelek szinkronizálásának ismétlődő sikertelensége
  
Ha a WSUS 3.0-ügyfelek többszörös letöltési hibát jelentenek, vagy ha az ügyfelek hosszabb ideig nem tudnak szinkronizálni a WSUS 3.0-kiszolgálóval, lehet, hogy sérült az ügyfél letöltési gyorsítótára. Megoldhatja a problémát, ha törli az ügyfél letöltési gyorsítótárát a fájlrendszerből.
  
Az ügyfél letöltési gyorsítótárának törlése:
  
1.  Töröljön minden fájlt és alkönyvtárat az ügyfélszámítógép következő helyéről: **%windir%\\SoftwareDistribution\\Download**  
2.  Ismét próbálja meg telepíteni a frissítést az ügyfélszámítógép WSUS 3.0-kiszolgálóval történő szinkronizálásával. A telepítési kísérlet sikertelen lesz, és a következő hibaüzenet jelenik meg: **WU\_E\_DM\_NOTDOWNLOADED, "A frissítés letöltése nem történt meg".**  
3.  Ezt követően az ügyfélszámítógép automatikusan újraindítja a letöltést, és a telepítést ekkor végre lehet hajtani.
  
#### Szinkronizálási hiba esetén meg kell ismételni a szinkronizálást
  
Ha a szinkronizálás sikertelen, a hibaelhárítás első lépéseként újból meg kell próbálni szinkronizálni a kiszolgálót. Ha ismét sikertelen a szinkronizálás, a [WSUS 3.0 üzemeltetési útmutatójában](http://go.microsoft.com/fwlink/?linkid=81072) talál útmutatást a hiba elhárításával kapcsolatban (http://go.microsoft.com/fwlink/?LinkId=81072 – lehet, a hivatkozás angol nyelvű anyagra mutat).
  
#### A WSUS 3.0 konfigurációjának közvetlenül az adatbázisban történő módosítását nem támogatjuk
  
A Windows Server Update Services szolgáltatás konfigurációs adatait egy SQL Server-adatbázis tárolja. A konfigurációs adatoknak közvetlenül az adatbázisban való módosítását azonban nem támogatjuk. Ne próbálkozzon tehát azzal, hogy közvetlenül az adatbázisban módosítja a WSUS 3.0 konfigurációját. Használja erre a célra a WSUS 3.0 konzolt vagy a WSUS 3.0 API-kat.
  
#### Lassan jelenti a rendszer a letöltés sikertelenségét, ha be vannak kapcsolva a merevlemezkvóták
  
Ha be vannak kapcsolva a merevlemezkvóták, és az adatok mennyisége eléri ezt a kvótát, előfordulhat, hogy nem érkezik meg időben a WSUS kiszolgálóra való letöltések esetleges sikertelenségének jelentése. A probléma elkerülhető, ha kikapcsolja a merevlemezkvótákat, vagy megnöveli a megfelelő kvótát.
  
#### Ha a WSUS 3.0 üzembe helyezése az SSL protokollal történik, előfordulhat, hogy az ügyfélszámítógépek telepítése leáll a 0x8024400a hibakóddal
  
Előfordulhat, hogy az ügyfélszámítógépek telepítése leáll a „0x8024400a” hibakóddal egy, az SSL protokollt használó WSUS 3.0-kiszolgálóval való kommunikáció közben. Az ezt a problémát kezelő frissítés megtalálható a [KB 905422](http://go.microsoft.com/fwlink/?linkid=70593) számú javításban (http://go.microsoft.com/fwlink/?LinkId=70593 – lehet, hogy a hivatkozás angol nyelvű anyagra mutat).
  
#### A WSUS-rendszergazdák tartományi fiók nem törlődik a WSUS eltávolítása esetén
  
A WSUS-rendszergazdák csoportja tartományi fiókként (és nem helyi fiókként) jön létre a tartományvezérlőkön, így az ezt a tartományi fiókot használó telepítések működésképtelenné válnának, ha a fiók törlődne a WSUS eltávolítása során. A WSUS eltávolításával tehát a WSUS-rendszergazdák tartományi fiók nem törlődik.
  
#### Ha egy alsóbb rétegbeli kiszolgálót felsőbb rétegbeli kiszolgálóvá alakít át, újra kell importálni a katalóguswebhelyről származó frissítéseket
  
Amikor egy alsóbb rétegbeli kiszolgálót felsőbb rétegbeli kiszolgálóvá léptet elő, a katalóguswebhely összes frissítéseit is újból importálnia kell. Ellenkező esetben a webhely nem fogja szinkronizálni erre a kiszolgálóra a katalóguswebhely frissítéseinek új verzióit.
  
#### Bár az SSL protokollal használja az IIS szolgáltatást, mégis lehetőség nyílik a titkosítatlan hozzáférésre, hacsak nincs bejelölve a „Biztonságos csatorna szükséges” beállítás
  
Bár azt állítja be, hogy az IIS szolgáltatás az SSL protokollt használja, és telepíti a szükséges tanúsítványt, a titkosítatlan hozzáférés mégis lehetséges, hacsak nincs bejelölve a „Biztonságos csatorna szükséges” beállítás. További tájékoztatás a [titkosítás engedélyezését ismertető útmutatóban](http://go.microsoft.com/fwlink/?linkid=70601) olvasható (http://go.microsoft.com/fwlink/?LinkId=70601 – lehet, hogy a hivatkozás angol nyelvű anyagra mutat).
  
#### A katalóguswebhelyről történő importálás leállhat, ha nincs írási és olvasási jogosultsága a %windir%\\TEMP mappához
  
Ha a Hálózati szolgáltatás fióknak nincs írási és olvasási joga a %windir%\\TEMP mappához a katalóguswebhelyről történő importálás során, az importálás leállhat a következő hibaüzenettel: „A kiszolgáló nem tudta feldolgozni a kérelmet. ---&gt; A fájl nem található: 'C:\\WINDOWS\\TEMP\\*ideiglenes\_fájl\_neve*.dll'."
  
#### Előfordulhat, hogy lassú a szinkronizálás a WSUS 3.0 és egy, a WSUS 2.0 szolgáltatást futtató alsóbb rétegbeli replikakiszolgáló között
  
Ha a WSUS 3.0 szolgáltatást telepíti egy felsőbb rétegbeli kiszolgálóra, és megpróbál szinkronizálást végezni egy, a WSUS 2.0 szolgáltatást futtató alsóbb rétegbeli replikakiszolgálóval, teljesítményproblémák léphetnek fel. A probléma megoldásáról a [KB 910847](http://go.microsoft.com/fwlink/?linkid=70669) dokumentum tartalmaz tájékoztatást (http://go.microsoft.com/fwlink/?LinkId=70669 – lehet, hogy a hivatkozás angol nyelvű tartalomra mutat).
  
#### Ha a levelezőkiszolgáló nem működik vagy nem lehet elérni, az értesítő e-mailek figyelmeztetés nélkül sikertelenek lesznek
  
Ha a hálózati levelezőkiszolgáló nem csatlakozik a hálózathoz, a WSUS 3.0 figyelmeztetés nélkül abbahagyja az értesítő e-mailek küldését. Beírja azonban az 10052-es számú eseményt (HealthCoreEmailNotificationRed) az eseménynaplóba.
  
#### A felsőbb rétegbeli kiszolgálón végzett módosításokat nem küldi le azonnal a rendszer az alsóbb rétegbeli kiszolgálónak
  
A felsőbb rétegbeli kiszolgáló konfigurációjának módosítását követően hosszabb idő is eltelhet, mire a módosítások valóban érvénybe lépnek. Ha például a felsőbb rétegbeli kiszolgálón új nyelvet választ, és ezután azonnal szinkronizálást indít el az alsóbb rétegbeli kiszolgálón, a változtatás nem fog megjelenni. Ez csak a következő ütemezett szinkronizáláskor kerül az alsóbb rétegbeli kiszolgálóra. A várakozási idő a felsőbb rétegbeli kiszolgálón található frissítések számától függ.
  
#### A WSUS 3.0 eltávolítása nem távolítja el az adatbázispéldányt
  
A WSUS 3.0 eltávolítása nem távolítja el az adatbázispéldányt. Lehet, hogy több alkalmazás használja az adatbázispéldányt, így az eltávolítása meghiúsítaná azok működését.
  
Ha el kell távolítani a Belső Windows-adatbázis összetevőt, a következő parancsokat használhatja:
  
(32 bites platformokon)
  
```  
msiexec /x {CEB5780F-1A70-44A9-850F-DE6C4F6AA8FB} callerid=ocsetup.exe  
```  
(64 bites platformokon)
  
```  
msiexec /x {BDD79957-5801-4A2D-B09E-852E7FA64D01} callerid=ocsetup.exe  
```  
Ha el szeretné távolítani a Belső Windows-adatbázis Service Pack 2 verzióját a Windows Server 2008 rendszerről, akkor ezt a Kiszolgálókezelővel teheti meg.
  
Előfordulhat, hogy az alkalmazás eltávolítása nem eredményezi az alapértelmezett .mdf és .ldf fájlok eltávolítását, és ennek következtében a WSUS 3.0 ezt követő telepítése sikertelen lehet. Ezek a fájlok törölhetők a %windir%\\SYSMSI\\SSEE könyvtárból.
  
#### Ha módosul egy alsóbb rétegbeli kiszolgáló felsőbb rétegbeli kiszolgálója, az „Ismeretlen” állapotú frissítések „Nem vonatkozik rá” állapotúként szerepelnek a jelentésekben
  
Ha egy alsóbb rétegbeli kiszolgáló egy másik felsőbb rétegbeli kiszolgálóról kezd el szinkronizálni, az „Ismeretlen” állapotú frissítések „Nem vonatkozik rá” állapotúként szerepelnek az új felsőbb rétegbeli kiszolgáló jelentéseiben. Ez az állapot ideiglenes, és amint az alsóbb rétegbeli kiszolgáló legközelebb jelenti az állapotát, miután a hozzá tartozó ügyfelek szinkronizálódtak vele, az állapot helyesen fog megjelenni.
  
#### Ha egy WSUS 3.0-replikakiszolgáló egyszerre egynél több számítógépet kezel, leáll a jelentések összegzése
  
Ha egy WSUS 3.0-replikakiszolgáló egyszerre egynél több számítógépet kezel, leáll a jelentések összegzése. Ennek következtében a gyökér WSUS-kiszolgálón elérhető jelentések hiányosak lesznek. Ezt a problémát úgy lehet megoldani, ha az egyik kivételével törli a replikakiszolgálóról az ismétlődő számítógép-bejegyzéseket.
  
#### Ha a Kiszolgáló karbantartása varázsló több kiszolgálón fut egy távoli konzolról, és az egyik kiszolgálón túllépi az időkorlátot, mindegyik kiszolgálóval megszakad a kapcsolat
  
A Kiszolgáló karbantartása varázsló futtatható több kiszolgálón egyetlen távoli konzolról. Ha azonban a karbantartási folyamat túllépi az időkorlátot az egyik kiszolgálón, a konzol kapcsolata mindegyik kiszolgálóval megszakad. Adatok nem vesznek el, a rendszergazdának viszont vissza kell állítania a távoli kapcsolatot mindegyik kiszolgálón.
  
#### A Kiszolgáló karbantartása varázsló nem három hónap, hanem harminc nap elmúltával törli a fájlokat
  
A Kiszolgáló karbantartása varázslóban megjelenő szöveg egy része pontatlanul van megfogalmazva. Így szól: "Az érvényüket vesztett és a három hónapja jóvá nem hagyott frissítések törlése, valamint a három hónapja jóvá nem hagyott új frissítésverziók törlése." A helyes időtartam nem három hónap, hanem harminc nap.
  
#### A kapcsolat gyors egymásutánban történő elindítása és leállítása a „nincs hiba” hibaüzenet megjelenítését eredményezi a konfigurálási varázslóban
  
A WSUS konfigurálása során kapcsolódni kell a felsőbb rétegbeli kiszolgálóhoz (vagy a Microsoft Update webhelyhez, vagy az intranetes felső rétegbeli kiszolgálóhoz), hogy alapvető információkat vigyen át a kiszolgálóról. Ha rákattint a **Kapcsolódás indítása** elemre, majd közvetlenül utána a **Kapcsolódás leállítása** elemre, akkor a következő téves hibaüzenet jelenik meg: „Nem történt szinkronizálási hiba.”
  
#### A Windows Vista RTM verzióját használó WSUS-ügyfelek mostantól meg tudják keresni a frissítéseket a Microsoft Update webhelyen
  
A WSUS korábbi verzióiban csak a WSUS-kiszolgálótól tudták letölteni a frissítést a Windows Vista RTM rendszerű ügyfelek. Most megjelent a WSUS 3.0 RTM verziója, és így a Microsoft Update webhelyről is le tudják tölteni a frissítéseket a Vista-ügyfelek. Úgy irányíthatja át a Vista-ügyfeleket a Microsoft Update webhelyre, hogy megnyitja a Windows Update párbeszédpanelt a Vezérlőpultról, majd rákattint az **Online frissítések keresése a következő forrásnál: Microsoft Update szolgáltatás** hivatkozásra. Ha be van kapcsolva **Az összes Windows Update-funkció hozzáférésének tiltása** csoportházirend-beállítás, akkor a Windows Update nem jeleníti meg a hivatkozást.
  
WSUS 3.0 Windows Server 2008 rendszeren  
---------------------------------------
  
#### Támogatott verziók
  
A WSUS 3.0 támogatja a Windows Server 2008 rendszer 32 és 64 bites verzióit is.
  
#### Előfeltételek
  
###  

<p> </p>
<table style="border:1px solid black;">
<colgroup>
<col width="50%" />
<col width="50%" />
</colgroup>
<thead>
<tr class="header">
<th>Követelmény</th>
<th>Részletek</th>
</tr>
</thead>
<tbody>
<tr class="odd">
<td style="border:1px solid black;"><p>Microsoft Internet Information Services (IIS)</p></td>
<td style="border:1px solid black;"><p>Az operációs rendszerből telepíthető. A következő összetevőknek engedélyezve kell lenniük:</p>
<p>Windows-hitelesítés</p>
<p>Statikus tartalom</p>
<p>ASP.NET</p>
<p>6.0 – kezeléskompatibilitás</p>
<p>IIS – metabázis-kompatibilitás</p></td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><p>Microsoft .NET-keretrendszer 2.0-s verziójának terjeszthető csomagja (x86)</p></td>
<td style="border:1px solid black;"><p>A Windows Server 2008 rendszeren nem szükséges, az operációs rendszer részeként települ.</p></td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><p>Microsoft Management Console 3.0</p></td>
<td style="border:1px solid black;"><p>A Windows Server 2008 rendszeren nem szükséges, az operációs rendszer részeként települ.</p></td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><p>Microsoft Report Viewer</p></td>
<td style="border:1px solid black;"><p>Ez előfeltétele a WSUS kezelőfelülete használatának. Lásd a Microsoft Report Viewer 2005 terjeszthető csomagját a <a href="http://go.microsoft.com/fwlink/?linkid=70410">Microsoft letöltőközpontjában</a> (http://go.microsoft.com/fwlink/?LinkId=70410).</p></td>
</tr>
</tbody>
</table>
  
#### 1. probléma: Az IIS 7.0 konfigurációs fájlját frissíteni kell a WSUS 3.0 futtatása előtt
  
Mielőtt futtatná a WSUS 3.0 alkalmazást a Windows Server 2008 rendszeren, frissítenie kell az IIS konfigurációs fájlját. Ehhez a következő lépéseket kell végrehajtania:
  
1. Nyissa meg az ISS konfigurációs fájlját: %WINDIR%\\system32\\inetsrv\\applicationhost.config
  
2. Törölje a &lt;System.webServer&gt;&lt;modules&gt; címkénél az esetleges &lt;add name="CustomErrorMode"&gt; bejegyzést.
  
3. Törölje a &lt;System.webServer&gt;&lt;modules&gt; címkénél az esetleges &lt;remove name="CustomErrorMode"&gt; bejegyzést.
  
Ennek eredményeképpen ilyen címkének kell keletkeznie:
  
```  
 &lt;System.webServer&gt; &lt;modules&gt; &lt;remove name="CustomErrorMode"&gt; &lt;/modules&gt; &lt;/System.webServer&gt;  
```
  
#### 2. probléma: Ha a Windows Server 2008 3-as béta verziójának egyéni portjára kívánja telepíteni a WSUS 3.0 összetevőt, előzetesen létre kell hoznia a webhelyet
  
Ha a WSUS 3.0 telepítését a Windows Server 2008 3-as béta verzióján kívánja végrehajtani, és a 8530-as egyéni port használatát szeretné beállítani, a WSUS telepítőprogramjának elindítása előtt létre kell hoznia egy „WSUS Administration” nevű webhelyet a 8530-as porton.
  
A WSUS 3.0 szolgáltatás a Windows Small Business Server 2003 rendszeren  
-----------------------------------------------------------------------
  
#### 1. probléma: Ha az IIS virtuális gyökér korlátozva van bizonyos IP-címekre vagy tartománynevekre, a WSUS 3.0 kiszolgáló nem fogja tudni magát frissíteni
  
Előfordulhat, hogy a Windows Small Business Server telepített példányán az alapértelmezett IIS webhelyre vonatkozóan be van állítva az „IP-cím és tartománynév korlátozása”. Ebben az esetben előfordulhat, hogy a kiszolgálón futó Windows Update ügyfél nem tudja frissíteni magát.
  
#### 2. probléma: A WSUS 3.0 telepítése Small Business Server operációs rendszerre – együttműködési problémák
  
-   Ha a Windows Small Business Server 2003 egy ISA proxykiszolgálót használ az internet eléréséhez, a következő adatok kell megadnia a **Beállítások** felhasználói felületen: a proxykiszolgáló beállításait, a proxykiszolgáló nevét és a proxykiszolgáló portszámát.  
-   Ha az ISA Windows-hitelesítést igényel, a proxykiszolgáló hitelesítő adatait a következő formátumban kell megadni: „TARTOMÁNY\\felhasználó”, és a felhasználónak az „Internetfelhasználók” csoportba kell tartoznia.
  
#### 3. probléma: Ha a Windows SBS varázslóinak használata nélkül adott alhálózatot a hálózathoz, végre kell hajtani az alábbi műveleteket
  
A WSUS-kiszolgáló telepítője két IIS virtuális gyökeret telepít a kiszolgálóra: a SelfUpdate és a ClientWebService nevűt. Ezenfelül néhány fájlt elhelyez a 80-as porton lévő alapértelmezett webhely kezdőkönyvtárába, amelyek segítségével az ügyfélszámítógépek az alapértelmezett webhelyen keresztül frissíthetik önmagukat. Alapértelmezés szerint az alapértelmezett webhely úgy van beállítva, hogy a localhost címen és a kiszolgálóhoz kapcsolódó megadott alhálózatokon kívül minden IP-címhez megtagadja a hozzáférést. Ennek következtében a nem a helyi állomáshoz vagy a megadott alhálózatokhoz tartozó ügyfélszámítógépek nem tudják önmagukat frissíteni. Ha a Microsoft Windows Small Business Server 2003 (Windows SBS) varázslói nélkül adott alhálózatot a hálózathoz, végre kell hajtania a következő műveleteket.
  
1.  Bontsa ki a Kiszolgálókezelés eszközben a **Speciális kezelés**, az **Internet Information Services**, a **Webhelyek**, majd az **Alapértelmezett webhely** elemet, kattintson a jobb gombbal a **Selfupdate** virtuális könyvtárra, végül kattintson a **Tulajdonságok** elemre.  
2.  Kattintson a **Könyvtárbiztonság** fülre.  
3.  Kattintson az **IP-cím és tartománynév korlátozása** csoportban a **Szerkesztés** gombra, majd a **hozzáférése engedélyezve** lehetőségre.  
4.  Kattintson az **OK** gombra, kattintson a jobb gombbal a **ClientWebService** virtuális könyvtárra, majd kattintson a **Tulajdonságok** pontra.  
5.  Kattintson a **Könyvtárbiztonság** elemre.  
6.  Kattintson az **IP-cím és tartománynév korlátozása** csoportban a **Szerkesztés** gombra, majd a **hozzáférése engedélyezve** lehetőségre.
  
#### Szerzői jogi tudnivalók
  
Ez a dokumentum egy szoftvertermék előzetes kiadásához nyújt tájékoztatást, amely nagy mértékben változhat a végleges, kereskedelmi forgalomba kerülő kiadás előtt. A dokumentum a Microsoft Corporation tulajdonában lévő, bizalmas információkat tartalmaz. Kiadása a felhasználó és a Microsoft közötti titoktartási szerződés szerint történik. A dokumentum csak tájékoztatási célokat szolgál, a Microsoft nem vállal sem kifejezett, sem hallgatólagos garanciát a dokumentumban foglaltakkal kapcsolatban. A jelen dokumentumban található adatok, az URL-címeket és más internetes weblapokra mutató hivatkozásokat is beleértve, előzetes bejelentés nélkül megváltozhatnak. A dokumentumban foglaltak felhasználásának kockázatát teljes mértékben a felhasználó viseli. A dokumentum példáiban szereplő vállalatok, szervezetek, termékek, tartománynevek, e-mail címek, emblémák, személyek, helyek és események a képzelet szüleményei. Az ettől eltérő eseteket külön jelezzük. A valódi vállalatokkal, szervezetekkel, termékekkel, tartományokkal, e-mail címekkel, emblémákkal, személyekkel, helyekkel vagy eseményekkel fennálló hasonlóság a véletlen műve. Az összes vonatkozó szerzői jogi rendelkezés és törvény betartása a felhasználó felelőssége. A bejegyzett szerzői jogok korlátozásait figyelembe véve a Microsoft Corporation kifejezett írásbeli engedélye nélkül a dokumentum egyetlen része sem másolható, nem rögzíthető és nem tárolható visszakereshető rendszerben. Továbbítása semmiféle formában és semmilyen módon (elektronikus, mechanikai, fénymásolás, hangrögzítési vagy más eljárással) vagy célból nem engedélyezett.
  
A Microsoft olyan szabadalmakkal, szabadalmaztatott alkalmazásokkal, védjegyekkel, szerzői jogokkal vagy egyéb szellemi tulajdonjogokkal rendelkezhet, amelyek benne foglaltatnak e dokumentumban. Hacsak a Microsoft valamelyik írásos licencszerződése másként nem rendelkezik, a jelen dokumentum rendelkezésre bocsátása nem jogosítja fel a felhasználót ezen szabadalmak, védjegyek, szerzői jogok vagy egyéb szellemi tulajdon használatára.
  
© 2007 Microsoft Corporation. Minden jog fenntartva.
  
A Microsoft és a Windows szó, valamint az SQL Server és a Windows Server szóösszetétel a Microsoft Corporation Amerikai Egyesült Államokban, illetve más országokban bejegyeztetett (kereskedelmi) védjegye.
  
Minden egyéb kereskedelmi védjegy a tulajdonosa védjegye.
