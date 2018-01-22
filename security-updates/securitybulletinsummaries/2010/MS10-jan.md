---
TOCTitle: 'MS10-JAN'
Title: 'Microsoft biztonsági közlemény - összefoglalás, január 2010'
ms:assetid: 'ms10-jan'
ms:contentKeyID: 61227742
ms:mtpsurl: 'https://technet.microsoft.com/hu-HU/library/ms10-jan(v=Security.10)'
---

Security Bulletin Summary

Microsoft biztonsági közlemény - összefoglalás, január 2010
===========================================================

Közzétéve: 2010. január 12. | Frissítve: 2010. január 21.

**Verzió:** 2.0

Az összefoglaló a 2010 januárjában kiadott biztonsági közleményeket összegzi.

A 2010. januári közlemények kiadása folytán az összefoglaló a 2010. január 20-án kiadott előzetes értesítés helyébe lép. A biztonsági közlemények kiadásáról szóló előzetes értesítés szolgáltatásról itt olvashat bővebben: [Előzetes értesítés a Microsoft biztonsági közleményeinek kiadásáról](http://technet.microsoft.com/security/bulletin/advance).

Ha automatikus értesítést szeretne kapni a Microsoft biztonsági közleményeinek megjelenéséről, fizessen elő a [Microsoft Technical Security Notifications](http://go.microsoft.com/fwlink/?linkid=21163) szolgáltatásra.

A közleményekkel kapcsolatos kérdések megválaszolására a Microsoft 2010. január 13-án, csendes-óceáni idő szerint 11 órakor webes szemináriumot tart. [Jelentkezzen most a januári közleményeket bemutató webes szemináriumra](http://msevents.microsoft.com/cui/webcasteventdetails.aspx?eventid=1032427677&eventcategory=4&culture=en-us&countrycode=us). Ezt követően a webes szeminárium igény szerint kerül megrendezésre. További információkért látogasson el a [Microsoft biztonsági közleményeit és a webes szemináriumokat](http://technet.microsoft.com/security/bulletin/summary)bemutató oldalra.

Az összefoglaló közlemény 2.0 verzióját kiegészítő, soron kívüli biztonsági közleménnyel (MS10-002) kapcsolatos kérdések megválaszolására a Microsoft 2010. január 21-én, csendes-óceáni idő szerint 13 órakor webes szemináriumot tart. [Jelentkezzen most a január 21-én 13 órakor tartandó szemináriumra](http://msevents.microsoft.com/cui/eventdetail.aspx?eventid=1032440627&culture=en-us). Ezt követően a webes szeminárium igény szerint kerül megrendezésre. További információkért látogasson el a [Microsoft biztonsági közleményeit és a webes szemináriumokat](http://technet.microsoft.com/security/bulletin/summary)bemutató oldalra.

A Microsoft abban is segítséget nyújt felhasználóinak, hogy a havi biztonsági közleményekkel azonos napon kiadott, nem biztonsági jellegű, de fontos frissítéseket megfelelően rangsorolhassák. Lásd az **Egyéb információ című részt**.

### A közleménnyel kapcsolatos információk

Összefoglalások
---------------

<span></span>
A következő táblázat összegzi az e havi biztonsági közleményeket súlyossági sorrendben.

Az érintett szoftverekkel kapcsolatban további tudnivalókat a következő, az **Érintett szoftverek és letöltési helyek** című részben talál.

 
<p> </p>
<table style="border:1px solid black;">
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
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=169348">MS10-001</a></td>
<td style="border:1px solid black;"><strong>A beágyazott OpenType betűtípusmotor biztonsági rése távolról történő kódfuttatást tehet lehetővé (972270)</strong><br />
<br />
A biztonsági frissítés a Microsoft Windows közvetlenül jelentett biztonsági rését szünteti meg. A biztonsági rés akkor okozhat távoli kódfuttatást, ha a felhasználó speciálisan létrehozott beágyazott OpenType (EOT) betűtípussal leképezett tartalmat tekint meg az EOT betűtípusokkal kompatibilis olyan ügyfélalkalmazások egyikében, mint a Microsoft Internet Explorer, Microsoft Office PowerPoint vagy Microsoft Office Word. Ha egy támadó kihasználja a biztonsági rést, teljes mértékben átveheti a rendszer irányítását. Ezt követően a támadó programokat telepíthet, illetve adatokat tekinthet meg, módosíthat és törölhet, de korlátozás nélküli jogosultságokkal rendelkező új fiókokat is létrehozhat. A kevesebb jogosultsággal bíró fiókkal rendelkező felhasználók esetében kisebb a veszélyeztetettség, mint a rendszergazdai jogosultságokkal rendelkezők esetén</td>
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=21140">Kritikus</a><br />
Távoli kódfuttatás</td>
<td style="border:1px solid black;">Esetleg újra kell indítani a rendszert</td>
<td style="border:1px solid black;">Microsoft Windows</td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=179104">MS10-002</a></td>
<td style="border:1px solid black;"><strong>Összesítő biztonsági frissítés az Internet Explorer programhoz (978207)</strong><br />
<br />
A biztonsági frissítés hét közvetlenül és egy nyilvánosan jelentett biztonsági rést szüntet meg az Internet Explorer programban. A súlyosabb besorolású biztonsági rések távoli kódfuttatást tesznek lehetővé, amennyiben a felhasználó egy speciálisan kialakított weboldalt tekint meg az Internet Explorer alkalmazás segítségével. A kevesebb jogosultsággal bíró fiókkal rendelkező felhasználók esetében kisebb a veszélyeztetettség, mint a rendszergazdai jogosultságokkal rendelkezők esetén</td>
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=21140">Kritikus</a><br />
Távoli kódfuttatás</td>
<td style="border:1px solid black;">Újraindítást igényel</td>
<td style="border:1px solid black;">Microsoft Windows</td>
</tr>
</tbody>
</table>
  
Kihasználhatósági információk  
-----------------------------
  
<span></span>
A következő táblázat az adott hónapban megoldott biztonsági rések kihasználhatósági jellemzőit ismerteti. A biztonsági rések a közlemény azonosítója és súlyossági besorolás azonosítója szerint vannak felsorolva.
  
**A táblázat használata**
  
A táblázat segítségével meghatározható annak valószínűsége, hogy a biztonsági közlemény kiadását követő 30 napon belül a telepíteni szükséges biztonsági frissítésekre működő rosszindulatú programkódot jelentetnek meg. A telepítés fontossági sorrendjének megállapításához az adott konfigurációnak megfelelően tekintse át az alábbi értékeléseket. A minősítések jelentéséről és meghatározásuk módjáról a [Microsoft biztonsági rések jegyzéke](http://technet.microsoft.com/en-us/security/cc998259.aspx) tartalmaz bővebb információt.
  
| Közlemény azonosítója                                     | A biztonsági rés címe                                                                                 | CVE-azonosító                                                                    | Kihasználhatósági információk értékelése                                                                                 | Fontos megjegyzések                                                                                                                                                                                                 |  
|-----------------------------------------------------------|-------------------------------------------------------------------------------------------------------|----------------------------------------------------------------------------------|--------------------------------------------------------------------------------------------------------------------------|---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|  
| [MS10-001](http://go.microsoft.com/fwlink/?linkid=169348) | Biztonsági rés a Microtype Express tömörített betűkészletek egészszám-hibája az LZCOMP-kibontás során | [CVE-2010-0018](http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2010-0018) | [**2**](http://technet.microsoft.com/en-us/security/cc998259.aspx) - Valószínűleg inkonzisztens rosszindulatú programkód | A kihasználhatósági információk értékelése Microsoft Windows 2000 alapú rendszerekre vonatkozik. A Windows XP és frissebb operációs rendszereknél a kihasználás valószínűtlen.                                      |  
| [MS10-002](http://go.microsoft.com/fwlink/?linkid=179104) | XSS-szűrő parancsfájlkezelés miatti biztonsági rése                                                   | [CVE-2009-4074](http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2009-4074) | Nincsenek                                                                                                                | A biztonsági rés nem tesz lehetővé kódfuttatást.                                                                                                                                                                    |  
| [MS10-002](http://go.microsoft.com/fwlink/?linkid=179104) | URL-hitelesítés biztonsági rése                                                                       | [CVE-2010-0027](http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2010-0027) | [**1**](http://technet.microsoft.com/en-us/security/cc998259.aspx) - Valószínűleg konzisztens rosszindulatú programkód   | (Nincs)                                                                                                                                                                                                             |  
| [MS10-002](http://go.microsoft.com/fwlink/?linkid=179104) | Inicializálás hiánya miatti memóriameghibásodás okozta biztonsági rés                                 | [CVE-2010-0244](http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2010-0244) | [**1**](http://technet.microsoft.com/en-us/security/cc998259.aspx) - Valószínűleg konzisztens rosszindulatú programkód   | (Nincs)                                                                                                                                                                                                             |  
| [MS10-002](http://go.microsoft.com/fwlink/?linkid=179104) | Inicializálás hiánya miatti memóriameghibásodás okozta biztonsági rés                                 | [CVE-2010-0245](http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2010-0245) | Nincsenek                                                                                                                | Az [MS09-072](http://go.microsoft.com/fwlink/?linkid=169404) frissítést már alkalmazó felhasználók védve vannak, mivel az MS09-072 frissítésben foglalt módosítások megakadályozzák a biztonsági rés kihasználását. |  
| [MS10-002](http://go.microsoft.com/fwlink/?linkid=179104) | Inicializálás hiánya miatti memóriameghibásodás okozta biztonsági rés                                 | [CVE-2010-0246](http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2010-0246) | Nincsenek                                                                                                                | Az [MS09-072](http://go.microsoft.com/fwlink/?linkid=169404) frissítést már alkalmazó felhasználók védve vannak, mivel az MS09-072 frissítésben foglalt módosítások megakadályozzák a biztonsági rés kihasználását. |  
| [MS10-002](http://go.microsoft.com/fwlink/?linkid=179104) | Inicializálás hiánya miatti memóriameghibásodás okozta biztonsági rés                                 | [CVE-2010-0247](http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2010-0247) | [**1**](http://technet.microsoft.com/en-us/security/cc998259.aspx) - Valószínűleg konzisztens rosszindulatú programkód   | (Nincs)                                                                                                                                                                                                             |  
| [MS10-002](http://go.microsoft.com/fwlink/?linkid=179104) | HTML objektum miatti memóriameghibásodás okozta biztonsági rés                                        | [CVE-2010-0248](http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2010-0248) | [**2**](http://technet.microsoft.com/en-us/security/cc998259.aspx) - Valószínűleg inkonzisztens rosszindulatú programkód | (Nincs)                                                                                                                                                                                                             |  
| [MS10-002](http://go.microsoft.com/fwlink/?linkid=179104) | HTML objektum miatti memóriameghibásodás okozta biztonsági rés                                        | [CVE-2010-0249](http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2010-0249) | [**1**](http://technet.microsoft.com/en-us/security/cc998259.aspx) - Valószínűleg konzisztens rosszindulatú programkód   | **A biztonsági rést jelenleg internetszerte kihasználják.**                                                                                                                                                         |
  
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
</tr>
<tr>
<th colspan="3">
Microsoft Windows 2000  
</th>
</tr>
<tr>
<td style="border:1px solid black;">
**Közlemény azonosítója**
</td>
<td style="border:1px solid black;">
[**MS10-001**](http://go.microsoft.com/fwlink/?linkid=169348)
</td>
<td style="border:1px solid black;">
[**MS10-002**](http://go.microsoft.com/fwlink/?linkid=179104)
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
</tr>
<tr>
<td style="border:1px solid black;">
Microsoft Windows 2000 Service Pack 4
</td>
<td style="border:1px solid black;">
[Microsoft Windows 2000 Service Pack 4](http://www.microsoft.com/downloads/details.aspx?familyid=47f85cbd-282e-4c92-9809-68bba49e0a12)  
(Kritikus)
</td>
<td style="border:1px solid black;">
[Internet Explorer 5.01 Service Pack 4 alkalmazás Microsoft Windows 2000 Service Pack 4 rendszeren](http://www.microsoft.com/downloads/details.aspx?familyid=51e99e4f-1670-4b12-a9fe-e0ccf50cdabc)  
(Kritikus)  
[Internet Explorer 6 Service Pack 1, Microsoft Windows 2000 Service Pack 4 rendszerre telepítve](http://www.microsoft.com/downloads/details.aspx?familyid=a38aa9d0-c3fe-4d41-8805-7d5370263c1b)  
(Kritikus)
</td>
</tr>
<tr>
<th colspan="3">
Windows XP
</th>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
**Közlemény azonosítója**
</td>
<td style="border:1px solid black;">
[**MS10-001**](http://go.microsoft.com/fwlink/?linkid=169348)
</td>
<td style="border:1px solid black;">
[**MS10-002**](http://go.microsoft.com/fwlink/?linkid=179104)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
**Összesített súlyossági besorolás**
</td>
<td style="border:1px solid black;">
[**Alacsony**](http://go.microsoft.com/fwlink/?linkid=21140)
</td>
<td style="border:1px solid black;">
[**Kritikus**](http://go.microsoft.com/fwlink/?linkid=21140)
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
Windows XP Service Pack 2 és Windows XP Service Pack 3
</td>
<td style="border:1px solid black;">
[Windows XP Service Pack 2 és Windows XP Service Pack 3](http://www.microsoft.com/downloads/details.aspx?familyid=793a6b3f-7660-40be-b7d5-7b0eec55e1cd)  
(Alacsony)
</td>
<td style="border:1px solid black;">
[Internet Explorer 6 alkalmazás Windows XP Service Pack 2 és Windows XP Service Pack 3 rendszeren](http://www.microsoft.com/downloads/details.aspx?familyid=207eecad-6e84-48e6-ae18-6794a3618ee0)  
(Kritikus)  
[Internet Explorer 7 Windows XP Service Pack 2 rendszeren és Windows XP Service Pack 3 rendszeren](http://www.microsoft.com/downloads/details.aspx?familyid=3510c7d8-7e8f-479e-b6f9-5745a845664d)  
(Kritikus)  
[Internet Explorer 8 alkalmazás Windows XP Service Pack 2 és Windows XP Service Pack 3 rendszeren](http://www.microsoft.com/downloads/details.aspx?familyid=7c2948fb-f486-4801-bc21-bbf40d5a78c2)  
(Kritikus)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Windows XP Professional x64 Edition Service Pack 2
</td>
<td style="border:1px solid black;">
[Windows XP Professional x64 Edition Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=31609ce9-656a-4f7d-a501-709a31ca34c3)  
(Alacsony)
</td>
<td style="border:1px solid black;">
[Internet Explorer 6 alkalmazás Windows XP Professional x64 Edition Service Pack 2 rendszeren](http://www.microsoft.com/downloads/details.aspx?familyid=eb2d8055-4d50-4f83-82b8-055c7b8f5422)  
(Kritikus)  
[Internet Explorer 7 Windows XP Professional x64 Edition Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=cc5aea0b-e553-4f7f-a2cc-cba41bb87ae7)  
(Kritikus)  
[Internet Explorer 8 alkalmazás Windows XP Professional x64 Edition Service Pack 2 rendszeren](http://www.microsoft.com/downloads/details.aspx?familyid=41b83fad-948b-4a9c-80ed-9c5a60bd35b4)  
(Kritikus)
</td>
</tr>
<tr>
<th colspan="3">
Windows Server 2003
</th>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
**Közlemény azonosítója**
</td>
<td style="border:1px solid black;">
[**MS10-001**](http://go.microsoft.com/fwlink/?linkid=169348)
</td>
<td style="border:1px solid black;">
[**MS10-002**](http://go.microsoft.com/fwlink/?linkid=179104)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
**Összesített súlyossági besorolás**
</td>
<td style="border:1px solid black;">
[**Alacsony**](http://go.microsoft.com/fwlink/?linkid=21140)
</td>
<td style="border:1px solid black;">
[**Kritikus**](http://go.microsoft.com/fwlink/?linkid=21140)
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
Windows Server 2003 Service Pack 2
</td>
<td style="border:1px solid black;">
[Windows Server 2003 Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=e1d6e338-dea9-458e-b35d-796e069d74d7)  
(Alacsony)
</td>
<td style="border:1px solid black;">
[Internet Explorer 6 alkalmazás Windows Server 2003 Service Pack 2 rendszeren](http://www.microsoft.com/downloads/details.aspx?familyid=fea91227-44ad-4549-8732-497a8ceff870)  
(Mérsékelt)  
[Internet Explorer 7 alkalmazás Windows Server 2003 Service Pack 2 rendszeren](http://www.microsoft.com/downloads/details.aspx?familyid=14726445-3ff4-463c-9fc1-c9b758079aca)  
(Kritikus)  
[Internet Explorer 8 alkalmazás Windows Server 2003 Service Pack 2 rendszeren](http://www.microsoft.com/downloads/details.aspx?familyid=7d480c87-2ca9-4505-a59d-a6d73d001fa5)  
(Kritikus)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Windows Server 2003 x64 Edition Service Pack 2
</td>
<td style="border:1px solid black;">
[Windows Server 2003 x64 Edition Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=ddbcf231-9fde-4dc2-ad04-a01b69d1a980)  
(Alacsony)
</td>
<td style="border:1px solid black;">
[Internet Explorer 6 alkalmazás Windows Server 2003 x64 Edition Service Pack 2 rendszeren](http://www.microsoft.com/downloads/details.aspx?familyid=633e63f4-605b-43c4-8a4b-2730312a1c72)  
(Mérsékelt)  
[Internet Explorer 7 alkalmazás Windows Server 2003 x64 Edition Service Pack 2 rendszeren](http://www.microsoft.com/downloads/details.aspx?familyid=c8742230-16d8-4b2f-bd3e-8834c759856b)  
(Kritikus)  
[Internet Explorer 8 alkalmazás Windows Server 2003 x64 Edition Service Pack 2 rendszeren](http://www.microsoft.com/downloads/details.aspx?familyid=3e2e740b-8417-4758-8468-15221249ec71)  
(Kritikus)
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
Windows Server 2003 SP2 for Itanium-based Systems
</td>
<td style="border:1px solid black;">
[Windows Server 2003 SP2 javítócsomaggal Itanium alapú rendszerekhez](http://www.microsoft.com/downloads/details.aspx?familyid=c71a13cf-7e2f-4b02-8684-1a4e4b46ddda)  
(Alacsony)
</td>
<td style="border:1px solid black;">
[Internet Explorer 6 alkalmazás Windows Server 2003 rendszeren SP2 javítócsomaggal, Itanium alapú rendszerekhez](http://www.microsoft.com/downloads/details.aspx?familyid=b9308d50-ca66-43ff-9dc5-d05c90baa764)  
(Mérsékelt)  
[Internet Explorer 7 alkalmazás Windows Server 2003 SP2 Itanium alapú rendszerekhez](http://www.microsoft.com/downloads/details.aspx?familyid=5622f223-df9c-4a6a-bdf0-feebaf9920fd)  
(Kritikus)
</td>
</tr>
<tr>
<th colspan="3">
Windows Vista
</th>
</tr>
<tr>
<td style="border:1px solid black;">
**Közlemény azonosítója**
</td>
<td style="border:1px solid black;">
[**MS10-001**](http://go.microsoft.com/fwlink/?linkid=169348)
</td>
<td style="border:1px solid black;">
[**MS10-002**](http://go.microsoft.com/fwlink/?linkid=179104)
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
**Összesített súlyossági besorolás**
</td>
<td style="border:1px solid black;">
[**Alacsony**](http://go.microsoft.com/fwlink/?linkid=21140)
</td>
<td style="border:1px solid black;">
[**Kritikus**](http://go.microsoft.com/fwlink/?linkid=21140)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Windows Vista, Windows Vista Service Pack 1 és Windows Vista Service Pack 2
</td>
<td style="border:1px solid black;">
[Windows Vista, Windows Vista Service Pack 1, és Windows Vista Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=6387228c-eedc-4511-b3c6-8922606f4c84)  
(Alacsony)
</td>
<td style="border:1px solid black;">
[Internet Explorer 7 alkalmazás Windows Vista, Windows Vista Service Pack 1 és Windows Vista Service Pack 2 rendszeren](http://www.microsoft.com/downloads/details.aspx?familyid=92495551-dedd-43d4-bb3a-51028bc5c6d6)  
(Kritikus)  
[Internet Explorer 8 alkalmazás Windows Vista, Windows Vista Service Pack 1 és Windows Vista Service Pack 2 rendszeren](http://www.microsoft.com/downloads/details.aspx?familyid=5e2cbd7d-f64f-49e5-a159-1965ebfe2a92)  
(Kritikus)
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
Windows Vista x64 Edition, Windows Vista x64 Edition Service Pack 1 és Windows Vista x64 Edition Service Pack 2
</td>
<td style="border:1px solid black;">
[Windows Vista x64 Edition, Windows Vista x64 Edition Service Pack 1 és Windows Vista x64 Edition Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=7b4f5089-13b1-421b-a00b-22632bba4229)  
(Alacsony)
</td>
<td style="border:1px solid black;">
[Internet Explorer 7 alkalmazás Windows Vista x64 Edition, Windows Vista x64 Edition Service Pack 1 és Windows Vista x64 Edition Service Pack 2 rendszeren](http://www.microsoft.com/downloads/details.aspx?familyid=3cb139b3-59f4-44ef-9911-4dd4e3b83e7d)  
(Kritikus)  
[Internet Explorer 8 alkalmazás Windows Vista x64 Edition, Windows Vista x64 Edition Service Pack 1 és Windows Vista x64 Edition Service Pack 2 rendszeren](http://www.microsoft.com/downloads/details.aspx?familyid=b7a7e8e7-f4c5-459d-ab6c-05a192e1e3f9)  
(Kritikus)
</td>
</tr>
<tr>
<th colspan="3">
Windows Server 2008
</th>
</tr>
<tr>
<td style="border:1px solid black;">
**Közlemény azonosítója**
</td>
<td style="border:1px solid black;">
[**MS10-001**](http://go.microsoft.com/fwlink/?linkid=169348)
</td>
<td style="border:1px solid black;">
[**MS10-002**](http://go.microsoft.com/fwlink/?linkid=179104)
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
**Összesített súlyossági besorolás**
</td>
<td style="border:1px solid black;">
[**Alacsony**](http://go.microsoft.com/fwlink/?linkid=21140)
</td>
<td style="border:1px solid black;">
[**Kritikus**](http://go.microsoft.com/fwlink/?linkid=21140)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Windows Server 2008 32 bites rendszerekhez és Windows Server 2008 32 bites rendszerekhez, Service Pack 2
</td>
<td style="border:1px solid black;">
[Windows Server 2008 32 bites rendszerekhez és Windows Server 2008 32 bites rendszerekhez Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=e175c436-37e0-497f-8b7f-6cacaa25ad7c)\*\*  
(Alacsony)
</td>
<td style="border:1px solid black;">
[Internet Explorer 7 alkalmazás Windows Server 2008 32 bites rendszerekhez és Windows Server 2008 32 bites rendszerekhez, Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=8c4c91ec-1b2b-4176-bd77-45245b590329)\*\*  
(Kritikus)  
[Internet Explorer 8 alkalmazás Windows Server 2008 32 bites rendszerekhez és Windows Server 2008 32 bites rendszerekhez, Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=f5ce8582-af63-4870-bee3-0abeeefa1458)\*\*  
(Kritikus)
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
Windows Server 2008 x64 alapú rendszerekhez és Windows Server 2008 x64 alapú rendszerekhez, Service Pack 2
</td>
<td style="border:1px solid black;">
[Windows Server 2008 x64 alapú rendszerekhez és Windows Server 2008 x64 alapú rendszerekhez Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=1b10a177-fd45-406f-8edc-b8d4b84881b7)\*\*  
(Alacsony)
</td>
<td style="border:1px solid black;">
[Internet Explorer 7 alkalmazás Windows Server 2008 x64 alapú rendszerekhez és Windows Server 2008 x64 alapú rendszerekhez, Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=4f9975b8-3f91-4116-9200-ef55ece75854)\*\*  
(Kritikus)  
[Internet Explorer 8 alkalmazás Windows Server 2008 x64 alapú rendszerekhez és Windows Server 2008 x64 alapú rendszerekhez, Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=be11981c-d286-4e3c-94bf-d4e67a975d5a)\*\*  
(Kritikus)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Windows Server 2008 Itanium alapú rendszerekhez és Windows Server 2008 Itanium alapú rendszerekhez, Service Pack 2
</td>
<td style="border:1px solid black;">
[Windows Server 2008 Itanium alapú rendszerekhez és Windows Server 2008 Itanium alapú rendszerekhez, Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=e8bc9a24-a794-4827-a6bb-785c6b2189f4)  
(Alacsony)
</td>
<td style="border:1px solid black;">
[Internet Explorer 7 alkalmazás Windows Server 2008 Itanium alapú rendszerekhez és Windows Server 2008 Itanium alapú rendszerekhez, Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=9395547f-b620-4cbd-9ff5-11b76cd73859)  
(Kritikus)
</td>
</tr>
<tr>
<th colspan="3">
Windows 7
</th>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
**Közlemény azonosítója**
</td>
<td style="border:1px solid black;">
[**MS10-001**](http://go.microsoft.com/fwlink/?linkid=169348)
</td>
<td style="border:1px solid black;">
[**MS10-002**](http://go.microsoft.com/fwlink/?linkid=179104)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
**Összesített súlyossági besorolás**
</td>
<td style="border:1px solid black;">
[**Alacsony**](http://go.microsoft.com/fwlink/?linkid=21140)
</td>
<td style="border:1px solid black;">
[**Kritikus**](http://go.microsoft.com/fwlink/?linkid=21140)
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
Windows 7 32 bites rendszerekhez
</td>
<td style="border:1px solid black;">
[Windows 7 32 bites rendszerekhez](http://www.microsoft.com/downloads/details.aspx?familyid=75491ad0-40a6-4efb-9574-d82210f6d0da)  
(Alacsony)
</td>
<td style="border:1px solid black;">
[Internet Explorer 8 alkalmazás Windows 7 32 bites rendszereken](http://www.microsoft.com/downloads/details.aspx?familyid=278443c1-15dc-436b-893b-ffea6d29d16d)  
(Kritikus)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Windows 7 x64 alapú rendszerekhez
</td>
<td style="border:1px solid black;">
[Windows 7 x64 alapú rendszerekhez](http://www.microsoft.com/downloads/details.aspx?familyid=8a53f0e9-0616-440e-90f2-a12524e1bee4)  
(Alacsony)
</td>
<td style="border:1px solid black;">
[Internet Explorer 8 alkalmazás Windows 7 x64 alapú rendszereken](http://www.microsoft.com/downloads/details.aspx?familyid=a584cd0f-2e05-4e36-8858-0ffead637162)  
(Kritikus)
</td>
</tr>
<tr>
<th colspan="3">
Windows Server 2008 R2
</th>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
**Közlemény azonosítója**
</td>
<td style="border:1px solid black;">
[**MS10-001**](http://go.microsoft.com/fwlink/?linkid=169348)
</td>
<td style="border:1px solid black;">
[**MS10-002**](http://go.microsoft.com/fwlink/?linkid=179104)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
**Összesített súlyossági besorolás**
</td>
<td style="border:1px solid black;">
[**Alacsony**](http://go.microsoft.com/fwlink/?linkid=21140)
</td>
<td style="border:1px solid black;">
[**Kritikus**](http://go.microsoft.com/fwlink/?linkid=21140)
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
Windows Server 2008 R2 x64 alapú rendszerekhez
</td>
<td style="border:1px solid black;">
[Windows Server 2008 R2 x64 alapú rendszerekhez](http://www.microsoft.com/downloads/details.aspx?familyid=308166e4-571b-4d6c-bd9f-3ed4afa4eafe)\*\*  
(Alacsony)
</td>
<td style="border:1px solid black;">
[Internet Explorer 8 alkalmazás Windows Server 2008 R2 x64 alapú rendszerekhez](http://www.microsoft.com/downloads/details.aspx?familyid=d3386793-a594-4bc5-8308-28b561d43087)\*\*  
(Kritikus)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Windows Server 2008 R2 Itanium alapú rendszerekhez
</td>
<td style="border:1px solid black;">
[Windows Server 2008 R2 Itanium alapú rendszerekhez](http://www.microsoft.com/downloads/details.aspx?familyid=1d0da42b-9755-4fd2-afd1-0d023d187133)  
(Alacsony)
</td>
<td style="border:1px solid black;">
[Internet Explorer 8 alkalmazás Windows Server 2008 R2 Itanium alapú rendszerekhez](http://www.microsoft.com/downloads/details.aspx?familyid=9d137bab-8312-4240-af74-c65ba652fde0)  
(Kritikus)
</td>
</tr>
</table>
 
**Megjegyzések a Windows Server 2008 és Windows Server 2008 R2 rendszerhez**

**\*\*A kiszolgálómag-telepítés nem érintett.** A frissítésben tárgyalt biztonsági rések nem érintik a jelzett módon a Windows Server 2008 és a Windows Server 2008 R2 támogatott kiadásait, amennyiben a telepítés a kiszolgálómag-telepítési opció használatával történt. Erről a telepítési opcióról bővebben a [Kiszolgálómag](http://msdn.microsoft.com/en-us/library/ms723891(vs.85).aspx) és a [Kiszolgálómag a Windows Server 2008 R2 rendszerhez](http://msdn.microsoft.com/en-us/library/ee391631(vs.85).aspx) MSDN-cikkekben olvashat. A kiszolgálómag-telepítési opció nem vonatkozik a Windows Server 2008 és a Windows Server 2008 R2 bizonyos kiadásaira; lásd: [A kiszolgálómag-telepítési opciók összehasonlítása](http://www.microsoft.com/windowsserver2008/en/us/compare-core-installation.aspx).

Észlelési és telepítési eszközök, útmutatás
-------------------------------------------

<span></span>
**Biztonsági központ**

A szoftveres és biztonsági frissítések kezeléséhez azokat a szervezet asztali és hordozható számítógépeire, valamint kiszolgálóira is telepíteni kell. További tájékoztatásért látogasson el a [TechNet Update Management Center](http://go.microsoft.com/fwlink/?linkid=69903) weboldalára. A [TechNet Security Center](http://go.microsoft.com/fwlink/?linkid=21171) bővebb tájékoztatással szolgál a Microsoft-termékek biztonsági funkcióival kapcsolatban. A [Biztonság otthon](http://go.microsoft.com/fwlink/?linkid=85102) weboldalon a megfelelő hivatkozásra kattintva elérhetőek a legújabb biztonsági frissítések.

A biztonsági frissítések a [Microsoft Update](http://go.microsoft.com/fwlink/?linkid=40747) és a [Windows Update](http://go.microsoft.com/fwlink/?linkid=21130) weboldalról tölthetők le. A biztonsági frissítések a [Microsoft letöltőközpontjában](http://go.microsoft.com/fwlink/?linkid=21129) is elérhetőek. Legegyszerűbben a „security update” kifejezésre irányuló kulcsszavas kereséssel találhatja meg ezeket.

A biztonsági frissítések a [Microsoft Update katalógusából](http://go.microsoft.com/fwlink/?linkid=96155) is letölthetőek. A Microsoft Update katalógus a Windows Update és Microsoft Update szolgáltatáson keresztül elérhető tartalom kereshető adatbázisa; ide tartoznak a biztonsági frissítések, illesztőprogramok és szervizcsomagok. A biztonsági közlemény azonosítójára (pl. „MS07-036”) történő kereséssel hozzáadhatja az összes vonatkozó frissítést a kosárhoz (beleértve a frissítés különböző nyelvi változatait), és letöltheti azokat a megadott mappába. A Microsoft Update katalógus részletes leírását lásd a vonatkozó [GYIK](http://go.microsoft.com/fwlink/?linkid=97900)részben.

**Megjegyzés** 2009. augusztus 1-től a Microsoft megszünteti az Office Update és az Office Update Inventory Tool támogatását. A Microsoft Office termékeihez készült legújabb frissítéseket a [Microsoft Update](http://go.microsoft.com/fwlink/?linkid=40747) segítségével érheti el. A további tudnivalókat lásd [Az Office Update bemutatása: Gyakran ismételt kérdések című témakört.](http://office.microsoft.com/en-us/downloads/fx010402221033.aspx)

**Útmutató az észleléshez és a telepítéshez**

A biztonsági frissítésekkel kapcsolatban a Microsoft észlelési és telepítési segítséget nyújt. Ez az útmutató olyan javaslatokat és tudnivalókat tartalmaz, amelyeket segítséget nyújthatnak az informatikusoknak a biztonsági frissítések észlelési és telepítési eszközeinek használatához. További tudnivalókat a [Microsoft Tudásbázis 961747. számú cikkében](http://support.microsoft.com/kb/961747) talál.

**Microsoft Baseline Security Analyzer**

A Microsoft Baseline Security Analyzer (MBSA) segítségével a rendszergazda mind a helyi, mind a távoli számítógépeken ellenőrizheti, hogy mely biztonsági frissítések hiányoznak, illetve hogy mely biztonsági beállítások vannak helytelenül megadva. Ha többet szeretne tudni az MBSA -eszközről, látogasson el a [Microsoft Baseline Security Analyzer webhelyre](http://go.microsoft.com/fwlink/?linkid=21134).

**Windows Server Update Services**

A Microsoft Server Update Services (WSUS) szolgáltatással a rendszergazdák gyorsan és megbízhatóan telepíthetik a legújabb fontos és biztonsági frissítéseket Microsoft Windows 2000 és újabb operációs rendszerekhez, Office XP és újabb operációs rendszerekhez, Exchange Server 2003 és SQL Server 2000 Microsoft Windows 2000 és újabb operációs rendszerekre.

A biztonsági frissítésnek Windows Server Update Services szolgáltatással történő központi telepítéséről a [Windows Server Update Services](http://go.microsoft.com/fwlink/?linkid=50120) webhelyen tudhat meg többet.

**Systems Management Server**

A Microsoft Systems Management Server (SMS) rendszer egy sokoldalúan beállítható vállalati megoldás, amely a frissítések kezelésére szolgál. Az SMS segítségével a rendszergazda megállapíthatja, hogy melyik Windows alapú számítógép szorul biztonsági frissítésre, és ezeket a frissítéseket szabályozott módon, a felhasználók minimális zavarásával központilag telepítheti a vállalat teljes informatikai környezetében. Az SMS, vagyis a System Center Configuration Manager 2007 újabb kiadása immáron elérhető, lásd még: [System Center Configuration Manager 2007](http://technet.microsoft.com/en-us/library/bb735860.aspx). Arról, hogy a rendszergazdák hogyan használhatják a biztonsági frissítések telepítéséhez az SMS 2003 alkalmazást, az [SMS 2003 Security Patch Management](http://go.microsoft.com/fwlink/?linkid=22939) részben olvashat. A biztonsági frissítések felderítéséhez az SMS 2.0 felhasználók a Security Update Inventory Tool (SUIT) eszközt is használhatják. Az SMS-szolgáltatásról bővebben a [Microsoft Systems Management Server](http://go.microsoft.com/fwlink/?linkid=21158) oldalán olvashat.

**Megjegyzés** Az SMS a Microsoft Baseline Security Analyzer eszközön keresztül széles körű támogatást nyújt a biztonsági közlemények frissítéseinek észleléséhez, valamint a frissítések telepítéséhez. Előfordulhat, hogy egyes szoftverfrissítéseket ezek az eszközök nem észlelnek. Az SMS-alkalmazás leltározási szolgáltatásai segítségével a rendszergazdák adott rendszereken hajthatják végre a frissítést. Az eljárással kapcsolatban olvassa el a [szoftverfrissítések telepítése az SMS szoftverelosztó ügynök segítségével](http://go.microsoft.com/fwlink/?linkid=33341) című tájékoztatót. Egyes biztonsági frissítésekhez rendszergazdai jogosultságokra van szükség a számítógép újraindítása után. A rendszergazdák az Elevated Rights Deployment Tool eszközt (az [SMS 2.0 Administration Feature Pack](http://go.microsoft.com/fwlink/?linkid=21161) része) alkalmazhatják a frissítések telepítéséhez.

**Az Update Compatibility Evaluator (a frissítéskompatibilitás kiértékelője) és az Application Compatibility Toolkit (alkalmazáskompatibilitási eszközkészlet)**

Az alkalmazások működése érdekében a frissítések gyakran írnak ugyanazokba a fájlokba, illetve regisztrációs bejegyzésekbe. Ez inkompatibilitást okozhat, és növelheti a biztonsági frissítések központi telepítésére használt időt. A Windows frissítések és az alkalmazásoknak való megfelelőség tesztelése és ellenőrzése egyszerűsíthető az [Update Compatibility Evaluator](http://technet2.microsoft.com/windowsvista/en/library/4279e239-37a4-44aa-aec5-4e70fe39f9de1033.mspx?mfr=true) eszközeivel, ami része az [Application Compatibility Toolkit](http://www.microsoft.com/downloads/details.aspx?familyid=24da89e9-b581-47b0-b45e-492dd6da2971&displaylang=hu) alkalmazáskompatibilitási eszközkészletnek.

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

-   A biztonsági frissítések a [Microsoft letöltőközpontban](http://go.microsoft.com/fwlink/?linkid=21129) érhetők el. Legegyszerűbben a „security update” kifejezésre irányuló kulcsszavas kereséssel találhatja meg ezeket.
-   Az ügyfélrendszerek frissítései a [Microsoft Update](http://go.microsoft.com/fwlink/?linkid=40747) oldalról elérhetőek.
-   A Windows Update szolgáltatáson keresztül terjesztett havi aktuális biztonsági frissítések a letöltőközpontból a biztonsági és kritikus frissítéseket tartalmazó ISO CD-képfájlként is letölthetőek. További információt a [Microsoft Tudásbázis 913086](http://support.microsoft.com/kb/913086) számú cikkében talál.

**IT Pro Security közösség**

Az [IT Pro Security Community](http://go.microsoft.com/fwlink/?linkid=21164) közösségben hasznos információt találhat a biztonság javításáról és az informatikai infrastruktúrák optimalizálásáról, továbbá eszmecserét folytathat a biztonsági kérdésekről más informatikai szakemberekkel.

#### Köszönetnyilvánítás

A Microsoft [köszönetét](http://go.microsoft.com/fwlink/?linkid=21127) fejezi ki a vásárlók védelmének biztosításában nyújtott segítségért az alábbi szervezet(ek)nek és szakember(ek)nek:

-   Tavis Ormandy, [Google Inc.](http://www.google.com/), az MS10-001 közleményben bemutatott probléma jelentéséért
-   [David Lindsay "thornmaker"](http://p42.us/) és [Eduardo A. Vela Nava "sirdarckcat"](http://www.sirdarckcat.net/), az MS10-002 közleményben ismertetett egyik probléma jelentéséért
-   Lostmon Lords, az MS10-002 közleményben ismertetett egyik probléma jelentéséért
-   Brett Moore, a [TippingPoint](http://www.tippingpoint.com/) és a [Zero Day Initiative](http://www.zerodayinitiative.com/), együttműködő partnere, az MS10-002 közleményben ismertetett egyik probléma jelentéséért
-   Wushi, a [team509](http://www.team509.com/) tagja, a [TippingPoint](http://www.tippingpoint.com/) és a [Zero Day Initiative](http://www.zerodayinitiative.com/) munkatársa, az MS10-002 közleményben bemutatott egyik probléma jelentéséért
-   Sam Thomas, eshu.co.uk, a [TippingPoint](http://www.tippingpoint.com/) és a [Zero Day Initiative](http://www.zerodayinitiative.com/) munkatársa, az MS10-002 számú közleményben bemutatott egyik probléma jelentéséért
-   Sam Thomas, eshu.co.uk, a [TippingPoint](http://www.tippingpoint.com/) és a [Zero Day Initiative](http://www.zerodayinitiative.com/) munkatársa, az MS10-002 számú közleményben bemutatott egyik probléma jelentéséért
-   Haifei Li, Fortinet, [FortiGuard Global Security Research Team,](http://www.fortiguardcenter.com/) az MS10-002 közleményben bemutatott egyik probléma jelentéséért
-   Peter Vreugdenhil, [Verisign iDefense Labs](http://labs.idefense.com/), a [TippingPoint](http://www.tippingpoint.com/) és a [Zero Day Initiative](http://www.zerodayinitiative.com/) munkatársa, az MS10-002 közleményben ismertetett egyik probléma jelentéséért
-   Meron Sellem, [BugSec](http://www.bugsec.com/), az MS10-002 közleményben ismertetett egyik probléma jelentéséért

A Microsoft [köszönetet mond](http://go.microsoft.com/fwlink/?linkid=21127) a következő cégeknek az együttműködésért és a részletek feltárásáért az MS10-002 közleményben ismertetett egyik probléma kapcsán:

-   [Google Inc.](http://www.google.com/) és [MANDIANT](http://www.mandiant.com/)
-   [Adobe](http://www.adobe.com/)
-   [McAfee](http://www.mcafee.com/)
-   French government CSIRT ([CERTA](http://www.certa.ssi.gouv.fr))

#### Terméktámogatás

-   Teszteléssel állapították meg a felsorolt szoftverek egyes verzióinak érintettségét. A többi verzió támogatási életciklusa végére ért. Az egyes szoftververziók támogatási életciklusáról a [Microsoft termékek terméktámogatási életciklusát ismertető webhelyen](http://go.microsoft.com/fwlink/?linkid=21742) talál felvilágosítást.
-   Az Amerikai Egyesült Államokban és Kanada területén élő ügyfelek technikai támogatást kérhetnek a [biztonsági támogatás szolgáltatójától](http://go.microsoft.com/fwlink/?linkid=21131) vagy az 1-866-PCSAFETY telefonszámon. A biztonsági frissítésekkel kapcsolatos hívások ingyenesek. Az elérhető támogatási lehetőségekről további információt talál a [Microsoft segítségnyújtással és támogatással foglalkozó webhelyén](http://support.microsoft.com/).
-   Más országokban a helyi Microsoft-képviseletek nyújtanak támogatást. A biztonsági frissítésekkel kapcsolatos hívások ingyenesek. A [nemzetközi támogatási webhely](http://go.microsoft.com/fwlink/?linkid=21155) felvilágosítást nyújt arról, támogatási kérdéseivel hogyan fordulhat a Microsofthoz.

#### Felelősséget kizáró nyilatkozat

A Microsoft Tudásbázisban leírtak előzetes bejelentés nélkül változhatnak, és a cikkek tartalmáért a Microsoft nem vállal garanciát. A Microsoft egyben elhárít minden kifejezett és értelemszerű garanciát, beleértve az eladhatóságra és az adott célra való alkalmasságra vonatkozó garanciát is. A Microsoft Corporation vagy annak szállítói semmilyen körülmények között nem tehetők felelőssé közvetlen, közvetett, eseti, ok-okozati vagy különleges kárért (beleértve az elmaradt hasznot is), még akkor sem, ha a Microsoft Corporation vagy szállítói tudatában voltak a kár lehetséges voltának. Egyes államok törvényi szabályozása nem teszi lehetővé a véletlen vagy ok-okozati károkért vállalt felelősség korlátozását vagy kizárását, így ezekben az államokban az ez a felelősségkizárás nincs érvényben.

#### Verziók

-   1.0 verzió (2010. január 12.): Összefoglaló közlemény közzététele.
-   2.0 verzió (2010. január 21.): Megjelent az **Összesítő frissítés az Internet Explorerhez (978207) az MS10-002** Microsoft biztonsági közleményhez. A soron kívüli biztonsági frissítés webes szemináriumokra vonatkozó hivatkozással is kiegészült.

*Built at 2014-04-18T01:50:00Z-07:00*
