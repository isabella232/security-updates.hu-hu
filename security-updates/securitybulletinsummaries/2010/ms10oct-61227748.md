---
TOCTitle: 'MS10-OCT'
Title: 'A Microsoft biztonsági közleményei – összefoglalás, 2010. október'
ms:assetid: 'ms10-oct'
ms:contentKeyID: 61227748
ms:mtpsurl: 'https://technet.microsoft.com/hu-HU/library/ms10-oct(v=Security.10)'
---

Security Bulletin Summary

A Microsoft biztonsági közleményei – összefoglalás, 2010. október
=================================================================

Közzétéve: 2010. október 12. | Frissítve: 2011. október 26.

**Verzió:** 4.1

Az összefoglaló a 2010 októberében kiadott biztonsági közleményeket összegzi.

A 2010. októberi közlemények kiadása folytán az összefoglaló a 2010. október 7-én kiadott előzetes értesítés helyébe lép. További információkat a biztonsági közlemények kiadásáról szóló előzetes értesítési szolgáltatásról lásd: [Előzetes értesítés a Microsoft biztonsági közleményeinek kiadásáról](http://technet.microsoft.com/security/bulletin/advance).

Ha automatikus értesítést szeretne kapni a Microsoft biztonsági közleményeinek megjelenéséről, fizessen elő a [Microsoft Technical Security Notifications](http://go.microsoft.com/fwlink/?linkid=21163) szolgáltatásra.

A közleményekkel kapcsolatos kérdések megválaszolására a Microsoft 2010. október 13-án, csendes-óceáni idő szerint 11 órakor webes szemináriumot tart. [Jelentkezzen most az októberi közleményeket bemutató webes szemináriumra](https://msevents.microsoft.com/cui/eventdetail.aspx?eventid=1032454437&culture=en-us). Ezt követően a webes szeminárium igény szerint kerül megrendezésre. További információkért látogasson el a [Microsoft biztonsági közleményeit és a webes szemináriumokat](http://technet.microsoft.com/security/bulletin/summary) bemutató oldalra.

A Microsoft abban is segítséget nyújt felhasználóinak, hogy a havi biztonsági közleményekkel azonos napon kiadott, nem biztonsági jellegű, de fontos frissítéseket megfelelően rangsorolhassák. Lásd az **Egyéb információ című részt**.

### A közleménnyel kapcsolatos információk

Összefoglalások
---------------

<span></span>
A következő táblázat összegzi az e havi biztonsági közleményeket súlyossági sorrendben.

Az érintett szoftverekkel kapcsolatban további tudnivalókat a következő, az **Érintett szoftverek és letöltési helyek** című részben talál.

 
<p> </p>
<table style="border:1px solid black;">
<colgroup>
<col width="20%" />
<col width="20%" />
<col width="20%" />
<col width="20%" />
<col width="20%" />
</colgroup>
<thead>
<tr class="header">
<th style="border:1px solid black;" >Közlemény azonosítója</th>
<th style="border:1px solid black;" >Közlemény címe és összefoglalás</th>
<th style="border:1px solid black;" >Súlyosság maximális foka és a biztonsági rés hatása</th>
<th style="border:1px solid black;" >Újraindítás szükségessége</th>
<th style="border:1px solid black;" >Érintett szoftverek</th>
</tr>
</thead>
<tbody>
<tr class="odd">
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=202013">MS10-071</a></td>
<td style="border:1px solid black;"><strong>Összesítő biztonsági frissítés az Internet Explorer programhoz (2360131)</strong><br />
<br />
A biztonsági frissítés hét közvetlenül és három nyilvánosan jelentett biztonsági rést szüntet meg az Internet Explorer programban. A súlyosabb biztonsági rések távoli kódfuttatást tesznek lehetővé, amennyiben a felhasználó speciálisan kialakított weboldalt tekint meg az Internet Explorer alkalmazással. A kevesebb jogosultsággal bíró fiókkal rendelkező felhasználók esetében kisebb a veszélyeztetettség, mint a rendszergazdai jogosultságokkal rendelkezők esetén</td>
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=21140">Kritikus</a><br />
Távoli kódfuttatás</td>
<td style="border:1px solid black;">Újraindítást igényel</td>
<td style="border:1px solid black;">Microsoft Windows,<br />
Internet Explorer</td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=201722">MS10-075</a></td>
<td style="border:1px solid black;"><strong>A Media Player hálózatmegosztó szolgáltatása távoli programkódfuttatást tesz lehetővé (2281679)</strong><br />
<br />
A biztonsági frissítés a Microsoft Windows Media Player hálózatmegosztó szolgáltatásának közvetlenül jelentett biztonsági rését szünteti meg. A biztonsági rés távolról történő programkódfuttatást tehet lehetővé, ha a támadó speciálisan kialakított RTSP-csomagot küld az érintett rendszernek. Ez annak ellenére tapasztalható, hogy az otthoni médiák internet-hozzáférése alapértelmezésben le van tiltva. Ebben az alapkonfigurációban a biztonsági rést csak azonos alhálózaton tartózkodó támadó használhatja ki.</td>
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=21140">Kritikus</a><br />
Távoli kódfuttatás</td>
<td style="border:1px solid black;">Esetleg újra kell indítani a rendszert</td>
<td style="border:1px solid black;">Microsoft Windows</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=194560">MS10-076</a></td>
<td style="border:1px solid black;"><strong>A beágyazott OpenType betűtípusmotor biztonsági rése távolról történő kódfuttatást tehet lehetővé (982132)</strong><br />
<br />
A biztonsági frissítés egy közvetlenül jelentett biztonsági rést szüntet meg a Microsoft Windows beágyazott OpenType (EOT) betűtípusmotor nevű összetevőjében. A biztonsági rés távolról történő programkódfuttatást tehet lehetővé. Ha egy támadó sikeresen kihasználja a biztonsági rést, teljes mértékben átveheti az érintett rendszer távoli irányítását. Ezt követően programokat telepíthet, illetve adatokat tekinthet meg, módosíthat és törölhet, de korlátozás nélküli jogosultságokkal rendelkező új fiókokat is létrehozhat. A kevesebb jogosultsággal bíró fiókkal rendelkező felhasználók esetében kisebb a veszélyeztetettség, mint a rendszergazdai jogosultságokkal rendelkezők esetén</td>
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=21140">Kritikus</a><br />
Távoli kódfuttatás</td>
<td style="border:1px solid black;">Esetleg újra kell indítani a rendszert</td>
<td style="border:1px solid black;">Microsoft Windows</td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=201704">MS10-077</a></td>
<td style="border:1px solid black;"><strong>A .NET Framework</strong> <strong>biztonsági rése távoli programkódfuttatást tehet lehetővé (2160841)</strong><br />
<br />
A biztonsági frissítés a Microsoft .NET Framework közvetlenül jelentett biztonsági rését szünteti meg. A biztonsági rés távoli kódfuttatást tehet lehetővé az ügyfélrendszereken, ha a felhasználó különlegesen kialakított weboldalt tekint meg az XAML böngészőalkalmazások (XBAP alkalmazások) futtatására alkalmas böngészőben. A kevesebb jogosultsággal bíró fiókkal rendelkező felhasználók esetében kisebb a veszélyeztetettség, mint a rendszergazdai jogosultságokkal rendelkezők esetén A biztonsági rések IIS szolgáltatást futtató kiszolgálórendszereken is lehetővé tehetik a távoli kódfuttatást, ha az adott kiszolgálón engedélyezett az ASP.NET oldalak feldolgozása, és a támadó sikeresen feltölt egy különlegesen kialakított ASP.NET oldalt a kiszolgálóra, és végrehajtja, mint az a webes tárolási forgatókönyv esetében történik.</td>
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=21140">Kritikus</a><br />
Távoli kódfuttatás</td>
<td style="border:1px solid black;">Esetleg újra kell indítani a rendszert</td>
<td style="border:1px solid black;">Microsoft Windows,<br />
Microsoft .NET Framework</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=202016">MS10-072</a></td>
<td style="border:1px solid black;"><strong>A SafeHTML biztonsági rései adatokhoz való illetéktelen hozzáférést tehetnek lehetővé (2412048)</strong><br />
<br />
A biztonsági frissítés a Microsoft SharePoint és a Windows SharePoint Services egy nyilvánosságra került és egy közvetlenül jelentett biztonsági résének hibáját hárítja el. A biztonsági rések adatokhoz való illetéktelen hozzáférést tehetnek lehetővé, ha a támadó speciálisan létrehozott parancsfájlt küld a megcélzott oldalnak, SafeHTML használatával.</td>
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=21140">Fontos</a><br />
Adatokhoz való illetéktelen hozzáférés</td>
<td style="border:1px solid black;">Esetleg újra kell indítani a rendszert</td>
<td style="border:1px solid black;">Microsoft Server Software</td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=201093">MS10-073</a></td>
<td style="border:1px solid black;"><strong>A Windows kernel módú</strong> <strong>illesztőprogramok biztonsági rése jogok kiterjesztéséhez vezethet (981957)</strong><br />
<br />
A biztonsági frissítés a Windows-kernel módú illesztőprogramok számos nyilvánosságra került biztonsági rését szünteti meg. A biztonsági rések legsúlyosabbika a jogok kiterjesztését teheti lehetővé, ha a támadó bejelentkezik az érintett rendszerre, és ott különlegesen kialakított alkalmazást futtat.
A támadónak a biztonsági rés kihasználásához érvényes bejelentkezési adatokkal kell rendelkeznie, és képesnek kell lennie helyileg bejelentkezni a rendszerbe. Névtelen felhasználók nem tudják távolról kiaknázni ezt a biztonsági rést.</td>
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=21140">Fontos</a><br />
Jogok kiterjesztése</td>
<td style="border:1px solid black;">Újraindítást igényel</td>
<td style="border:1px solid black;">Microsoft Windows</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=201084">MS10-078</a></td>
<td style="border:1px solid black;"><strong>Az OpenType Font Format (OTF) illesztőprogramjának biztonsági rései jogok kiterjesztését tehetik lehetővé (2279986)</strong><br />
<br />
A biztonsági frissítés a Windows OpenType Font Format (OTF) illesztőprogram két közvetlenül jelentett biztonsági rését szünteti meg. A biztonsági frissítés a Windows XP és Windows Server 2003 összes támogatott kiadására nézve Fontos besorolású. A Windows Vista, Windows Server 2008, Windows 7 és Windows Server 2008 R2 támogatott kiadásait nem érinti a biztonsági rés okozta probléma.<br />
<br />
A biztonsági rések jogok kiterjesztését tehetik lehetővé, ha a felhasználó speciálisan kialakított OpenType betűtípussal megjelenített tartalmat tekint meg. A támadónak a biztonsági rés kihasználásához érvényes bejelentkezési adatokkal kell rendelkeznie, és képesnek kell lennie helyileg bejelentkezni a rendszerbe. Névtelen felhasználók nem tudják távolról kiaknázni ezt a biztonsági rést.</td>
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=21140">Fontos</a><br />
Jogok kiterjesztése</td>
<td style="border:1px solid black;">Újraindítást igényel</td>
<td style="border:1px solid black;">Microsoft Windows</td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=201696">MS10-079</a></td>
<td style="border:1px solid black;"><strong>A Microsoft Word biztonsági rései távolról történő programkódfuttatást tehetnek lehetővé (2293194)</strong><br />
<br />
Ez a biztonsági frissítés a Microsoft Office tizenegy, közvetlenül jelzett biztonsági rését szünteti meg. A biztonsági rések távoli kódvégrehajtást tehetnek lehetővé, amennyiben a felhasználó egy speciálisan kialakított Word fájlt nyit meg. A biztonsági rések valamelyikét sikeresen kihasználó támadó a helyi felhasználóval egyező hozzáférést nyer a rendszerhez. A kevesebb jogosultsággal bíró fiókkal rendelkező felhasználók esetében kisebb a veszélyeztetettség, mint a rendszergazdai jogosultságokkal rendelkezők esetén</td>
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=21140">Fontos</a><br />
Távoli kódfuttatás</td>
<td style="border:1px solid black;">Esetleg újra kell indítani a rendszert</td>
<td style="border:1px solid black;">Microsoft Office</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=200529">MS10-080</a></td>
<td style="border:1px solid black;"><strong>A Microsoft Excel biztonsági rései távolról történő kódfuttatást tehetnek lehetővé (2293211)</strong><br />
<br />
Ez a biztonsági frissítés a Microsoft Office tizenhárom, közvetlenül jelzett biztonsági rését szünteti meg. A biztonsági rések távoli kódfuttatást tesznek lehetővé, ha a felhasználó egy különlegesen kialakított Excel fájlt vagy Lotus 1-2-3 fájlt nyit meg. A biztonsági rések valamelyikét sikeresen kihasználó támadó a helyi felhasználóval egyező hozzáférést nyer a rendszerhez. A kevesebb jogosultsággal bíró fiókkal rendelkező felhasználók esetében kisebb a veszélyeztetettség, mint a rendszergazdai jogosultságokkal rendelkezők esetén</td>
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=21140">Fontos</a><br />
Távoli kódfuttatás</td>
<td style="border:1px solid black;">Esetleg újra kell indítani a rendszert</td>
<td style="border:1px solid black;">Microsoft Office</td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=201086">MS10-081</a></td>
<td style="border:1px solid black;"><strong>A Windows Common Controls Library biztonsági rése távoli programkódfuttatást tehet lehetővé (2296011)</strong><br />
<br />
Ez a biztonsági frissítés a Windows common control library közvetlenül jelentett biztonsági rését szünteti meg. A biztonsági rés távoli kódfuttatást tehet lehetővé, amennyiben a felhasználó egy különlegesen kialakított weboldalra látogat. Ha a felhasználó rendszergazda jogosultságokkal jelentkezett be a rendszerbe, akkor a biztonsági rést kihasználó támadó teljes mértékben átveheti az irányítást az érintett rendszer felett. Ezt követően programokat telepíthet, illetve adatokat tekinthet meg, módosíthat és törölhet, de korlátozás nélküli jogosultságokkal rendelkező új fiókokat is létrehozhat. A kevesebb jogosultsággal bíró fiókkal rendelkező felhasználók esetében kisebb a veszélyeztetettség, mint a rendszergazdai jogosultságokkal rendelkezők esetén</td>
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=21140">Fontos</a><br />
Távoli kódfuttatás</td>
<td style="border:1px solid black;">Újraindítást igényel</td>
<td style="border:1px solid black;">Microsoft Windows</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=201098">MS10-082</a></td>
<td style="border:1px solid black;"><strong>A Windows Media Player biztonsági rése távoli programkódfuttatást tesz lehetővé (2378111)</strong><br />
<br />
A biztonsági frissítés a Windows Media Player közvetlenül jelentett biztonsági rését szünteti meg. A biztonsági rés távolról történő programkódfuttatást tehet lehetővé, ha a Windows Media Player egy rosszindulatú webhelyen tárolt, speciálisan kialakított médiatartalmat nyit meg. A biztonsági rést kihasználó támadó a helyi felhasználóval egyező hozzáférést nyer a rendszerhez. A kevesebb jogosultsággal bíró fiókkal rendelkező felhasználók esetében kisebb a veszélyeztetettség, mint a rendszergazdai jogosultságokkal rendelkezők esetén</td>
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=21140">Fontos</a><br />
Távoli kódfuttatás</td>
<td style="border:1px solid black;">Esetleg újra kell indítani a rendszert</td>
<td style="border:1px solid black;">Microsoft Windows</td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=190553">MS10-083</a></td>
<td style="border:1px solid black;"><strong>A Windows-rendszerhéj, valamint a WordPad COM-érvényesítés biztonsági rése távoli kódfuttatást tehet lehetővé (2405882)</strong><br />
<br />
A biztonsági frissítés a Microsoft Windows közvetlenül jelentett biztonsági rését szünteti meg. A biztonsági rés távolról történő programkódfuttatást tehet lehetővé, ha a felhasználó megnyit egy speciálisan kialakított fájlt a WordPad-del, vagy kiválaszt, illetve megnyit egy hálózaton vagy WebDAV megosztáson lévő parancsikonfájlt. A biztonsági rést kihasználó támadó a helyi felhasználóval egyező hozzáférést nyer a rendszerhez. A kevesebb jogosultsággal bíró fiókkal rendelkező felhasználók esetében kisebb a veszélyeztetettség, mint a rendszergazdai jogosultságokkal rendelkezők esetén</td>
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=21140">Fontos</a><br />
Távoli kódfuttatás</td>
<td style="border:1px solid black;">Újraindítást igényel</td>
<td style="border:1px solid black;">Microsoft Windows</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=201720">MS10-084</a></td>
<td style="border:1px solid black;"><strong>A Windows helyi eljáráshívása biztonsági rése jogok kiterjesztését okozhatja (2360937)</strong><br />
<br />
A biztonsági frissítés a Microsoft Windows nyilvánosan jelentett biztonsági rését szünteti meg. A biztonsági frissítés a Windows XP és Windows Server 2003 összes támogatott kiadására nézve Fontos besorolású. A Windows Vista, Windows Server 2008, Windows 7 és Windows Server 2008 R2 támogatott kiadásait nem érinti a biztonsági rés okozta probléma.<br />
<br />
A biztonsági rés a jogok kiterjesztését teszi lehetővé, ha egy támadó bejelentkezik az érintett rendszerre és ott különlegesen kialakított kódot futtat, ami LPC üzenetet küld a helyi LRPC szerverre. Az üzenet ezután egy hitelesített felhasználó számára hozzáférést nyújthat a NetworkService fiók környezetében futó erőforrásokhoz. A támadónak a biztonsági rés kihasználásához érvényes bejelentkezési adatokkal kell rendelkeznie, és képesnek kell lennie helyileg bejelentkezni a rendszerbe.</td>
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=21140">Fontos</a><br />
Jogok kiterjesztése</td>
<td style="border:1px solid black;">Újraindítást igényel</td>
<td style="border:1px solid black;">Microsoft Windows</td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=201705">MS10-085</a></td>
<td style="border:1px solid black;"><strong>Szolgáltatásmegtagadást lehetővé tévő SChannel biztonsági rés (2207566)</strong><br />
<br />
A biztonsági frissítés a Windows biztonságos csatorna (SChannel) biztonsági csomagjának közvetlenül jelentett biztonsági rését szünteti meg. A biztonsági rés szolgáltatásmegtagadást tehet lehetővé, amennyiben az érintett rendszer a biztonságos szoftvercsatornán (SSL) keresztül speciálisan kialakított csomag üzenetet kapott. Alapértelmezés szerint a Windows Vista, a Windows Server 2008, a Windows 7 és a Windows Server 2008 R2 egyetlen támogatott kiadásán sincs konfigurálva az SSL hálózati forgalom fogadása.</td>
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=21140">Fontos</a><br />
Szolgáltatásmegtagadás</td>
<td style="border:1px solid black;">Újraindítást igényel</td>
<td style="border:1px solid black;">Microsoft Windows</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=201703">MS10-074</a></td>
<td style="border:1px solid black;"><strong>A Microsoft Foundation Classes biztonsági rése távolról történő programkódfuttatást tehet lehetővé (2387149)</strong><br />
<br />
A biztonsági frissítés a Microsoft Foundation Class (MFC) Library egy nyilvánosan jelentett biztonsági rését szünteti meg. A biztonsági rés távoli kódfuttatást okozhat, ha a felhasználó rendszergazda jogosultságokkal jelentkezett be a rendszerbe, és egy MFC Library alapú alkalmazást nyit meg. A biztonsági rést sikeresen kihasználó támadó az éppen bejelentkezett felhasználóval egyező engedélyeket szerez a rendszerhez. Ha valamely felhasználó felügyeleti jogosultságokkal bejelentkezett a rendszerbe, akkor a támadó teljes mértékben átveheti az irányítást a számítógép felett. Ezt követően programokat telepíthet, illetve adatokat tekinthet meg, módosíthat és törölhet, de korlátozás nélküli jogosultságokkal rendelkező új fiókokat is létrehozhat. A kevesebb jogosultsággal bíró fiókkal rendelkező felhasználók esetében kisebb a veszélyeztetettség, mint a rendszergazdai jogosultságokkal rendelkezők esetén</td>
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=21140">Mérsékelt.</a><br />
Távoli kódfuttatás</td>
<td style="border:1px solid black;">Esetleg újra kell indítani a rendszert</td>
<td style="border:1px solid black;">Microsoft Windows</td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=201721">MS10-086</a></td>
<td style="border:1px solid black;"><strong>A Windows megosztott fürtlemezeinek biztonsági rése beavatkozásra adhat lehetőséget (2294255)</strong><br />
<br />
A biztonsági frissítés a közvetlenül jelentett biztonsági rés hibáit oldja meg a megosztott feladatátvevő fürtként használatos Windows Server 2008 R2 rendszerben. A biztonsági rés az adatok manipulálását teheti lehetővé a feladatátvevő fürtlemezek rendszergazdáknak szóló megosztásain. Alapértelmezés szerint a Windows Server 2008 R2 szervereket nem érinti ez a biztonsági rés. A biztonsági rés kizárólag a feladatátvevő fürtnél használt fürtlemezekre vonatkozik.</td>
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=21140">Mérsékelt.</a><br />
Beavatkozás</td>
<td style="border:1px solid black;">Újraindítást igényel</td>
<td style="border:1px solid black;">Microsoft Windows</td>
</tr>
</tbody>
</table>
  
Kihasználhatósági információk  
-----------------------------
  
<span></span>
A következő táblázat az adott hónapban megoldott biztonsági rések kihasználhatósági jellemzőit ismerteti. A biztonsági rések a kihasználhatósági kockázat, majd a CVE azonosító szerint vannak felsorolva. Csak a kritikus és fontos besorolású biztonsági rések szerepelnek.
  
**A táblázat használata**
  
A táblázat segítségével meghatározható annak valószínűsége, hogy a biztonsági közlemény kiadását követő 30 napon belül a telepíteni szükséges biztonsági frissítésekre működő rosszindulatú programkódot jelentetnek meg. A telepítés fontossági sorrendjének megállapításához az adott konfigurációnak megfelelően tekintse át az alábbi értékeléseket. A minősítések jelentéséről és meghatározásuk módjáról a [Microsoft kihasználhatósági információk](http://technet.microsoft.com/en-us/security/cc998259.aspx) című rész tartalmaz bővebb információt.
  
| Közlemény azonosítója                                     | A biztonsági rés címe                                                               | CVE-azonosító                                                                    | Kihasználhatósági információk értékelése                                                                                 | Fontos megjegyzések                                                                                                                                                                                                                           |  
|-----------------------------------------------------------|-------------------------------------------------------------------------------------|----------------------------------------------------------------------------------|--------------------------------------------------------------------------------------------------------------------------|-----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|  
| [MS10-083](http://go.microsoft.com/fwlink/?linkid=190553) | COM-hitelesítés biztonsági rése                                                     | [CVE-2010-1263](http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2010-1263) | [**1**](http://technet.microsoft.com/en-us/security/cc998259.aspx) - Valószínűleg konzisztens rosszindulatú programkód   | (Nincs)                                                                                                                                                                                                                                       |  
| [MS10-076](http://go.microsoft.com/fwlink/?linkid=194560) | Beágyazott OpenType betűtípus egészszám-túlcsordulást okozó biztonsági rése         | [CVE-2010-1883](http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2010-1883) | [**1**](http://technet.microsoft.com/en-us/security/cc998259.aspx) - Valószínűleg konzisztens rosszindulatú programkód   | Az újabb operációs rendszerekben található ASLR technológia nehezíti a biztonsági rés kihasználását                                                                                                                                           |  
| [MS10-078](http://go.microsoft.com/fwlink/?linkid=201084) | Az OpenType betűtípus-elemzés biztonsági rése                                       | [CVE-2010-2740](http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2010-2740) | [**1**](http://technet.microsoft.com/en-us/security/cc998259.aspx) - Valószínűleg konzisztens rosszindulatú programkód   | (Nincs)                                                                                                                                                                                                                                       |  
| [MS10-078](http://go.microsoft.com/fwlink/?linkid=201084) | Az OpenType betűtípus-hitelesítés biztonsági rése                                   | [CVE-2010-2741](http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2010-2741) | [**1**](http://technet.microsoft.com/en-us/security/cc998259.aspx) - Valószínűleg konzisztens rosszindulatú programkód   | (Nincs)                                                                                                                                                                                                                                       |  
| [MS10-073](http://go.microsoft.com/fwlink/?linkid=201093) | A Win32k billentyűzetkiosztással kapcsolatos biztonsági rése                        | [CVE-2010-2743](http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2010-2743) | [**1**](http://technet.microsoft.com/en-us/security/cc998259.aspx) - Valószínűleg konzisztens rosszindulatú programkód   | **A biztonsági rés nyilvánosságra került, és jelenleg internetszerte kihasználják**                                                                                                                                                           |  
| [MS10-073](http://go.microsoft.com/fwlink/?linkid=201093) | A Win32K ablakosztállyal kapcsolatos biztonsági rése                                | [CVE-2010-2744](http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2010-2744) | [**1**](http://technet.microsoft.com/en-us/security/cc998259.aspx) - Valószínűleg konzisztens rosszindulatú programkód   | **A biztonsági rés nyilvánosságra került**                                                                                                                                                                                                    |  
| [MS10-082](http://go.microsoft.com/fwlink/?linkid=201098) | A Windows Media Player memória-meghibásodást okozó biztonsági rése                  | [CVE-2010-2745](http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2010-2745) | [**1**](http://technet.microsoft.com/en-us/security/cc998259.aspx) - Valószínűleg konzisztens rosszindulatú programkód   | (Nincs)                                                                                                                                                                                                                                       |  
| [MS10-081](http://go.microsoft.com/fwlink/?linkid=201086) | A Comctl32 halomtúlcsordulást okozó biztonsági rése                                 | [CVE-2010-2746](http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2010-2746) | [**1**](http://technet.microsoft.com/en-us/security/cc998259.aspx) - Valószínűleg konzisztens rosszindulatú programkód   | (Nincs)                                                                                                                                                                                                                                       |  
| [MS10-079](http://go.microsoft.com/fwlink/?linkid=201696) | A Word kötegtúlcsordulást okozó biztonsági rése                                     | [CVE-2010-3214](http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2010-3214) | [**1**](http://technet.microsoft.com/en-us/security/cc998259.aspx) - Valószínűleg konzisztens rosszindulatú programkód   | (Nincs)                                                                                                                                                                                                                                       |  
| [MS10-079](http://go.microsoft.com/fwlink/?linkid=201696) | A Word könyvjelzők biztonsági rése                                                  | [CVE-2010-3216](http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2010-3216) | [**1**](http://technet.microsoft.com/en-us/security/cc998259.aspx) - Valószínűleg konzisztens rosszindulatú programkód   | (Nincs)                                                                                                                                                                                                                                       |  
| [MS10-084](http://go.microsoft.com/fwlink/?linkid=201720) | LPC-üzenet puffertúlcsordulást okozó biztonsági rése                                | [CVE-2010-3222](http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2010-3222) | [**1**](http://technet.microsoft.com/en-us/security/cc998259.aspx) - Valószínűleg konzisztens rosszindulatú programkód   | **A biztonsági rés nyilvánosságra került**                                                                                                                                                                                                    |  
| [MS10-075](http://go.microsoft.com/fwlink/?linkid=201722) | Az RTSP használat utáni felszabadítás biztonsági rése                               | [CVE-2010-3225](http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2010-3225) | [**1**](http://technet.microsoft.com/en-us/security/cc998259.aspx) - Valószínűleg konzisztens rosszindulatú programkód   | (Nincs)                                                                                                                                                                                                                                       |  
| [MS10-077](http://go.microsoft.com/fwlink/?linkid=201704) | A .NET Framework x64 JIT Compiler biztonsági rése                                   | [CVE-2010-3228](http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2010-3228) | [**1**](http://technet.microsoft.com/en-us/security/cc998259.aspx) - Valószínűleg konzisztens rosszindulatú programkód   | (Nincs)                                                                                                                                                                                                                                       |  
| [MS10-080](http://go.microsoft.com/fwlink/?linkid=200529) | Az Excel fájlformátum elemzése okozta biztonsági rés                                | [CVE-2010-3232](http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2010-3232) | [**1**](http://technet.microsoft.com/en-us/security/cc998259.aspx) - Valószínűleg konzisztens rosszindulatú programkód   | (Nincs)                                                                                                                                                                                                                                       |  
| [MS10-080](http://go.microsoft.com/fwlink/?linkid=200529) | Képletek részadatfolyama okozta memóriameghibásodás biztonsági rése                 | [CVE-2010-3234](http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2010-3234) | [**1**](http://technet.microsoft.com/en-us/security/cc998259.aspx) - Valószínűleg konzisztens rosszindulatú programkód   | (Nincs)                                                                                                                                                                                                                                       |  
| [MS10-080](http://go.microsoft.com/fwlink/?linkid=200529) | A képletek hibásan létrehozott Biff-rekordjához kapcsolódó biztonsági rés           | [CVE-2010-3235](http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2010-3235) | [**1**](http://technet.microsoft.com/en-us/security/cc998259.aspx) - Valószínűleg konzisztens rosszindulatú programkód   | (Nincs)                                                                                                                                                                                                                                       |  
| [MS10-080](http://go.microsoft.com/fwlink/?linkid=200529) | Határokon kívüli tömb biztonsági rése                                               | [CVE-2010-3236](http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2010-3236) | [**1**](http://technet.microsoft.com/en-us/security/cc998259.aspx) - Valószínűleg konzisztens rosszindulatú programkód   | (Nincs)                                                                                                                                                                                                                                       |  
| [MS10-080](http://go.microsoft.com/fwlink/?linkid=200529) | Negatív jövőbeni függvény biztonsági rése                                           | [CVE-2010-3238](http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2010-3238) | [**1**](http://technet.microsoft.com/en-us/security/cc998259.aspx) - Valószínűleg konzisztens rosszindulatú programkód   | (Nincs)                                                                                                                                                                                                                                       |  
| [MS10-080](http://go.microsoft.com/fwlink/?linkid=200529) | Határokon kívüli különleges bejegyzés elemzésének biztonsági rése                   | [CVE-2010-3239](http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2010-3239) | [**1**](http://technet.microsoft.com/en-us/security/cc998259.aspx) - Valószínűleg konzisztens rosszindulatú programkód   | (Nincs)                                                                                                                                                                                                                                       |  
| [MS10-071](http://go.microsoft.com/fwlink/?linkid=202013) | Inicializálás hiánya miatti memóriameghibásodás okozta biztonsági rés               | [CVE-2010-3326](http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2010-3326) | [**1**](http://technet.microsoft.com/en-us/security/cc998259.aspx) - Valószínűleg konzisztens rosszindulatú programkód   | (Nincs)                                                                                                                                                                                                                                       |  
| [MS10-071](http://go.microsoft.com/fwlink/?linkid=202013) | Inicializálás hiánya miatti memóriameghibásodás okozta biztonsági rés               | [CVE-2010-3328](http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2010-3328) | [**1**](http://technet.microsoft.com/en-us/security/cc998259.aspx) - Valószínűleg konzisztens rosszindulatú programkód   | (Nincs)                                                                                                                                                                                                                                       |  
| [MS10-071](http://go.microsoft.com/fwlink/?linkid=202013) | Inicializálás hiánya miatti memóriameghibásodás okozta biztonsági rés               | [CVE-2010-3329](http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2010-3329) | [**1**](http://technet.microsoft.com/en-us/security/cc998259.aspx) - Valószínűleg konzisztens rosszindulatú programkód   | (Nincs)                                                                                                                                                                                                                                       |  
| [MS10-071](http://go.microsoft.com/fwlink/?linkid=202013) | Inicializálás hiánya miatti memóriameghibásodás okozta biztonsági rés               | [CVE-2010-3331](http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2010-3331) | [**1**](http://technet.microsoft.com/en-us/security/cc998259.aspx) - Valószínűleg konzisztens rosszindulatú programkód   | (Nincs)                                                                                                                                                                                                                                       |  
| [MS10-079](http://go.microsoft.com/fwlink/?linkid=201696) | A Word nem inicializált mutatót okozó biztonsági rése                               | [CVE-2010-2747](http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2010-2747) | [**2**](http://technet.microsoft.com/en-us/security/cc998259.aspx) - Valószínűleg inkonzisztens rosszindulatú programkód | (Nincs)                                                                                                                                                                                                                                       |  
| [MS10-079](http://go.microsoft.com/fwlink/?linkid=201696) | A Word határ-ellenőrzési biztonsági rése                                            | [CVE-2010-2748](http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2010-2748) | [**2**](http://technet.microsoft.com/en-us/security/cc998259.aspx) - Valószínűleg inkonzisztens rosszindulatú programkód | (Nincs)                                                                                                                                                                                                                                       |  
| [MS10-079](http://go.microsoft.com/fwlink/?linkid=201696) | A Word indexértékekre vonatkozó biztonsági rése                                     | [CVE-2010-2750](http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2010-2750) | [**2**](http://technet.microsoft.com/en-us/security/cc998259.aspx) - Valószínűleg inkonzisztens rosszindulatú programkód | (Nincs)                                                                                                                                                                                                                                       |  
| [MS10-079](http://go.microsoft.com/fwlink/?linkid=201696) | A Word visszatérési értékekre vonatkozó biztonsági rése                             | [CVE-2010-3215](http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2010-3215) | [**2**](http://technet.microsoft.com/en-us/security/cc998259.aspx) - Valószínűleg inkonzisztens rosszindulatú programkód | (Nincs)                                                                                                                                                                                                                                       |  
| [MS10-079](http://go.microsoft.com/fwlink/?linkid=201696) | A Word mutatót okozó biztonsági rése                                                | [CVE-2010-3217](http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2010-3217) | [**2**](http://technet.microsoft.com/en-us/security/cc998259.aspx) - Valószínűleg inkonzisztens rosszindulatú programkód | (Nincs)                                                                                                                                                                                                                                       |  
| [MS10-079](http://go.microsoft.com/fwlink/?linkid=201696) | A Word halomtúlcsordulást okozó biztonsági rése                                     | [CVE-2010-3218](http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2010-3218) | [**2**](http://technet.microsoft.com/en-us/security/cc998259.aspx) - Valószínűleg inkonzisztens rosszindulatú programkód | (Nincs)                                                                                                                                                                                                                                       |  
| [MS10-079](http://go.microsoft.com/fwlink/?linkid=201696) | A Word indexelemzési biztonsági rése                                                | [CVE-2010-3219](http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2010-3219) | [**2**](http://technet.microsoft.com/en-us/security/cc998259.aspx) - Valószínűleg inkonzisztens rosszindulatú programkód | (Nincs)                                                                                                                                                                                                                                       |  
| [MS10-079](http://go.microsoft.com/fwlink/?linkid=201696) | A Word elemzési biztonsági rése                                                     | [CVE-2010-3220](http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2010-3220) | [**2**](http://technet.microsoft.com/en-us/security/cc998259.aspx) - Valószínűleg inkonzisztens rosszindulatú programkód | (Nincs)                                                                                                                                                                                                                                       |  
| [MS10-079](http://go.microsoft.com/fwlink/?linkid=201696) | A Word elemzési biztonsági rése                                                     | [CVE-2010-3221](http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2010-3221) | [**2**](http://technet.microsoft.com/en-us/security/cc998259.aspx) - Valószínűleg inkonzisztens rosszindulatú programkód | (Nincs)                                                                                                                                                                                                                                       |  
| [MS10-080](http://go.microsoft.com/fwlink/?linkid=200529) | Az Excel-bejegyzések elemzésének egészszám-túlcsordulást okozó biztonsági rése      | [CVE-2010-3230](http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2010-3230) | [**2**](http://technet.microsoft.com/en-us/security/cc998259.aspx) - Valószínűleg inkonzisztens rosszindulatú programkód | (Nincs)                                                                                                                                                                                                                                       |  
| [MS10-080](http://go.microsoft.com/fwlink/?linkid=200529) | Az Excel bejegyzéselemzés miatti memória-meghibásodást okozó biztonsági rése        | [CVE-2010-3231](http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2010-3231) | [**2**](http://technet.microsoft.com/en-us/security/cc998259.aspx) - Valószínűleg inkonzisztens rosszindulatú programkód | (Nincs)                                                                                                                                                                                                                                       |  
| [MS10-080](http://go.microsoft.com/fwlink/?linkid=200529) | A Lotus 1-2-3 munkafüzet elemzése okozta biztonsági rés                             | [CVE-2010-3233](http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2010-3233) | [**2**](http://technet.microsoft.com/en-us/security/cc998259.aspx) - Valószínűleg inkonzisztens rosszindulatú programkód | (Nincs)                                                                                                                                                                                                                                       |  
| [MS10-080](http://go.microsoft.com/fwlink/?linkid=200529) | Cellaegyesítés bejegyzésmutatójának biztonsági rése                                 | [CVE-2010-3237](http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2010-3237) | [**2**](http://technet.microsoft.com/en-us/security/cc998259.aspx) - Valószínűleg inkonzisztens rosszindulatú programkód | (Nincs)                                                                                                                                                                                                                                       |  
| [MS10-080](http://go.microsoft.com/fwlink/?linkid=200529) | Valós idejű adattömb bejegyzésének biztonsági rése                                  | [CVE-2010-3240](http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2010-3240) | [**2**](http://technet.microsoft.com/en-us/security/cc998259.aspx) - Valószínűleg inkonzisztens rosszindulatú programkód | (Nincs)                                                                                                                                                                                                                                       |  
| [MS10-080](http://go.microsoft.com/fwlink/?linkid=200529) | Elemzés közbeni határokon kívüli memóriaírás biztonsági rése                        | [CVE-2010-3241](http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2010-3241) | [**2**](http://technet.microsoft.com/en-us/security/cc998259.aspx) - Valószínűleg inkonzisztens rosszindulatú programkód | (Nincs)                                                                                                                                                                                                                                       |  
| [MS10-080](http://go.microsoft.com/fwlink/?linkid=200529) | Ghost-bejegyzéstípus elemzési biztonsági rése                                       | [CVE-2010-3242](http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2010-3242) | [**2**](http://technet.microsoft.com/en-us/security/cc998259.aspx) - Valószínűleg inkonzisztens rosszindulatú programkód | (Nincs)                                                                                                                                                                                                                                       |  
| [MS10-073](http://go.microsoft.com/fwlink/?linkid=201093) | A Win32k hivatkozások számával kapcsolatos biztonsági rése                          | [CVE-2010-2549](http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2010-2549) | [**3**](http://technet.microsoft.com/en-us/security/cc998259.aspx) - Nem valószínű működő rosszindulatú programkód       | **A biztonsági rés nyilvánosságra került**                                                                                                                                                                                                    |  
| [MS10-085](http://go.microsoft.com/fwlink/?linkid=201705) | A TLSv1 szolgáltatásmegtagadást okozó biztonsági rése                               | [CVE-2010-3229](http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2010-3229) | [**3**](http://technet.microsoft.com/en-us/security/cc998259.aspx) - Nem valószínű működő rosszindulatú programkód       | A maximális biztonsági hatás mindössze a szolgáltatásmegtagadás                                                                                                                                                                               |  
| [MS10-071](http://go.microsoft.com/fwlink/?linkid=202013) | HTML-törlés miatti biztonsági rés                                                   | [CVE-2010-3243](http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2010-3243) | [**3**](http://technet.microsoft.com/en-us/security/cc998259.aspx) - Nem valószínű működő rosszindulatú programkód       | Az [MS10-072](http://go.microsoft.com/fwlink/?linkid=202016) közlemény szintén foglalkozik a biztonsági réssel. A maximális biztonsági hatás mindössze az adatokhoz való illetéktelen hozzáférés.                                             |  
| [MS10-072](http://go.microsoft.com/fwlink/?linkid=202016) | HTML-törlés miatti biztonsági rés                                                   | [CVE-2010-3243](http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2010-3243) | [**3**](http://technet.microsoft.com/en-us/security/cc998259.aspx) - Nem valószínű működő rosszindulatú programkód       | Az [MS10-071](http://go.microsoft.com/fwlink/?linkid=202013) közlemény szintén foglalkozik a biztonsági réssel. A maximális biztonsági hatás mindössze az adatokhoz való illetéktelen hozzáférés.                                             |  
| [MS10-071](http://go.microsoft.com/fwlink/?linkid=202013) | HTML-törlés miatti biztonsági rés                                                   | [CVE-2010-3324](http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2010-3324) | [**3**](http://technet.microsoft.com/en-us/security/cc998259.aspx) - Nem valószínű működő rosszindulatú programkód       | Az [MS10-072](http://go.microsoft.com/fwlink/?linkid=202016) közlemény szintén foglalkozik a biztonsági réssel. **A biztonsági rés nyilvánosságra került.** A maximális biztonsági hatás mindössze az adatokhoz való illetéktelen hozzáférés. |  
| [MS10-072](http://go.microsoft.com/fwlink/?linkid=202016) | HTML-törlés miatti biztonsági rés                                                   | [CVE-2010-3324](http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2010-3324) | [**3**](http://technet.microsoft.com/en-us/security/cc998259.aspx) - Nem valószínű működő rosszindulatú programkód       | Az [MS10-071](http://go.microsoft.com/fwlink/?linkid=202013) közlemény szintén foglalkozik a biztonsági réssel. **A biztonsági rés nyilvánosságra került.** A maximális biztonsági hatás mindössze az adatokhoz való illetéktelen hozzáférés. |  
| [MS10-071](http://go.microsoft.com/fwlink/?linkid=202013) | A CSS különleges karakter miatti illetéktelen adathozzáférést okozó biztonsági rése | [CVE-2010-3325](http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2010-3325) | [**3**](http://technet.microsoft.com/en-us/security/cc998259.aspx) - Nem valószínű működő rosszindulatú programkód       | **A biztonsági rés nyilvánosságra került.** A maximális biztonsági hatás mindössze az adatokhoz való illetéktelen hozzáférés.                                                                                                                 |  
| [MS10-071](http://go.microsoft.com/fwlink/?linkid=202013) | Tartományok közötti illetéktelen adathozzáférést okozó biztonsági rés               | [CVE-2010-3330](http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2010-3330) | [**3**](http://technet.microsoft.com/en-us/security/cc998259.aspx) - Nem valószínű működő rosszindulatú programkód       | A maximális biztonsági hatás mindössze az adatokhoz való illetéktelen hozzáférés                                                                                                                                                              |
  
Érintett szoftverek és letöltési helyek  
---------------------------------------
  
<span></span>
A következő táblázatok a közleményeket a főbb szoftverkategóriák és súlyosság szerint sorolják fel.
  
**A táblázatok használata**
  
A táblázatok segítségével megtudhatja a szükséges információt a telepítendő biztonsági frissítésekről. Nézzen meg minden felsorolt szoftvert vagy összetevőt annak megállapításához, hogy elérhető-e a rendszerhez való frissítés. Ha a szoftver vagy összetevő szerepel a listán, hiperhivatkozással kapcsolódik hozzá az elérhető szoftverfrissítés, és a frissítés besorolása is fel van tüntetve.
  
**Megjegyzés:** Előfordulhat, hogy egy biztonsági rés megszüntetéséhez több biztonsági frissítést kell telepíteni. Nézze át az egyes közleményazonosítókhoz tartozó teljes oszlopot, és ellenőrizze a telepítendő frissítéseket a rendszerre telepített programok vagy összetevők alapján.
  
#### A Windows operációs rendszer és összetevői

 
<p> </p>
<table style="border:1px solid black;">
<tr class="thead">
<th style="border:1px solid black;" >
</th>
<th style="border:1px solid black;" >
</th>
<th style="border:1px solid black;" >
</th>
<th style="border:1px solid black;" >
</th>
<th style="border:1px solid black;" >
</th>
<th style="border:1px solid black;" >
</th>
<th style="border:1px solid black;" >
</th>
<th style="border:1px solid black;" >
</th>
<th style="border:1px solid black;" >
</th>
<th style="border:1px solid black;" >
</th>
<th style="border:1px solid black;" >
</th>
<th style="border:1px solid black;" >
</th>
<th style="border:1px solid black;" >
</th>
<th style="border:1px solid black;" >
</th>
</tr>
<tr>
<th colspan="14">
Windows XP  
</th>
</tr>
<tr>
<td style="border:1px solid black;">
**Közlemény** **azonosítója**
</td>
<td style="border:1px solid black;">
[**MS10-071**](http://go.microsoft.com/fwlink/?linkid=202013)
</td>
<td style="border:1px solid black;">
[**MS10-075**](http://go.microsoft.com/fwlink/?linkid=201722)
</td>
<td style="border:1px solid black;">
[**MS10-076**](http://go.microsoft.com/fwlink/?linkid=194560)
</td>
<td style="border:1px solid black;">
[**MS10-077**](http://go.microsoft.com/fwlink/?linkid=201704)
</td>
<td style="border:1px solid black;">
[**MS10-073**](http://go.microsoft.com/fwlink/?linkid=201093)
</td>
<td style="border:1px solid black;">
[**MS10-078**](http://go.microsoft.com/fwlink/?linkid=201084)
</td>
<td style="border:1px solid black;">
[**MS10-081**](http://go.microsoft.com/fwlink/?linkid=201086)
</td>
<td style="border:1px solid black;">
[**MS10-082**](http://go.microsoft.com/fwlink/?linkid=201098)
</td>
<td style="border:1px solid black;">
[**MS10-083**](http://go.microsoft.com/fwlink/?linkid=190553)
</td>
<td style="border:1px solid black;">
[**MS10-084**](http://go.microsoft.com/fwlink/?linkid=201720)
</td>
<td style="border:1px solid black;">
[**MS10-085**](http://go.microsoft.com/fwlink/?linkid=201705)
</td>
<td style="border:1px solid black;">
[**MS10-074**](http://go.microsoft.com/fwlink/?linkid=201703)
</td>
<td style="border:1px solid black;">
[**MS10-086**](http://go.microsoft.com/fwlink/?linkid=201721)
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
**Összesített súlyossági** **besorolás**
</td>
<td style="border:1px solid black;">
[**Kritikus**](http://go.microsoft.com/fwlink/?linkid=21140)
</td>
<td style="border:1px solid black;">
Nincsenek
</td>
<td style="border:1px solid black;">
[**Kritikus**](http://go.microsoft.com/fwlink/?linkid=21140)
</td>
<td style="border:1px solid black;">
[**Kritikus**](http://go.microsoft.com/fwlink/?linkid=21140)
</td>
<td style="border:1px solid black;">
[**Fontos**](http://go.microsoft.com/fwlink/?linkid=21140)
</td>
<td style="border:1px solid black;">
[**Fontos**](http://go.microsoft.com/fwlink/?linkid=21140)
</td>
<td style="border:1px solid black;">
[**Fontos**](http://go.microsoft.com/fwlink/?linkid=21140)
</td>
<td style="border:1px solid black;">
[**Fontos**](http://go.microsoft.com/fwlink/?linkid=21140)
</td>
<td style="border:1px solid black;">
[**Fontos**](http://go.microsoft.com/fwlink/?linkid=21140)
</td>
<td style="border:1px solid black;">
[**Fontos**](http://go.microsoft.com/fwlink/?linkid=21140)
</td>
<td style="border:1px solid black;">
Nincsenek
</td>
<td style="border:1px solid black;">
[**Mérsékelt.**](http://go.microsoft.com/fwlink/?linkid=21140)
</td>
<td style="border:1px solid black;">
Nincsenek
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Windows XP Service Pack 3
</td>
<td style="border:1px solid black;">
[Internet Explorer 6](http://www.microsoft.com/downloads/details.aspx?familyid=3b029696-cf98-4935-b3d6-846110aaa4bb)  
(Kritikus)  
[Internet Explorer 7](http://www.microsoft.com/downloads/details.aspx?familyid=c77ee103-7e97-44b2-bbf3-ee9f0de37fed)  
(Kritikus)  
[Internet Explorer 8](http://www.microsoft.com/downloads/details.aspx?familyid=93580299-d764-417f-a7fa-ee441fea2bb3)  
(Kritikus)
</td>
<td style="border:1px solid black;">
Nem érintett
</td>
<td style="border:1px solid black;">
[Windows XP Service Pack 3](http://www.microsoft.com/downloads/details.aspx?familyid=c3799399-ca72-4dec-a2a2-3571ad0b2f63)  
(Kritikus)
</td>
<td style="border:1px solid black;">
Nem érintett
</td>
<td style="border:1px solid black;">
[Windows XP Service Pack 3](http://www.microsoft.com/downloads/details.aspx?familyid=3966d754-d298-4e4a-9ce6-8205accd2215)  
(Fontos)
</td>
<td style="border:1px solid black;">
[Windows XP Service Pack 3](http://www.microsoft.com/downloads/details.aspx?familyid=0553fc7c-deed-4594-a133-d621551310dc)  
(Fontos)
</td>
<td style="border:1px solid black;">
[Windows XP Service Pack 3](http://www.microsoft.com/downloads/details.aspx?familyid=912a7c20-8177-4f65-b986-43fca6375ec1)  
(Fontos)
</td>
<td style="border:1px solid black;">
[Windows Media Player 9 Series](http://www.microsoft.com/downloads/details.aspx?familyid=bbf153e7-e764-46a0-a33b-81b7288d346c)  
(Fontos)  
[Windows Media Player 10](http://www.microsoft.com/downloads/details.aspx?familyid=bbf153e7-e764-46a0-a33b-81b7288d346c)  
(Fontos)  
[Windows Media Player 11](http://www.microsoft.com/downloads/details.aspx?familyid=bbf153e7-e764-46a0-a33b-81b7288d346c)  
(Fontos)
</td>
<td style="border:1px solid black;">
[Windows XP Service Pack 3](http://www.microsoft.com/downloads/details.aspx?familyid=211d95be-5630-4af5-85a7-c50268c475a9)  
(KB979687)  
(Fontos)
</td>
<td style="border:1px solid black;">
[Windows XP Service Pack 3](http://www.microsoft.com/downloads/details.aspx?familyid=6049c879-b81a-4d10-b96b-b2837cb24834)  
(Fontos)
</td>
<td style="border:1px solid black;">
Nem érintett
</td>
<td style="border:1px solid black;">
[Windows XP Service Pack 3](http://www.microsoft.com/downloads/details.aspx?familyid=22f46b3b-9be6-45ea-a639-9974324ce4bd)  
(Mérsékelt)
</td>
<td style="border:1px solid black;">
Nem érintett
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
Windows XP Professional x64 Edition Service Pack 2
</td>
<td style="border:1px solid black;">
[Internet Explorer 6](http://www.microsoft.com/downloads/details.aspx?familyid=d494535a-b68e-4242-af85-5fa62f631ffc)  
(Kritikus)  
[Internet Explorer 7](http://www.microsoft.com/downloads/details.aspx?familyid=ff9c65fe-437c-426d-9096-dd89ff7927fd)  
(Kritikus)  
[Internet Explorer 8](http://www.microsoft.com/downloads/details.aspx?familyid=05413f6c-b4be-4892-b4b3-c54dd01fd95d)  
(Kritikus)
</td>
<td style="border:1px solid black;">
Nem érintett
</td>
<td style="border:1px solid black;">
[Windows XP Professional x64 Edition Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=860ff738-205d-430e-b223-b333813fc590)  
(Kritikus)
</td>
<td style="border:1px solid black;">
[Microsoft .NET-keretrendszer 4.0](http://www.microsoft.com/downloads/details.aspx?familyid=bbc22169-996f-48d1-beed-0ee0dc4fbf4f)<sup>[1]</sup>
(Kritikus)
</td>
<td style="border:1px solid black;">
[Windows XP Professional x64 Edition Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=7fd7c675-0675-4a87-a709-edc47a30f1e2)  
(Fontos)
</td>
<td style="border:1px solid black;">
[Windows XP Professional x64 Edition Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=1ad30596-bac6-4d48-8b15-0245960c443b)  
(Fontos)
</td>
<td style="border:1px solid black;">
[Windows XP Professional x64 Edition Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=6c651bca-adb1-4172-9714-cd5a6e5d2c2a)  
(Fontos)
</td>
<td style="border:1px solid black;">
[Windows Media Player 10](http://www.microsoft.com/downloads/details.aspx?familyid=0663e0e8-c5d1-4cd2-b6d3-ff78fb56bba1)  
(Fontos)  
[Windows Media Player 11](http://www.microsoft.com/downloads/details.aspx?familyid=474b5618-dfe6-40de-b59b-1fd61a05749e)  
(Fontos)
</td>
<td style="border:1px solid black;">
[Windows XP Professional x64 Edition Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=4b6f0898-8f77-4ce1-9c96-2b17c496230b)  
(KB979687)  
(Fontos)
</td>
<td style="border:1px solid black;">
[Windows XP Professional x64 Edition Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=d690846c-5e0b-4216-84cd-d17e366dd16d)  
(Fontos)
</td>
<td style="border:1px solid black;">
Nem érintett
</td>
<td style="border:1px solid black;">
[Windows XP Professional x64 Edition Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=285627b9-242d-4247-a4c8-55dc89386b62)  
(Mérsékelt)
</td>
<td style="border:1px solid black;">
Nem érintett
</td>
</tr>
<tr>
<th colspan="14">
Windows Server 2003
</th>
</tr>
<tr>
<td style="border:1px solid black;">
**Közlemény azonosítója**
</td>
<td style="border:1px solid black;">
[**MS10-071**](http://go.microsoft.com/fwlink/?linkid=202013)
</td>
<td style="border:1px solid black;">
[**MS10-075**](http://go.microsoft.com/fwlink/?linkid=201722)
</td>
<td style="border:1px solid black;">
[**MS10-076**](http://go.microsoft.com/fwlink/?linkid=194560)
</td>
<td style="border:1px solid black;">
[**MS10-077**](http://go.microsoft.com/fwlink/?linkid=201704)
</td>
<td style="border:1px solid black;">
[**MS10-073**](http://go.microsoft.com/fwlink/?linkid=201093)
</td>
<td style="border:1px solid black;">
[**MS10-078**](http://go.microsoft.com/fwlink/?linkid=201084)
</td>
<td style="border:1px solid black;">
[**MS10-081**](http://go.microsoft.com/fwlink/?linkid=201086)
</td>
<td style="border:1px solid black;">
[**MS10-082**](http://go.microsoft.com/fwlink/?linkid=201098)
</td>
<td style="border:1px solid black;">
[**MS10-083**](http://go.microsoft.com/fwlink/?linkid=190553)
</td>
<td style="border:1px solid black;">
[**MS10-084**](http://go.microsoft.com/fwlink/?linkid=201720)
</td>
<td style="border:1px solid black;">
[**MS10-085**](http://go.microsoft.com/fwlink/?linkid=201705)
</td>
<td style="border:1px solid black;">
[**MS10-074**](http://go.microsoft.com/fwlink/?linkid=201703)
</td>
<td style="border:1px solid black;">
[**MS10-086**](http://go.microsoft.com/fwlink/?linkid=201721)
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
**Összesített súlyossági besorolás**
</td>
<td style="border:1px solid black;">
[**Fontos**](http://go.microsoft.com/fwlink/?linkid=21140)
</td>
<td style="border:1px solid black;">
Nincsenek
</td>
<td style="border:1px solid black;">
[**Kritikus**](http://go.microsoft.com/fwlink/?linkid=21140)
</td>
<td style="border:1px solid black;">
[**Kritikus**](http://go.microsoft.com/fwlink/?linkid=21140)
</td>
<td style="border:1px solid black;">
[**Fontos**](http://go.microsoft.com/fwlink/?linkid=21140)
</td>
<td style="border:1px solid black;">
[**Fontos**](http://go.microsoft.com/fwlink/?linkid=21140)
</td>
<td style="border:1px solid black;">
[**Fontos**](http://go.microsoft.com/fwlink/?linkid=21140)
</td>
<td style="border:1px solid black;">
[**Fontos**](http://go.microsoft.com/fwlink/?linkid=21140)
</td>
<td style="border:1px solid black;">
[**Fontos**](http://go.microsoft.com/fwlink/?linkid=21140)
</td>
<td style="border:1px solid black;">
[**Fontos**](http://go.microsoft.com/fwlink/?linkid=21140)
</td>
<td style="border:1px solid black;">
Nincsenek
</td>
<td style="border:1px solid black;">
[**Mérsékelt**](http://go.microsoft.com/fwlink/?linkid=21140)
</td>
<td style="border:1px solid black;">
Nincsenek
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Windows Server 2003 Service Pack 2
</td>
<td style="border:1px solid black;">
[Internet Explorer 6](http://www.microsoft.com/downloads/details.aspx?familyid=f64af3cd-591d-4212-94a0-3bc9a4d9782a)  
(Fontos)  
[Internet Explorer 7](http://www.microsoft.com/downloads/details.aspx?familyid=fbcf0e65-c9f4-47f8-b4fc-ae46a66ab339)  
(Fontos)  
[Internet Explorer 8](http://www.microsoft.com/downloads/details.aspx?familyid=9af37f62-5585-4ff5-9dd3-3fa0b148ae08)  
(Fontos)
</td>
<td style="border:1px solid black;">
Nem érintett
</td>
<td style="border:1px solid black;">
[Windows Server 2003 Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=7b240b65-f3ca-465c-a606-b561999c1977)  
(Kritikus)
</td>
<td style="border:1px solid black;">
Nem érintett
</td>
<td style="border:1px solid black;">
[Windows Server 2003 Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=8ef4378e-21ff-4290-96ba-e00a60f372d1)  
(Fontos)
</td>
<td style="border:1px solid black;">
[Windows Server 2003 Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=f94763e7-b1db-4043-aa79-d5be1a42307d)  
(Fontos)
</td>
<td style="border:1px solid black;">
[Windows Server 2003 Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=3b2eb449-ad55-4dfb-a3c5-aac767de6f45)  
(Fontos)
</td>
<td style="border:1px solid black;">
[Windows Media Player 10](http://www.microsoft.com/downloads/details.aspx?familyid=5479fd20-50d1-447a-8555-a98ce0723f71)  
(Fontos)
</td>
<td style="border:1px solid black;">
[Windows Server 2003 Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=13c08ec0-53ae-4b85-b669-8c88f6089259)  
(KB979687)  
(Fontos)
</td>
<td style="border:1px solid black;">
[Windows Server 2003 Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=b31e18b0-da9f-4b3b-82c6-603e08b3b241)  
(Fontos)
</td>
<td style="border:1px solid black;">
Nem érintett
</td>
<td style="border:1px solid black;">
[Windows Server 2003 Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=d220f04e-9dbb-4b6d-924a-23065b48b8b6)  
(Mérsékelt)
</td>
<td style="border:1px solid black;">
Nem érintett
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
Windows Server 2003 x64 Edition Service Pack 2
</td>
<td style="border:1px solid black;">
[Internet Explorer 6](http://www.microsoft.com/downloads/details.aspx?familyid=12c3b950-b955-4820-9b4c-5206deb0cd3e)  
(Fontos)  
[Internet Explorer 7](http://www.microsoft.com/downloads/details.aspx?familyid=59a715a5-10ff-40e6-88e0-096c9b640799)  
(Fontos)  
[Internet Explorer 8](http://www.microsoft.com/downloads/details.aspx?familyid=c8052f0c-e62c-46c4-bb59-d515fa388ea8)  
(Fontos)
</td>
<td style="border:1px solid black;">
Nem érintett
</td>
<td style="border:1px solid black;">
[Windows Server 2003 x64 Edition Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=70c9e826-b80b-4a20-82d2-8e52e5cca839)  
(Kritikus)
</td>
<td style="border:1px solid black;">
[Microsoft .NET-keretrendszer 4.0](http://www.microsoft.com/downloads/details.aspx?familyid=bbc22169-996f-48d1-beed-0ee0dc4fbf4f)<sup>[1]</sup>
(Kritikus)
</td>
<td style="border:1px solid black;">
[Windows Server 2003 x64 Edition Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=4a95c74b-cfd8-45b5-8887-777429d21745)  
(Fontos)
</td>
<td style="border:1px solid black;">
[Windows Server 2003 x64 Edition Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=6fca5cab-7e11-4911-a6a8-f73f113b2963)  
(Fontos)
</td>
<td style="border:1px solid black;">
[Windows Server 2003 x64 Edition Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=54fc4bc6-f46c-447c-8307-afd8338e7ffb)  
(Fontos)
</td>
<td style="border:1px solid black;">
[Windows Media Player 10](http://www.microsoft.com/downloads/details.aspx?familyid=a9515e69-c147-4810-8c5a-6cb94c398a95)  
(Fontos)
</td>
<td style="border:1px solid black;">
[Windows Server 2003 x64 Edition Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=02519f9e-e1c5-48a1-8420-01898c45ec01)  
(KB979687)  
(Fontos)
</td>
<td style="border:1px solid black;">
[Windows Server 2003 x64 Edition Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=1d73f0f1-6ec8-4304-a20e-345d8b6c225a)  
(Fontos)
</td>
<td style="border:1px solid black;">
Nem érintett
</td>
<td style="border:1px solid black;">
[Windows Server 2003 x64 Edition Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=de908137-33e0-4f23-b32b-cc1bdbcb349c)  
(Mérsékelt)
</td>
<td style="border:1px solid black;">
Nem érintett
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Windows Server 2003 SP2 Itanium-alapú rendszerekhez
</td>
<td style="border:1px solid black;">
[Internet Explorer 6](http://www.microsoft.com/downloads/details.aspx?familyid=97b3f6dc-8df5-4c93-aaee-f191498c7ce4)  
(Fontos)  
[Internet Explorer 7](http://www.microsoft.com/downloads/details.aspx?familyid=ba194be9-24f9-4c62-9aa9-9e98c81ddba1)  
(Fontos)
</td>
<td style="border:1px solid black;">
Nem érintett
</td>
<td style="border:1px solid black;">
[Windows Server 2003 SP2 Itanium-alapú rendszerekhez](http://www.microsoft.com/downloads/details.aspx?familyid=bd5878bb-f565-4303-afed-4e17b44a02f2)  
(Kritikus)
</td>
<td style="border:1px solid black;">
[Microsoft .NET-keretrendszer 4.0](http://www.microsoft.com/downloads/details.aspx?familyid=bbc22169-996f-48d1-beed-0ee0dc4fbf4f)<sup>[1]</sup>
(Kritikus)
</td>
<td style="border:1px solid black;">
[Windows Server 2003 SP2 Itanium-alapú rendszerekhez](http://www.microsoft.com/downloads/details.aspx?familyid=21637cd8-c75c-43b4-9948-be7be54af6bf)  
(Fontos)
</td>
<td style="border:1px solid black;">
[Windows Server 2003 SP2 Itanium-alapú rendszerekhez](http://www.microsoft.com/downloads/details.aspx?familyid=e8f297e2-0dfd-421a-b598-a78199ad6baa)  
(Fontos)
</td>
<td style="border:1px solid black;">
[Windows Server 2003 SP2 Itanium-alapú rendszerekhez](http://www.microsoft.com/downloads/details.aspx?familyid=64f5c311-d74a-4665-9775-ac91c6885ed3)  
(Fontos)
</td>
<td style="border:1px solid black;">
Nem érintett
</td>
<td style="border:1px solid black;">
[Windows Server 2003 SP2 Itanium-alapú rendszerekhez](http://www.microsoft.com/downloads/details.aspx?familyid=1064bccb-3ce6-4a72-8788-56d8021bca91)  
(KB979687)  
(Fontos)
</td>
<td style="border:1px solid black;">
[Windows Server 2003 SP2 Itanium-alapú rendszerekhez](http://www.microsoft.com/downloads/details.aspx?familyid=8fad4f77-7c89-4684-b957-9c00ced248d3)  
(Fontos)
</td>
<td style="border:1px solid black;">
Nem érintett
</td>
<td style="border:1px solid black;">
[Windows Server 2003 SP2 Itanium-alapú rendszerekhez](http://www.microsoft.com/downloads/details.aspx?familyid=873dea9d-44cc-4e16-8a6d-dca678ce3a80)  
(Mérsékelt)
</td>
<td style="border:1px solid black;">
Nem érintett
</td>
</tr>
<tr>
<th colspan="14">
Windows Vista
</th>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
**Közlemény azonosítója**
</td>
<td style="border:1px solid black;">
[**MS10-071**](http://go.microsoft.com/fwlink/?linkid=202013)
</td>
<td style="border:1px solid black;">
[**MS10-075**](http://go.microsoft.com/fwlink/?linkid=201722)
</td>
<td style="border:1px solid black;">
[**MS10-076**](http://go.microsoft.com/fwlink/?linkid=194560)
</td>
<td style="border:1px solid black;">
[**MS10-077**](http://go.microsoft.com/fwlink/?linkid=201704)
</td>
<td style="border:1px solid black;">
[**MS10-073**](http://go.microsoft.com/fwlink/?linkid=201093)
</td>
<td style="border:1px solid black;">
[**MS10-078**](http://go.microsoft.com/fwlink/?linkid=201084)
</td>
<td style="border:1px solid black;">
[**MS10-081**](http://go.microsoft.com/fwlink/?linkid=201086)
</td>
<td style="border:1px solid black;">
[**MS10-082**](http://go.microsoft.com/fwlink/?linkid=201098)
</td>
<td style="border:1px solid black;">
[**MS10-083**](http://go.microsoft.com/fwlink/?linkid=190553)
</td>
<td style="border:1px solid black;">
[**MS10-084**](http://go.microsoft.com/fwlink/?linkid=201720)
</td>
<td style="border:1px solid black;">
[**MS10-085**](http://go.microsoft.com/fwlink/?linkid=201705)
</td>
<td style="border:1px solid black;">
[**MS10-074**](http://go.microsoft.com/fwlink/?linkid=201703)
</td>
<td style="border:1px solid black;">
[**MS10-086**](http://go.microsoft.com/fwlink/?linkid=201721)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
**Összesített súlyossági besorolás**
</td>
<td style="border:1px solid black;">
[**Kritikus**](http://go.microsoft.com/fwlink/?linkid=21140)
</td>
<td style="border:1px solid black;">
[**Fontos**](http://go.microsoft.com/fwlink/?linkid=21140)
</td>
<td style="border:1px solid black;">
[**Kritikus**](http://go.microsoft.com/fwlink/?linkid=21140)
</td>
<td style="border:1px solid black;">
[**Kritikus**](http://go.microsoft.com/fwlink/?linkid=21140)
</td>
<td style="border:1px solid black;">
[**Fontos**](http://go.microsoft.com/fwlink/?linkid=21140)
</td>
<td style="border:1px solid black;">
Nincsenek
</td>
<td style="border:1px solid black;">
[**Fontos**](http://go.microsoft.com/fwlink/?linkid=21140)
</td>
<td style="border:1px solid black;">
[**Fontos**](http://go.microsoft.com/fwlink/?linkid=21140)
</td>
<td style="border:1px solid black;">
[**Fontos**](http://go.microsoft.com/fwlink/?linkid=21140)
</td>
<td style="border:1px solid black;">
Nincsenek
</td>
<td style="border:1px solid black;">
[**Fontos**](http://go.microsoft.com/fwlink/?linkid=21140)
</td>
<td style="border:1px solid black;">
[**Mérsékelt.**](http://go.microsoft.com/fwlink/?linkid=21140)
</td>
<td style="border:1px solid black;">
Nincsenek
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
Windows Vista Service Pack 1 és Windows Vista Service Pack 2
</td>
<td style="border:1px solid black;">
[Internet Explorer 7](http://www.microsoft.com/downloads/details.aspx?familyid=4f656d16-2a7e-4d18-8a5a-ebf8a1a10e2b)  
(Kritikus)  
[Internet Explorer 8](http://www.microsoft.com/downloads/details.aspx?familyid=191c8388-f1ef-45b6-9f07-d5654a973abe)  
(Kritikus)
</td>
<td style="border:1px solid black;">
[Windows Vista Service Pack 1 és Windows Vista Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=4a481825-d9ad-4a7c-aa89-f40fb9651961)  
(Fontos)
</td>
<td style="border:1px solid black;">
[Windows Vista Service Pack 1 és Windows Vista Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=29c4afb1-227d-4572-b136-a78ef7e1df77)  
(Kritikus)
</td>
<td style="border:1px solid black;">
Nem érintett
</td>
<td style="border:1px solid black;">
[Windows Vista Service Pack 1 és Windows Vista Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=e9f735ab-d995-4209-b2dc-197f53fdee0f)  
(Fontos)
</td>
<td style="border:1px solid black;">
Nem érintett
</td>
<td style="border:1px solid black;">
[Windows Vista Service Pack 1 és Windows Vista Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=95ceafc6-e37a-4c77-b16e-c9c94a7d89bd)  
(Fontos)
</td>
<td style="border:1px solid black;">
[Windows Media Player 11](http://www.microsoft.com/downloads/details.aspx?familyid=95e24a63-d21a-4756-a16e-17a977595396)  
(Fontos)
</td>
<td style="border:1px solid black;">
[Windows Vista Service Pack 1 és Windows Vista Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=80c99d69-4b97-4af2-8f8e-f3b300a89a5a)<sup>[1]</sup>
(KB979687)  
(Fontos)  
[Windows Vista Service Pack 1 és Windows Vista Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=dff92449-22ad-49a8-8b28-5295a8af5b8b)<sup>[1]</sup>
(KB979688)  
(Fontos)
</td>
<td style="border:1px solid black;">
Nem érintett
</td>
<td style="border:1px solid black;">
[Windows Vista Service Pack 1 és Windows Vista Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=4af2f6e6-6905-498c-bfba-a565976b3365)  
(Fontos)
</td>
<td style="border:1px solid black;">
[Windows Vista Service Pack 1 és Windows Vista Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=75ca4e2c-b0ae-46f4-a0fc-616510c41a55)  
(Mérsékelt)
</td>
<td style="border:1px solid black;">
Nem érintett
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Windows Vista x64 Edition Service Pack 1 és Windows Vista x64 Edition Service Pack 2
</td>
<td style="border:1px solid black;">
[Internet Explorer 7](http://www.microsoft.com/downloads/details.aspx?familyid=02c6260c-8e21-401a-992d-884c6ff7141d)  
(Kritikus)  
[Internet Explorer 8](http://www.microsoft.com/downloads/details.aspx?familyid=adeb3036-62fa-4a29-b82f-ff4a50c05996)  
(Kritikus)
</td>
<td style="border:1px solid black;">
[Windows Vista x64 Edition Service Pack 1 és Windows Vista x64 Edition Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=15d8f81b-97b0-43d9-b218-1cdd759cb2ec)  
(Fontos)
</td>
<td style="border:1px solid black;">
[Windows Vista x64 Edition Service Pack 1 és Windows Vista x64 Edition Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=880ad9a0-6ddd-41f4-a608-171d59a31b6a)  
(Kritikus)
</td>
<td style="border:1px solid black;">
[Microsoft .NET-keretrendszer 4.0](http://www.microsoft.com/downloads/details.aspx?familyid=bbc22169-996f-48d1-beed-0ee0dc4fbf4f)<sup>[1]</sup>
(Kritikus)
</td>
<td style="border:1px solid black;">
[Windows Vista x64 Edition Service Pack 1 és Windows Vista x64 Edition Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=738c8f70-b46a-4a59-bea6-078074a9c4db)  
(Fontos)
</td>
<td style="border:1px solid black;">
Nem érintett
</td>
<td style="border:1px solid black;">
[Windows Vista x64 Edition Service Pack 1 és Windows Vista x64 Edition Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=dfe7cd18-53a3-433e-9a33-bd96b04b4deb)  
(Fontos)
</td>
<td style="border:1px solid black;">
[Windows Media Player 11](http://www.microsoft.com/downloads/details.aspx?familyid=277151a2-b74f-4da6-8203-e774af75e44c)  
(Fontos)
</td>
<td style="border:1px solid black;">
[Windows Vista x64 Edition Service Pack 1 és Windows Vista x64 Edition Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=b73951f2-a7eb-4c7c-bf60-fdcfee83574f)<sup>[1]</sup>
(KB979687)  
(Fontos)  
[Windows Vista x64 Edition Service Pack 1 és Windows Vista x64 Edition Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=c9d2261f-bd9a-4495-a2f1-3c3b2208b01e)<sup>[1]</sup>
(KB979688)  
(Fontos)
</td>
<td style="border:1px solid black;">
Nem érintett
</td>
<td style="border:1px solid black;">
[Windows Vista x64 Edition Service Pack 1 és Windows Vista x64 Edition Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=8c56ba29-b2a8-47a8-a605-4c54c0a7fa7c)  
(Fontos)
</td>
<td style="border:1px solid black;">
[Windows Vista x64 Edition Service Pack 1 és Windows Vista x64 Edition Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=0a12ff95-ea5c-4c48-96c5-9494eb8f9f0d)  
(Mérsékelt)
</td>
<td style="border:1px solid black;">
Nem érintett
</td>
</tr>
<tr>
<th colspan="14">
Windows Server 2008
</th>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
**Közlemény azonosítója**
</td>
<td style="border:1px solid black;">
[**MS10-071**](http://go.microsoft.com/fwlink/?linkid=202013)
</td>
<td style="border:1px solid black;">
[**MS10-075**](http://go.microsoft.com/fwlink/?linkid=201722)
</td>
<td style="border:1px solid black;">
[**MS10-076**](http://go.microsoft.com/fwlink/?linkid=194560)
</td>
<td style="border:1px solid black;">
[**MS10-077**](http://go.microsoft.com/fwlink/?linkid=201704)
</td>
<td style="border:1px solid black;">
[**MS10-073**](http://go.microsoft.com/fwlink/?linkid=201093)
</td>
<td style="border:1px solid black;">
[**MS10-078**](http://go.microsoft.com/fwlink/?linkid=201084)
</td>
<td style="border:1px solid black;">
[**MS10-081**](http://go.microsoft.com/fwlink/?linkid=201086)
</td>
<td style="border:1px solid black;">
[**MS10-082**](http://go.microsoft.com/fwlink/?linkid=201098)
</td>
<td style="border:1px solid black;">
[**MS10-083**](http://go.microsoft.com/fwlink/?linkid=190553)
</td>
<td style="border:1px solid black;">
[**MS10-084**](http://go.microsoft.com/fwlink/?linkid=201720)
</td>
<td style="border:1px solid black;">
[**MS10-085**](http://go.microsoft.com/fwlink/?linkid=201705)
</td>
<td style="border:1px solid black;">
[**MS10-074**](http://go.microsoft.com/fwlink/?linkid=201703)
</td>
<td style="border:1px solid black;">
[**MS10-086**](http://go.microsoft.com/fwlink/?linkid=201721)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
**Összesített súlyossági besorolás**
</td>
<td style="border:1px solid black;">
[**Fontos**](http://go.microsoft.com/fwlink/?linkid=21140)
</td>
<td style="border:1px solid black;">
Nincsenek
</td>
<td style="border:1px solid black;">
[**Kritikus**](http://go.microsoft.com/fwlink/?linkid=21140)
</td>
<td style="border:1px solid black;">
[**Fontos**](http://go.microsoft.com/fwlink/?linkid=21140)
</td>
<td style="border:1px solid black;">
[**Fontos**](http://go.microsoft.com/fwlink/?linkid=21140)
</td>
<td style="border:1px solid black;">
Nincsenek
</td>
<td style="border:1px solid black;">
[**Fontos**](http://go.microsoft.com/fwlink/?linkid=21140)
</td>
<td style="border:1px solid black;">
[**Mérsékelt.**](http://go.microsoft.com/fwlink/?linkid=21140)
</td>
<td style="border:1px solid black;">
[**Fontos**](http://go.microsoft.com/fwlink/?linkid=21140)
</td>
<td style="border:1px solid black;">
Nincsenek
</td>
<td style="border:1px solid black;">
[**Fontos**](http://go.microsoft.com/fwlink/?linkid=21140)
</td>
<td style="border:1px solid black;">
[**Mérsékelt.**](http://go.microsoft.com/fwlink/?linkid=21140)
</td>
<td style="border:1px solid black;">
Nincsenek
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
Windows Server 2008 32 bites rendszerekhez és Windows Server 2008 32 bites rendszerekhez, Service Pack 2
</td>
<td style="border:1px solid black;">
[Internet Explorer 7](http://www.microsoft.com/downloads/details.aspx?familyid=0107dd61-7b3e-4fcf-9743-d9ae594b2278)\*\*  
(Fontos)  
[Internet Explorer 8](http://www.microsoft.com/downloads/details.aspx?familyid=ea5b7c86-3878-43a9-a4bc-12e04bfbd06e)\*\*  
(Fontos)
</td>
<td style="border:1px solid black;">
Nem érintett
</td>
<td style="border:1px solid black;">
[Windows Server 2008 32 bites rendszerekhez és Windows Server 2008 32 bites rendszerekhez Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=50386655-982e-4126-8261-2c972d695bbd)\*\*  
(Kritikus)
</td>
<td style="border:1px solid black;">
Nem érintett
</td>
<td style="border:1px solid black;">
[Windows Server 2008 32 bites rendszerekhez és Windows Server 2008 32 bites rendszerekhez, Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=4dff0ebe-ccba-4675-98ca-9903f1cb6763)\*  
(Fontos)
</td>
<td style="border:1px solid black;">
Nem érintett
</td>
<td style="border:1px solid black;">
[Windows Server 2008 32 bites rendszerekhez és Windows Server 2008 32 bites rendszerekhez Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=d5f079b0-d8e1-47fe-b9dd-41eeb463a93c)\*\*  
(Fontos)
</td>
<td style="border:1px solid black;">
[Windows Media Player 11](http://www.microsoft.com/downloads/details.aspx?familyid=67eb3a70-9ca7-4184-b9fe-cc3e66b1bf36) \*\*  
(Mérsékelt)
</td>
<td style="border:1px solid black;">
[Windows Server 2008 32 bites rendszerekhez és Windows Server 2008 32 bites rendszerekhez Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=fd507e7a-4516-474b-8f33-7fa8fd2afa6d)\*\*<sup>[1]</sup>
(KB979687)  
(Fontos)  
[Windows Server 2008 32 bites rendszerekhez és Windows Server 2008 32 bites rendszerekhez Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=4a8c2358-36ea-4757-abfc-5bffcad0a872)\*\*<sup>[1]</sup>
(KB979688)  
(Fontos)
</td>
<td style="border:1px solid black;">
Nem érintett
</td>
<td style="border:1px solid black;">
[Windows Server 2008 32 bites rendszerekhez és Windows Server 2008 32 bites rendszerekhez, Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=0566915f-2a1b-474b-b5f1-e1a9cedd836a)\*  
(Fontos)
</td>
<td style="border:1px solid black;">
[Windows Server 2008 32 bites rendszerekhez és Windows Server 2008 32 bites rendszerekhez Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=952b3594-d980-45b1-8fa3-49403784afbf)\*\*  
(Mérsékelt)
</td>
<td style="border:1px solid black;">
Nem érintett
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Windows Server 2008 x64-alapú rendszerekhez és Windows Server 2008 x64-alapú rendszerekhez, Service Pack 2
</td>
<td style="border:1px solid black;">
[Internet Explorer 7](http://www.microsoft.com/downloads/details.aspx?familyid=139f3bb2-eefc-4cf4-9c15-de78f5a736c1)\*\*  
(Fontos)  
[Internet Explorer 8](http://www.microsoft.com/downloads/details.aspx?familyid=71ecdb27-46aa-4db1-b86a-3268cda88632)\*\*  
(Fontos)
</td>
<td style="border:1px solid black;">
Nem érintett
</td>
<td style="border:1px solid black;">
[Windows Server 2008 x64 alapú rendszerekhez és Windows Server 2008 x64 alapú rendszerekhez Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=a6b2ae1d-9225-4495-8560-97860f87d7b4)\*\*  
(Kritikus)
</td>
<td style="border:1px solid black;">
[Microsoft .NET-keretrendszer 4.0](http://www.microsoft.com/downloads/details.aspx?familyid=bbc22169-996f-48d1-beed-0ee0dc4fbf4f)\*\*<sup>[1]</sup>
(Fontos)
</td>
<td style="border:1px solid black;">
[Windows Server 2008 x64 alapú rendszerekhez és Windows Server 2008 x64 alapú rendszerekhez, Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=da7905a9-9587-4184-8fca-ecc636a3b67e)\*  
(Fontos)
</td>
<td style="border:1px solid black;">
Nem érintett
</td>
<td style="border:1px solid black;">
[Windows Server 2008 x64 alapú rendszerekhez és Windows Server 2008 x64 alapú rendszerekhez Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=8e88d9c5-eb57-4d39-a880-a478c5f286da)\*\*  
(Fontos)
</td>
<td style="border:1px solid black;">
[Windows Media Player 11](http://www.microsoft.com/downloads/details.aspx?familyid=33a06f0e-81ab-445a-bc89-14350ebfe688) \*\*  
(Mérsékelt)
</td>
<td style="border:1px solid black;">
[Windows Server 2008 x64 alapú rendszerekhez és Windows Server 2008 x64 alapú rendszerekhez Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=b5f53faf-61e2-4b4e-8b85-c5e8f38e5c30)\*\*<sup>[1]</sup>
(KB979687)  
(Fontos)  
[Windows Server 2008 x64 alapú rendszerekhez és Windows Server 2008 x64 alapú rendszerekhez Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=612ab78c-1ff1-45d2-96cc-ae831fb0a563)\*\*<sup>[1]</sup>
(KB979688)  
(Fontos)
</td>
<td style="border:1px solid black;">
Nem érintett
</td>
<td style="border:1px solid black;">
[Windows Server 2008 x64 alapú rendszerekhez és Windows Server 2008 x64 alapú rendszerekhez, Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=74ac2233-02ec-454c-8aa0-64b18071e16a)\*  
(Fontos)
</td>
<td style="border:1px solid black;">
[Windows Server 2008 x64 alapú rendszerekhez és Windows Server 2008 x64 alapú rendszerekhez Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=21128031-d935-4e2d-b001-c502a2d6022c)\*\*  
(Mérsékelt)
</td>
<td style="border:1px solid black;">
Nem érintett
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
Windows Server 2008 Itanium-alapú rendszerekhez és Windows Server 2008 Itanium-alapú rendszerekhez, Service Pack 2
</td>
<td style="border:1px solid black;">
[Internet Explorer 7](http://www.microsoft.com/downloads/details.aspx?familyid=1a971fb2-7dc4-43bf-ae25-3a420bb1acf9)  
(Fontos)
</td>
<td style="border:1px solid black;">
Nem érintett
</td>
<td style="border:1px solid black;">
[Windows Server 2008 Itanium-alapú rendszerekhez és Windows Server 2008 Itanium-alapú rendszerekhez, Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=a4e38a77-3835-47b3-bd86-6c039169abf5)  
(Kritikus)
</td>
<td style="border:1px solid black;">
[Microsoft .NET-keretrendszer 4.0](http://www.microsoft.com/downloads/details.aspx?familyid=bbc22169-996f-48d1-beed-0ee0dc4fbf4f)<sup>[1]</sup>
(Fontos)
</td>
<td style="border:1px solid black;">
[Windows Server 2008 Itanium-alapú rendszerekhez és Windows Server 2008 Itanium-alapú rendszerekhez, Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=b9096046-8c7a-450c-b8c5-6e9fb001e6cd)  
(Fontos)
</td>
<td style="border:1px solid black;">
Nem érintett
</td>
<td style="border:1px solid black;">
[Windows Server 2008 Itanium-alapú rendszerekhez és Windows Server 2008 Itanium-alapú rendszerekhez, Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=76e46d08-22d9-4a0c-82cd-d2753d07efe6)  
(Fontos)
</td>
<td style="border:1px solid black;">
Nem érintett
</td>
<td style="border:1px solid black;">
[Windows Server 2008 Itanium-alapú rendszerekhez és Windows Server 2008 Itanium-alapú rendszerekhez, Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=5efe55b0-d34d-4f00-98b2-cc0e9807a8b9)<sup>[1]</sup>
(KB979687)  
(Fontos)  
[Windows Server 2008 Itanium-alapú rendszerekhez és Windows Server 2008 Itanium-alapú rendszerekhez, Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=d30368cb-c6e8-403e-aaf6-425f96b6211e)<sup>[1]</sup>
(KB979688)  
(Fontos)
</td>
<td style="border:1px solid black;">
Nem érintett
</td>
<td style="border:1px solid black;">
[Windows Server 2008 Itanium-alapú rendszerekhez és Windows Server 2008 Itanium-alapú rendszerekhez, Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=2fff281a-2221-42a3-a2b7-07b5c5e66ae7)  
(Fontos)
</td>
<td style="border:1px solid black;">
[Windows Server 2008 Itanium-alapú rendszerekhez és Windows Server 2008 Itanium-alapú rendszerekhez, Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=2eca0c38-73f5-4f83-ab62-97f979716a1d)  
(Mérsékelt)
</td>
<td style="border:1px solid black;">
Nem érintett
</td>
</tr>
<tr>
<th colspan="14">
Windows 7
</th>
</tr>
<tr>
<td style="border:1px solid black;">
**Közlemény azonosítója**
</td>
<td style="border:1px solid black;">
[**MS10-071**](http://go.microsoft.com/fwlink/?linkid=202013)
</td>
<td style="border:1px solid black;">
[**MS10-075**](http://go.microsoft.com/fwlink/?linkid=201722)
</td>
<td style="border:1px solid black;">
[**MS10-076**](http://go.microsoft.com/fwlink/?linkid=194560)
</td>
<td style="border:1px solid black;">
[**MS10-077**](http://go.microsoft.com/fwlink/?linkid=201704)
</td>
<td style="border:1px solid black;">
[**MS10-073**](http://go.microsoft.com/fwlink/?linkid=201093)
</td>
<td style="border:1px solid black;">
[**MS10-078**](http://go.microsoft.com/fwlink/?linkid=201084)
</td>
<td style="border:1px solid black;">
[**MS10-081**](http://go.microsoft.com/fwlink/?linkid=201086)
</td>
<td style="border:1px solid black;">
[**MS10-082**](http://go.microsoft.com/fwlink/?linkid=201098)
</td>
<td style="border:1px solid black;">
[**MS10-083**](http://go.microsoft.com/fwlink/?linkid=190553)
</td>
<td style="border:1px solid black;">
[**MS10-084**](http://go.microsoft.com/fwlink/?linkid=201720)
</td>
<td style="border:1px solid black;">
[**MS10-085**](http://go.microsoft.com/fwlink/?linkid=201705)
</td>
<td style="border:1px solid black;">
[**MS10-074**](http://go.microsoft.com/fwlink/?linkid=201703)
</td>
<td style="border:1px solid black;">
[**MS10-086**](http://go.microsoft.com/fwlink/?linkid=201721)
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
**Összesített súlyossági besorolás**
</td>
<td style="border:1px solid black;">
[**Kritikus**](http://go.microsoft.com/fwlink/?linkid=21140)
</td>
<td style="border:1px solid black;">
[**Kritikus**](http://go.microsoft.com/fwlink/?linkid=21140)
</td>
<td style="border:1px solid black;">
[**Kritikus**](http://go.microsoft.com/fwlink/?linkid=21140)
</td>
<td style="border:1px solid black;">
[**Kritikus**](http://go.microsoft.com/fwlink/?linkid=21140)
</td>
<td style="border:1px solid black;">
[**Fontos**](http://go.microsoft.com/fwlink/?linkid=21140)
</td>
<td style="border:1px solid black;">
[Nincsenek](http://go.microsoft.com/fwlink/?linkid=21140)
</td>
<td style="border:1px solid black;">
[**Fontos**](http://go.microsoft.com/fwlink/?linkid=21140)
</td>
<td style="border:1px solid black;">
[**Fontos**](http://go.microsoft.com/fwlink/?linkid=21140)
</td>
<td style="border:1px solid black;">
[**Fontos**](http://go.microsoft.com/fwlink/?linkid=21140)
</td>
<td style="border:1px solid black;">
Nincsenek
</td>
<td style="border:1px solid black;">
[**Fontos**](http://go.microsoft.com/fwlink/?linkid=21140)
</td>
<td style="border:1px solid black;">
[**Mérsékelt**](http://go.microsoft.com/fwlink/?linkid=21140)
</td>
<td style="border:1px solid black;">
Nincsenek
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Windows 7 32 bites rendszerekhez
</td>
<td style="border:1px solid black;">
[Internet Explorer 8](http://www.microsoft.com/downloads/details.aspx?familyid=6595770f-e580-4613-a83a-3b8ee4cc30f1)  
(Kritikus)
</td>
<td style="border:1px solid black;">
[Windows 7 32 bites rendszerekhez](http://www.microsoft.com/downloads/details.aspx?familyid=1a3953fe-ba48-4980-a65d-74e3b756d53c)  
(Kritikus)
</td>
<td style="border:1px solid black;">
[Windows 7 32 bites rendszerekhez](http://www.microsoft.com/downloads/details.aspx?familyid=f6cae091-e9f1-48e9-a035-4346b9c6fec6)  
(Kritikus)
</td>
<td style="border:1px solid black;">
Nem érintett
</td>
<td style="border:1px solid black;">
[Windows 7 32 bites rendszerekhez](http://www.microsoft.com/downloads/details.aspx?familyid=b5b31499-d242-42bf-ac78-b787ffb4d602)  
(Fontos)
</td>
<td style="border:1px solid black;">
Nem érintett
</td>
<td style="border:1px solid black;">
[Windows 7 32 bites rendszerekhez](http://www.microsoft.com/downloads/details.aspx?familyid=bdff9057-381a-44e8-b093-84f07d8d7e3c)  
(Fontos)
</td>
<td style="border:1px solid black;">
[Windows Media Player 12](http://www.microsoft.com/downloads/details.aspx?familyid=59a2ef36-9c32-488b-b5b1-30b5bcd83358)  
(Fontos)
</td>
<td style="border:1px solid black;">
[Windows 7 32 bites rendszerekhez](http://www.microsoft.com/downloads/details.aspx?familyid=b0d46bc3-24db-4207-b6fc-46b8cc64f075)<sup>[1]</sup>
(KB979687)  
(Fontos)  
[Windows 7 32 bites rendszerekhez](http://www.microsoft.com/downloads/details.aspx?familyid=4a422192-d7fa-47e5-9661-2c65eaefaf62)<sup>[1]</sup>
(KB979688)  
(Fontos)
</td>
<td style="border:1px solid black;">
Nem érintett
</td>
<td style="border:1px solid black;">
[Windows 7 32 bites rendszerekhez](http://www.microsoft.com/downloads/details.aspx?familyid=d7a08a66-08b4-421c-afad-f2f367d4a9f0)  
(Fontos)
</td>
<td style="border:1px solid black;">
[Windows 7 32 bites rendszerekhez](http://www.microsoft.com/downloads/details.aspx?familyid=f09fbc23-cb6b-4525-8e41-8c14e8d03de9)  
(Mérsékelt)
</td>
<td style="border:1px solid black;">
Nem érintett
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
Windows 7 x64-alapú rendszerekhez
</td>
<td style="border:1px solid black;">
[Internet Explorer 8](http://www.microsoft.com/downloads/details.aspx?familyid=ffe364ee-e2ae-466c-b727-14b1a976a860)  
(Kritikus)
</td>
<td style="border:1px solid black;">
[Windows 7 x64-alapú rendszerekhez](http://www.microsoft.com/downloads/details.aspx?familyid=5759d2a3-7f35-4fa1-8ab4-17145839fa26)  
(Kritikus)
</td>
<td style="border:1px solid black;">
[Windows 7 x64-alapú rendszerekhez](http://www.microsoft.com/downloads/details.aspx?familyid=35882477-4e0a-4783-a4b4-0f1ea3398360)  
(Kritikus)
</td>
<td style="border:1px solid black;">
[Microsoft .NET-keretrendszer 4.0](http://www.microsoft.com/downloads/details.aspx?familyid=bbc22169-996f-48d1-beed-0ee0dc4fbf4f)<sup>[1]</sup>
(Kritikus)
</td>
<td style="border:1px solid black;">
[Windows 7 x64-alapú rendszerekhez](http://www.microsoft.com/downloads/details.aspx?familyid=c47e8b74-8cfe-42d9-9362-8786687c88ad)  
(Fontos)
</td>
<td style="border:1px solid black;">
Nem érintett
</td>
<td style="border:1px solid black;">
[Windows 7 x64-alapú rendszerekhez](http://www.microsoft.com/downloads/details.aspx?familyid=35a2b1a9-6dd6-4a7e-bc0a-b4fcffa06b28)  
(Fontos)
</td>
<td style="border:1px solid black;">
[Windows Media Player 12](http://www.microsoft.com/downloads/details.aspx?familyid=00176d56-8a93-4780-96fc-a7ab715e7291)  
(Fontos)
</td>
<td style="border:1px solid black;">
[Windows 7 x64-alapú rendszerekhez](http://www.microsoft.com/downloads/details.aspx?familyid=2de197c0-6d9e-460e-9509-f337fac8ee85)<sup>[1]</sup>
(KB979687)  
(Fontos)  
[Windows 7 x64-alapú rendszerekhez](http://www.microsoft.com/downloads/details.aspx?familyid=03665687-8fd4-4afd-ac33-5f6824f51df8)<sup>[1]</sup>
(KB979688)  
(Fontos)
</td>
<td style="border:1px solid black;">
Nem érintett
</td>
<td style="border:1px solid black;">
[Windows 7 x64-alapú rendszerekhez](http://www.microsoft.com/downloads/details.aspx?familyid=50d27c23-5f69-40fa-b517-32c245009467)  
(Fontos)
</td>
<td style="border:1px solid black;">
[Windows 7 x64-alapú rendszerekhez](http://www.microsoft.com/downloads/details.aspx?familyid=abc24826-b83a-4e01-be68-8e3a73c10494)  
(Mérsékelt)
</td>
<td style="border:1px solid black;">
Nem érintett
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Windows 7 x64 alapú rendszerekhez, Service Pack 1
</td>
<td style="border:1px solid black;">
Nem érintett
</td>
<td style="border:1px solid black;">
Nem érintett
</td>
<td style="border:1px solid black;">
Nem érintett
</td>
<td style="border:1px solid black;">
[Microsoft .NET-keretrendszer 4.0](http://www.microsoft.com/downloads/details.aspx?familyid=bbc22169-996f-48d1-beed-0ee0dc4fbf4f)<sup>[1]</sup>
(Kritikus)
</td>
<td style="border:1px solid black;">
Nem érintett
</td>
<td style="border:1px solid black;">
Nem érintett
</td>
<td style="border:1px solid black;">
Nem érintett
</td>
<td style="border:1px solid black;">
Nem érintett
</td>
<td style="border:1px solid black;">
Nem érintett
</td>
<td style="border:1px solid black;">
Nem érintett
</td>
<td style="border:1px solid black;">
Nem érintett
</td>
<td style="border:1px solid black;">
Nem érintett
</td>
<td style="border:1px solid black;">
Nem érintett
</td>
</tr>
<tr>
<th colspan="14">
Windows Server 2008 R2
</th>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
**Közlemény azonosítója**
</td>
<td style="border:1px solid black;">
[**MS10-071**](http://go.microsoft.com/fwlink/?linkid=202013)
</td>
<td style="border:1px solid black;">
[**MS10-075**](http://go.microsoft.com/fwlink/?linkid=201722)
</td>
<td style="border:1px solid black;">
[**MS10-076**](http://go.microsoft.com/fwlink/?linkid=194560)
</td>
<td style="border:1px solid black;">
[**MS10-077**](http://go.microsoft.com/fwlink/?linkid=201704)
</td>
<td style="border:1px solid black;">
[**MS10-073**](http://go.microsoft.com/fwlink/?linkid=201093)
</td>
<td style="border:1px solid black;">
[**MS10-078**](http://go.microsoft.com/fwlink/?linkid=201084)
</td>
<td style="border:1px solid black;">
[**MS10-081**](http://go.microsoft.com/fwlink/?linkid=201086)
</td>
<td style="border:1px solid black;">
[**MS10-082**](http://go.microsoft.com/fwlink/?linkid=201098)
</td>
<td style="border:1px solid black;">
[**MS10-083**](http://go.microsoft.com/fwlink/?linkid=190553)
</td>
<td style="border:1px solid black;">
[**MS10-084**](http://go.microsoft.com/fwlink/?linkid=201720)
</td>
<td style="border:1px solid black;">
[**MS10-085**](http://go.microsoft.com/fwlink/?linkid=201705)
</td>
<td style="border:1px solid black;">
[**MS10-074**](http://go.microsoft.com/fwlink/?linkid=201703)
</td>
<td style="border:1px solid black;">
[**MS10-086**](http://go.microsoft.com/fwlink/?linkid=201721)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
**Összesített súlyossági besorolás**
</td>
<td style="border:1px solid black;">
[**Fontos**](http://go.microsoft.com/fwlink/?linkid=21140)
</td>
<td style="border:1px solid black;">
Nincsenek
</td>
<td style="border:1px solid black;">
[**Kritikus**](http://go.microsoft.com/fwlink/?linkid=21140)
</td>
<td style="border:1px solid black;">
[**Fontos**](http://go.microsoft.com/fwlink/?linkid=21140)
</td>
<td style="border:1px solid black;">
[**Fontos**](http://go.microsoft.com/fwlink/?linkid=21140)
</td>
<td style="border:1px solid black;">
Nincsenek
</td>
<td style="border:1px solid black;">
[**Fontos**](http://go.microsoft.com/fwlink/?linkid=21140)
</td>
<td style="border:1px solid black;">
[**Mérsékelt.**](http://go.microsoft.com/fwlink/?linkid=21140)
</td>
<td style="border:1px solid black;">
[**Fontos**](http://go.microsoft.com/fwlink/?linkid=21140)
</td>
<td style="border:1px solid black;">
Nincsenek
</td>
<td style="border:1px solid black;">
[**Fontos**](http://go.microsoft.com/fwlink/?linkid=21140)
</td>
<td style="border:1px solid black;">
[**Mérsékelt.**](http://go.microsoft.com/fwlink/?linkid=21140)
</td>
<td style="border:1px solid black;">
[**Mérsékelt.**](http://go.microsoft.com/fwlink/?linkid=21140)
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
Windows Server 2008 R2 x64-alapú rendszerekhez
</td>
<td style="border:1px solid black;">
[Internet Explorer 8](http://www.microsoft.com/downloads/details.aspx?familyid=d8b563ce-5db1-4490-8a63-44833d55152b)\*\*  
(Fontos)
</td>
<td style="border:1px solid black;">
Nem érintett
</td>
<td style="border:1px solid black;">
[Windows Server 2008 R2 x64 alapú rendszerekhez](http://www.microsoft.com/downloads/details.aspx?familyid=b060c516-233a-4e1e-9237-698420e97b2f)\*\*  
(Kritikus)
</td>
<td style="border:1px solid black;">
[Microsoft .NET-keretrendszer 4.0](http://www.microsoft.com/downloads/details.aspx?familyid=bbc22169-996f-48d1-beed-0ee0dc4fbf4f)<sup>[1]</sup>
(Fontos)
</td>
<td style="border:1px solid black;">
[Windows Server 2008 R2 x64 alapú rendszerekhez](http://www.microsoft.com/downloads/details.aspx?familyid=98e0c6ac-c30b-4d39-8ed9-1fe69e7644e5)\*  
(Fontos)
</td>
<td style="border:1px solid black;">
Nem érintett
</td>
<td style="border:1px solid black;">
[Windows Server 2008 R2 x64 alapú rendszerekhez](http://www.microsoft.com/downloads/details.aspx?familyid=25fff010-3abc-45e6-979e-21d2bae49418)\*\*  
(Fontos)
</td>
<td style="border:1px solid black;">
[Windows Media Player 12](http://www.microsoft.com/downloads/details.aspx?familyid=4cf0e3b1-4b72-4f99-b716-2489ea42ed72)\*\*  
(Mérsékelt)
</td>
<td style="border:1px solid black;">
[Windows Server 2008 R2 x64 alapú rendszerekhez](http://www.microsoft.com/downloads/details.aspx?familyid=70622d35-4877-4cbb-bdbf-7648dc1ea8ed)\*\*<sup>[1]</sup>
(KB979687)  
(Fontos)  
[Windows Server 2008 R2 x64 alapú rendszerekhez](http://www.microsoft.com/downloads/details.aspx?familyid=1c2ff242-65e3-4d47-bfca-4db30f809ed8)\*\*<sup>[1]</sup>
(KB979688)  
(Fontos)
</td>
<td style="border:1px solid black;">
Nem érintett
</td>
<td style="border:1px solid black;">
[Windows Server 2008 R2 x64 alapú rendszerekhez](http://www.microsoft.com/downloads/details.aspx?familyid=d356af2f-eadf-4bf2-82d1-efa0d01ac92d)\*  
(Fontos)
</td>
<td style="border:1px solid black;">
[Windows Server 2008 R2 x64 alapú rendszerekhez](http://www.microsoft.com/downloads/details.aspx?familyid=e4d27aa6-9739-4e41-9536-5f0b8d26503c)\*\*  
(Mérsékelt)
</td>
<td style="border:1px solid black;">
[Windows Server 2008 R2 x64 alapú rendszerekhez](http://www.microsoft.com/downloads/details.aspx?familyid=1de12fdf-b439-4020-9313-a193d47dcfb2)\*  
(Mérsékelt)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Windows Server 2008 R2 x64-alapú rendszerekhez, Service Pack 1
</td>
<td style="border:1px solid black;">
Nem érintett
</td>
<td style="border:1px solid black;">
Nem érintett
</td>
<td style="border:1px solid black;">
Nem érintett
</td>
<td style="border:1px solid black;">
[Microsoft .NET-keretrendszer 4.0](http://www.microsoft.com/downloads/details.aspx?familyid=bbc22169-996f-48d1-beed-0ee0dc4fbf4f)\*\*<sup>[1]</sup>
(Fontos)
</td>
<td style="border:1px solid black;">
Nem érintett
</td>
<td style="border:1px solid black;">
Nem érintett
</td>
<td style="border:1px solid black;">
Nem érintett
</td>
<td style="border:1px solid black;">
Nem érintett
</td>
<td style="border:1px solid black;">
Nem érintett
</td>
<td style="border:1px solid black;">
Nem érintett
</td>
<td style="border:1px solid black;">
Nem érintett
</td>
<td style="border:1px solid black;">
Nem érintett
</td>
<td style="border:1px solid black;">
Nem érintett
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
Windows Server 2008 R2 Itanium-alapú rendszerekhez
</td>
<td style="border:1px solid black;">
[Internet Explorer 8](http://www.microsoft.com/downloads/details.aspx?familyid=bbaa9f46-8fc7-4c44-b38c-dc3d5210f63d)  
(Fontos)
</td>
<td style="border:1px solid black;">
Nem érintett
</td>
<td style="border:1px solid black;">
[Windows Server 2008 R2 Itanium-alapú rendszerekhez](http://www.microsoft.com/downloads/details.aspx?familyid=0ead2ed9-8b2f-496e-b7d1-3ad2b04be5cc)  
(Kritikus)
</td>
<td style="border:1px solid black;">
[Microsoft .NET-keretrendszer 4.0](http://www.microsoft.com/downloads/details.aspx?familyid=bbc22169-996f-48d1-beed-0ee0dc4fbf4f)<sup>[1]</sup>
(Fontos)
</td>
<td style="border:1px solid black;">
[Windows Server 2008 R2 Itanium-alapú rendszerekhez](http://www.microsoft.com/downloads/details.aspx?familyid=44080c75-036e-4bd0-914a-74ab72189ee3)  
(Fontos)
</td>
<td style="border:1px solid black;">
Nem érintett
</td>
<td style="border:1px solid black;">
[Windows Server 2008 R2 Itanium-alapú rendszerekhez](http://www.microsoft.com/downloads/details.aspx?familyid=d0742526-b5ec-4658-82f1-c3680f33a790)  
(Fontos)
</td>
<td style="border:1px solid black;">
Nem érintett
</td>
<td style="border:1px solid black;">
[Windows Server 2008 R2 Itanium-alapú rendszerekhez](http://www.microsoft.com/downloads/details.aspx?familyid=3cec2b70-f694-4c0d-bf82-96a4fd50675d)<sup>[1]</sup>
(KB979687)  
(Fontos)  
[Windows Server 2008 R2 Itanium-alapú rendszerekhez](http://www.microsoft.com/downloads/details.aspx?familyid=f478020b-0305-47d5-bcb2-0758f292db29)<sup>[1]</sup>
(KB979688)  
(Fontos)
</td>
<td style="border:1px solid black;">
Nem érintett
</td>
<td style="border:1px solid black;">
[Windows Server 2008 R2 Itanium-alapú rendszerekhez](http://www.microsoft.com/downloads/details.aspx?familyid=334d39e6-8e4c-4e83-94c1-1db3d636e865)  
(Fontos)
</td>
<td style="border:1px solid black;">
[Windows Server 2008 R2 Itanium-alapú rendszerekhez](http://www.microsoft.com/downloads/details.aspx?familyid=c1634278-5598-45e0-81c6-f18fb5ba54cf)  
(Mérsékelt)
</td>
<td style="border:1px solid black;">
[Windows Server 2008 R2 Itanium-alapú rendszerekhez](http://www.microsoft.com/downloads/details.aspx?familyid=1c607c7d-6144-4a39-beea-a31b62085047)  
(Mérsékelt)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Windows Server 2008 R2 Itanium alapú rendszerekhez, Service Pack 1
</td>
<td style="border:1px solid black;">
Nem érintett
</td>
<td style="border:1px solid black;">
Nem érintett
</td>
<td style="border:1px solid black;">
Nem érintett
</td>
<td style="border:1px solid black;">
[Microsoft .NET-keretrendszer 4.0](http://www.microsoft.com/downloads/details.aspx?familyid=bbc22169-996f-48d1-beed-0ee0dc4fbf4f)<sup>[1]</sup>
(Fontos)
</td>
<td style="border:1px solid black;">
Nem érintett
</td>
<td style="border:1px solid black;">
Nem érintett
</td>
<td style="border:1px solid black;">
Nem érintett
</td>
<td style="border:1px solid black;">
Nem érintett
</td>
<td style="border:1px solid black;">
Nem érintett
</td>
<td style="border:1px solid black;">
Nem érintett
</td>
<td style="border:1px solid black;">
Nem érintett
</td>
<td style="border:1px solid black;">
Nem érintett
</td>
<td style="border:1px solid black;">
Nem érintett
</td>
</tr>
</table>
 
**Megjegyzés az MS10-077 közleményhez**

<sup>[1]</sup>**.érintett .NET-keretrendszer 4.0 és .NET-keretrendszer 4.0 Client Profile.** A .NET-keretrendszer 4-es verziójú terjeszthető csomagjai két profilban érhetőek el: a .NET-keretrendszer 4.0 és a .NET-keretrendszer 4.0 verziójához tartozó ügyfélprofil. a .NET-keretrendszer 4.0 verziójához tartozó ügyfélprofil része a .NET-keretrendszer 4.0 verziójának. A jelen frissítés érinti mindkét, a .NET-keretrendszer 4.0 verziójához tartozó ügyfélprofilt és .NET-keretrendszer 4.0 verzióját. További információk A .NET keretrendszer telepítése c. MSDN cikkben.

**Megjegyzés az MS10-083 közleményhez**

<sup>[1]</sup>Ahol mindkét, KB979687 és KB979688 biztonsági frissítés elérhető az operációs rendszerre, az ügyfeleknek mindkét frissítést telepíteniük kell az MS10-083 közleményben ismertetett biztonsági rések elleni védelem érdekében.

**Megjegyzések a Windows Server 2008 és Windows Server 2008 R2 rendszerhez**

**\*Érinti** **a kiszolgálómag telepítését.** Ez a frissítés ugyanolyan biztonsági besorolás mellett, a megadottak szerint érvényes az Windows Server 2008 és a Windows Server 2008 R2 összes támogatott kiadására, függetlenül attól, hogy a kiszolgálómag-telepítési opcióval telepítették-e. Erről a telepítési opcióról bővebben a [Kiszolgálómag-telepítés kezelése](http://technet.microsoft.com/en-us/library/ee441255(ws.10).aspx) és [Kiszolgálómag-telepítés szervizelése](http://technet.microsoft.com/en-us/library/ff698994(ws.10).aspx) TechNet cikkekben olvashat. A kiszolgálómag-telepítési opció nem vonatkozik a Windows Server 2008 és a Windows Server 2008 R2 bizonyos kiadásaira; lásd: [A kiszolgálómag-telepítési opciók összehasonlítása](http://www.microsoft.com/windowsserver2008/en/us/compare-core-installation.aspx).

**\*\*A kiszolgálómag-telepítés nem érintett.** A frissítésben tárgyalt biztonsági rések nem érintik a jelzett módon a Windows Server 2008 támogatott kiadásait, amennyiben a telepítés a kiszolgálómag-telepítési opció használatával történt. Erről a telepítési opcióról bővebben a [Kiszolgálómag-telepítés kezelése](http://technet.microsoft.com/en-us/library/ee441255(ws.10).aspx) és [Kiszolgálómag-telepítés szervizelése](http://technet.microsoft.com/en-us/library/ff698994(ws.10).aspx) TechNet cikkekben olvashat. A kiszolgálómag-telepítési opció nem vonatkozik a Windows Server 2008 és a Windows Server 2008 R2 bizonyos kiadásaira; lásd: [A kiszolgálómag-telepítési opciók összehasonlítása](http://www.microsoft.com/windowsserver2008/en/us/compare-core-installation.aspx).

#### Microsoft Office programcsomagok és szoftverek

 
<p> </p>
<table style="border:1px solid black;">
<tr class="thead">
<th style="border:1px solid black;" >
</th>
<th style="border:1px solid black;" >
</th>
<th style="border:1px solid black;" >
</th>
</tr>
<tr>
<th colspan="3">
Microsoft Office programcsomagok és összetevők
</th>
</tr>
<tr>
<td style="border:1px solid black;">
**Közlemény azonosítója**
</td>
<td style="border:1px solid black;">
[**MS10-079**](http://go.microsoft.com/fwlink/?linkid=201696)
</td>
<td style="border:1px solid black;">
[**MS10-080**](http://go.microsoft.com/fwlink/?linkid=200529)
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
**Összesített súlyossági besorolás**
</td>
<td style="border:1px solid black;">
[**Fontos**](http://go.microsoft.com/fwlink/?linkid=21140)
</td>
<td style="border:1px solid black;">
[**Fontos**](http://go.microsoft.com/fwlink/?linkid=21140)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Microsoft Office XP Service Pack 3
</td>
<td style="border:1px solid black;">
[Microsoft Word 2002 Service Pack 3](http://www.microsoft.com/downloads/details.aspx?familyid=f22d10fd-cb12-43e8-88d5-2116cf4317c4)  
(KB2328360)  
(Fontos)
</td>
<td style="border:1px solid black;">
[Microsoft Excel 2002 Service Pack 3](http://www.microsoft.com/downloads/details.aspx?familyid=ea859881-2cc5-407b-a394-5d00c5d9fd97)  
(KB2345017)  
(Fontos)
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
Microsoft Office 2003 Service Pack 3
</td>
<td style="border:1px solid black;">
[Microsoft Word 2003 Service Pack 3](http://www.microsoft.com/downloads/details.aspx?familyid=172f3743-cdfa-42d7-aeb4-27ba0e4139f7)  
(KB2344911)  
(Fontos)
</td>
<td style="border:1px solid black;">
[Microsoft Excel 2003 Service Pack 3](http://www.microsoft.com/downloads/details.aspx?familyid=3d9a00b8-0f80-4d36-b92a-89b61350fb36)  
(KB2344893)  
(Fontos)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Microsoft Office 2007 Service Pack 2
</td>
<td style="border:1px solid black;">
[Microsoft Word 2007 Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=ccad4871-32f2-4982-a23e-9b5824397615)<sup>[1]</sup>
(KB2344993)  
(Fontos)
</td>
<td style="border:1px solid black;">
[Microsoft Excel 2007 Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=dc9b9af5-50b0-4a07-8923-a30fd5548760)<sup>[1]</sup>
(KB2345035)  
(Fontos)
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
Microsoft Office 2010 (32 bites kiadások)
</td>
<td style="border:1px solid black;">
[Microsoft Word 2010 (32 bites kiadások)](http://www.microsoft.com/downloads/details.aspx?familyid=6c3b8690-e568-42ed-a858-0cbdd5ea3669)  
(KB2345000)  
(Fontos)
</td>
<td style="border:1px solid black;">
Nem érintett
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Microsoft Office 2010 (64 bites kiadások)
</td>
<td style="border:1px solid black;">
[Microsoft Word 2010 (64 bites kiadások)](http://www.microsoft.com/downloads/details.aspx?familyid=f31a1f9b-02df-4a85-a7d1-7d1e31baa30f)  
(KB2345000)  
(Fontos)
</td>
<td style="border:1px solid black;">
Nem érintett
</td>
</tr>
<tr>
<th colspan="3">
Microsoft Office for Mac
</th>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
**Közlemény azonosítója**
</td>
<td style="border:1px solid black;">
[**MS10-079**](http://go.microsoft.com/fwlink/?linkid=201696)
</td>
<td style="border:1px solid black;">
[**MS10-080**](http://go.microsoft.com/fwlink/?linkid=200529)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
**Összesített súlyossági besorolás**
</td>
<td style="border:1px solid black;">
[**Fontos**](http://go.microsoft.com/fwlink/?linkid=21140)
</td>
<td style="border:1px solid black;">
[**Fontos**](http://go.microsoft.com/fwlink/?linkid=21140)
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
Microsoft Office 2004 for Mac
</td>
<td style="border:1px solid black;">
[Microsoft Office 2004 for Mac](http://www.microsoft.com/downloads/details.aspx?familyid=464965fa-971a-49dd-bcee-c4d91fac86a9)  
(KB2422343)  
(Fontos)
</td>
<td style="border:1px solid black;">
[Microsoft Office 2004 for Mac](http://www.microsoft.com/downloads/details.aspx?familyid=464965fa-971a-49dd-bcee-c4d91fac86a9)  
(KB2422343)  
(Fontos)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Microsoft Office 2008 for Mac
</td>
<td style="border:1px solid black;">
[Microsoft Office 2008 for Mac](http://www.microsoft.com/downloads/details.aspx?familyid=abd05074-8ffc-41a4-a2f3-1d8047574552)  
(KB2422352)  
(Fontos)
</td>
<td style="border:1px solid black;">
[Microsoft Office 2008 for Mac](http://www.microsoft.com/downloads/details.aspx?familyid=abd05074-8ffc-41a4-a2f3-1d8047574552)  
(KB2422352)  
(Fontos)
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
Open XML File Format Converter for Mac
</td>
<td style="border:1px solid black;">
[Open XML File Format Converter for Mac](http://www.microsoft.com/downloads/details.aspx?familyid=5c759c46-ead3-44ea-b7c8-a308b3140d2e)  
(KB2422398)  
(Fontos)
</td>
<td style="border:1px solid black;">
[Open XML File Format Converter for Mac](http://www.microsoft.com/downloads/details.aspx?familyid=5c759c46-ead3-44ea-b7c8-a308b3140d2e)  
(KB2422398)  
(Fontos)
</td>
</tr>
<tr>
<th colspan="3">
További Office-szoftverek
</th>
</tr>
<tr>
<td style="border:1px solid black;">
**Közlemény azonosítója**
</td>
<td style="border:1px solid black;">
[**MS10-079**](http://go.microsoft.com/fwlink/?linkid=201696)
</td>
<td style="border:1px solid black;">
[**MS10-080**](http://go.microsoft.com/fwlink/?linkid=200529)
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
**Összesített súlyossági besorolás**
</td>
<td style="border:1px solid black;">
[**Fontos**](http://go.microsoft.com/fwlink/?linkid=21140)
</td>
<td style="border:1px solid black;">
[**Fontos**](http://go.microsoft.com/fwlink/?linkid=21140)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Microsoft Word megjelenítő
</td>
<td style="border:1px solid black;">
[Microsoft Word megjelenítő](http://www.microsoft.com/downloads/details.aspx?familyid=1cb5ab02-074d-4877-b378-7058959705ae)  
(KB2345009)  
(Fontos)
</td>
<td style="border:1px solid black;">
Nem érintett
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
Microsoft Excel Megtekintő
</td>
<td style="border:1px solid black;">
Nem érintett
</td>
<td style="border:1px solid black;">
[Microsoft Excel megjelenítő Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=a833a94a-2dc0-4864-9c14-e196dc54c5a7)  
(KB2345088)  
(Fontos)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Microsoft Office kompatibilitási csomag a Word, Excel és a PowerPoint 2007 fájlformátumokhoz Service Pack 2
</td>
<td style="border:1px solid black;">
[Microsoft Office kompatibilitási csomag a Word, Excel és a PowerPoint 2007 fájlformátumokhoz Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=553d28ae-c352-4985-97c3-e5038414be45)  
(KB2345043)  
(Fontos)
</td>
<td style="border:1px solid black;">
[Microsoft Office kompatibilitási csomag a Word, Excel és a PowerPoint 2007 fájlformátumokhoz Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=7391ec2f-12c9-483c-91d8-e3ec5754da1c)  
(KB2344875)  
(Fontos)
</td>
</tr>
</table>
 
**Megjegyzések az MS10-079 közleményhez**

<sup>[1]</sup> A Microsoft Word 2007 Service Pack 2 felhasználóknak a KB2344993 frissítésen kívül a Microsoft Office kompatibilitási csomag a Word, Excel és PowerPoint 2007 fájlformátumhoz Service Pack 2 (KB2345043) biztonsági frissítését is telepíteniük kell, hogy megvédjék rendszerüket az MS10-079 közleményben ismertetett biztonsági résektől.

Az ugyanezen a közleményazonosító alatt található, további frissített fájlokat illetően lásd még az egyéb szoftverkategóriák részt ebben a fejezetben, **Érintett szoftverek és letöltési helyek**. Ez a közlemény több szoftverkategóriát ölel fel.

**Megjegyzés az MS10-080 közleményhez**

<sup>[1]</sup> A Microsoft Office Excel 2007 Service Pack 2 felhasználóknak a KB2345035 frissítésen kívül a Microsoft Office kompatibilitási csomag a Word, Excel és PowerPoint 2007 fájlformátumhoz Service Pack 2 (KB2344875) biztonsági frissítését is telepíteniük kell, hogy megvédjék rendszerüket az MS10-080 közleményben ismertetett biztonsági résektől.

#### Microsoft Server Software

 
<p> </p>
<table style="border:1px solid black;">
<tr class="thead">
<th style="border:1px solid black;" >
</th>
<th style="border:1px solid black;" >
</th>
<th style="border:1px solid black;" >
</th>
</tr>
<tr>
<th colspan="3">
Microsoft SharePoint Services és Microsoft SharePoint Foundation
</th>
</tr>
<tr>
<td style="border:1px solid black;">
**Közlemény azonosítója**
</td>
<td style="border:1px solid black;">
[**MS10-072**](http://go.microsoft.com/fwlink/?linkid=202016)
</td>
<td style="border:1px solid black;">
[**MS10-079**](http://go.microsoft.com/fwlink/?linkid=201696)
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
**Összesített súlyossági besorolás**
</td>
<td style="border:1px solid black;">
[**Fontos**](http://go.microsoft.com/fwlink/?linkid=21140)
</td>
<td style="border:1px solid black;">
Nincsenek
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Microsoft Windows SharePoint Services 3.0
</td>
<td style="border:1px solid black;">
[Microsoft Windows SharePoint Services 3.0 Service Pack 2 (32 bites verziók)](http://www.microsoft.com/downloads/details.aspx?familyid=12fd97a9-6fb8-4b65-a497-a56587f114e1)  
(KB2345304)  
(Fontos)  
[Microsoft Windows SharePoint Services 3.0 Service Pack 2 (64 bites verziók)](http://www.microsoft.com/downloads/details.aspx?familyid=58d1e91d-a037-485d-a6d9-80fbf403b108)  
(KB2345304)  
(Fontos)
</td>
<td style="border:1px solid black;">
Nem érintett
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
Microsoft SharePoint Foundation 2010
</td>
<td style="border:1px solid black;">
[Microsoft SharePoint Foundation 2010](http://www.microsoft.com/downloads/details.aspx?familyid=fc146fcb-c2cb-4860-a0cd-4b09fa3f44eb)  
(KB2345322)  
(Fontos)
</td>
<td style="border:1px solid black;">
Nem érintett
</td>
</tr>
<tr>
<th colspan="3">
Microsoft SharePoint és Microsoft Groove Server
</th>
</tr>
<tr>
<td style="border:1px solid black;">
**Közlemény azonosítója**
</td>
<td style="border:1px solid black;">
[**MS10-072**](http://go.microsoft.com/fwlink/?linkid=202016)
</td>
<td style="border:1px solid black;">
[**MS10-079**](http://go.microsoft.com/fwlink/?linkid=201696)
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
**Összesített súlyossági besorolás**
</td>
<td style="border:1px solid black;">
[**Fontos**](http://go.microsoft.com/fwlink/?linkid=21140)
</td>
<td style="border:1px solid black;">
Nincsenek
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Microsoft Office SharePoint Server 2007
</td>
<td style="border:1px solid black;">
[Microsoft Office SharePoint Server 2007 Service Pack 2 (32 bites kiadások)](http://www.microsoft.com/downloads/details.aspx?familyid=aee3f2de-ccf3-4d32-b468-eede4e8afcd4)<sup>[1]</sup>
(KB2345212)  
(Fontos)  
[Microsoft Office SharePoint Server 2007 Service Pack 2 (64 bites kiadások)](http://www.microsoft.com/downloads/details.aspx?familyid=e5e60751-242a-4fdb-9852-6d94050d3d0e)<sup>[1]</sup>
(KB2345212)  
(Fontos)
</td>
<td style="border:1px solid black;">
Nem érintett
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
Microsoft Groove Server 2010
</td>
<td style="border:1px solid black;">
[Microsoft Groove Server 2010](http://www.microsoft.com/downloads/details.aspx?familyid=e032aef8-dd30-41c6-99bb-8cf0491451cc)  
(KB2346298)  
(Fontos)
</td>
<td style="border:1px solid black;">
Nem érintett
</td>
</tr>
<tr>
<th colspan="3">
Microsoft Office Web Apps
</th>
</tr>
<tr>
<td style="border:1px solid black;">
**Közlemény azonosítója**
</td>
<td style="border:1px solid black;">
[**MS10-072**](http://go.microsoft.com/fwlink/?linkid=202016)
</td>
<td style="border:1px solid black;">
[**MS10-079**](http://go.microsoft.com/fwlink/?linkid=201696)
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
**Összesített súlyossági besorolás**
</td>
<td style="border:1px solid black;">
[**Fontos**](http://go.microsoft.com/fwlink/?linkid=21140)
</td>
<td style="border:1px solid black;">
[**Fontos**](http://go.microsoft.com/fwlink/?linkid=21140)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Microsoft Office Web Apps
</td>
<td style="border:1px solid black;">
[Microsoft Office Web Apps](http://www.microsoft.com/downloads/details.aspx?familyid=8fb56eb9-9601-4c1e-905a-9fe4802b2c8d)  
(KB2346411)  
(Fontos)
</td>
<td style="border:1px solid black;">
[Microsoft Office Web Apps](http://www.microsoft.com/downloads/details.aspx?familyid=8fb56eb9-9601-4c1e-905a-9fe4802b2c8d)<sup>[2]</sup>
(KB2346411)  
(Fontos)  
[Microsoft Word Web App](http://www.microsoft.com/downloads/details.aspx?familyid=13b24264-ec3d-44e8-81e3-82ac767defd3)<sup>[2]</sup>
(KB2345015)  
(Fontos)
</td>
</tr>
</table>
 
**Megjegyzés az MS10-072 közleményhez**

<sup>[1]</sup>A Microsoft SharePoint Server 2007 támogatott kiadásai esetén a KB2345212 biztonsági frissítőcsomag mellett a Microsoft Windows SharePoint Services 3.0 (KB2345304) szolgáltatást is telepíteniük kell a felhasználóknak annak érdekében, hogy megvédjék rendszerüket az MS10-072 közleményben foglalt biztonsági résektől.

**Megjegyzések az MS10-079 közleményhez**

<sup>[2]</sup>A Microsoft Office Web Apps felhasználóknak telepíteni kell a KB2346411 és a KB2345015 biztonsági frissítést: csak ez biztosít védelmet az MS10-079 közleményben foglalt biztonsági rések ellen.

Az ugyanezen a közleményazonosító alatt található, további frissített fájlokat illetően lásd még az egyéb szoftverkategóriák részt ebben a fejezetben, **Érintett szoftverek és letöltési helyek**. Ez a közlemény több szoftverkategóriát ölel fel.

Észlelési és telepítési eszközök, útmutatás
-------------------------------------------

<span></span>
**Biztonsági központ**

A szoftveres és biztonsági frissítések kezeléséhez azokat a szervezet asztali és hordozható számítógépeire, valamint kiszolgálóira is telepíteni kell. További tájékoztatásért látogasson el a [TechNet Update Management Center](http://go.microsoft.com/fwlink/?linkid=69903) weboldalára. A [TechNet Security Center](http://go.microsoft.com/fwlink/?linkid=21171) bővebb tájékoztatással szolgál a Microsoft termékek biztonsági funkcióival kapcsolatban. A [Biztonság otthon](http://go.microsoft.com/fwlink/?linkid=85102) weboldalon a megfelelő hivatkozásra kattintva elérhetőek a legújabb biztonsági frissítések.

A biztonsági frissítések a [Microsoft Update](http://go.microsoft.com/fwlink/?linkid=40747) és a [Windows Update](http://go.microsoft.com/fwlink/?linkid=21130) weboldalról tölthetők le. A biztonsági frissítések a [Microsoft letöltő központjában](http://go.microsoft.com/fwlink/?linkid=21129) is elérhetőek. Legegyszerűbben a „security update” kifejezésre irányuló kulcsszavas kereséssel találhatja meg ezeket.

A biztonsági frissítések a [Microsoft Update katalógusából](http://go.microsoft.com/fwlink/?linkid=96155) is letölthetőek. A Microsoft Update katalógus a Windows Update és Microsoft Update szolgáltatáson keresztül elérhető tartalom kereshető adatbázisa; ide tartoznak a biztonsági frissítések, illesztőprogramok és szervizcsomagok. A biztonsági közlemény azonosítójára (pl. „MS07-036”) történő kereséssel hozzáadhatja az összes vonatkozó frissítést a kosárhoz (beleértve a frissítés különböző nyelvi változatait), és letöltheti azokat a megadott mappába. A Microsoft Update katalógus részletes leírását lásd a vonatkozó [GYIK](http://go.microsoft.com/fwlink/?linkid=97900)részben.

**Útmutató az észleléshez és a telepítéshez**

A biztonsági frissítésekkel kapcsolatban a Microsoft észlelési és telepítési segítséget nyújt. Ez az útmutató olyan javaslatokat és tudnivalókat tartalmaz, amelyeket segítséget nyújthatnak az informatikusoknak a biztonsági frissítések észlelési és telepítési eszközeinek használatához. További tudnivalókat a [Microsoft Tudásbázis 961747. számú cikkében](http://support.microsoft.com/kb/961747) talál.

**Microsoft Baseline Security Analyzer**

A Microsoft Baseline Security Analyzer (MBSA) segítségével a rendszergazda mind a helyi, mind a távoli számítógépeken ellenőrizheti, hogy mely biztonsági frissítések hiányoznak, illetve hogy mely biztonsági beállítások vannak helytelenül megadva. Ha többet szeretne tudni az MBSA eszközről, látogasson el a [Microsoft Baseline Security Analyzer](http://go.microsoft.com/fwlink/?linkid=21134) webhelyre.

**Windows Server Update Services**

A Microsoft Server Update Services (WSUS) szolgáltatással a rendszergazdák gyorsan és megbízhatóan telepíthetik a legújabb fontos és biztonsági frissítéseket Microsoft Windows 2000 és újabb operációs rendszerekhez, Office XP és újabb operációs rendszerekhez, Exchange Server 2003 és SQL Server 2000 Microsoft Windows 2000 és újabb operációs rendszerekre.

A biztonsági frissítésnek Windows Server Update Services szolgáltatással történő központi telepítéséről a [Windows Server Update Services](http://go.microsoft.com/fwlink/?linkid=50120) webhelyen tudhat meg többet.

**Systems Management Server**

A Microsoft Systems Management Server (SMS) rendszer egy sokoldalúan beállítható vállalati megoldás, amely a frissítések kezelésére szolgál. Az SMS segítségével a rendszergazda megállapíthatja, hogy melyik Windows alapú számítógép szorul biztonsági frissítésre, és ezeket a frissítéseket szabályozott módon, a felhasználók minimális zavarásával központilag telepítheti a vállalat teljes informatikai környezetében. Az SMS, vagyis a System Center Configuration Manager 2007 újabb kiadása immár elérhető, lásd még: [System Center Configuration Manager 2007](http://technet.microsoft.com/en-us/library/bb735860.aspx). Arról, hogy a rendszergazdák hogyan használhatják a biztonsági frissítések telepítéséhez az SMS 2003 alkalmazást, az [SMS 2003 Security Patch Management](http://go.microsoft.com/fwlink/?linkid=22939) részben olvashat. A biztonsági frissítések felderítéséhez az SMS 2.0 felhasználók a Security Update Inventory Tool (SUIT) eszközt is használhatják. Az SMS-szolgáltatásról bővebben a [Microsoft Systems Management Server](http://go.microsoft.com/fwlink/?linkid=21158) oldalán olvashat.

**Megjegyzés** Az SMS a Microsoft Baseline Security Analyzer eszközön keresztül széles körű támogatást nyújt a biztonsági közlemények frissítéseinek észleléséhez, valamint a frissítések telepítéséhez. Előfordulhat, hogy egyes szoftverfrissítéseket ezek az eszközök nem észlelnek. Az SMS-alkalmazás leltározási szolgáltatásai segítségével a rendszergazdák adott rendszereken hajthatják végre a frissítést. Az eljárással kapcsolatban olvassa el a [Szoftverfrissítések telepítése az SMS szoftverelosztó ügynök segítségével](http://go.microsoft.com/fwlink/?linkid=33341) című tájékoztatót. Egyes biztonsági frissítésekhez rendszergazdai jogosultságokra van szükség a számítógép újraindítása után. A rendszergazdák az Elevated Rights Deployment Tool eszközt (az [SMS 2.0 Administration Feature Pack](http://go.microsoft.com/fwlink/?linkid=21161) része) alkalmazhatják a frissítések telepítéséhez.

**Az Update Compatibility Evaluator (a frissítéskompatibilitás kiértékelője) és az Application Compatibility Toolkit (alkalmazáskompatibilitási eszközkészlet)**

Az alkalmazások működése érdekében a frissítések gyakran írnak ugyanazokba a fájlokba, illetve regisztrációs bejegyzésekbe. Ez inkompatibilitást okozhat, és növelheti a biztonsági frissítések központi telepítésére használt időt. A Windows frissítések és az alkalmazásoknak való megfelelőség tesztelése és ellenőrzése egyszerűsíthető az [Update Compatibility Evaluator](http://technet2.microsoft.com/windowsvista/en/library/4279e239-37a4-44aa-aec5-4e70fe39f9de1033.mspx?mfr=true) összetevőivel, amelyek az [Application Compatibility Toolkit](http://www.microsoft.com/downloads/details.aspx?familyid=24da89e9-b581-47b0-b45e-492dd6da2971&displaylang=hu) alkalmazáskompatibilitási eszközkészletben megtalálhatók.

Az Application Compatibility Toolkit (ACT) tartalmazza a Microsoft Windows Vista, a Windows Update, a Microsoft Security Update vagy a Windows Internet Explorer új verziójának központi telepítése előtt az alkalmazáskompatibilitási problémák kiértékeléséhez és enyhítéséhez szükséges eszközöket és dokumentációt.

### Egyéb információ

#### A Microsoft Windows rosszindulatú szoftvereket eltávolító eszköze

A Microsoft a Windows Update, Microsoft Update, Windows Server Update Services és Letöltőközpont szolgáltatásán keresztül elérhetővé tette a Microsoft Windows rosszindulatú szoftvereket eltávolító eszközének frissített változatát.

#### Nem biztonsági jellegű, kiemelt fontosságú frissítések a MU, WU és WSUS-szolgáltatásokban

A Windows Update és a Microsoft Update helyen elérhető, nem biztonsági jellegű frissítésekről tájékozódjon itt:

-   [Microsoft Tudásbázis 894199. cikke](http://support.microsoft.com/kb/894199): Tartalommódosítás a Software Update Services és Windows Server Update Services rendszerek leírásában. Az összes Windows-tartalmat érinti.
-   [Az elmúlt hónapok frissítései Windows Server Frissítési szolgáltatások esetén](http://technet.microsoft.com/en-us/wsus/bb456965.aspx). Microsoft termékek új, módosított és újra kiadott frissítései, a Microsoft Windows rendszert kivéve.

#### Microsoft Active Protections Program (MAPP)

Az ügyfelek védelmének növelése érdekében a biztonsági szoftverekkel foglalkozó nagyobb gyártók a Microsoft a havi biztonsági közlemények megjelenése előtt ellátja biztonsági résekkel kapcsolatos információkkal. Így a biztonságiszoftver-gyártók a kapott biztonsági résekkel kapcsolatos információt felhasználhatják ügyfeleik hatásosabb védelmére az olyan biztonsági szoftverek vagy eszközök (például víruskeresők, hálózati behatolásérzékelő rendszerek vagy kiszolgálóalapú behatolásvédelmi rendszerek) frissítése által. A biztonságiszoftver-gyártók által kiadott aktív védelem elérhetőségéről a [Microsoft Active Protections Program (MAPP) Partners](http://www.microsoft.com/security/msrc/mapp/partners.mspx) webhelyén található listán szereplő és a programban részt vevő gyártók aktív védelmi webhelyein tájékozódhat.

#### Biztonsági stratégiák és közösségek

**Frissítésekkel kapcsolatos stratégiák**

[A frissítések kezelésére vonatkozó útmutatás](http://go.microsoft.com/fwlink/?linkid=21168) a Microsoft által a biztonsági frissítések telepítéséhez ajánlott legjobban bevált eljárást ismerteti.

**Egyéb biztonsági frissítések beszerzése**

Az alábbi helyekről más típusú biztonsági problémákhoz szerezhetők be frissítések:

-   A biztonsági frissítések a [Microsoft letöltő központjában](http://go.microsoft.com/fwlink/?linkid=21129) érhetők el. Legegyszerűbben a „security update” kifejezésre irányuló kulcsszavas kereséssel találhatja meg ezeket.
-   Az ügyfélrendszerek frissítései a [Microsoft Update](http://go.microsoft.com/fwlink/?linkid=40747) oldalról elérhetőek.
-   A Windows Update szolgáltatáson keresztül terjesztett havi aktuális biztonsági frissítések a letöltőközpontból a biztonsági és kritikus frissítéseket tartalmazó ISO CD-képfájlként is letölthetőek. További információt a [Microsoft Tudásbázis 913086. számú cikkében](http://support.microsoft.com/kb/913086) talál.

**IT Pro Security közösség**

Az [IT Pro Security Community](http://go.microsoft.com/fwlink/?linkid=21164) közösségben hasznos információt találhat a biztonság javításáról és az informatikai infrastruktúrák optimalizálásáról, továbbá eszmecserét folytathat a biztonsági kérdésekről más informatikai szakemberekkel.

#### Köszönetnyilvánítás

A Microsoft [köszönetét](http://go.microsoft.com/fwlink/?linkid=21127) fejezi ki a vásárlók védelmének biztosításában nyújtott segítségért az alábbi szervezet(ek)nek és szakember(ek)nek:

-   [Sirdarckcat](http://www.sirdarckcat.net/), [Google Inc.](http://www.google.com/), az MS10-071 közleményben bemutatott probléma jelentéséért
-   Mario Heiderich az MS10-071 közleményben leírt probléma jelentéséért
-   Takehiro Takahashi, [IBM ISS X-Force](http://www.iss.net/), az MS10-071 közleményben ismertetett egyik probléma jelentéséért
-   [Peter Vreugdenhil](http://vreugdenhilresearch.nl), a [TippingPoint](http://www.tippingpoint.com/)[Zero Day Initiative](http://www.zerodayinitiative.com/) programjával együttműködésben, az MS10-071 közleményben ismertetett probléma jelentéséért
-   Damián Frizza, [Core Security Technologies](http://www.coresecurity.com/), az MS10-071 közleményben leírt probléma jelentéséért
-   Aldwin Saugere és Radoslav Vasilev, [Cigital](http://www.cigital.com/), az MS10-071 közleményben leírt probléma jelentéséért
-   Rodrigo Rubira Branco, [Check Point](http://www.checkpoint.com/) IPS Research Team, az MS10-071 közleményben ismertetett probléma jelentéséért
-   [Sirdarckcat](http://www.sirdarckcat.net/), [Google Inc.](http://www.google.com/), az MS10-072 közleményben bemutatott probléma jelentéséért
-   Mario Heiderich az MS10-072 közleményben leírt probléma jelentéséért
-   Sergey Golovanov, Alexander Gostev, Maxim Golovkin és Alexey Monastyrsky, a [Kaspersky Lab](http://www.kaspersky.com), valamint Vitaly Kiktenko és Alexander Saprykin, a [Design and Test Lab](http://www.dnt-lab.com) munkatársai az MS10-073 közleményben leírt probléma jelentéséért
-   Eric Chien, [Symantec](http://www.symantec.com/index.jsp), az MS10-073 közleményben leírt probléma jelentéséért
-   Tarjei Mandt, [Norman](http://www.norman.com), az MS10-073 közleményben ismertetett probléma közös megoldásában való részvételéért
-   Carsten H. Eiram, [Secunia](http://secunia.com/), az MS10-074 közleményben említett probléma megoldásában való együttműködésért
-   Oleksandr Mirosh, [TippingPoint](http://www.tippingpoint.com/)[Zero Day Initiative](http://www.zerodayinitiative.com/), az MS10-075 közleményben ismertetett probléma jelentéséért
-   Sebastian Apelt, a [TippingPoint](http://www.tippingpoint.com/)[Zero Day Initiative](http://www.zerodayinitiative.com/) programjával együttműködésben, az MS10-076 közleményben ismertetett probléma jelentéséért
-   Ivan Fratric, [iSIGHT Partners Global Vulnerability Partnership](https://gvp.isightpartners.com/), az MS10-076 közleményben ismertetett probléma jelentéséért
-   Jeroen Frijters, [Sumatra](http://www.sumatra.nl/), az MS10-077 közleményben ismertetett probléma jelentéséért
-   Sebastian Apelt, [Siberas](http://www.siberas.de/), az MS10-078 közleményben leírt probléma jelentéséért
-   Diego Juarez, [Core Security Technologies](http://www.coresecurity.com/), az MS10-078 közleményben leírt probléma jelentéséért
-   Chaouki Bekrar, [VUPEN Vulnerability Research Team](http://www.vupen.com/), az MS10-079 közleményben leírt tíz probléma jelentéséért
-   Nicolas Joly, [VUPEN Vulnerability Research Team](http://www.vupen.com/), az MS10-079 közleményben leírt probléma jelentéséért
-   Alin Rad Pop, [Secunia Research](http://secunia.com/), az MS10-079 közleményben leírt problémák egyikének jelentéséért
-   Alin Rad Pop, [Secunia](http://secunia.com/), az MS10-080 közleményben ismertetett két probléma jelentéséért
-   Chaouki Bekrar, [VUPEN Vulnerability Research Team](http://www.vupen.com/), az MS10-080 közleményben leírt tíz probléma jelentéséért
-   Omair az MS10-080 közleményben leírt probléma jelentéséért
-   Carsten H. Eiram, [Secunia](http://secunia.com/), az MS10-080 közleményben ismertetett két probléma jelentéséért
-   Krystian Kloskowski (h07), [Secunia](http://secunia.com/), az MS10-081 közleményben ismertetett egyik probléma jelentéséért
-   SkyLined, [Google Inc.](http://www.google.com/), az MS10-082 közleményben bemutatott probléma jelentéséért
-   HD Moore, [Rapid7,](http://www.rapid7.com/) az MS10-083 számú közleményben bemutatott probléma jelentéséért
-   David Dewey, [IBM ISS X-Force](http://www.iss.net/) és Ryan Smith, [Accuvant](http://www.accuvant.com/) (korábban a [VeriSign iDefense Labs](http://labs.idefense.com/) munkatársa), az MS10-083 közlemény részét képező hatékony védelmi módosításokkal kapcsolatos együttműködésért
-   A [Mu Test Suite Team](http://www.mudynamics.com/products/mu-test-suite.html), [Mu Dynamics](http://www.mudynamics.com/), az MS10-085 közleményben bemutatott probléma jelentéséért

#### Terméktámogatás

-   Teszteléssel állapították meg a felsorolt szoftverek egyes verzióinak érintettségét. A többi verzió támogatási életciklusa végére ért. Az egyes szoftververziók támogatási életciklusáról a [Microsoft termékek terméktámogatási életciklusát ismertető webhelyen](http://go.microsoft.com/fwlink/?linkid=21742) talál felvilágosítást.
-   Az Amerikai Egyesült Államokban és Kanada területén élő ügyfelek technikai támogatást kérhetnek a [biztonsági támogatás szolgáltatójától](http://go.microsoft.com/fwlink/?linkid=21131) vagy az 1-866-PCSAFETY telefonszámon. A biztonsági frissítésekkel kapcsolatos hívások ingyenesek. Az elérhető támogatási lehetőségekről további információt talál a [Microsoft segítségnyújtással és támogatással foglalkozó webhelyén](http://support.microsoft.com/).
-   Más országokban a helyi Microsoft-képviseletek nyújtanak támogatást. A biztonsági frissítésekkel kapcsolatos hívások ingyenesek. A [nemzetközi támogatási webhely](http://go.microsoft.com/fwlink/?linkid=21155) felvilágosítást nyújt arról, támogatási kérdéseivel hogyan fordulhat a Microsofthoz.

#### Felelősséget kizáró nyilatkozat

A Microsoft Tudásbázisban leírtak előzetes bejelentés nélkül változhatnak, és a cikkek tartalmáért a Microsoft nem vállal garanciát. A Microsoft egyben elhárít minden kifejezett és értelemszerű garanciát, beleértve az eladhatóságra és az adott célra való alkalmasságra vonatkozó garanciát is. A Microsoft Corporation vagy annak szállítói semmilyen körülmények között nem tehetők felelőssé közvetlen, közvetett, eseti, ok-okozati vagy különleges kárért (beleértve az elmaradt hasznot is), még akkor sem, ha a Microsoft Corporation vagy szállítói tudatában voltak a kár lehetséges voltának. Egyes államok törvényi szabályozása nem teszi lehetővé a véletlen vagy ok-okozati károkért vállalt felelősség korlátozását vagy kizárását, így ezekben az államokban az ez a felelősségkizárás nincs érvényben.

#### Verziók

-   1.0 verzió (2010. október 12.): Összefoglaló közlemény közzététele.
-   1.1 verzió (2010. október 13.): Az MS10-077 esetében a Windows Server 2008 és a Windows Server 2008 R2 esetében Fontosra változtattuk a súlyossági besorolást. Az MS10-082 esetében a Windows XP Professional x64 Edition Service Pack 2 rendszeren futó Windows Media Player 11 letöltési hivatkozását is módosítottuk.
-   2.0 verzió (2010. október 18.): Az MS10-085 biztonsági közleményben változott az Összefoglalásban található leírás: pontosítottuk, hogy a biztonsági rés olyan érintett rendszereken használható ki, melyek konfigurálva vannak SSL hálózati forgalom fogadására. A módosítás csak tájékoztató jellegű. A rendszer frissítését sikeresen elvégző felhasználóknak, ideértve az automatikus frissítést alkalmazókat is, nincs tennivalójuk. A frissítést nem telepített felhasználóknak először érdemes felmérniük, hogy rendszerükhöz szükség van-e a frissítésre.
-   3.0 verzió (2010. december 14.): A közleményt a következő bejelentés miatt frissítette a Microsoft: A.NET Framework 4.0 verzió MS10-07 keretében elérhető új frissítőcsomagjai egy olyan telepítési hiba kijavítására szolgálnak, amely akadályozhatja más frissítések és/vagy termékek sikeres telepítését. A rendszer frissítését már elvégzett felhasználóknak több tennivalójuk nincsen. Az MS10-083 közlemény keretében kiegészítő frissítést adtak ki a Windows Vista Service Pack 2 (KB979688) és a Windows Server 2008 Service Pack 2 (KB979688) azon felhasználói számára, akik a Windows Search 4.0 alkalmazást Windows Vista Service Pack 1 illetve Windows Server 2008 rendszerre telepítették, majd alkalmazták a KB2405882 közleményben felajánlott biztonsági frissítést, és ezután áttelepültek a Windows Vista Service Pack 2 vagy Windows Server 2008 Service Pack 2 rendszerre. Az új frissítés a [Microsoft Tudásbázis 2405882. cikkéből](http://support.microsoft.com/kb/2405882) elérhető.
-   4.0 verzió (2011. február 22.): Az MS10-077 közlemény frissítésében közölt észlelési módosítás folytán a rendszer felajánlja a Microsoft .NET-keretrendszer 4.0 frissítőcsomagjait a Microsoft .NET-keretrendszer 4.0 verzióját telepítő felhasználók számára, akik korábban már telepítették a Windows 7 x64 alapú rendszerekhez Service Pack 1, Windows Server 2008 R2 x64 alapú rendszerekhez Service Pack 1, illetve a Windows Server 2008 R2 Itanium alapú rendszerekhez Service Pack 1 operációs rendszert. A rendszer frissítését már elvégzett felhasználóknak több tennivalójuk nincsen.
-   4.1 verzió (2011. október 26.): Az MS10-077 közleménnyel kapcsolatban javították a .NET Framework 4 keretrendszerhez tartozó kiszolgálómag-telepítés alkalmazhatóságát a Windows Server 2008 R2 x64 alapú rendszerekhez operációs rendszeren.

*Built at 2014-04-18T01:50:00Z-07:00*
