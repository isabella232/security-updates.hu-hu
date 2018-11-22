---
TOCTitle: 'MS12-FEB'
Title: 'A Microsoft biztonsági közleményei - összefoglalás, 2012. február'
ms:assetid: 'ms12-feb'
ms:contentKeyID: 61227764
ms:mtpsurl: 'https://technet.microsoft.com/hu-HU/library/ms12-feb(v=Security.10)'
author: SharonSears
ms.author: SharonSears
---

Security Bulletin Summary

A Microsoft biztonsági közleményei - összefoglalás, 2012. február
=================================================================

Közzétéve: 2012. február 14.

**Verzió:** 1.0

Az összefoglaló a 2012 februárjában kiadott biztonsági közleményeket összegzi.

A 2012. februári biztonsági közlemények kiadása folytán az összefoglaló a 2012. február 9-én kiadott előzetes értesítés helyébe lép. További információk a biztonsági közlemények kiadásáról szóló előzetes értesítés szolgáltatásról lásd: [Előzetes értesítés a Microsoft biztonsági közleményeinek kiadásáról](http://go.microsoft.com/fwlink/?linkid=217213).

Ha automatikus értesítést szeretne kapni a Microsoft biztonsági közleményeinek megjelenéséről, fizessen elő a [Microsoft Technical Security Notifications](http://go.microsoft.com/fwlink/?linkid=21163) szolgáltatásra.

A közleményekkel kapcsolatos kérdések megválaszolására a Microsoft 2012. február 15-én, csendes-óceáni idő szerint 11 órakor webes szemináriumot tart. Jelentkezzen most a [februári közleményeket bemutató webes szemináriumra](https://msevents.microsoft.com/cui/eventdetail.aspx?eventid=1032499501). Ezt követően a webes szeminárium igény szerint kerül megrendezésre. További információkért látogasson el a [Microsoft biztonsági közleményeit és a webes szemináriumokat](http://go.microsoft.com/fwlink/?linkid=217214) bemutató oldalra.

A Microsoft abban is segítséget nyújt felhasználóinak, hogy a havi biztonsági közleményekkel azonos napon kiadott, nem biztonsági jellegű frissítéseket megfelelően rangsorolhassák. Lásd az **Egyéb információ című részt**.

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
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=238387">MS12-008</a></td>
<td style="border:1px solid black;"><strong>A kernelmódú Windows illesztőprogramok biztonsági rései távoli programkódfuttatásra adhatnak lehetőséget (2660465)</strong><br />
<br />
Ez a biztonsági frissítés egy közvetlenül jelentett és egy nyilvánosságra került biztonsági rést szüntet meg a Microsoft Windows rendszerben. A súlyosabb besorolású biztonsági rés távoli kódfuttatást tehet lehetővé, ha a felhasználó egy speciálisan kialakított tartalmú webhelyre látogat el, vagy helyileg futtat egy speciálisan kialakított alkalmazást. A támadónak nincs lehetősége arra, hogy a felhasználót a rosszindulatú kódot tartalmazó webhely megnyitására kényszerítse. Csupán megkísérelheti rávenni a felhasználókat arra, hogy kattintsanak az e-mailben vagy azonnali üzenetben megjelenő hivatkozásra, amelyen keresztül a támadó weboldalára jutnak.</td>
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=21140">Kritikus</a><br />
Távoli kódfuttatás</td>
<td style="border:1px solid black;">Újraindítást igényel</td>
<td style="border:1px solid black;">Microsoft Windows</td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=236989">MS12-010</a></td>
<td style="border:1px solid black;"><strong>Összesítő biztonsági frissítés az Internet Explorer programhoz (2647516)</strong><br />
<br />
Ez a biztonsági frissítés az Internet Explorer nyolc közvetlenül jelzett biztonsági rését szünteti meg. A súlyosabb biztonsági rések távoli kódfuttatást tesznek lehetővé, amennyiben a felhasználó speciálisan kialakított weboldalt tekint meg az Internet Explorer alkalmazással. A biztonsági rések valamelyikét sikeresen kihasználó támadó a bejelentkezett felhasználóval egyező hozzáférést nyer a rendszerhez. A kevesebb jogosultsággal bíró fiókkal rendelkező felhasználók esetében kisebb a veszélyeztetettség, mint a rendszergazdai jogosultságokkal rendelkezők esetén</td>
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=21140">Kritikus</a><br />
Távoli kódfuttatás</td>
<td style="border:1px solid black;">Újraindítást igényel</td>
<td style="border:1px solid black;">Microsoft Windows,<br />
Internet Explorer</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=238617">MS12-013</a></td>
<td style="border:1px solid black;"><strong>A futásidejű C függvénytár biztonsági rése távoli programkódfuttatást tehet lehetővé (2654428)</strong><br />
<br />
A biztonsági frissítés a Microsoft Windows közvetlenül jelentett biztonsági rését szünteti meg. A biztonsági rés akkor tehet lehetővé távoli kódfuttatást, ha a felhasználó olyan különlegesen kialakított médiafájlt nyit meg, amelyik a webhelyén volt, vagy e-mail mellékleteként lett küldve. A biztonsági rést sikeresen kihasználó támadó a helyi felhasználóéval megegyező felhasználói jogokat nyerhet. A kevesebb jogosultsággal bíró fiókkal rendelkező felhasználók esetében kisebb a veszélyeztetettség, mint a rendszergazdai jogosultságokkal rendelkezők esetén</td>
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=21140">Kritikus</a><br />
Távoli kódfuttatás</td>
<td style="border:1px solid black;">Újraindítást igényel</td>
<td style="border:1px solid black;">Microsoft Windows</td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=235370">MS12-016</a></td>
<td style="border:1px solid black;"><strong>A .NET-keretrendszer és a Microsoft Silverlight biztonsági rései távoli programkódfuttatást tehetnek lehetővé (2651026)</strong><br />
<br />
A biztonsági frissítés a Microsoft.NET Framework és a Microsoft Silverlight egy nyilvánosságra került és egy közvetlenül jelentett biztonsági résének hibáját hárítja el. A biztonsági rések távoli kódfuttatást tehetnek lehetővé az ügyfélrendszereken, ha a felhasználó különlegesen kialakított weboldalt tekint meg az XAML böngészőalkalmazások (XBAP alkalmazások) vagy Silverlight alkalmazások futtatására alkalmas böngészőben. A kevesebb jogosultsággal bíró fiókkal rendelkező felhasználók esetében kisebb a veszélyeztetettség, mint a rendszergazdai jogosultságokkal rendelkezők esetén</td>
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=21140">Kritikus</a><br />
Távoli kódfuttatás</td>
<td style="border:1px solid black;">Esetleg újra kell indítani a rendszert</td>
<td style="border:1px solid black;">Microsoft .NET-keretrendszer,<br />
Microsoft Silverlight</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=238474">MS12-009</a></td>
<td style="border:1px solid black;"><strong>A kiegészítő funkció-illesztőprogramban lévő biztonsági rések a jogok kiterjesztését tehetik lehetővé (2645640)</strong><br />
<br />
Ez a biztonsági frissítés a Microsoft Windows két közvetlenül jelzett biztonsági rését szünteti meg. A biztonsági rések jogok kiterjesztését tehetik lehetővé, ha a támadó bejelentkezik a felhasználó rendszerére, és ott speciálisan kialakított alkalmazást futtat. A támadónak ezen biztonsági rések kihasználásához érvényes bejelentkezési adatokkal kell rendelkeznie, és képesnek kell lennie helyileg bejelentkezni a rendszerbe.</td>
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=21140">Fontos</a><br />
Jogok kiterjesztése</td>
<td style="border:1px solid black;">Újraindítást igényel</td>
<td style="border:1px solid black;">Microsoft Windows</td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=238500">MS12-011</a></td>
<td style="border:1px solid black;"><strong>A Microsoft SharePoint biztonsági rései jog kiterjesztését tehetik lehetővé (2663841)</strong><br />
<br />
Ez a biztonsági frissítés a Microsoft SharePoint és a Microsoft SharePoint Foundation három, közvetlenül jelentett biztonsági rését szünteti meg. E biztonsági rések a jogok kiterjesztését vagy az adatokhoz való illetéktelen hozzáférést teszik lehetővé, ha a felhasználó egy speciálisan kialakított URL-címre kattintott.</td>
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=21140">Fontos</a><br />
Jogok kiterjesztése</td>
<td style="border:1px solid black;">Esetleg újra kell indítani a rendszert</td>
<td style="border:1px solid black;">Microsoft Office,<br />
Microsoft Server Software</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=239941">MS12-012</a></td>
<td style="border:1px solid black;"><strong>A Színek vezérlőpult biztonsági rése távolról történő programkódfuttatást tehet lehetővé (2643719)</strong><br />
<br />
A biztonsági frissítés a Microsoft Windows egy nyilvánosan jelentett biztonsági rését szünteti meg. A biztonsági rés távoli kódfuttatást tehet lehetővé, ha a felhasználó olyan megbízható fájlt (például .icm vagy .icc fájlt) nyit meg, amely ugyanabban a könyvtárban található, mint egy különlegesen kialakított dinamikus csatolású függvénytár (DLL) fájl. A biztonsági rést kihasználó támadó a bejelentkezett felhasználóval egyező hozzáférést nyer a rendszerhez. A kevesebb jogosultsággal bíró fiókkal rendelkező felhasználók esetében kisebb a veszélyeztetettség, mint a rendszergazdai jogosultságokkal rendelkezők esetén</td>
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=21140">Fontos</a><br />
Távoli kódfuttatás</td>
<td style="border:1px solid black;">Esetleg újra kell indítani a rendszert</td>
<td style="border:1px solid black;">Microsoft Windows</td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=239945">MS12-014</a></td>
<td style="border:1px solid black;"><strong>Az Indeo Codec biztonsági rése távolról történő kódfuttatást tesz lehetővé (2661637)</strong><br />
<br />
A biztonsági frissítés a Microsoft Windows egy nyilvánosan jelentett biztonsági rését szünteti meg. A biztonsági rés távoli kódfuttatást tehet lehetővé, ha a felhasználó olyan megbízható fájlt (például .avi fájlt) nyit meg, amelyik ugyanabban a könyvtárban található, mint egy különlegesen kialakított dinamikus csatolású függvénytár (DLL) fájl. A biztonsági rést sikeresen kihasználó támadó tetszőleges programkódot futtathat a bejelentkezett felhasználó nevében. Ezt követően a támadó programokat telepíthet, illetve adatokat tekinthet meg, módosíthat és törölhet, de korlátozás nélküli jogosultságokkal rendelkező új fiókokat is létrehozhat. Ha valamely felhasználó felügyeleti jogosultságokkal bejelentkezett a rendszerbe, akkor a támadó teljes mértékben átveheti az irányítást a számítógép felett. A kevesebb jogosultsággal bíró fiókkal rendelkező felhasználók esetében kisebb a veszélyeztetettség, mint a rendszergazdai jogosultságokkal rendelkezők esetén</td>
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=21140">Fontos</a><br />
Távoli kódfuttatás</td>
<td style="border:1px solid black;">Esetleg újra kell indítani a rendszert</td>
<td style="border:1px solid black;">Microsoft Windows</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=238400">MS12-015</a></td>
<td style="border:1px solid black;"><strong>A Microsoft Visio Viewer 2010 biztonsági rései távolról történő programkódfuttatást tehetnek lehetővé (2663510)</strong><br />
<br />
Ez a biztonsági frissítés a Microsoft Office öt, közvetlenül jelzett biztonsági rését szünteti meg. A biztonsági rések távoli kódvégrehajtást tehetnek lehetővé, amennyiben a felhasználó egy speciálisan kialakított Visio fájlt nyit meg. A biztonsági réseket sikeresen kihasználó támadó a bejelentkezett felhasználóval egyező hozzáférést nyer a rendszerhez. A kevesebb jogosultsággal bíró fiókkal rendelkező felhasználók esetében kisebb a veszélyeztetettség, mint a rendszergazdai jogosultságokkal rendelkezők esetén</td>
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=21140">Fontos</a><br />
Távoli kódfuttatás</td>
<td style="border:1px solid black;">Esetleg újra kell indítani a rendszert</td>
<td style="border:1px solid black;">Microsoft Office</td>
</tr>
</tbody>
</table>
  
Kihasználhatósági információk  
-----------------------------
  
<span></span>
A következő táblázat az adott hónapban megoldott biztonsági rések kihasználhatósági jellemzőit ismerteti. A biztonsági rések a közlemény azonosítója és súlyossági besorolás azonosítója szerint vannak felsorolva. Csak a kritikus és fontos besorolású biztonsági rések szerepelnek.
  
**A táblázat használata**
  
Az alábbi táblázatból minden telepítendő biztonsági frissítésről megtudhatja, hogy mekkora a valószínűsége annak, hogy a biztonsági közlemény kiadása után 30 napon belül kódvégrehajtási és szolgáltatásmegtagadási támadások jelenhetnek meg. A havi frissítések telepítési sorrendjének meghatározásához, az adott konfigurációnak megfelelően tekintse át az alábbi értékeléseket. A minősítések jelentéséről és meghatározásuk módjáról a [Microsoft kihasználhatósági információk](http://technet.microsoft.com/security/cc998259.aspx) című rész tartalmaz bővebb információt.
  
Az alábbi oszlopokban a „legújabb szoftver” kifejezés az adott szoftver legutóbb kiadott változatára vonatkozik, a „korábbi szoftver” kifejezés az adott szoftver valamennyi, korábban kiadott támogatott verziójára vonatkozik, amint az az érintett vagy a nem érintett szoftverek felsorolásában szerepel.
  
| Közlemény azonosítója                                     | A biztonsági rés címe                                                                   | CVE-azonosító                                                                    | Kihasználhatóság felmérése a legújabb szoftvereknél                                                                   | Kihasználhatóság felmérése a korábbi szoftvereknél                                                                    | Szolgáltatásmegtagadás kihasználhatóságának felmérése | Fontos megjegyzések                                                                                                         |  
|-----------------------------------------------------------|-----------------------------------------------------------------------------------------|----------------------------------------------------------------------------------|-----------------------------------------------------------------------------------------------------------------------|-----------------------------------------------------------------------------------------------------------------------|-------------------------------------------------------|-----------------------------------------------------------------------------------------------------------------------------|  
| [MS12-008](http://go.microsoft.com/fwlink/?linkid=238387) | Billentyűkiosztás használata utáni felszabadítás biztonsági rése                        | [CVE-2012-0154](http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2012-0154) | [1](http://technet.microsoft.com/en-us/security/cc998259.aspx) - Konzisztens rosszindulatú programkódról van szó      | [1](http://technet.microsoft.com/en-us/security/cc998259.aspx) - Konzisztens rosszindulatú programkódról van szó      | Nem érintett                                          | (Nincs)                                                                                                                     |  
| [MS12-008](http://go.microsoft.com/fwlink/?linkid=238387) | A GDI hozzáférés-megsértési biztonsági rése                                             | [CVE-2011-5046](http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2011-5046) | [2](http://technet.microsoft.com/en-us/security/cc998259.aspx) - A kihasználáshoz szükséges kód nehezen szerkeszthető | [2](http://technet.microsoft.com/en-us/security/cc998259.aspx) - A kihasználáshoz szükséges kód nehezen szerkeszthető | Állandó                                               | A biztonsági rés nyilvánosságra került,                                                                                     |  
| [MS12-009](http://go.microsoft.com/fwlink/?linkid=238474) | Az AfdPoll jogok kiterjesztését eredményező biztonsági rése                             | [CVE-2012-0148](http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2012-0148) | [1](http://technet.microsoft.com/en-us/security/cc998259.aspx) - Konzisztens rosszindulatú programkódról van szó      | [3](http://technet.microsoft.com/en-us/security/cc998259.aspx) - Nem valószínű rosszindulatú programkód               | Állandó                                               | x64 rendszereken ki lehet használni a biztonsági rést , x86 rendszereken nem.                                               |  
| [MS12-009](http://go.microsoft.com/fwlink/?linkid=238474) | A kiegészítő funkció-illesztőprogram jogok kiterjesztését lehetővé tévő biztonsági rése | [CVE-2012-0149](http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2012-0149) | Nem érintett                                                                                                          | [1](http://technet.microsoft.com/en-us/security/cc998259.aspx) - Konzisztens rosszindulatú programkódról van szó      | Állandó                                               | Csak a Windows Server 2003 érintett.                                                                                        |  
| [MS12-010](http://go.microsoft.com/fwlink/?linkid=236989) | HTML elemek távolról történő kódfuttatást lehetővé tévő biztonsági rése                 | [CVE-2012-0011](http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2012-0011) | [1](http://technet.microsoft.com/en-us/security/cc998259.aspx) - Konzisztens rosszindulatú programkódról van szó      | [1](http://technet.microsoft.com/en-us/security/cc998259.aspx) - Konzisztens rosszindulatú programkódról van szó      | Ideiglenes                                            | (Nincs)                                                                                                                     |  
| [MS12-010](http://go.microsoft.com/fwlink/?linkid=236989) | A NULL bájt adatokhoz való illetéktelen hozzáférést okozó biztonsági rése               | [CVE-2012-0012](http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2012-0012) | [3](http://technet.microsoft.com/en-us/security/cc998259.aspx) - Nem valószínű rosszindulatú programkód               | Nem érintett                                                                                                          | Nem érintett                                          | A biztonsági rés illetéktelen adatelérést okoz.                                                                             |  
| [MS12-010](http://go.microsoft.com/fwlink/?linkid=236989) | A VML távoli kódfuttatást okozó biztonsági rése                                         | [CVE-2012-0155](http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2012-0155) | [1](http://technet.microsoft.com/en-us/security/cc998259.aspx) - Konzisztens rosszindulatú programkódról van szó      | Nem érintett                                                                                                          | Ideiglenes                                            | (Nincs)                                                                                                                     |  
| [MS12-011](http://go.microsoft.com/fwlink/?linkid=238500) | Az XSS inplview.aspx biztonsági rése                                                    | [CVE-2012-0017](http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2012-0017) | [1](http://technet.microsoft.com/en-us/security/cc998259.aspx) - Konzisztens rosszindulatú programkódról van szó      | Nem érintett                                                                                                          | Nem érintett                                          | (Nincs)                                                                                                                     |  
| [MS12-011](http://go.microsoft.com/fwlink/?linkid=238500) | Az XSS themeweb.aspx biztonsági rése                                                    | [CVE-2012-0144](http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2012-0144) | [1](http://technet.microsoft.com/en-us/security/cc998259.aspx) - Konzisztens rosszindulatú programkódról van szó      | Nem érintett                                                                                                          | Nem érintett                                          | (Nincs)                                                                                                                     |  
| [MS12-011](http://go.microsoft.com/fwlink/?linkid=238500) | Az XSS wizardlist.aspx biztonsági rése                                                  | [CVE-2012-0145](http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2012-0145) | [1](http://technet.microsoft.com/en-us/security/cc998259.aspx) - Konzisztens rosszindulatú programkódról van szó      | Nem érintett                                                                                                          | Nem érintett                                          | (Nincs)                                                                                                                     |  
| [MS12-012](http://go.microsoft.com/fwlink/?linkid=239941) | A Színek vezérlőpult függvénytárainak nem biztonságos betöltése miatti biztonsági rés   | [CVE-2010-5082](http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2010-5082) | [1](http://technet.microsoft.com/en-us/security/cc998259.aspx) - Konzisztens rosszindulatú programkódról van szó      | [1](http://technet.microsoft.com/en-us/security/cc998259.aspx) - Konzisztens rosszindulatú programkódról van szó      | Nem érintett                                          | A biztonsági rés nyilvánosságra került,                                                                                     |  
| [MS12-013](http://go.microsoft.com/fwlink/?linkid=238617) | Az Msvcrt.dll puffertúlcsordulást okozó biztonsági rése                                 | [CVE-2012-0150](http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2012-0150) | [1](http://technet.microsoft.com/en-us/security/cc998259.aspx) - Konzisztens rosszindulatú programkódról van szó      | [1](http://technet.microsoft.com/en-us/security/cc998259.aspx) - Konzisztens rosszindulatú programkódról van szó      | Ideiglenes                                            | (Nincs)                                                                                                                     |  
| [MS12-014](http://go.microsoft.com/fwlink/?linkid=239945) | Az Indeo Codec biztonsági rése a nem biztonságos betöltés miatt                         | [CVE-2010-3138](http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2010-3138) | Nem érintett                                                                                                          | [1](http://technet.microsoft.com/en-us/security/cc998259.aspx) - Konzisztens rosszindulatú programkódról van szó      | Nem érintett                                          | A biztonsági rés nyilvánosságra került,                                                                                     |  
| [MS12-015](http://go.microsoft.com/fwlink/?linkid=238400) | VSD fájlformátum memóriameghibásodás miatti biztonsági rése                             | [CVE-2012-0019](http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2012-0019) | [1](http://technet.microsoft.com/en-us/security/cc998259.aspx) - Konzisztens rosszindulatú programkódról van szó      | Nem érintett                                                                                                          | Nem érintett                                          | Ez a Visio Viewer 2010 és Visio Viewer 2010 Service Pack 1 alkalmazást érinti (csak a Visio Viewer támogatott változatait). |  
| [MS12-015](http://go.microsoft.com/fwlink/?linkid=238400) | VSD fájlformátum memóriameghibásodás miatti biztonsági rése                             | [CVE-2012-0020](http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2012-0020) | [1](http://technet.microsoft.com/en-us/security/cc998259.aspx) - Konzisztens rosszindulatú programkódról van szó      | Nem érintett                                                                                                          | Nem érintett                                          | Ez a Visio Viewer 2010 és Visio Viewer 2010 Service Pack 1 alkalmazást érinti (csak a Visio Viewer támogatott változatait). |  
| [MS12-015](http://go.microsoft.com/fwlink/?linkid=238400) | VSD fájlformátum memóriameghibásodás miatti biztonsági rése                             | [CVE-2012-0136](http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2012-0136) | [3](http://technet.microsoft.com/en-us/security/cc998259.aspx) - Nem valószínű rosszindulatú programkód               | Nem érintett                                                                                                          | Nem érintett                                          | Ez a Visio Viewer 2010 és Visio Viewer 2010 Service Pack 1 alkalmazást érinti (csak a Visio Viewer támogatott változatait). |  
| [MS12-015](http://go.microsoft.com/fwlink/?linkid=238400) | VSD fájlformátum memóriameghibásodás miatti biztonsági rése                             | [CVE-2012-0137](http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2012-0137) | [3](http://technet.microsoft.com/en-us/security/cc998259.aspx) - Nem valószínű rosszindulatú programkód               | Nem érintett                                                                                                          | Nem érintett                                          | Ez a Visio Viewer 2010 és Visio Viewer 2010 Service Pack 1 alkalmazást érinti (csak a Visio Viewer támogatott változatait). |  
| [MS12-015](http://go.microsoft.com/fwlink/?linkid=238400) | VSD fájlformátum memóriameghibásodás miatti biztonsági rése                             | [CVE-2012-0138](http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2012-0138) | [3](http://technet.microsoft.com/en-us/security/cc998259.aspx) - Nem valószínű rosszindulatú programkód               | Nem érintett                                                                                                          | Nem érintett                                          | Ez a Visio Viewer 2010 és Visio Viewer 2010 Service Pack 1 alkalmazást érinti (csak a Visio Viewer támogatott változatait). |  
| [MS12-016](http://go.microsoft.com/fwlink/?linkid=235370) | A .NET-keretrendszer nem kezelt objektumai miatti biztonsági rése                       | [CVE-2012-0014](http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2012-0014) | [1](http://technet.microsoft.com/en-us/security/cc998259.aspx) - Konzisztens rosszindulatú programkódról van szó      | [1](http://technet.microsoft.com/en-us/security/cc998259.aspx) - Konzisztens rosszindulatú programkódról van szó      | Nem érintett                                          | (Nincs)                                                                                                                     |  
| [MS12-016](http://go.microsoft.com/fwlink/?linkid=235370) | A .NET-keretrendszer memória-meghibásodási biztonsági rése                              | [CVE-2012-0015](http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2012-0015) | Nem érintett                                                                                                          | [1](http://technet.microsoft.com/en-us/security/cc998259.aspx) - Konzisztens rosszindulatú programkódról van szó      | Nem érintett                                          | A biztonsági rés nyilvánosságra került,                                                                                     |
  
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
<tr>
<th colspan="8">
Windows XP  
</th>
</tr>
<tr>
<td style="border:1px solid black;">
**Közlemény azonosítója**
</td>
<td style="border:1px solid black;">
[**MS12-008**](http://go.microsoft.com/fwlink/?linkid=238387)
</td>
<td style="border:1px solid black;">
[**MS12-010**](http://go.microsoft.com/fwlink/?linkid=236989)
</td>
<td style="border:1px solid black;">
[**MS12-013**](http://go.microsoft.com/fwlink/?linkid=238617)
</td>
<td style="border:1px solid black;">
[**MS12-016**](http://go.microsoft.com/fwlink/?linkid=235370)
</td>
<td style="border:1px solid black;">
[**MS12-009**](http://go.microsoft.com/fwlink/?linkid=238474)
</td>
<td style="border:1px solid black;">
[**MS12-012**](http://go.microsoft.com/fwlink/?linkid=239941)
</td>
<td style="border:1px solid black;">
[**MS12-014**](http://go.microsoft.com/fwlink/?linkid=239945)
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
Nincsenek
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
</tr>
<tr>
<td style="border:1px solid black;">
Windows XP Service Pack 3
</td>
<td style="border:1px solid black;">
[Windows XP Service Pack 3](http://www.microsoft.com/downloads/details.aspx?familyid=832afe5e-d61e-4554-b889-9174df042b32)  
(Kritikus)
</td>
<td style="border:1px solid black;">
[Internet Explorer 6](http://www.microsoft.com/downloads/details.aspx?familyid=a7d59fa8-0a49-4985-9f14-92218d3b5cea)  
(Mérsékelt)  
[Internet Explorer 7](http://www.microsoft.com/downloads/details.aspx?familyid=6025c5d6-696c-49cd-9264-96af5766d318)  
(Kritikus)  
[Internet Explorer 8](http://www.microsoft.com/downloads/details.aspx?familyid=5b37f5b1-207f-4fa1-9769-c873d672e80c)  
(Kritikus)
</td>
<td style="border:1px solid black;">
Nem érintett
</td>
<td style="border:1px solid black;">
[Microsoft .NET-keretrendszer 2.0 Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=5269e18b-d4f0-4c64-8df8-283a2ca66c59)  
(KB2633880)  
(Kritikus)  
[Microsoft .NET Framework 4](http://www.microsoft.com/downloads/details.aspx?familyid=70aadf34-abdc-4577-8da9-a0669dccc119)<sup>[1]</sup>
(KB2633870)  
(Kritikus)
</td>
<td style="border:1px solid black;">
Nem érintett
</td>
<td style="border:1px solid black;">
Nem érintett
</td>
<td style="border:1px solid black;">
[Windows XP Service Pack 3](http://www.microsoft.com/downloads/details.aspx?familyid=32e5c9ad-b610-4afb-b6f0-bb0b5fbdd1f6)  
(Fontos)
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
Windows XP Professional x64 Edition Service Pack 2
</td>
<td style="border:1px solid black;">
[Windows XP Professional x64 Edition Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=ff2c141c-08b4-42c6-9f66-580f8678c01f)  
(Kritikus)
</td>
<td style="border:1px solid black;">
[Internet Explorer 6](http://www.microsoft.com/downloads/details.aspx?familyid=96d404e7-8928-494e-8a3c-3897817cda7b)  
(Mérsékelt)  
[Internet Explorer 7](http://www.microsoft.com/downloads/details.aspx?familyid=b40bc334-edbc-48d5-9196-b7fb0e19966e)  
(Kritikus)  
[Internet Explorer 8](http://www.microsoft.com/downloads/details.aspx?familyid=2fc9d519-94b3-4b56-92fd-4c0ccf8210fe)  
(Kritikus)
</td>
<td style="border:1px solid black;">
Nem érintett
</td>
<td style="border:1px solid black;">
[Microsoft .NET-keretrendszer 2.0 Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=5269e18b-d4f0-4c64-8df8-283a2ca66c59)  
(KB2633880)  
(Kritikus)  
[Microsoft .NET Framework 4](http://www.microsoft.com/downloads/details.aspx?familyid=70aadf34-abdc-4577-8da9-a0669dccc119)<sup>[1]</sup>
(KB2633870)  
(Kritikus)
</td>
<td style="border:1px solid black;">
[Windows XP Professional x64 Edition Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=82f5c503-d2ea-4fed-8f9d-f30bee2f60b3)  
(Fontos)
</td>
<td style="border:1px solid black;">
Nem érintett
</td>
<td style="border:1px solid black;">
Nem érintett
</td>
</tr>
<tr>
<th colspan="8">
Windows Server 2003
</th>
</tr>
<tr>
<td style="border:1px solid black;">
**Közlemény azonosítója**
</td>
<td style="border:1px solid black;">
[**MS12-008**](http://go.microsoft.com/fwlink/?linkid=238387)
</td>
<td style="border:1px solid black;">
[**MS12-010**](http://go.microsoft.com/fwlink/?linkid=236989)
</td>
<td style="border:1px solid black;">
[**MS12-013**](http://go.microsoft.com/fwlink/?linkid=238617)
</td>
<td style="border:1px solid black;">
[**MS12-016**](http://go.microsoft.com/fwlink/?linkid=235370)
</td>
<td style="border:1px solid black;">
[**MS12-009**](http://go.microsoft.com/fwlink/?linkid=238474)
</td>
<td style="border:1px solid black;">
[**MS12-012**](http://go.microsoft.com/fwlink/?linkid=239941)
</td>
<td style="border:1px solid black;">
[**MS12-014**](http://go.microsoft.com/fwlink/?linkid=239945)
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
**Összesített** **súlyossági besorolás**
</td>
<td style="border:1px solid black;">
[**Kritikus**](http://go.microsoft.com/fwlink/?linkid=21140)
</td>
<td style="border:1px solid black;">
[**Mérsékelt**](http://go.microsoft.com/fwlink/?linkid=21140)
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
Nincsenek
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
[Windows Server 2003 Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=f0e6e06d-89db-45ad-9660-7959c6f9b546)  
(Kritikus)
</td>
<td style="border:1px solid black;">
[Internet Explorer 6](http://www.microsoft.com/downloads/details.aspx?familyid=c4642890-2fba-45da-bbe9-fcaa84e4aa0c)  
(Nincs súlyossági besorolás<sup>[1]</sup>)  
[Internet Explorer 7](http://www.microsoft.com/downloads/details.aspx?familyid=9e157b88-2c11-44dc-b13d-1051f9c39890)  
(Mérsékelt)  
[Internet Explorer 8](http://www.microsoft.com/downloads/details.aspx?familyid=bf8ad019-e710-4e16-be4f-8168df5c5343)  
(Mérsékelt)
</td>
<td style="border:1px solid black;">
Nem érintett
</td>
<td style="border:1px solid black;">
[Microsoft .NET-keretrendszer 2.0 Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=5269e18b-d4f0-4c64-8df8-283a2ca66c59)  
(KB2633880)  
(Kritikus)  
[Microsoft .NET Framework 4](http://www.microsoft.com/downloads/details.aspx?familyid=70aadf34-abdc-4577-8da9-a0669dccc119)<sup>[1]</sup>
(KB2633870)  
(Kritikus)
</td>
<td style="border:1px solid black;">
[Windows Server 2003 Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=5ee4bef7-b355-4aae-8bba-834a16d44744)  
(Fontos)
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
Windows Server 2003 x64 Edition Service Pack 2
</td>
<td style="border:1px solid black;">
[Windows Server 2003 x64 Edition Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=b81decda-9d82-4ffb-baae-78b190e553ea)  
(Kritikus)
</td>
<td style="border:1px solid black;">
[Internet Explorer 6](http://www.microsoft.com/downloads/details.aspx?familyid=c4a52801-55b5-4eef-9db3-c29a45863198)  
(Nincs súlyossági besorolás<sup>[1]</sup>)  
[Internet Explorer 7](http://www.microsoft.com/downloads/details.aspx?familyid=f162ad36-c096-43ba-a440-ec4d3fb54c21)  
(Mérsékelt)  
[Internet Explorer 8](http://www.microsoft.com/downloads/details.aspx?familyid=ef4a9002-b2da-40af-abc0-737565fea179)  
(Mérsékelt)
</td>
<td style="border:1px solid black;">
Nem érintett
</td>
<td style="border:1px solid black;">
[Microsoft .NET-keretrendszer 2.0 Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=5269e18b-d4f0-4c64-8df8-283a2ca66c59)  
(KB2633880)  
(Kritikus)  
[Microsoft .NET Framework 4](http://www.microsoft.com/downloads/details.aspx?familyid=70aadf34-abdc-4577-8da9-a0669dccc119)<sup>[1]</sup>
(KB2633870)  
(Kritikus)
</td>
<td style="border:1px solid black;">
[Windows Server 2003 x64 Edition Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=b53cf810-0ea3-4cb0-91f9-de1406ccfc96)  
(Fontos)
</td>
<td style="border:1px solid black;">
Nem érintett
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
[Windows Server 2003 SP2 Itanium-alapú rendszerekhez](http://www.microsoft.com/downloads/details.aspx?familyid=8dcd71c8-82ad-4f86-b386-7f1ea09e157f)  
(Kritikus)
</td>
<td style="border:1px solid black;">
[Internet Explorer 6](http://www.microsoft.com/downloads/details.aspx?familyid=3b42f935-7f59-4871-a01f-480033c3ad40)  
(Nincs súlyossági besorolás<sup>[1]</sup>)  
[Internet Explorer 7](http://www.microsoft.com/downloads/details.aspx?familyid=24fe7c08-4736-455b-9b98-1b6a65718143)  
(Mérsékelt)
</td>
<td style="border:1px solid black;">
Nem érintett
</td>
<td style="border:1px solid black;">
[Microsoft .NET-keretrendszer 2.0 Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=5269e18b-d4f0-4c64-8df8-283a2ca66c59)  
(KB2633880)  
(Kritikus)  
[Microsoft .NET Framework 4](http://www.microsoft.com/downloads/details.aspx?familyid=70aadf34-abdc-4577-8da9-a0669dccc119)<sup>[1]</sup>
(KB2633870)  
(Kritikus)
</td>
<td style="border:1px solid black;">
[Windows Server 2003 SP2 Itanium-alapú rendszerekhez](http://www.microsoft.com/downloads/details.aspx?familyid=3b18d22d-e192-498b-a105-b946a5f5bfad)  
(Fontos)
</td>
<td style="border:1px solid black;">
Nem érintett
</td>
<td style="border:1px solid black;">
Nem érintett
</td>
</tr>
<tr>
<th colspan="8">
Windows Vista
</th>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
**Közlemény azonosítója**
</td>
<td style="border:1px solid black;">
[**MS12-008**](http://go.microsoft.com/fwlink/?linkid=238387)
</td>
<td style="border:1px solid black;">
[**MS12-010**](http://go.microsoft.com/fwlink/?linkid=236989)
</td>
<td style="border:1px solid black;">
[**MS12-013**](http://go.microsoft.com/fwlink/?linkid=238617)
</td>
<td style="border:1px solid black;">
[**MS12-016**](http://go.microsoft.com/fwlink/?linkid=235370)
</td>
<td style="border:1px solid black;">
[**MS12-009**](http://go.microsoft.com/fwlink/?linkid=238474)
</td>
<td style="border:1px solid black;">
[**MS12-012**](http://go.microsoft.com/fwlink/?linkid=239941)
</td>
<td style="border:1px solid black;">
[**MS12-014**](http://go.microsoft.com/fwlink/?linkid=239945)
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
Nincsenek
</td>
<td style="border:1px solid black;">
Nincsenek
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
Windows Vista Service Pack 2
</td>
<td style="border:1px solid black;">
[Windows Vista Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=5852118c-fc39-45e2-8b44-ce1401d310e2)  
(Kritikus)
</td>
<td style="border:1px solid black;">
[Internet Explorer 7](http://www.microsoft.com/downloads/details.aspx?familyid=6ec23c7e-0166-47dc-ae86-c49b505206bb)  
(Kritikus)  
[Internet Explorer 8](http://www.microsoft.com/downloads/details.aspx?familyid=bbf627df-0bc0-478f-aa34-a7e5f039e589)  
(Kritikus)  
[Internet Explorer 9](http://www.microsoft.com/downloads/details.aspx?familyid=d287496a-411c-4c1b-9d98-bacc553041ae)  
(Kritikus)
</td>
<td style="border:1px solid black;">
[Windows Vista Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=c503c7b1-24f8-40a4-8283-c1e4abf90b57)  
(Kritikus)
</td>
<td style="border:1px solid black;">
[Microsoft .NET-keretrendszer 2.0 Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=aab7826d-539b-4e36-b3a1-afa94b37dbe7)  
(KB2633874)  
(Kritikus)  
[Microsoft .NET Framework 4](http://www.microsoft.com/downloads/details.aspx?familyid=70aadf34-abdc-4577-8da9-a0669dccc119)<sup>[1]</sup>
(KB2633870)  
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
</tr>
<tr>
<td style="border:1px solid black;">
Windows Vista x64 Edition Service Pack 2
</td>
<td style="border:1px solid black;">
[Windows Vista x64 Edition Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=5161d16d-1037-49d5-8d4d-c353288cb41c)  
(Kritikus)
</td>
<td style="border:1px solid black;">
[Internet Explorer 7](http://www.microsoft.com/downloads/details.aspx?familyid=b30a8cc5-b9ad-476f-928c-c49c993d0e80)  
(Kritikus)  
[Internet Explorer 8](http://www.microsoft.com/downloads/details.aspx?familyid=3a8b966a-bf34-42fd-8758-9a5e8e3c7689)  
(Kritikus)  
[Internet Explorer 9](http://www.microsoft.com/downloads/details.aspx?familyid=22cc0245-1877-4c76-914f-dd68f6cd45f0)  
(Kritikus)
</td>
<td style="border:1px solid black;">
[Windows Vista x64 Edition Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=ddbd9fcf-10c4-4089-88c0-c2a6c288222b)  
(Kritikus)
</td>
<td style="border:1px solid black;">
[Microsoft .NET-keretrendszer 2.0 Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=aab7826d-539b-4e36-b3a1-afa94b37dbe7)  
(KB2633874)  
(Kritikus)  
[Microsoft .NET Framework 4](http://www.microsoft.com/downloads/details.aspx?familyid=70aadf34-abdc-4577-8da9-a0669dccc119)<sup>[1]</sup>
(KB2633870)  
(Kritikus)
</td>
<td style="border:1px solid black;">
[Windows Vista x64 Edition Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=73e240a6-2d5e-4ceb-8500-8dacca0e4a43)  
(Fontos)
</td>
<td style="border:1px solid black;">
Nem érintett
</td>
<td style="border:1px solid black;">
Nem érintett
</td>
</tr>
<tr>
<th colspan="8">
Windows Server 2008
</th>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
**Közlemény azonosítója**
</td>
<td style="border:1px solid black;">
[**MS12-008**](http://go.microsoft.com/fwlink/?linkid=238387)
</td>
<td style="border:1px solid black;">
[**MS12-010**](http://go.microsoft.com/fwlink/?linkid=236989)
</td>
<td style="border:1px solid black;">
[**MS12-013**](http://go.microsoft.com/fwlink/?linkid=238617)
</td>
<td style="border:1px solid black;">
[**MS12-016**](http://go.microsoft.com/fwlink/?linkid=235370)
</td>
<td style="border:1px solid black;">
[**MS12-009**](http://go.microsoft.com/fwlink/?linkid=238474)
</td>
<td style="border:1px solid black;">
[**MS12-012**](http://go.microsoft.com/fwlink/?linkid=239941)
</td>
<td style="border:1px solid black;">
[**MS12-014**](http://go.microsoft.com/fwlink/?linkid=239945)
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
[**Mérsékelt**](http://go.microsoft.com/fwlink/?linkid=21140)
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
Nincsenek
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
Windows Server 2008 32 bites rendszerekhez, Service Pack 2
</td>
<td style="border:1px solid black;">
[Windows Server 2008 32 bites rendszerekhez, Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=45c6c511-a4fa-4c3b-af26-6c113f6f5f5e)\*\*\*\*  
(Kritikus)
</td>
<td style="border:1px solid black;">
[Internet Explorer 7](http://www.microsoft.com/downloads/details.aspx?familyid=21f7dba4-fe97-487e-8b37-45914e106db0)\*\*  
(Mérsékelt)  
[Internet Explorer 8](http://www.microsoft.com/downloads/details.aspx?familyid=98d5b024-0eda-4e5d-ba9d-b828ad3d048e)\*\*  
(Mérsékelt)  
[Internet Explorer 9](http://www.microsoft.com/downloads/details.aspx?familyid=025a5af0-39f1-481c-920c-43d2b3d85dc5)\*\*  
(Mérsékelt)
</td>
<td style="border:1px solid black;">
[Windows Server 2008 32 bites rendszerekhez, Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=0c1812af-f57d-455d-a81d-5e03db99b2f7)\*  
(Kritikus)
</td>
<td style="border:1px solid black;">
[Microsoft .NET-keretrendszer 2.0 Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=aab7826d-539b-4e36-b3a1-afa94b37dbe7)  
(KB2633874)  
(Kritikus)  
[Microsoft .NET Framework 4](http://www.microsoft.com/downloads/details.aspx?familyid=70aadf34-abdc-4577-8da9-a0669dccc119)<sup>[1]</sup>
(KB2633870)  
(Kritikus)
</td>
<td style="border:1px solid black;">
Nem érintett
</td>
<td style="border:1px solid black;">
[Windows Server 2008 32 bites rendszerekhez, Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=3f6f89b3-3bc8-4325-b8d8-9a5a398b99c6)\*\*  
(Fontos)
</td>
<td style="border:1px solid black;">
Nem érintett
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Windows Server 2008 x64-alapú rendszerekhez, Service Pack 2
</td>
<td style="border:1px solid black;">
[Windows Server 2008 x64-alapú rendszerekhez, Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=046932cf-0671-49e6-8ddf-98abfc97c5f0)\*\*\*\*  
(Kritikus)
</td>
<td style="border:1px solid black;">
[Internet Explorer 7](http://www.microsoft.com/downloads/details.aspx?familyid=2cd8e296-dae8-41ce-8373-f8a71b4555e9)\*\*  
(Mérsékelt)  
[Internet Explorer 8](http://www.microsoft.com/downloads/details.aspx?familyid=246f9995-fe19-43d0-8f67-0e91eb961bab)\*\*  
(Mérsékelt)  
[Internet Explorer 9](http://www.microsoft.com/downloads/details.aspx?familyid=c216e01d-2f46-4a46-bdc7-9d0fe98193a3)\*\*  
(Mérsékelt)
</td>
<td style="border:1px solid black;">
[Windows Server 2008 x64 alapú rendszerekhez, Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=e1b66bb5-ea12-44a5-807a-f21ede0dc76d)\*  
(Kritikus)
</td>
<td style="border:1px solid black;">
[Microsoft .NET-keretrendszer 2.0 Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=aab7826d-539b-4e36-b3a1-afa94b37dbe7)  
(KB2633874)  
(Kritikus)  
[Microsoft .NET Framework 4](http://www.microsoft.com/downloads/details.aspx?familyid=70aadf34-abdc-4577-8da9-a0669dccc119)<sup>[1]</sup>
(KB2633870)  
(Kritikus)
</td>
<td style="border:1px solid black;">
[Windows Server 2008 x64 alapú rendszerekhez, Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=0e06e77d-7e5d-4d57-98b2-0817f68a1ebb)\*  
(Fontos)
</td>
<td style="border:1px solid black;">
[Windows Server 2008 x64 alapú rendszerekhez, Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=35e6bd04-594f-42ef-97f8-abcf578b4f10)\*\*  
(Fontos)
</td>
<td style="border:1px solid black;">
Nem érintett
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
Windows Server 2008 Itanium-alapú rendszerekhez, Service Pack 2
</td>
<td style="border:1px solid black;">
[Windows Server 2008 Itanium-alapú rendszerekhez, Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=304bd0c5-f4ee-4f8c-89b4-4cbaaf418679)  
(Kritikus)
</td>
<td style="border:1px solid black;">
[Internet Explorer 7](http://www.microsoft.com/downloads/details.aspx?familyid=05c0e6eb-c641-43ab-958a-f43933cdbba7)  
(Mérsékelt)
</td>
<td style="border:1px solid black;">
[Windows Server 2008 Itanium-alapú rendszerekhez, Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=3a96ab34-8f45-48bf-a98b-9e683b50aaa0)  
(Kritikus)
</td>
<td style="border:1px solid black;">
[Microsoft .NET-keretrendszer 2.0 Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=aab7826d-539b-4e36-b3a1-afa94b37dbe7)  
(KB2633874)  
(Kritikus)  
[Microsoft .NET Framework 4](http://www.microsoft.com/downloads/details.aspx?familyid=70aadf34-abdc-4577-8da9-a0669dccc119)<sup>[1]</sup>
(KB2633870)  
(Kritikus)
</td>
<td style="border:1px solid black;">
[Windows Server 2008 Itanium-alapú rendszerekhez, Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=56cbeba9-0c39-4418-9042-7244ac9d03db)  
(Fontos)
</td>
<td style="border:1px solid black;">
[Windows Server 2008 Itanium-alapú rendszerekhez, Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=d1d51b26-2d01-42a9-9bb1-9fb82c1fb914)  
(Fontos)
</td>
<td style="border:1px solid black;">
Nem érintett
</td>
</tr>
<tr>
<th colspan="8">
Windows 7
</th>
</tr>
<tr>
<td style="border:1px solid black;">
**Közlemény azonosítója**
</td>
<td style="border:1px solid black;">
[**MS12-008**](http://go.microsoft.com/fwlink/?linkid=238387)
</td>
<td style="border:1px solid black;">
[**MS12-010**](http://go.microsoft.com/fwlink/?linkid=236989)
</td>
<td style="border:1px solid black;">
[**MS12-013**](http://go.microsoft.com/fwlink/?linkid=238617)
</td>
<td style="border:1px solid black;">
[**MS12-016**](http://go.microsoft.com/fwlink/?linkid=235370)
</td>
<td style="border:1px solid black;">
[**MS12-009**](http://go.microsoft.com/fwlink/?linkid=238474)
</td>
<td style="border:1px solid black;">
[**MS12-012**](http://go.microsoft.com/fwlink/?linkid=239941)
</td>
<td style="border:1px solid black;">
[**MS12-014**](http://go.microsoft.com/fwlink/?linkid=239945)
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
Nincsenek
</td>
<td style="border:1px solid black;">
Nincsenek
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Windows 7 32 bites rendszerekhez és Windows 7 32 bites rendszerekhez Service Pack 1
</td>
<td style="border:1px solid black;">
[Windows 7 32 bites rendszerekhez és Windows 7 32 bites rendszerekhez Service Pack 1](http://www.microsoft.com/downloads/details.aspx?familyid=3e5ca1bf-9415-412c-9dff-dd1abc57e74d)  
(Kritikus)
</td>
<td style="border:1px solid black;">
[Internet Explorer 8](http://www.microsoft.com/downloads/details.aspx?familyid=8b423683-cd29-4049-82d6-f0845842e7f0)  
(Kritikus)  
[Internet Explorer 9](http://www.microsoft.com/downloads/details.aspx?familyid=c83a9c74-a5a7-4b3e-ba36-7a7024d99fd8)  
(Kritikus)
</td>
<td style="border:1px solid black;">
[Windows 7 32 bites rendszerekhez és Windows 7 32 bites rendszerekhez Service Pack 1](http://www.microsoft.com/downloads/details.aspx?familyid=403f355c-2273-42ac-8263-d662f5d7740c)  
(Kritikus)
</td>
<td style="border:1px solid black;">
Csak Windows 7 32 bites rendszerekhez:  
[Microsoft .NET-keretrendszer 3.5.1](http://www.microsoft.com/downloads/details.aspx?familyid=5a5f3ee7-ca49-41c8-aeec-7c76b66712fc)  
(KB2633879)  
(Kritikus)  
Csak Windows 7 32 bites rendszerekhez, Service Pack 1:  
[Microsoft .NET-keretrendszer 3.5.1](http://www.microsoft.com/downloads/details.aspx?familyid=243e8c64-8b6e-4cea-9e99-58d4b1ad35b5)  
(KB2633873)  
(Kritikus)  
[Microsoft .NET Framework 4](http://www.microsoft.com/downloads/details.aspx?familyid=70aadf34-abdc-4577-8da9-a0669dccc119)<sup>[1]</sup>
(KB2633870)  
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
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
Windows 7 x64 alapú rendszerekhez és Windows 7 x64 alapú rendszerekhez Service Pack 1
</td>
<td style="border:1px solid black;">
[Windows 7 x64 alapú rendszerekhez és Windows 7 x64 alapú rendszerekhez Service Pack 1](http://www.microsoft.com/downloads/details.aspx?familyid=78cbbe02-a3d3-4cef-9b54-a3e78c1b885a)  
(Kritikus)
</td>
<td style="border:1px solid black;">
[Internet Explorer 8](http://www.microsoft.com/downloads/details.aspx?familyid=a5d00138-4e24-4a07-92dd-3d8a14476197)  
(Kritikus)  
[Internet Explorer 9](http://www.microsoft.com/downloads/details.aspx?familyid=bbc9d6ae-9ec5-401f-bf16-4811b63709d1)  
(Kritikus)
</td>
<td style="border:1px solid black;">
[Windows 7 x64 alapú rendszerekhez és Windows 7 x64 alapú rendszerekhez Service Pack 1](http://www.microsoft.com/downloads/details.aspx?familyid=8bd8e804-ca4d-4326-bc60-345e2975b7aa)  
(Kritikus)
</td>
<td style="border:1px solid black;">
Csak Windows 7 x64 alapú rendszerekhez:  
[Microsoft .NET-keretrendszer 3.5.1](http://www.microsoft.com/downloads/details.aspx?familyid=5a5f3ee7-ca49-41c8-aeec-7c76b66712fc)  
(KB2633879)  
(Kritikus)  
Csak Windows 7 x64-alapú rendszerekhez, Service Pack 1:  
[Microsoft .NET-keretrendszer 3.5.1](http://www.microsoft.com/downloads/details.aspx?familyid=243e8c64-8b6e-4cea-9e99-58d4b1ad35b5)  
(KB2633873)  
(Kritikus)  
[Microsoft .NET Framework 4](http://www.microsoft.com/downloads/details.aspx?familyid=70aadf34-abdc-4577-8da9-a0669dccc119)<sup>[1]</sup>
(KB2633870)  
(Kritikus)
</td>
<td style="border:1px solid black;">
[Windows 7 x64 alapú rendszerekhez és Windows 7 x64 alapú rendszerekhez Service Pack 1](http://www.microsoft.com/downloads/details.aspx?familyid=299d107d-ab9f-42b6-8f94-a2f1d242c127)  
(Fontos)
</td>
<td style="border:1px solid black;">
Nem érintett
</td>
<td style="border:1px solid black;">
Nem érintett
</td>
</tr>
<tr>
<th colspan="8">
Windows Server 2008 R2
</th>
</tr>
<tr>
<td style="border:1px solid black;">
**Közlemény azonosítója**
</td>
<td style="border:1px solid black;">
[**MS12-008**](http://go.microsoft.com/fwlink/?linkid=238387)
</td>
<td style="border:1px solid black;">
[**MS12-010**](http://go.microsoft.com/fwlink/?linkid=236989)
</td>
<td style="border:1px solid black;">
[**MS12-013**](http://go.microsoft.com/fwlink/?linkid=238617)
</td>
<td style="border:1px solid black;">
[**MS12-016**](http://go.microsoft.com/fwlink/?linkid=235370)
</td>
<td style="border:1px solid black;">
[**MS12-009**](http://go.microsoft.com/fwlink/?linkid=238474)
</td>
<td style="border:1px solid black;">
[**MS12-012**](http://go.microsoft.com/fwlink/?linkid=239941)
</td>
<td style="border:1px solid black;">
[**MS12-014**](http://go.microsoft.com/fwlink/?linkid=239945)
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
[**Mérsékelt**](http://go.microsoft.com/fwlink/?linkid=21140)
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
Nincsenek
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Windows Server 2008 R2 x64 alapú rendszerekhez és Windows Server 2008 R2 x64 alapú rendszerekhez Service Pack 1
</td>
<td style="border:1px solid black;">
[Windows Server 2008 R2 x64 alapú rendszerekhez és Windows Server 2008 R2 x64 alapú rendszerekhez, Service Pack 1](http://www.microsoft.com/downloads/details.aspx?familyid=6b228ad6-d5a4-4b91-8aa8-0874deb22116)\*\*\*\*  
(Kritikus)
</td>
<td style="border:1px solid black;">
[Internet Explorer 8](http://www.microsoft.com/downloads/details.aspx?familyid=3074a898-54bb-44ff-a8f4-77f831c28771)\*\*  
(Mérsékelt)  
[Internet Explorer 9](http://www.microsoft.com/downloads/details.aspx?familyid=1896a6da-f7ee-484b-a97c-455fce7b82b8)\*\*  
(Mérsékelt)
</td>
<td style="border:1px solid black;">
[Windows Server 2008 R2 x64 alapú rendszerekhez és Windows Server 2008 R2 x64 alapú rendszerekhez Service Pack 1](http://www.microsoft.com/downloads/details.aspx?familyid=d868c5ef-165a-46a0-b832-e6ca55a910f9)\*  
(Kritikus)
</td>
<td style="border:1px solid black;">
Csak Windows Server 2008 R2 x64 alapú rendszerekhez:  
[Microsoft .NET Framework 3.5.1](http://www.microsoft.com/downloads/details.aspx?familyid=5a5f3ee7-ca49-41c8-aeec-7c76b66712fc)\*  
(KB2633879)  
(Kritikus)  
Csak Windows Server 2008 R2 x64 alapú rendszerekhez:  
[Microsoft .NET Framework 4](http://www.microsoft.com/downloads/details.aspx?familyid=70aadf34-abdc-4577-8da9-a0669dccc119)<sup>[1]</sup>
(KB2633870)  
(Kritikus)  
Csak Windows Server 2008 R2 x64-alapú rendszerekhez, Service Pack 1:  
[Microsoft .NET Framework 3.5.1](http://www.microsoft.com/downloads/details.aspx?familyid=243e8c64-8b6e-4cea-9e99-58d4b1ad35b5)\*  
(KB2633873)  
(Kritikus)  
[Microsoft .NET Framework 4](http://www.microsoft.com/downloads/details.aspx?familyid=70aadf34-abdc-4577-8da9-a0669dccc119)\*<sup>[1]</sup>
(KB2633870)  
(Kritikus)
</td>
<td style="border:1px solid black;">
[Windows Server 2008 R2 x64 alapú rendszerekhez és Windows Server 2008 R2 x64 alapú rendszerekhez Service Pack 1](http://www.microsoft.com/downloads/details.aspx?familyid=576192d3-f050-4718-a7da-c84fce6bf744)\*  
(Fontos)
</td>
<td style="border:1px solid black;">
[Windows Server 2008 R2 x64 alapú rendszerekhez és Windows Server 2008 R2 x64 alapú rendszerekhez Service Pack 1](http://www.microsoft.com/downloads/details.aspx?familyid=8c51e09b-51c3-4860-836e-6bcffde75f04)\*\*  
(Fontos)
</td>
<td style="border:1px solid black;">
Nem érintett
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
Windows Server 2008 R2 Itanium alapú rendszerekhez és Windows Server 2008 R2 Itanium alapú rendszerekhez Service Pack 1
</td>
<td style="border:1px solid black;">
[Windows Server 2008 R2 Itanium alapú rendszerekhez és Windows Server 2008 R2 Itanium alapú rendszerekhez Service Pack 1](http://www.microsoft.com/downloads/details.aspx?familyid=922b2438-0cfc-49e3-b9a0-52c68b69126a)  
(Kritikus)
</td>
<td style="border:1px solid black;">
[Internet Explorer 8](http://www.microsoft.com/downloads/details.aspx?familyid=7f7c0bc3-fc26-4ee8-aedb-c251247cbeb5)  
(Mérsékelt)
</td>
<td style="border:1px solid black;">
[Windows Server 2008 R2 Itanium alapú rendszerekhez és Windows Server 2008 R2 Itanium alapú rendszerekhez Service Pack 1](http://www.microsoft.com/downloads/details.aspx?familyid=e5416371-495b-4dc7-a239-f9185f968969)  
(Kritikus)
</td>
<td style="border:1px solid black;">
Csak Windows Server 2008 R2 Itanium-alapú rendszerekhez:  
[Microsoft .NET-keretrendszer 3.5.1](http://www.microsoft.com/downloads/details.aspx?familyid=5a5f3ee7-ca49-41c8-aeec-7c76b66712fc)  
(KB2633879)  
(Kritikus)  
Csak Windows Server 2008 R2 Itanium-alapú rendszerekhez, Service Pack 1:  
[Microsoft .NET-keretrendszer 3.5.1](http://www.microsoft.com/downloads/details.aspx?familyid=243e8c64-8b6e-4cea-9e99-58d4b1ad35b5)  
(KB2633873)  
(Kritikus)  
[Microsoft .NET Framework 4](http://www.microsoft.com/downloads/details.aspx?familyid=70aadf34-abdc-4577-8da9-a0669dccc119)<sup>[1]</sup>
(KB2633870)  
(Kritikus)
</td>
<td style="border:1px solid black;">
[Windows Server 2008 R2 Itanium alapú rendszerekhez és Windows Server 2008 R2 Itanium alapú rendszerekhez Service Pack 1](http://www.microsoft.com/downloads/details.aspx?familyid=d6a9b2c9-7582-4953-8ab1-a55c63fcc8dc)  
(Fontos)
</td>
<td style="border:1px solid black;">
[Windows Server 2008 R2 Itanium alapú rendszerekhez és Windows Server 2008 R2 Itanium alapú rendszerekhez Service Pack 1](http://www.microsoft.com/downloads/details.aspx?familyid=fba58a1b-9d9f-4a10-b1df-08a0ebfa2358)  
(Fontos)
</td>
<td style="border:1px solid black;">
Nem érintett
</td>
</tr>
</table>
 
**Megjegyzések a Windows Server 2008 és Windows Server 2008 R2 rendszerhez**

**\*Érinti a kiszolgálómag telepítését.** Ez a frissítés ugyanolyan biztonsági besorolás mellett, a megadottak szerint érvényes az Windows Server 2008 és a Windows Server 2008 R2 összes támogatott kiadására, függetlenül attól, hogy a kiszolgálómag-telepítési opcióval telepítették-e. Erről a telepítési opcióról bővebben a [Kiszolgálómag-telepítés kezelése](http://technet.microsoft.com/en-us/library/ee441255(ws.10).aspx) és [Kiszolgálómag-telepítés szervizelése](http://technet.microsoft.com/en-us/library/ff698994(ws.10).aspx) TechNet cikkekben olvashat. A kiszolgálómag-telepítési opció nem vonatkozik a Windows Server 2008 és a Windows Server 2008 R2 bizonyos kiadásaira; lásd: [A kiszolgálómag-telepítési opciók összehasonlítása](http://www.microsoft.com/windowsserver2008/en/us/compare-core-installation.aspx).

**\*\*A kiszolgálómag-telepítés nem érintett.** A frissítésben tárgyalt biztonsági rések nem érintik a jelzett módon a Windows Server 2008 és a Windows Server 2008 R2 támogatott kiadásait, amennyiben a telepítés a kiszolgálómag-telepítési opció használatával történt. Erről a telepítési opcióról bővebben a [Kiszolgálómag-telepítés kezelése](http://technet.microsoft.com/en-us/library/ee441255(ws.10).aspx) és [Kiszolgálómag-telepítés szervizelése](http://technet.microsoft.com/en-us/library/ff698994(ws.10).aspx) TechNet cikkekben olvashat. A kiszolgálómag-telepítési opció nem vonatkozik a Windows Server 2008 és a Windows Server 2008 R2 bizonyos kiadásaira; lásd: [A kiszolgálómag-telepítési opciók összehasonlítása](http://www.microsoft.com/windowsserver2008/en/us/compare-core-installation.aspx).

**\*\*\*\*Érinti a kiszolgálómag telepítését.** Ez a frissítés alacsonyabb biztonsági besorolás mellett, a megadottak szerint érvényes a Windows Server 2008 és a Windows Server 2008 R2 támogatott kiadásaira, ha azokat a kiszolgálómag-telepítési opcióval telepítették. Erről a telepítési opcióról bővebben a [Kiszolgálómag-telepítés kezelése](http://technet.microsoft.com/en-us/library/ee441255(ws.10).aspx) és [Kiszolgálómag-telepítés szervizelése](http://technet.microsoft.com/en-us/library/ff698994(ws.10).aspx) TechNet cikkekben olvashat. A kiszolgálómag-telepítési opció nem vonatkozik a Windows Server 2008 és a Windows Server 2008 R2 bizonyos kiadásaira; lásd: [A kiszolgálómag-telepítési opciók összehasonlítása](http://www.microsoft.com/windowsserver2008/en/us/compare-core-installation.aspx).

**Megjegyzés azr MS12-010 közleménnyel kapcsolatban**

<sup>[1]</sup>A szóban forgó szoftver frissítésére nem vonatkozik súlyossági besorolás, mert a közleményben taglalt biztonsági réshez tartozó, ismert támadási módszereket az alapértelmezett konfiguráció blokkolja. Mivel a frissítésben mélyreható védelmi módosítások is vannak, a Microsoft azt ajánlja, hogy a szoftver felhasználói telepítsék ezt a biztonsági frissítést.

**Megjegyzés az MS12-016 közleménnyel kapcsolatban**

<sup>[1]</sup>**A .NET Framework 4 verziója és a .NET Framework 4 verziójához tartozó ügyfélprofil.** A .NET-keretrendszer 4-es verziójú terjeszthető csomagjai két profilban érhetőek el: a .NET Framework 4 és a .NET Framework 4 verziójához tartozó ügyfélprofil. A .NET Framework 4 verziójához tartozó ügyfélprofil a .NET Framework 4 részhalmaza. Az ebben a frissítésben tárgyalt biztonsági rés egyaránt érinti a .NET Framework 4 verzióját és a .NET Framework 4 verziójához tartozó ügyfélprofilt is. További információk [A .NET keretrendszer telepítése](http://msdn.microsoft.com/en-us/library/5a4x27ek.aspx) c. MSDN cikkben.

Az ugyanezen a közleményazonosító alatt található, további frissített fájlokat illetően lásd még az egyéb szoftverkategóriák részt ebben a fejezetben, **Érintett szoftverek és letöltési helyek**. Ez a közlemény több szoftverkategóriát ölel fel.

#### Microsoft Office programcsomagok és szoftverek

 
<p> </p>
<table style="border:1px solid black;">
<tr>
<th colspan="2">
Egyéb Microsoft Office szoftver
</th>
</tr>
<tr>
<td style="border:1px solid black;">
**Közlemény azonosítója**
</td>
<td style="border:1px solid black;">
[**MS12-015**](http://go.microsoft.com/fwlink/?linkid=238400)
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
**Összesített súlyossági besorolás**
</td>
<td style="border:1px solid black;">
[**Fontos**](http://go.microsoft.com/fwlink/?linkid=21140)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Microsoft Visio Viewer 2010 és Microsoft Visio Viewer 2010 Service Pack 1 (32 bites kiadás)
</td>
<td style="border:1px solid black;">
[Microsoft Visio Viewer 2010 és Microsoft Visio Viewer 2010 Service Pack 1 (32 bites kiadás)](http://www.microsoft.com/downloads/details.aspx?familyid=173dc4e6-31b4-42ec-808c-f8cd005517ab)  
(KB2597170)  
(Fontos)
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
Microsoft Visio Viewer 2010 és Microsoft Visio Viewer 2010 Service Pack 1 (64 bites kiadás)
</td>
<td style="border:1px solid black;">
[Microsoft Visio Viewer 2010 és Microsoft Visio Viewer 2010 Service Pack 1 (64 bites kiadás)](http://www.microsoft.com/downloads/details.aspx?familyid=34b234e1-1322-4edc-829c-7bc2fbd99338)  
(KB2597170)  
(Fontos)
</td>
</tr>
</table>
 

#### Microsoft Server Software

 
<p> </p>
<table style="border:1px solid black;">
<tr>
<th colspan="2">
Microsoft SharePoint Server
</th>
</tr>
<tr>
<td style="border:1px solid black;">
**Közlemény azonosítója**
</td>
<td style="border:1px solid black;">
[**MS12-011**](http://go.microsoft.com/fwlink/?linkid=238500)
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
**Összesített súlyossági besorolás**
</td>
<td style="border:1px solid black;">
[**Fontos**](http://go.microsoft.com/fwlink/?linkid=21140)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Microsoft SharePoint Server 2010 és Microsoft SharePoint Server 2010 Service Pack 1
</td>
<td style="border:1px solid black;">
[Microsoft SharePoint Server 2010 és Microsoft SharePoint Server 2010 Service Pack 1 (moss)](http://www.microsoft.com/downloads/details.aspx?familyid=44a8eb5a-e469-4d36-b5a0-7e030c1d3244)  
(KB2597124)  
(Fontos)
</td>
</tr>
<tr>
<th colspan="2">
Microsoft SharePoint Foundation
</th>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
**Közlemény azonosítója**
</td>
<td style="border:1px solid black;">
[**MS12-011**](http://go.microsoft.com/fwlink/?linkid=238500)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
**Összesített súlyossági besorolás**
</td>
<td style="border:1px solid black;">
[**Fontos**](http://go.microsoft.com/fwlink/?linkid=21140)
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
Microsoft SharePoint Foundation 2010 és Microsoft SharePoint Foundation 2010 Service Pack 1
</td>
<td style="border:1px solid black;">
[Microsoft SharePoint Foundation 2010 és Microsoft SharePoint Foundation 2010 Service Pack 1 (sts)](http://www.microsoft.com/downloads/details.aspx?familyid=dd348109-953b-4154-b265-85e4694238e6)  
(KB2553413)  
(Fontos)
</td>
</tr>
</table>
 

#### Microsoft fejlesztői eszközök és szoftver

 
<p> </p>
<table style="border:1px solid black;">
<tr>
<th colspan="2">
Microsoft Silverlight
</th>
</tr>
<tr>
<td style="border:1px solid black;">
**Közlemény azonosítója**
</td>
<td style="border:1px solid black;">
[**MS12-016**](http://go.microsoft.com/fwlink/?linkid=235370)
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
**Összesített súlyossági besorolás**
</td>
<td style="border:1px solid black;">
[**Kritikus**](http://go.microsoft.com/fwlink/?linkid=21140)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Microsoft Silverlight 4
</td>
<td style="border:1px solid black;">
Mac számítógépre telepített [Microsoft Silverlight 4](http://www.microsoft.com/downloads/details.aspx?familyid=4c3602f0-9781-4374-8fef-669ddd2c0d40) alkalmazás  
(KB2668562)  
(Kritikus)  
A [Microsoft Silverlight 4](http://www.microsoft.com/downloads/details.aspx?familyid=4c3602f0-9781-4374-8fef-669ddd2c0d40) Microsoft Windows ügyfelek minden támogatott kiadására telepített verziója esetén  
(KB2668562)  
(Kritikus)  
[Microsoft Silverlight 4](http://www.microsoft.com/downloads/details.aspx?familyid=4c3602f0-9781-4374-8fef-669ddd2c0d40)Microsoft Windows ügyfelek minden támogatott kiadására telepített verziója esetén  
(KB2668562)  
(Kritikus)
</td>
</tr>
</table>
 
**Megjegyzés az MS12-016 közleménnyel kapcsolatban**

Az ugyanezen a közleményazonosító alatt található, további frissített fájlokat illetően lásd még az egyéb szoftverkategóriák részt ebben a fejezetben, **Érintett szoftverek és letöltési helyek**. Ez a közlemény több szoftverkategóriát ölel fel.

Észlelési és telepítési eszközök, útmutatás
-------------------------------------------

<span></span>
**Biztonsági központ**

A szoftveres és biztonsági frissítések kezeléséhez azokat a szervezet asztali és hordozható számítógépeire, valamint kiszolgálóira is telepíteni kell. További tájékoztatásért látogasson el a [TechNet Update Management Center](http://go.microsoft.com/fwlink/?linkid=69903) weboldalára. A [TechNet Security Center](http://go.microsoft.com/fwlink/?linkid=21171) bővebb tájékoztatással szolgál a Microsoft termékek biztonsági funkcióival kapcsolatban. A [Biztonság otthon](http://go.microsoft.com/fwlink/?linkid=85102) weboldalon a megfelelő hivatkozásra kattintva elérhetőek a legújabb biztonsági frissítések.

A biztonsági frissítések a [Microsoft Update](http://go.microsoft.com/fwlink/?linkid=40747) és a [Windows Update](http://go.microsoft.com/fwlink/?linkid=21130) weboldalról tölthetők le. A biztonsági frissítések a [Microsoft letöltő központjában](http://go.microsoft.com/fwlink/?linkid=21129) is elérhetőek. Legegyszerűbben a „security update” kifejezésre irányuló kulcsszavas kereséssel találhatja meg ezeket.

A Microsoft Office for Mac felhasználói számára a Microsoft AutoUpdate for Mac szolgáltatás biztosítja a Microsoft szoftverek naprakész állapotát. A Microsoft AutoUpdate for Mac működésének részleteiről lásd: [Szoftverfrissítések automatikus keresése](http://mac2.microsoft.com/help/office/14/en-us/word/item/ffe35357-8f25-4df8-a0a3-c258526c64ea).

A biztonsági frissítések a [Microsoft Update katalógusából](http://go.microsoft.com/fwlink/?linkid=96155) is letölthetőek. A Microsoft Update katalógus a Windows Update és Microsoft Update szolgáltatáson keresztül elérhető tartalom kereshető adatbázisa; ide tartoznak a biztonsági frissítések, illesztőprogramok és szervizcsomagok. A biztonsági közlemény azonosítójára (pl. „MS07-036”) történő kereséssel hozzáadhatja az összes vonatkozó frissítést a kosárhoz (beleértve a frissítés különböző nyelvi változatait), és letöltheti azokat a megadott mappába. A Microsoft Update katalógus részletes leírását lásd a vonatkozó [GYIK](http://go.microsoft.com/fwlink/?linkid=97900)részben.

**Útmutató az észleléshez és a telepítéshez**

A biztonsági frissítésekkel kapcsolatban a Microsoft észlelési és telepítési segítséget nyújt. Ez az útmutató olyan javaslatokat és tudnivalókat tartalmaz, amelyeket segítséget nyújthatnak az informatikusoknak a biztonsági frissítések észlelési és telepítési eszközeinek használatához. További tudnivalókat a [Microsoft Tudásbázis 961747. számú cikkében](http://support.microsoft.com/kb/961747) talál.

**Microsoft Baseline Security Analyzer**

A Microsoft Baseline Security Analyzer (MBSA) segítségével a rendszergazda mind a helyi, mind a távoli számítógépeken ellenőrizheti, hogy mely biztonsági frissítések hiányoznak, illetve hogy mely biztonsági beállítások vannak helytelenül megadva. Ha többet szeretne tudni az MBSA eszközről, látogasson el a [Microsoft Baseline Security Analyzer](http://go.microsoft.com/fwlink/?linkid=21134) webhelyre.

**Windows Server Update Services**

A Microsoft Server Update Services (WSUS) szolgáltatással a rendszergazdák gyorsan és megbízhatóan telepíthetik a legújabb fontos és biztonsági frissítéseket Microsoft Windows 2000 és újabb operációs rendszerekhez, Office XP és újabb operációs rendszerekhez, Exchange Server 2003 és SQL Server 2000 Microsoft Windows 2000 és újabb operációs rendszerekre.

A biztonsági frissítésnek Windows Server Update Services szolgáltatással történő központi telepítéséről a [Windows Server Update Services](http://technet.microsoft.com/en-us/wsus/default.aspx) webhelyen tudhat meg többet.

**System Center Configuration Manager 2007**

A Configuration Manager 2007 szoftverfrissítés-kezelés leegyszerűsíti a frissítéseknek a vállalat minden IT-rendszerére történő eljuttatása és kezelése összetett feladatát. A Configuration Manager 2007 segítségével az IT-rendszergazdák a Microsoft-termékek frissítéseit számos készülékre juttathatják el, köztük asztali számítógépekre, hordozható számítógépekre, kiszolgálókra és mobilkészülékekre.

A Configuration Manager 2007 automatizált biztonságirés-elemzése jelzi a frissítések szükségességét és jelentést küld a javasolt lépésekről. A Configuration Manager 2007 szoftverfrissítés-kezelése a Microsoft Windows Software Update Services (WSUS) szolgáltatására épül, amely az IT-rendszergazdák számára világszerte ismerős, jól bevált frissítési infrastruktúra. Ha többet szeretne tudni arról, hogy a rendszergazdák miként telepíthetik a frissítéseket a Configuration Manager 2007 alkalmazással, lásd a [Szoftverfrissítés-kezelés](http://www.microsoft.com/systemcenter/en/us/configuration-manager/cm-software-update-management.aspx) című részt. A Configuration Manager alkalmazással kapcsolatos bővebb információt lásd: [System Center Configuration Manager](http://www.microsoft.com/systemcenter/en/us/configuration-manager.aspx).

**Systems Management Server 2003**

A Microsoft Systems Management Server (SMS) rendszer egy sokoldalúan beállítható vállalati megoldás, amely a frissítések kezelésére szolgál. Az SMS segítségével a rendszergazda megállapíthatja, hogy melyik Windows alapú számítógép szorul biztonsági frissítésre, és ezeket a frissítéseket szabályozott módon, a felhasználók minimális zavarásával központilag telepítheti a vállalat teljes informatikai környezetében.

**Megjegyzés** A System Management Server 2003 rendszer általános támogatása 2010. január 12-én lejár. Ha többet szeretne tudni a Windows termékek életciklusáról, keresse fel a [Microsoft támogatási életciklusokkal foglalkozó webhelyét](http://support.microsoft.com/common/international.aspx?rdpath=dm;en-us;lifecycle). Az SMS, vagyis a System Center Configuration Manager 2007 újabb kiadása már elérhető, lásd a korábbi, **System Center Configuration Manager 2007** c. részben.

Ha többet szeretne tudni arról, hogy a rendszergazdák miként telepíthetik a biztonsági frissítéseket az SMS 2003 alkalmazással, látogasson el a [Forgatókönyvek és eljárások a Microsoft Systems Management Server 2003 alkalmazáshoz: Szoftverterjesztés és javításkezelés](http://www.microsoft.com/downloads/en/details.aspx?familyid=32f2bb4c-42f8-4b8d-844f-2553fd78049f&displaylang=en) oldalra. Az SMS szolgáltatásról bővebben a [Microsoft Systems Management Server TechCenter](http://technet.microsoft.com/en-us/systemcenter/bb545936.aspx) oldalán olvashat.

**Megjegyzés** Az SMS a Microsoft Baseline Security Analyzer eszközön keresztül széles körű támogatást nyújt a biztonsági közlemények frissítéseinek észleléséhez, valamint a frissítések telepítéséhez. Előfordulhat, hogy egyes szoftverfrissítéseket ezek az eszközök nem észlelnek. Az SMS-alkalmazás leltározási szolgáltatásai segítségével a rendszergazdák adott rendszereken hajthatják végre a frissítést. Az eljárással kapcsolatban olvassa el a [Szoftverfrissítések telepítése az SMS szoftverelosztó ügynök segítségével](http://go.microsoft.com/fwlink/?linkid=33341) című tájékoztatót. Egyes biztonsági frissítésekhez rendszergazdai jogosultságokra van szükség a számítógép újraindítása után. A rendszergazdák az Elevated Rights Deployment Tool eszközt (az [SMS 2003 Administration Feature Pack](http://www.microsoft.com/downloads/en/details.aspx?familyid=7bd3a16e-1899-4e0b-bb99-1320e816167d&displaylang=en) része) alkalmazhatják a frissítések telepítéséhez.

**Az Update Compatibility Evaluator (a frissítéskompatibilitás kiértékelője) és az Application Compatibility Toolkit (alkalmazáskompatibilitási eszközkészlet)**

Az alkalmazások működése érdekében a frissítések gyakran írnak ugyanazokba a fájlokba, illetve regisztrációs bejegyzésekbe. Ez inkompatibilitást okozhat, és növelheti a biztonsági frissítések központi telepítésére használt időt. A Windows frissítések és az alkalmazásoknak való megfelelőség tesztelése és ellenőrzése egyszerűsíthető az [Update Compatibility Evaluator](http://technet2.microsoft.com/windowsvista/en/library/4279e239-37a4-44aa-aec5-4e70fe39f9de1033.mspx?mfr=true) összetevőivel, amelyek az [Application Compatibility Toolkit](http://www.microsoft.com/downloads/details.aspx?familyid=24da89e9-b581-47b0-b45e-492dd6da2971&displaylang=en) alkalmazáskompatibilitási eszközkészletben megtalálhatók.

Az Application Compatibility Toolkit (ACT) tartalmazza a Windows Vista, a Windows Update, a Microsoft Security Update vagy a Windows Internet Explorer új verziójának központi telepítése előtt az alkalmazáskompatibilitási problémák kiértékeléséhez és enyhítéséhez szükséges eszközöket és dokumentációt.

### Egyéb információ

#### A Microsoft Windows rosszindulatú szoftvereket eltávolító eszköze

A Microsoft a Windows Update, Microsoft Update, Windows Server Update Services és Letöltőközpont szolgáltatásán keresztül elérhetővé tette a Microsoft Windows rosszindulatú szoftvereket eltávolító eszközének frissített változatát.

#### Nem biztonsági jellegű frissítések a MU, WU és WSUS-szolgáltatásokban

A Windows Update és a Microsoft Update helyen elérhető, nem biztonsági jellegű frissítésekről tájékozódjon itt:

-   [Microsoft Tudásbázis 894199. cikke](http://support.microsoft.com/kb/894199): Tartalommódosítás a Software Update Services és Windows Server Update Services rendszerek leírásában. Az összes Windows-tartalmat érinti.
-   [Az elmúlt hónapok frissítései Windows Server Frissítési szolgáltatások esetén](http://technet.microsoft.com/en-us/wsus/bb456965.aspx). Microsoft termékek új, módosított és újra kiadott frissítései, a Microsoft Windows rendszert kivéve.

#### Microsoft Active Protections Program (MAPP)

Az ügyfelek védelmének növelése érdekében a biztonsági szoftverekkel foglalkozó nagyobb gyártók a Microsoft a havi biztonsági közlemények megjelenése előtt ellátja biztonsági résekkel kapcsolatos információkkal. Így a biztonságiszoftver-gyártók a kapott biztonsági résekkel kapcsolatos információt felhasználhatják ügyfeleik hatásosabb védelmére az olyan biztonsági szoftverek vagy eszközök (például víruskeresők, hálózati behatolásérzékelő rendszerek vagy kiszolgálóalapú behatolásvédelmi rendszerek) frissítése által. A biztonságiszoftver-gyártók által kiadott aktív védelem elérhetőségéről a [Microsoft Active Protections Program (MAPP) Partners](http://go.microsoft.com/fwlink/?linkid=215201) webhelyén található listán szereplő és a programban részt vevő gyártók aktív védelmi webhelyein tájékozódhat.

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

-   Tarjei Mandt, [Azimuth Security](http://www.azimuthsecurity.com/), az MS12-008 közleményben leírt probléma jelentéséért
-   Tarjei Mandt, [Azimuth Security](http://www.azimuthsecurity.com/), az MS12-009 közleményben leírt két probléma jelentéséért
-   [Jan Schejbal](http://janschejbal.wordpress.com/) az MS12-010 közleményben leírt probléma jelentéséért
-   Stephen Fewer, [Harmony Security](http://www.harmonysecurity.com/), a [TippingPoint](http://www.tippingpoint.com/)[Zero Day Initiative](http://www.zerodayinitiative.com/) programjával együttműködve, az MS12-010 közleményben ismertetett két probléma jelentéséért
-   Jason Hullinger, [HP Cloud Services](http://www.hpcloud.com/), az MS12-010 közleményben leírt probléma jelentéséért
-   John Hollenberger, az MS12-011 közleményben leírt probléma jelentéséért
-   Rocco Calvi, stratsec, az MS12-011 közleményben leírt probléma jelentéséért
-   Giorgio Fedon, Minded Security, az MS12-011 közleményben ismertetett probléma miatti mélyreható védelmi módosítások kialakításában való közreműködésért
-   Alexander Gavrun, a [TippingPoint's](http://www.tippingpoint.com/)[Zero Day Initiative](http://www.zerodayinitiative.com/) programjával együttműködve, az MS12-013 közleményben leírt probléma jelentéséért
-   Xin Ouyang, [Palo Alto Networks](http://www.paloaltonetworks.com/), az MS12-015 közleményben ismertetett öt probléma jelentéséért
-   Jeroen Frijters, [Sumatra](http://www.sumatra.nl/), az MS12-016 közleményben ismertetett probléma jelentéséért

#### Terméktámogatás

-   Teszteléssel állapították meg a felsorolt szoftverek egyes verzióinak érintettségét. A többi verzió támogatási életciklusa végére ért. Az egyes szoftververziók támogatási életciklusáról a [Microsoft termékek terméktámogatási életciklusát ismertető webhelyen](http://go.microsoft.com/fwlink/?linkid=21742) talál felvilágosítást.
-   Az Amerikai Egyesült Államokban és Kanada területén élő ügyfelek technikai támogatást kérhetnek a [biztonsági támogatás szolgáltatójától](http://go.microsoft.com/fwlink/?linkid=21131) vagy az 1-866-PCSAFETY (1-866-727-2338) telefonszámon. A biztonsági frissítésekkel kapcsolatos hívások ingyenesek. Az elérhető támogatási lehetőségekről további információt talál a [Microsoft segítségnyújtással és támogatással foglalkozó webhelyén](http://support.microsoft.com/).
-   Más országokban a helyi Microsoft-képviseletek nyújtanak támogatást. A biztonsági frissítésekkel kapcsolatos hívások ingyenesek. A [nemzetközi támogatási webhely](http://go.microsoft.com/fwlink/?linkid=21155) felvilágosítást nyújt arról, támogatási kérdéseivel hogyan fordulhat a Microsofthoz.

#### Felelősséget kizáró nyilatkozat

A Microsoft Tudásbázisban leírtak előzetes bejelentés nélkül változhatnak, és a cikkek tartalmáért a Microsoft nem vállal garanciát. A Microsoft egyben elhárít minden kifejezett és értelemszerű garanciát, beleértve az eladhatóságra és az adott célra való alkalmasságra vonatkozó garanciát is. A Microsoft Corporation vagy annak szállítói semmilyen körülmények között nem tehetők felelőssé közvetlen, közvetett, eseti, ok-okozati vagy különleges kárért (beleértve az elmaradt hasznot is), még akkor sem, ha a Microsoft Corporation vagy szállítói tudatában voltak a kár lehetséges voltának. Egyes államok törvényi szabályozása nem teszi lehetővé a véletlen vagy ok-okozati károkért vállalt felelősség korlátozását vagy kizárását, így ezekben az államokban az ez a felelősségkizárás nincs érvényben.

#### Verziók

-   1.0 verzió (2012. február 14.): Összefoglaló közlemény közzététele.

*Built at 2014-04-18T01:50:00Z-07:00*
