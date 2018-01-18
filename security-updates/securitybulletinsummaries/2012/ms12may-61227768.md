---
TOCTitle: 'MS12-MAY'
Title: 'A Microsoft biztonsági közleményei - összefoglalás, 2012. május'
ms:assetid: 'ms12-may'
ms:contentKeyID: 61227768
ms:mtpsurl: 'https://technet.microsoft.com/hu-HU/library/ms12-may(v=Security.10)'
---

Security Bulletin Summary

A Microsoft biztonsági közleményei - összefoglalás, 2012. május
===============================================================

Közzétéve: 2012. május 8. | Frissítve: 2012. május 22.

**Verzió:** 2.1

Az összefoglaló a 2012 áprilisában kiadott biztonsági közleményeket összegzi.

A 2012. májusi biztonsági közlemények kiadása folytán az összefoglaló a 2012. május 3-án kiadott előzetes értesítés helyébe lép. További információk a biztonsági közlemények kiadásáról szóló előzetes értesítés szolgáltatásról lásd: [Előzetes értesítés a Microsoft biztonsági közleményeinek kiadásáról](http://go.microsoft.com/fwlink/?linkid=217213).

Ha automatikus értesítést szeretne kapni a Microsoft biztonsági közleményeinek megjelenéséről, fizessen elő a [Microsoft Technical Security Notifications](http://go.microsoft.com/fwlink/?linkid=21163) szolgáltatásra.

A közleményekkel kapcsolatos kérdések megválaszolására a Microsoft 2012. május 9-én, csendes-óceáni idő szerint 11 órakor webes szemináriumot tart. Jelentkezzen most a [májusi közleményeket bemutató webes szemináriumra](https://msevents.microsoft.com/cui/eventdetail.aspx?eventid=1032499667). Ezt követően a webes szeminárium igény szerint kerül megrendezésre. További információkért látogasson el a [Microsoft biztonsági közleményeit és a webes szemináriumokat](http://go.microsoft.com/fwlink/?linkid=217214) bemutató oldalra.

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
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=248419"><strong>MS12-029</strong></a></td>
<td style="border:1px solid black;"><strong>A Microsoft Word biztonsági rése távoli kódfuttatást tehet lehetővé (2680352)</strong><br />
<br />
A biztonsági frissítés a Microsoft Office közvetlenül jelentett biztonsági rését szünteti meg. A biztonsági rés távoli kódvégrehajtást tehet lehetővé, ha a felhasználó megnyit egy speciálisan kialakított RTF fájlt. A biztonsági rést sikeresen kihasználó támadó az aktuális felhasználóéval megegyező felhasználói jogokat nyerhet. A kevesebb jogosultsággal bíró fiókkal rendelkező felhasználók esetében kisebb a veszélyeztetettség, mint a rendszergazdai jogosultságokkal rendelkezők esetén</td>
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=21140">Kritikus</a><br />
Távoli kódfuttatás</td>
<td style="border:1px solid black;">Esetleg újra kell indítani a rendszert</td>
<td style="border:1px solid black;">Microsoft Office</td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=251038"><strong>MS12-034</strong></a></td>
<td style="border:1px solid black;"><strong>Összesített biztonsági frissítés a Microsoft Office, Windows, .NET-keretrendszer és Silverlight szoftverekhez (2681578)</strong><br />
<br />
A biztonsági frissítés a Microsoft Office, a Microsoft Windows, a Microsoft .NET-keretrendszer és a Microsoft Silverlight három nyilvánosságra került és hét közvetlenül jelentett biztonsági rését szünteti meg. A súlyosabb besorolású biztonsági rések távoli kódfuttatást tesznek lehetővé, ha a felhasználó különlegesen kialakított dokumentumot nyit meg, vagy TrueType betűkészletfájlt tartalmazó káros weboldalra látogat. A támadónak nincs lehetősége arra, hogy a felhasználót a rosszindulatú kódot tartalmazó webhely megnyitására kényszerítse. Csupán megkísérelheti rávenni a felhasználókat arra, hogy kattintsanak az e-mailben vagy azonnali üzenetben megjelenő hivatkozásra, amelyen keresztül a támadó weboldalára jutnak.</td>
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=21140">Kritikus</a><br />
Távoli kódfuttatás</td>
<td style="border:1px solid black;">Esetleg újra kell indítani a rendszert</td>
<td style="border:1px solid black;">Microsoft Windows, Microsoft .NET-keretrendszer, Microsoft Silverlight,<br />
Microsoft Office</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=246970"><strong>MS12-035</strong></a></td>
<td style="border:1px solid black;"><strong>A .NET Framework biztonsági rése programkód távolról történő végrehajtására adhat lehetőséget (2693777)</strong><br />
<br />
Ez a biztonsági frissítés a .NET-keretrendszer két közvetlenül jelzett biztonsági rését szünteti meg. A biztonsági rések távoli kódfuttatást tehetnek lehetővé az ügyfélrendszereken, ha a felhasználó különlegesen kialakított weboldalt tekint meg az XAML böngészőalkalmazások (XBAP alkalmazások) futtatására alkalmas böngészőben. A kevesebb jogosultsággal bíró fiókkal rendelkező felhasználók esetében kisebb a veszélyeztetettség, mint a rendszergazdai jogosultságokkal rendelkezők esetén</td>
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=21140">Kritikus</a><br />
Távoli kódfuttatás</td>
<td style="border:1px solid black;">Esetleg újra kell indítani a rendszert</td>
<td style="border:1px solid black;">Microsoft Windows, Microsoft .NET Framework</td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=238499"><strong>MS12-030</strong></a></td>
<td style="border:1px solid black;"><strong>A Microsoft</strong> <strong>Office</strong> <strong>biztonsági rései távolról történő programkódfuttatást tehetnek lehetővé (2663830)</strong><br />
<br />
Ez a biztonsági frissítés egy nyilvánosságra került és öt közvetlenül jelentett biztonsági rést szüntet meg a Microsoft Office alkalmazásban. A biztonsági rések távoli kódvégrehajtást tehetnek lehetővé, amennyiben a felhasználó speciálisan kialakított Office fájlt nyit meg. A biztonsági réseket sikeresen kihasználó támadó a bejelentkezett felhasználóval egyező hozzáférést nyer a rendszerhez. A kevesebb jogosultsággal bíró fiókkal rendelkező felhasználók esetében kisebb a veszélyeztetettség, mint a rendszergazdai jogosultságokkal rendelkezők esetén</td>
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=21140">Fontos</a><br />
Távoli kódfuttatás</td>
<td style="border:1px solid black;">Esetleg újra kell indítani a rendszert</td>
<td style="border:1px solid black;">Microsoft Office</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=248385"><strong>MS12-031</strong></a></td>
<td style="border:1px solid black;"><strong>A Microsoft Visio Viewer 2010 biztonsági rése távolról történő programkódfuttatást tehet lehetővé (2597981)</strong><br />
<br />
A biztonsági frissítés a Microsoft Office közvetlenül jelentett biztonsági rését szünteti meg. A biztonsági rés távoli kódvégrehajtást tehet lehetővé, ha a felhasználó megnyit egy speciálisan kialakított Visio fájlt. A biztonsági rést sikeresen kihasználó támadó az aktuális felhasználóéval megegyező felhasználói jogokat nyerhet. A kevesebb jogosultsággal bíró fiókkal rendelkező felhasználók esetében kisebb a veszélyeztetettség, mint a rendszergazdai jogosultságokkal rendelkezők esetén</td>
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=21140">Fontos</a><br />
Távoli kódfuttatás</td>
<td style="border:1px solid black;">Esetleg újra kell indítani a rendszert</td>
<td style="border:1px solid black;">Microsoft Office</td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=246964"><strong>MS12-032</strong></a></td>
<td style="border:1px solid black;"><strong>A TCP/IP biztonsági rése jogok kiterjesztését teheti lehetővé (2688338)</strong><br />
<br />
Ez a biztonsági frissítés egy közvetlenül jelentett és egy nyilvánosságra került biztonsági rést szüntet meg a Microsoft Windows rendszerben. A súlyosabb biztonsági rés jogok kiterjesztését teheti lehetővé, ha a támadó bejelentkezik a rendszerre, és ott speciálisan kialakított alkalmazást futtat.</td>
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=21140">Fontos</a><br />
Jogok kiterjesztése</td>
<td style="border:1px solid black;">Újraindítást igényel</td>
<td style="border:1px solid black;">Microsoft Windows</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=247902"><strong>MS12-033</strong></a></td>
<td style="border:1px solid black;"><strong>A Windows Partíciókezelő biztonsági rése jogok kiterjesztését teheti lehetővé (2690533)</strong><br />
<br />
A biztonsági frissítés a Microsoft Windows közvetlenül jelentett biztonsági rését szünteti meg. A biztonsági rés jogok kiterjesztését teheti lehetővé, ha a támadó bejelentkezik a rendszerre, és ott speciálisan kialakított alkalmazást futtat. A támadónak a biztonsági rés kihasználásához érvényes bejelentkezési adatokkal kell rendelkeznie, és képesnek kell lennie helyileg bejelentkezni a rendszerbe.</td>
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=21140">Fontos</a><br />
Jogok kiterjesztése</td>
<td style="border:1px solid black;">Újraindítást igényel</td>
<td style="border:1px solid black;">Microsoft Windows</td>
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

 
<p> </p>
<table style="border:1px solid black;">
<thead>
<tr class="header">
<th style="border:1px solid black;" >Közlemény azonosítója</th>
<th style="border:1px solid black;" >A biztonsági rés címe</th>
<th style="border:1px solid black;" >CVE-azonosító</th>
<th style="border:1px solid black;" >Kihasználhatóság felmérése a legújabb szoftvereknél</th>
<th style="border:1px solid black;" >Kihasználhatóság felmérése a korábbi szoftvereknél</th>
<th style="border:1px solid black;" >Szolgáltatásmegtagadás kihasználhatóságának felmérése</th>
<th style="border:1px solid black;" >Fontos megjegyzések</th>
</tr>
</thead>
<tbody>
<tr class="odd">
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=248419"><strong>MS12-029</strong></a></td>
<td style="border:1px solid black;">RTF eltérés biztonsági rés</td>
<td style="border:1px solid black;"><a href="http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2012-0183">CVE-2012-0183</a></td>
<td style="border:1px solid black;">Nem érintett</td>
<td style="border:1px solid black;"><a href="http://technet.microsoft.com/en-us/security/cc998259.aspx">1</a> - Konzisztens rosszindulatú programkódról van szó</td>
<td style="border:1px solid black;">Nem érintett</td>
<td style="border:1px solid black;">(Nincs)</td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=238499"><strong>MS12-030</strong></a></td>
<td style="border:1px solid black;">Excel fájlformátum memóriameghibásodás miatti biztonsági rése</td>
<td style="border:1px solid black;"><a href="http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2012-0141">CVE-2012-0141</a></td>
<td style="border:1px solid black;"><a href="http://technet.microsoft.com/en-us/security/cc998259.aspx">3</a> - Nem valószínű rosszindulatú programkód</td>
<td style="border:1px solid black;"><a href="http://technet.microsoft.com/en-us/security/cc998259.aspx">3</a> - Nem valószínű rosszindulatú programkód</td>
<td style="border:1px solid black;">Nem érintett</td>
<td style="border:1px solid black;">(Nincs)</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=238499"><strong>MS12-030</strong></a></td>
<td style="border:1px solid black;">Excel fájlformátum OBJECTLINK bejegyzésben lévő memóriameghibásodás miatti biztonsági rés</td>
<td style="border:1px solid black;"><a href="http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2012-0142">CVE-2012-0142</a></td>
<td style="border:1px solid black;"><a href="http://technet.microsoft.com/en-us/security/cc998259.aspx">3</a> - Nem valószínű rosszindulatú programkód</td>
<td style="border:1px solid black;"><a href="http://technet.microsoft.com/en-us/security/cc998259.aspx">3</a> - Nem valószínű rosszindulatú programkód</td>
<td style="border:1px solid black;">Nem érintett</td>
<td style="border:1px solid black;">(Nincs)</td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=238499"><strong>MS12-030</strong></a></td>
<td style="border:1px solid black;">Különböző módosított bájtokat használó Excel memóriameghibásodás miatti biztonsági rés</td>
<td style="border:1px solid black;"><a href="http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2012-0143">CVE-2012-0143</a></td>
<td style="border:1px solid black;">Nem érintett</td>
<td style="border:1px solid black;"><a href="http://technet.microsoft.com/en-us/security/cc998259.aspx">1</a> - Konzisztens rosszindulatú programkódról van szó</td>
<td style="border:1px solid black;">Nem érintett</td>
<td style="border:1px solid black;">Csak a Microsoft Office 2003 szoftvert érinti<br />
<br />
A biztonsági rés nyilvánosságra került,</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=238499"><strong>MS12-030</strong></a></td>
<td style="border:1px solid black;">Az SXLI bejegyzés miatti memóriameghibásodást okozó biztonsági rése</td>
<td style="border:1px solid black;"><a href="http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2012-0184">CVE-2012-0184</a></td>
<td style="border:1px solid black;"><a href="http://technet.microsoft.com/en-us/security/cc998259.aspx">3</a> - Nem valószínű rosszindulatú programkód</td>
<td style="border:1px solid black;"><a href="http://technet.microsoft.com/en-us/security/cc998259.aspx">1</a> - Konzisztens rosszindulatú programkódról van szó</td>
<td style="border:1px solid black;">Nem érintett</td>
<td style="border:1px solid black;">(Nincs)</td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=238499"><strong>MS12-030</strong></a></td>
<td style="border:1px solid black;">Excel MergeCells bejegyzés halomtúlcsordulást okozó biztonsági rése</td>
<td style="border:1px solid black;"><a href="http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2012-0185">CVE-2012-0185</a></td>
<td style="border:1px solid black;"><a href="http://technet.microsoft.com/en-us/security/cc998259.aspx">2</a> - A kihasználáshoz szükséges kód nehezen szerkeszthető</td>
<td style="border:1px solid black;"><a href="http://technet.microsoft.com/en-us/security/cc998259.aspx">2</a> - A kihasználáshoz szükséges kód nehezen szerkeszthető</td>
<td style="border:1px solid black;">Nem érintett</td>
<td style="border:1px solid black;">(Nincs)</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=238499"><strong>MS12-030</strong></a></td>
<td style="border:1px solid black;">Excel sorozat bejegyzéselemzési típustévesztése biztonsági rés</td>
<td style="border:1px solid black;"><a href="http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2012-1847">CVE-2012-1847</a></td>
<td style="border:1px solid black;"><a href="http://technet.microsoft.com/en-us/security/cc998259.aspx">1</a> - Konzisztens rosszindulatú programkódról van szó</td>
<td style="border:1px solid black;"><a href="http://technet.microsoft.com/en-us/security/cc998259.aspx">1</a> - Konzisztens rosszindulatú programkódról van szó</td>
<td style="border:1px solid black;">Nem érintett</td>
<td style="border:1px solid black;">(Nincs)</td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=248385"><strong>MS12-031</strong></a></td>
<td style="border:1px solid black;">VSD fájlformátum memóriameghibásodás miatti biztonsági rése</td>
<td style="border:1px solid black;"><a href="http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2012-0018">CVE-2012-0018</a></td>
<td style="border:1px solid black;"><a href="http://technet.microsoft.com/en-us/security/cc998259.aspx">1</a> - Konzisztens rosszindulatú programkódról van szó</td>
<td style="border:1px solid black;">Nem érintett</td>
<td style="border:1px solid black;">Nem érintett</td>
<td style="border:1px solid black;">Ez a Visio Viewer 2010 és Visio Viewer 2010 Service Pack 1 alkalmazást érinti (csak a Visio Viewer támogatott változatait).</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=246964"><strong>MS12-032</strong></a></td>
<td style="border:1px solid black;">Windows tűzfal megkerülési biztonsági rése</td>
<td style="border:1px solid black;"><a href="http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2012-0174">CVE-2012-0174</a></td>
<td style="border:1px solid black;">Nem érintett</td>
<td style="border:1px solid black;">Nem érintett</td>
<td style="border:1px solid black;">Nem érintett</td>
<td style="border:1px solid black;">A biztonsági rés biztonsági funkció megkerülésére adhat lehetőséget.</td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=246964"><strong>MS12-032</strong></a></td>
<td style="border:1px solid black;">TCP/IP kétszeres felszabadítási biztonsági rése</td>
<td style="border:1px solid black;"><a href="http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2012-0179">CVE-2012-0179</a></td>
<td style="border:1px solid black;"><a href="http://technet.microsoft.com/en-us/security/cc998259.aspx">1</a> - Konzisztens rosszindulatú programkódról van szó</td>
<td style="border:1px solid black;">Nem érintett</td>
<td style="border:1px solid black;">Állandó</td>
<td style="border:1px solid black;">A biztonsági rés nyilvánosságra került,</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=247902"><strong>MS12-033</strong></a></td>
<td style="border:1px solid black;">Plug and Play (PnP) Konfigurációkezelő biztonsági rése</td>
<td style="border:1px solid black;"><a href="http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2012-0178">CVE-2012-0178</a></td>
<td style="border:1px solid black;"><a href="http://technet.microsoft.com/en-us/security/cc998259.aspx">1</a> - Konzisztens rosszindulatú programkódról van szó</td>
<td style="border:1px solid black;"><a href="http://technet.microsoft.com/en-us/security/cc998259.aspx">1</a> - Konzisztens rosszindulatú programkódról van szó</td>
<td style="border:1px solid black;">Ideiglenes</td>
<td style="border:1px solid black;">(Nincs)</td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=251038"><strong>MS12-034</strong></a></td>
<td style="border:1px solid black;">TrueType betűtípus-elemzés biztonsági rése</td>
<td style="border:1px solid black;"><a href="http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2011-3402">CVE-2011-3402</a></td>
<td style="border:1px solid black;"><a href="http://technet.microsoft.com/en-us/security/cc998259.aspx">1</a> - Konzisztens rosszindulatú programkódról van szó</td>
<td style="border:1px solid black;"><a href="http://technet.microsoft.com/en-us/security/cc998259.aspx">1</a> - Konzisztens rosszindulatú programkódról van szó</td>
<td style="border:1px solid black;">Állandó</td>
<td style="border:1px solid black;">A biztonsági rés nyilvánosságra került,</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=251038"><strong>MS12-034</strong></a></td>
<td style="border:1px solid black;">TrueType betűtípus-elemzés biztonsági rése</td>
<td style="border:1px solid black;"><a href="http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2012-0159">CVE-2012-0159</a></td>
<td style="border:1px solid black;"><a href="http://technet.microsoft.com/en-us/security/cc998259.aspx">1</a> - Konzisztens rosszindulatú programkódról van szó</td>
<td style="border:1px solid black;"><a href="http://technet.microsoft.com/en-us/security/cc998259.aspx">1</a> - Konzisztens rosszindulatú programkódról van szó</td>
<td style="border:1px solid black;">Állandó</td>
<td style="border:1px solid black;">(Nincs)</td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=251038"><strong>MS12-034</strong></a></td>
<td style="border:1px solid black;">.NET-keretrendszer pufferfoglalás miatti biztonsági rése</td>
<td style="border:1px solid black;"><a href="http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2012-0162">CVE-2012-0162</a></td>
<td style="border:1px solid black;"><a href="http://technet.microsoft.com/en-us/security/cc998259.aspx">1</a> - Konzisztens rosszindulatú programkódról van szó</td>
<td style="border:1px solid black;">Nem érintett</td>
<td style="border:1px solid black;">Nem érintett</td>
<td style="border:1px solid black;">(Nincs)</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=251038"><strong>MS12-034</strong></a></td>
<td style="border:1px solid black;">GDI+ bejegyzéstípus miatti biztonsági rése</td>
<td style="border:1px solid black;"><a href="http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2012-0165">CVE-2012-0165</a></td>
<td style="border:1px solid black;"><a href="http://technet.microsoft.com/en-us/security/cc998259.aspx">2</a> - A kihasználáshoz szükséges kód nehezen szerkeszthető</td>
<td style="border:1px solid black;"><a href="http://technet.microsoft.com/en-us/security/cc998259.aspx">1</a> - Konzisztens rosszindulatú programkódról van szó</td>
<td style="border:1px solid black;">Nem érintett</td>
<td style="border:1px solid black;">(Nincs)</td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=251038"><strong>MS12-034</strong></a></td>
<td style="border:1px solid black;">GDI+ halomtúlcsordulást okozó biztonsági rése</td>
<td style="border:1px solid black;"><a href="http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2012-0167">CVE-2012-0167</a></td>
<td style="border:1px solid black;">Nem érintett</td>
<td style="border:1px solid black;"><a href="http://technet.microsoft.com/en-us/security/cc998259.aspx">1</a> - Konzisztens rosszindulatú programkódról van szó</td>
<td style="border:1px solid black;">Nem érintett</td>
<td style="border:1px solid black;">(Nincs)</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=251038"><strong>MS12-034</strong></a></td>
<td style="border:1px solid black;">Silverlight kétszeres felszabadítási biztonsági rése</td>
<td style="border:1px solid black;"><a href="http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2012-0176">CVE-2012-0176</a></td>
<td style="border:1px solid black;">Nem érintett</td>
<td style="border:1px solid black;"><a href="http://technet.microsoft.com/en-us/security/cc998259.aspx">1</a> - Konzisztens rosszindulatú programkódról van szó</td>
<td style="border:1px solid black;">Nem érintett</td>
<td style="border:1px solid black;">(Nincs)</td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=251038"><strong>MS12-034</strong></a></td>
<td style="border:1px solid black;">Ablakok és üzenetek biztonsági rése</td>
<td style="border:1px solid black;"><a href="http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2012-0180">CVE-2012-0180</a></td>
<td style="border:1px solid black;"><a href="http://technet.microsoft.com/en-us/security/cc998259.aspx">1</a> - Konzisztens rosszindulatú programkódról van szó</td>
<td style="border:1px solid black;"><a href="http://technet.microsoft.com/en-us/security/cc998259.aspx">1</a> - Konzisztens rosszindulatú programkódról van szó</td>
<td style="border:1px solid black;">Állandó</td>
<td style="border:1px solid black;">(Nincs)</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=251038"><strong>MS12-034</strong></a></td>
<td style="border:1px solid black;">Billentyűzetkiosztás-fájlok biztonsági rése</td>
<td style="border:1px solid black;"><a href="http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2012-0181">CVE-2012-0181</a></td>
<td style="border:1px solid black;"><a href="http://technet.microsoft.com/en-us/security/cc998259.aspx">3</a> - Nem valószínű rosszindulatú programkód</td>
<td style="border:1px solid black;"><a href="http://technet.microsoft.com/en-us/security/cc998259.aspx">1</a> - Konzisztens rosszindulatú programkódról van szó</td>
<td style="border:1px solid black;">Állandó</td>
<td style="border:1px solid black;">A biztonsági rés nyilvánosságra került,</td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=251038"><strong>MS12-034</strong></a></td>
<td style="border:1px solid black;">Görgetősáv-számítás biztonsági rése</td>
<td style="border:1px solid black;"><a href="http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2012-1848">CVE-2012-1848</a></td>
<td style="border:1px solid black;"><a href="http://technet.microsoft.com/en-us/security/cc998259.aspx">1</a> - Konzisztens rosszindulatú programkódról van szó</td>
<td style="border:1px solid black;"><a href="http://technet.microsoft.com/en-us/security/cc998259.aspx">1</a> - Konzisztens rosszindulatú programkódról van szó</td>
<td style="border:1px solid black;">Állandó</td>
<td style="border:1px solid black;">(Nincs)</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=246970"><strong>MS12-035</strong></a></td>
<td style="border:1px solid black;">.NET-keretrendszer szerializációs biztonsági rése</td>
<td style="border:1px solid black;"><a href="http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2012-0160">CVE-2012-0160</a></td>
<td style="border:1px solid black;"><a href="http://technet.microsoft.com/en-us/security/cc998259.aspx">1</a> - Konzisztens rosszindulatú programkódról van szó</td>
<td style="border:1px solid black;"><a href="http://technet.microsoft.com/en-us/security/cc998259.aspx">1</a> - Konzisztens rosszindulatú programkódról van szó</td>
<td style="border:1px solid black;">Nem érintett</td>
<td style="border:1px solid black;">(Nincs)</td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=246970"><strong>MS12-035</strong></a></td>
<td style="border:1px solid black;">.NET-keretrendszer szerializációs biztonsági rése</td>
<td style="border:1px solid black;"><a href="http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2012-0161">CVE-2012-0161</a></td>
<td style="border:1px solid black;"><a href="http://technet.microsoft.com/en-us/security/cc998259.aspx">1</a> - Konzisztens rosszindulatú programkódról van szó</td>
<td style="border:1px solid black;"><a href="http://technet.microsoft.com/en-us/security/cc998259.aspx">1</a> - Konzisztens rosszindulatú programkódról van szó</td>
<td style="border:1px solid black;">Nem érintett</td>
<td style="border:1px solid black;">(Nincs)</td>
</tr>
</tbody>
</table>
  
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
<th colspan="5">
Windows XP  
</th>
</tr>
<tr>
<td style="border:1px solid black;">
**Közlemény azonosítója**
</td>
<td style="border:1px solid black;">
[**MS12-034**](http://go.microsoft.com/fwlink/?linkid=251038)
</td>
<td style="border:1px solid black;">
[**MS12-035**](http://go.microsoft.com/fwlink/?linkid=246970)
</td>
<td style="border:1px solid black;">
[**MS12-032**](http://go.microsoft.com/fwlink/?linkid=246964)
</td>
<td style="border:1px solid black;">
[**MS12-033**](http://go.microsoft.com/fwlink/?linkid=247902)
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
Nincsenek
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Windows XP Service Pack 3
</td>
<td style="border:1px solid black;">
[Windows XP Service Pack 3](http://www.microsoft.com/downloads/details.aspx?familyid=b2ea7a8d-a537-441c-8e80-2ba4ac37e320)  
(KB2660649)  
(Csak a Tablet PC Edition 2005 Service Pack 3)  
(Fontos)  
[Windows XP Service Pack 3](http://www.microsoft.com/downloads/details.aspx?familyid=9a4db1b4-15b2-4fae-83c4-a86331425c9e)  
(KB2659262)  
(Fontos)  
[Windows XP Service Pack 3](http://www.microsoft.com/downloads/details.aspx?familyid=8d341077-8fcd-4666-a27e-2141a04a321e)  
(KB2676562)  
(Kritikus)  
[Windows XP Service Pack 3](http://www.microsoft.com/downloads/details.aspx?familyid=954e8ae9-9247-496a-bbde-76981c49e3b3)  
(KB2686509)  
(Fontos)  
[Microsoft .NET-keretrendszer 3.0 Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=c9bf7fde-3b6f-44fe-93b3-8a4dc01c1cc5)  
(KB2656407)  
(Nincs súlyossági besorolás<sup>[2]</sup>)  
[Microsoft .NET Framework 4](http://www.microsoft.com/downloads/details.aspx?familyid=4ee3cb61-542e-4e42-aa0e-0cbf8dd89648)<sup>[1]</sup>
(KB2656405)  
(Kritikus)
</td>
<td style="border:1px solid black;">
[Microsoft .NET-keretrendszer 1.0 Service Pack 3](http://www.microsoft.com/downloads/details.aspx?familyid=b0803633-7fda-4862-a908-3450180cdaaa)  
(KB2604042)  
(Csak Media Center Edition 2005 Service Pack 3 és Tablet PC Edition 2005 Service Pack 3)  
(Kritikus)  
[Microsoft .NET-keretrendszer 1.1 Service Pack 1](http://www.microsoft.com/downloads/details.aspx?familyid=88501ecb-dcf6-4956-8eab-e1076a975846)  
(KB2656353)  
(Kritikus)  
[Microsoft .NET-keretrendszer 2.0 Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=cb5afeaf-a500-4b71-a91b-a300884b040e)  
(KB2604092)  
(Kritikus)  
[Microsoft .NET-keretrendszer 3.0 Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=18a66b7c-f062-4236-8340-a867b1e31b78)  
(KB2604110)  
(Kritikus)  
[Microsoft .NET-keretrendszer 3.5 Service Pack 1](http://www.microsoft.com/downloads/details.aspx?familyid=d6f0ccd6-c8ec-45a0-beba-155989ca19b3)  
(KB2604111)  
(Kritikus)  
[Microsoft .NET Framework 4](http://www.microsoft.com/downloads/details.aspx?familyid=38b389d8-d534-4b0a-8dd4-b72a5ce7c4e8)<sup>[1]</sup>
(KB2604121)  
(Kritikus)
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
Windows XP Professional x64 Edition Service Pack 2
</td>
<td style="border:1px solid black;">
[Windows XP Professional x64 Edition Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=6ebaccbc-512b-4f2f-bf2a-8958f012e13f)  
(KB2659262)  
(Fontos)  
[Windows XP Professional x64 Edition Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=e0357165-4400-40a6-a7a4-7b762a1793ba)  
(KB2676562)  
(Kritikus)  
[Windows XP Professional x64 Edition Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=f3b1568f-d7ad-4e6e-b45b-53b16b303d9d)  
(KB2686509)  
(Fontos)  
[Microsoft .NET-keretrendszer 3.0 Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=c9bf7fde-3b6f-44fe-93b3-8a4dc01c1cc5)  
(KB2656407)  
(Nincs súlyossági besorolás<sup>[2]</sup>)  
[Microsoft .NET Framework 4](http://www.microsoft.com/downloads/details.aspx?familyid=4ee3cb61-542e-4e42-aa0e-0cbf8dd89648)<sup>[1]</sup>
(KB2656405)  
(Kritikus)
</td>
<td style="border:1px solid black;">
[Microsoft .NET-keretrendszer 1.1 Service Pack 1](http://www.microsoft.com/downloads/details.aspx?familyid=88501ecb-dcf6-4956-8eab-e1076a975846)  
(KB2656353)  
(Kritikus)  
[Microsoft .NET-keretrendszer 2.0 Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=cb5afeaf-a500-4b71-a91b-a300884b040e)  
(KB2604092)  
(Kritikus)  
[Microsoft .NET-keretrendszer 3.0 Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=18a66b7c-f062-4236-8340-a867b1e31b78)  
(KB2604110)  
(Kritikus)  
[Microsoft .NET-keretrendszer 3.5 Service Pack 1](http://www.microsoft.com/downloads/details.aspx?familyid=d6f0ccd6-c8ec-45a0-beba-155989ca19b3)  
(KB2604111)  
(Kritikus)  
[Microsoft .NET Framework 4](http://www.microsoft.com/downloads/details.aspx?familyid=38b389d8-d534-4b0a-8dd4-b72a5ce7c4e8)<sup>[1]</sup>
(KB2604121)  
(Kritikus)
</td>
<td style="border:1px solid black;">
Nem érintett
</td>
<td style="border:1px solid black;">
Nem érintett
</td>
</tr>
<tr>
<th colspan="5">
Windows Server 2003
</th>
</tr>
<tr>
<td style="border:1px solid black;">
**Közlemény azonosítója**
</td>
<td style="border:1px solid black;">
[**MS12-034**](http://go.microsoft.com/fwlink/?linkid=251038)
</td>
<td style="border:1px solid black;">
[**MS12-035**](http://go.microsoft.com/fwlink/?linkid=246970)
</td>
<td style="border:1px solid black;">
[**MS12-032**](http://go.microsoft.com/fwlink/?linkid=246964)
</td>
<td style="border:1px solid black;">
[**MS12-033**](http://go.microsoft.com/fwlink/?linkid=247902)
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
[**Kritikus**](http://go.microsoft.com/fwlink/?linkid=21140)
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
[Windows Server 2003 Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=bc7bfb79-8eaf-4c22-b1c9-e774c55eb06d)  
(KB2659262)  
(Fontos)  
[Windows Server 2003 Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=6287b994-041f-45b7-a230-d689bf1901a8)  
(KB2676562)  
(Kritikus)  
[Windows Server 2003 Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=167e8c49-f9f6-488b-86ad-4056d3d20213)  
(KB2686509)  
(Fontos)  
[Microsoft .NET-keretrendszer 3.0 Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=c9bf7fde-3b6f-44fe-93b3-8a4dc01c1cc5)  
(KB2656407)  
(Nincs súlyossági besorolás<sup>[2]</sup>)  
[Microsoft .NET Framework 4](http://www.microsoft.com/downloads/details.aspx?familyid=4ee3cb61-542e-4e42-aa0e-0cbf8dd89648)<sup>[1]</sup>
(KB2656405)  
(Kritikus)
</td>
<td style="border:1px solid black;">
[Microsoft .NET-keretrendszer 1.1 Service Pack 1](http://www.microsoft.com/downloads/details.aspx?familyid=b0df42a4-7444-4da6-a9b2-35a56bdc64a4)  
(KB2604078)  
(Kritikus)  
[Microsoft .NET-keretrendszer 2.0 Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=cb5afeaf-a500-4b71-a91b-a300884b040e)  
(KB2604092)  
(Kritikus)  
[Microsoft .NET-keretrendszer 3.0 Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=18a66b7c-f062-4236-8340-a867b1e31b78)  
(KB2604110)  
(Kritikus)  
[Microsoft .NET-keretrendszer 3.5 Service Pack 1](http://www.microsoft.com/downloads/details.aspx?familyid=d6f0ccd6-c8ec-45a0-beba-155989ca19b3)  
(KB2604111)  
(Kritikus)  
[Microsoft .NET Framework 4](http://www.microsoft.com/downloads/details.aspx?familyid=38b389d8-d534-4b0a-8dd4-b72a5ce7c4e8)<sup>[1]</sup>
(KB2604121)  
(Kritikus)
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
[Windows Server 2003 x64 Edition Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=bf7c9aea-dc18-499f-b456-2c29e9a74a15)  
(KB2659262)  
(Fontos)  
[Windows Server 2003 x64 Edition Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=f9f49cd0-24db-4438-afde-aa7113ec2035)  
(KB2676562)  
(Kritikus)  
[Windows Server 2003 x64 Edition Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=4614161c-ae05-43ad-8dd3-85975ec2bc4c)  
(KB2686509)  
(Fontos)  
[Microsoft .NET-keretrendszer 3.0 Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=c9bf7fde-3b6f-44fe-93b3-8a4dc01c1cc5)  
(KB2656407)  
(Nincs súlyossági besorolás<sup>[2]</sup>)  
[Microsoft .NET Framework 4](http://www.microsoft.com/downloads/details.aspx?familyid=4ee3cb61-542e-4e42-aa0e-0cbf8dd89648)<sup>[1]</sup>
(KB2656405)  
(Kritikus)
</td>
<td style="border:1px solid black;">
[Microsoft .NET-keretrendszer 1.1 Service Pack 1](http://www.microsoft.com/downloads/details.aspx?familyid=88501ecb-dcf6-4956-8eab-e1076a975846)  
(KB2656353)  
(Kritikus)  
[Microsoft .NET-keretrendszer 2.0 Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=cb5afeaf-a500-4b71-a91b-a300884b040e)  
(KB2604092)  
(Kritikus)  
[Microsoft .NET-keretrendszer 3.0 Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=18a66b7c-f062-4236-8340-a867b1e31b78)  
(KB2604110)  
(Kritikus)  
[Microsoft .NET-keretrendszer 3.5 Service Pack 1](http://www.microsoft.com/downloads/details.aspx?familyid=d6f0ccd6-c8ec-45a0-beba-155989ca19b3)  
(KB2604111)  
(Kritikus)  
[Microsoft .NET Framework 4](http://www.microsoft.com/downloads/details.aspx?familyid=38b389d8-d534-4b0a-8dd4-b72a5ce7c4e8)<sup>[1]</sup>
(KB2604121)  
(Kritikus)
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
[Windows Server 2003 SP2 Itanium-alapú rendszerekhez](http://www.microsoft.com/downloads/details.aspx?familyid=6414b607-6fb1-4527-b218-c3cb5adfd4d1)  
(KB2659262)  
(Fontos)  
[Windows Server 2003 SP2 Itanium-alapú rendszerekhez](http://www.microsoft.com/downloads/details.aspx?familyid=2563425d-4f6e-4f33-b775-a8d421b0e254)  
(KB2676562)  
(Kritikus)  
[Windows Server 2003 SP2 Itanium-alapú rendszerekhez](http://www.microsoft.com/downloads/details.aspx?familyid=67f659ee-0d28-40f3-ae2f-f8fceeac8bff)  
(KB2686509)  
(Fontos)
</td>
<td style="border:1px solid black;">
[Microsoft .NET-keretrendszer 1.1 Service Pack 1](http://www.microsoft.com/downloads/details.aspx?familyid=88501ecb-dcf6-4956-8eab-e1076a975846)  
(KB2656353)  
(Kritikus)  
[Microsoft .NET-keretrendszer 2.0 Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=cb5afeaf-a500-4b71-a91b-a300884b040e)  
(KB2604092)  
(Kritikus)  
[Microsoft .NET-keretrendszer 3.5 Service Pack 1](http://www.microsoft.com/downloads/details.aspx?familyid=d6f0ccd6-c8ec-45a0-beba-155989ca19b3)  
(KB2604111)  
(Kritikus)  
[Microsoft .NET Framework 4](http://www.microsoft.com/downloads/details.aspx?familyid=38b389d8-d534-4b0a-8dd4-b72a5ce7c4e8)<sup>[1]</sup>
(KB2604121)  
(Kritikus)
</td>
<td style="border:1px solid black;">
Nem érintett
</td>
<td style="border:1px solid black;">
Nem érintett
</td>
</tr>
<tr>
<th colspan="5">
Windows Vista
</th>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
**Közlemény azonosítója**
</td>
<td style="border:1px solid black;">
[**MS12-034**](http://go.microsoft.com/fwlink/?linkid=251038)
</td>
<td style="border:1px solid black;">
[**MS12-035**](http://go.microsoft.com/fwlink/?linkid=246970)
</td>
<td style="border:1px solid black;">
[**MS12-032**](http://go.microsoft.com/fwlink/?linkid=246964)
</td>
<td style="border:1px solid black;">
[**MS12-033**](http://go.microsoft.com/fwlink/?linkid=247902)
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
[**Fontos**](http://go.microsoft.com/fwlink/?linkid=21140)
</td>
<td style="border:1px solid black;">
[**Fontos**](http://go.microsoft.com/fwlink/?linkid=21140)
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
Windows Vista Service Pack 2
</td>
<td style="border:1px solid black;">
[Windows Vista Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=e11d8738-379a-4dfe-b21c-495041d9523a)  
(KB2658846)  
(Fontos)  
[Windows Vista Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=d8068e95-ac4d-45e8-84b7-b12d633c70b5)  
(KB2659262)  
(Fontos)  
[Windows Vista Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=02c857c6-5dfa-46fb-adef-35eac2bf5f41)  
(KB2660649)  
(Fontos)  
[Windows Vista Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=292d1f3b-a065-4d7d-9046-f35ab7f0591b)  
(KB2676562)  
(Kritikus)  
[Microsoft .NET-keretrendszer 3.0 Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=0511303a-79f6-4bd9-8f50-b5836c9c476f)  
(KB2656409)  
(Nincs súlyossági besorolás<sup>[2]</sup>)  
[Microsoft .NET Framework 4](http://www.microsoft.com/downloads/details.aspx?familyid=4ee3cb61-542e-4e42-aa0e-0cbf8dd89648)<sup>[1]</sup>
(KB2656405)  
(Kritikus)
</td>
<td style="border:1px solid black;">
[Microsoft .NET-keretrendszer 1.1 Service Pack 1](http://www.microsoft.com/downloads/details.aspx?familyid=88501ecb-dcf6-4956-8eab-e1076a975846)  
(KB2656353)  
(Kritikus)  
[Microsoft .NET-keretrendszer 2.0 Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=8b504a01-1e6b-42c0-b974-811350302ace)  
(KB2604094)  
(Kritikus)  
[Microsoft .NET-keretrendszer 3.0 Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=06273728-7f22-40db-be11-8fb03e7e0bfb)  
(KB2604105)  
(Kritikus)  
[Microsoft .NET-keretrendszer 3.5 Service Pack 1](http://www.microsoft.com/downloads/details.aspx?familyid=d6f0ccd6-c8ec-45a0-beba-155989ca19b3)  
(KB2604111)  
(Kritikus)  
[Microsoft .NET Framework 4](http://www.microsoft.com/downloads/details.aspx?familyid=38b389d8-d534-4b0a-8dd4-b72a5ce7c4e8)<sup>[1]</sup>
(KB2604121)  
(Kritikus)
</td>
<td style="border:1px solid black;">
[Windows Vista Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=b1dc6e10-34eb-45ea-92b3-9983c00f6cb5)  
(KB2688338)  
(Fontos)
</td>
<td style="border:1px solid black;">
[Windows Vista Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=d9d5e290-dc57-4587-b31d-706b541924ec)  
(KB2690533)  
(Fontos)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Windows Vista x64 Edition Service Pack 2
</td>
<td style="border:1px solid black;">
[Windows Vista x64 Edition Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=838f588b-2a0d-4dae-b54d-782e6985fd83)  
(KB2658846)  
(Fontos)  
[Windows Vista x64 Edition Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=3bde7f59-163c-4491-abc9-a822daa8142f)  
(KB2659262)  
(Fontos)  
[Windows Vista x64 Edition Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=9f97c5a4-62ee-4e4f-8811-a43545d76327)  
(KB2660649)  
(Fontos)  
[Windows Vista x64 Edition Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=8f90c09c-a2cb-4adb-ace7-a8bc38d78ba6)  
(KB2676562)  
(Kritikus)  
[Microsoft .NET-keretrendszer 3.0 Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=0511303a-79f6-4bd9-8f50-b5836c9c476f)  
(KB2656409)  
(Nincs súlyossági besorolás<sup>[2]</sup>)  
[Microsoft .NET Framework 4](http://www.microsoft.com/downloads/details.aspx?familyid=4ee3cb61-542e-4e42-aa0e-0cbf8dd89648)<sup>[1]</sup>
(KB2656405)  
(Kritikus)
</td>
<td style="border:1px solid black;">
[Microsoft .NET-keretrendszer 1.1 Service Pack 1](http://www.microsoft.com/downloads/details.aspx?familyid=88501ecb-dcf6-4956-8eab-e1076a975846)  
(KB2656353)  
(Kritikus)  
[Microsoft .NET-keretrendszer 2.0 Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=8b504a01-1e6b-42c0-b974-811350302ace)  
(KB2604094)  
(Kritikus)  
[Microsoft .NET-keretrendszer 3.0 Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=06273728-7f22-40db-be11-8fb03e7e0bfb)  
(KB2604105)  
(Kritikus)  
[Microsoft .NET-keretrendszer 3.5 Service Pack 1](http://www.microsoft.com/downloads/details.aspx?familyid=d6f0ccd6-c8ec-45a0-beba-155989ca19b3)  
(KB2604111)  
(Kritikus)  
[Microsoft .NET Framework 4](http://www.microsoft.com/downloads/details.aspx?familyid=38b389d8-d534-4b0a-8dd4-b72a5ce7c4e8)<sup>[1]</sup>
(KB2604121)  
(Kritikus)
</td>
<td style="border:1px solid black;">
[Windows Vista x64 Edition Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=d65565d4-d865-438a-bfb7-d71af9dd884e)  
(KB2688338)  
(Fontos)
</td>
<td style="border:1px solid black;">
[Windows Vista x64 Edition Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=827b9f15-b67d-4dd4-a39b-7c148bae5041)  
(KB2690533)  
(Fontos)
</td>
</tr>
<tr>
<th colspan="5">
Windows Server 2008
</th>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
**Közlemény azonosítója**
</td>
<td style="border:1px solid black;">
[**MS12-034**](http://go.microsoft.com/fwlink/?linkid=251038)
</td>
<td style="border:1px solid black;">
[**MS12-035**](http://go.microsoft.com/fwlink/?linkid=246970)
</td>
<td style="border:1px solid black;">
[**MS12-032**](http://go.microsoft.com/fwlink/?linkid=246964)
</td>
<td style="border:1px solid black;">
[**MS12-033**](http://go.microsoft.com/fwlink/?linkid=247902)
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
[**Fontos**](http://go.microsoft.com/fwlink/?linkid=21140)
</td>
<td style="border:1px solid black;">
[**Fontos**](http://go.microsoft.com/fwlink/?linkid=21140)
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
Windows Server 2008 32 bites rendszerekhez, Service Pack 2
</td>
<td style="border:1px solid black;">
[Windows Server 2008 32 bites rendszerekhez, Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=360adbed-a451-44ed-8675-ca5624ef1cf3)  
(KB2658846)  
(Fontos)  
[Windows Server 2008 32 bites rendszerekhez, Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=47a0df29-f42e-463b-9c15-a93385ff8705)  
(KB2659262)  
(Fontos)  
[Windows Server 2008 32 bites rendszerekhez, Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=278c378b-6ee4-4f80-b9c3-ede885f4bbda)<sup>[3]</sup>
(KB2660649)  
(Fontos)  
[Windows Server 2008 32 bites rendszerekhez, Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=728a84b9-c1b8-46e2-8365-1b542963508a)  
(KB2676562)  
(Kritikus)  
[Microsoft .NET-keretrendszer 3.0 Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=0511303a-79f6-4bd9-8f50-b5836c9c476f)  
(KB2656409)  
(Nincs súlyossági besorolás<sup>[2]</sup>)  
[Microsoft .NET Framework 4](http://www.microsoft.com/downloads/details.aspx?familyid=4ee3cb61-542e-4e42-aa0e-0cbf8dd89648)<sup>[1]</sup>
(KB2656405)  
(Kritikus)
</td>
<td style="border:1px solid black;">
[Microsoft .NET-keretrendszer 1.1 Service Pack 1](http://www.microsoft.com/downloads/details.aspx?familyid=88501ecb-dcf6-4956-8eab-e1076a975846)  
(KB2656353)  
(Kritikus)  
[Microsoft .NET-keretrendszer 2.0 Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=8b504a01-1e6b-42c0-b974-811350302ace)  
(KB2604094)  
(Kritikus)  
[Microsoft .NET-keretrendszer 3.0 Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=06273728-7f22-40db-be11-8fb03e7e0bfb)  
(KB2604105)  
(Kritikus)  
[Microsoft .NET-keretrendszer 3.5 Service Pack 1](http://www.microsoft.com/downloads/details.aspx?familyid=d6f0ccd6-c8ec-45a0-beba-155989ca19b3)  
(KB2604111)  
(Kritikus)  
[Microsoft .NET Framework 4](http://www.microsoft.com/downloads/details.aspx?familyid=38b389d8-d534-4b0a-8dd4-b72a5ce7c4e8)<sup>[1]</sup>
(KB2604121)  
(Kritikus)
</td>
<td style="border:1px solid black;">
[Windows Server 2008 32 bites rendszerekhez, Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=7ef72aab-7fd2-4330-bb6a-0c77c3943345)  
(KB2688338)  
(Fontos)
</td>
<td style="border:1px solid black;">
[Windows Server 2008 32 bites rendszerekhez, Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=46e6e960-b700-4154-b91d-aca74ea9e5df)  
(KB2690533)  
(Fontos)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Windows Server 2008 x64-alapú rendszerekhez, Service Pack 2
</td>
<td style="border:1px solid black;">
[Windows Server 2008 x64-alapú rendszerekhez, Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=d5a6d617-8ef6-42fa-a325-c15fa7ece7aa)  
(KB2658846)  
(Fontos)  
[Windows Server 2008 x64-alapú rendszerekhez, Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=4e6d29e1-17fc-4670-9e69-988c040f06e2)  
(KB2659262)  
(Fontos)  
[Windows Server 2008 x64 alapú rendszerekhez, Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=98c4ac87-eec2-4e02-b0e1-00626bcb0ffd)<sup>[3]</sup>
(KB2660649)  
(Fontos)  
[Windows Server 2008 x64-alapú rendszerekhez, Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=ab897da8-a927-42eb-87da-1e5cd820f4c0)  
(KB2676562)  
(Kritikus)  
[Microsoft .NET-keretrendszer 3.0 Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=0511303a-79f6-4bd9-8f50-b5836c9c476f)  
(KB2656409)  
(Nincs súlyossági besorolás<sup>[2]</sup>)  
[Microsoft .NET Framework 4](http://www.microsoft.com/downloads/details.aspx?familyid=4ee3cb61-542e-4e42-aa0e-0cbf8dd89648)<sup>[1]</sup>
(KB2656405)  
(Kritikus)
</td>
<td style="border:1px solid black;">
[Microsoft .NET-keretrendszer 1.1 Service Pack 1](http://www.microsoft.com/downloads/details.aspx?familyid=88501ecb-dcf6-4956-8eab-e1076a975846)  
(KB2656353)  
(Kritikus)  
[Microsoft .NET-keretrendszer 2.0 Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=8b504a01-1e6b-42c0-b974-811350302ace)  
(KB2604094)  
(Kritikus)  
[Microsoft .NET-keretrendszer 3.0 Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=06273728-7f22-40db-be11-8fb03e7e0bfb)  
(KB2604105)  
(Kritikus)  
[Microsoft .NET-keretrendszer 3.5 Service Pack 1](http://www.microsoft.com/downloads/details.aspx?familyid=d6f0ccd6-c8ec-45a0-beba-155989ca19b3)  
(KB2604111)  
(Kritikus)  
[Microsoft .NET Framework 4](http://www.microsoft.com/downloads/details.aspx?familyid=38b389d8-d534-4b0a-8dd4-b72a5ce7c4e8)<sup>[1]</sup>
(KB2604121)  
(Kritikus)
</td>
<td style="border:1px solid black;">
[Windows Server 2008 x64-alapú rendszerekhez, Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=9569d980-766d-4825-bd1c-f30c93d4b035)  
(KB2688338)  
(Fontos)
</td>
<td style="border:1px solid black;">
[Windows Server 2008 x64-alapú rendszerekhez, Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=e4ab05ae-3a1c-4d6b-8c84-1165ed741356)  
(KB2690533)  
(Fontos)
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
Windows Server 2008 Itanium-alapú rendszerekhez, Service Pack 2
</td>
<td style="border:1px solid black;">
[Windows Server 2008 Itanium-alapú rendszerekhez, Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=c65df271-8b7d-46d3-81b3-87c0ad05e8d0)  
(KB2659262)  
(Fontos)  
[Windows Server 2008 Itanium-alapú rendszerekhez, Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=11da5031-1733-43ea-9204-294eb483c858)  
(KB2676562)  
(Kritikus)
</td>
<td style="border:1px solid black;">
[Microsoft .NET-keretrendszer 1.1 Service Pack 1](http://www.microsoft.com/downloads/details.aspx?familyid=88501ecb-dcf6-4956-8eab-e1076a975846)  
(KB2656353)  
(Kritikus)  
[Microsoft .NET-keretrendszer 2.0 Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=8b504a01-1e6b-42c0-b974-811350302ace)  
(KB2604094)  
(Kritikus)  
[Microsoft .NET-keretrendszer 3.5 Service Pack 1](http://www.microsoft.com/downloads/details.aspx?familyid=d6f0ccd6-c8ec-45a0-beba-155989ca19b3)  
(KB2604111)  
(Kritikus)  
[Microsoft .NET Framework 4](http://www.microsoft.com/downloads/details.aspx?familyid=38b389d8-d534-4b0a-8dd4-b72a5ce7c4e8)<sup>[1]</sup>
(KB2604121)  
(Kritikus)
</td>
<td style="border:1px solid black;">
[Windows Server 2008 Itanium-alapú rendszerekhez, Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=c5f7ee25-2fc1-44c7-b3e6-e2c969ecf1bc)  
(KB2688338)  
(Fontos)
</td>
<td style="border:1px solid black;">
[Windows Server 2008 Itanium-alapú rendszerekhez, Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=c081b058-b95e-4467-a2fc-fb1a68345c8f)  
(KB2690533)  
(Fontos)
</td>
</tr>
<tr>
<th colspan="5">
Windows 7
</th>
</tr>
<tr>
<td style="border:1px solid black;">
**Közlemény azonosítója**
</td>
<td style="border:1px solid black;">
[**MS12-034**](http://go.microsoft.com/fwlink/?linkid=251038)
</td>
<td style="border:1px solid black;">
[**MS12-035**](http://go.microsoft.com/fwlink/?linkid=246970)
</td>
<td style="border:1px solid black;">
[**MS12-032**](http://go.microsoft.com/fwlink/?linkid=246964)
</td>
<td style="border:1px solid black;">
[**MS12-033**](http://go.microsoft.com/fwlink/?linkid=247902)
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
[**Fontos**](http://go.microsoft.com/fwlink/?linkid=21140)
</td>
<td style="border:1px solid black;">
[**Fontos**](http://go.microsoft.com/fwlink/?linkid=21140)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Windows 7 32 bites rendszerekhez
</td>
<td style="border:1px solid black;">
[Windows 7 32 bites rendszerekhez](http://www.microsoft.com/downloads/details.aspx?familyid=f4d52649-4afc-4c01-b275-93818152f6b7)  
(KB2658846)  
(Fontos)  
[Windows 7 32 bites rendszerekhez](http://www.microsoft.com/downloads/details.aspx?familyid=31607fd8-fae8-47a0-971e-0e68be67fb5a)  
(KB2659262)  
(Fontos)  
[Windows 7 32 bites rendszerekhez](http://www.microsoft.com/downloads/details.aspx?familyid=35443cfc-0f51-412a-a9d9-91bfb19d805e)  
(KB2660649)  
(Fontos)  
[Windows 7 32 bites rendszerekhez](http://www.microsoft.com/downloads/details.aspx?familyid=572af8d4-effb-41a6-8448-7576b03f18fd)  
(KB2676562)  
(Kritikus)  
[Microsoft .NET-keretrendszer 3.5.1](http://www.microsoft.com/downloads/details.aspx?familyid=d04bfc77-d05f-4890-9175-27ad00e84c4a)  
(KB2656410)  
(Nincs súlyossági besorolás<sup>[2]</sup>)  
[Microsoft .NET Framework 4](http://www.microsoft.com/downloads/details.aspx?familyid=4ee3cb61-542e-4e42-aa0e-0cbf8dd89648)<sup>[1]</sup>
(KB2656405)  
(Kritikus)
</td>
<td style="border:1px solid black;">
[Microsoft .NET-keretrendszer 3.5.1](http://www.microsoft.com/downloads/details.aspx?familyid=cd42511f-788c-4473-84cc-19bb1623e337)  
(KB2604114)  
(Kritikus)  
[Microsoft .NET Framework 4](http://www.microsoft.com/downloads/details.aspx?familyid=38b389d8-d534-4b0a-8dd4-b72a5ce7c4e8)<sup>[1]</sup>
(KB2604121)  
(Kritikus)
</td>
<td style="border:1px solid black;">
[Windows 7 32 bites rendszerekhez](http://www.microsoft.com/downloads/details.aspx?familyid=46b8749e-3d8f-472f-a1ea-419f44c6bc00)  
(KB2688338)  
(Fontos)
</td>
<td style="border:1px solid black;">
[Windows 7 32 bites rendszerekhez](http://www.microsoft.com/downloads/details.aspx?familyid=2a4433e4-7f3f-4083-b3e1-eff2d18483af)  
(KB2690533)  
(Fontos)
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
Windows 7 32 bites rendszerekhez, Service Pack 1
</td>
<td style="border:1px solid black;">
[Windows 7 32 bites rendszerekhez, Service Pack 1](http://www.microsoft.com/downloads/details.aspx?familyid=f4d52649-4afc-4c01-b275-93818152f6b7)  
(KB2658846)  
(Fontos)  
[Windows 7 32 bites rendszerekhez, Service Pack 1](http://www.microsoft.com/downloads/details.aspx?familyid=31607fd8-fae8-47a0-971e-0e68be67fb5a)  
(KB2659262)  
(Fontos)  
[Windows 7 32 bites rendszerekhez, Service Pack 1](http://www.microsoft.com/downloads/details.aspx?familyid=35443cfc-0f51-412a-a9d9-91bfb19d805e)  
(KB2660649)  
(Fontos)  
[Windows 7 32 bites rendszerekhez, Service Pack 1](http://www.microsoft.com/downloads/details.aspx?familyid=572af8d4-effb-41a6-8448-7576b03f18fd)  
(KB2676562)  
(Kritikus)  
[Microsoft .NET-keretrendszer 3.5.1](http://www.microsoft.com/downloads/details.aspx?familyid=c06506e6-5838-4bba-9b12-b54dfa30a944)  
(KB2656411)  
(Nincs súlyossági besorolás<sup>[2]</sup>)  
[Microsoft .NET Framework 4](http://www.microsoft.com/downloads/details.aspx?familyid=4ee3cb61-542e-4e42-aa0e-0cbf8dd89648)<sup>[1]</sup>
(KB2656405)  
(Kritikus)
</td>
<td style="border:1px solid black;">
[Microsoft .NET-keretrendszer 3.5.1](http://www.microsoft.com/downloads/details.aspx?familyid=85e0f8be-cdc7-464b-be43-da23d82b3486)  
(KB2604115)  
(Kritikus)  
[Microsoft .NET Framework 4](http://www.microsoft.com/downloads/details.aspx?familyid=38b389d8-d534-4b0a-8dd4-b72a5ce7c4e8)<sup>[1]</sup>
(KB2604121)  
(Kritikus)
</td>
<td style="border:1px solid black;">
[Windows 7 32 bites rendszerekhez, Service Pack 1](http://www.microsoft.com/downloads/details.aspx?familyid=46b8749e-3d8f-472f-a1ea-419f44c6bc00)  
(KB2688338)  
(Fontos)
</td>
<td style="border:1px solid black;">
[Windows 7 32 bites rendszerekhez, Service Pack 1](http://www.microsoft.com/downloads/details.aspx?familyid=2a4433e4-7f3f-4083-b3e1-eff2d18483af)  
(KB2690533)  
(Fontos)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Windows 7 x64-alapú rendszerekhez
</td>
<td style="border:1px solid black;">
[Windows 7 x64-alapú rendszerekhez](http://www.microsoft.com/downloads/details.aspx?familyid=7aa0b61b-b42c-4d60-8a7f-c61cbd25d6d9)  
(KB2658846)  
(Fontos)  
[Windows 7 x64-alapú rendszerekhez](http://www.microsoft.com/downloads/details.aspx?familyid=fa38b001-eef8-4153-b077-ea524e8a1e18)  
(KB2659262)  
(Fontos)  
[Windows 7 x64-alapú rendszerekhez](http://www.microsoft.com/downloads/details.aspx?familyid=7e551e0f-3f02-49ee-a5a1-8a7480722a6b)  
(KB2660649)  
(Fontos)  
[Windows 7 x64-alapú rendszerekhez](http://www.microsoft.com/downloads/details.aspx?familyid=c09cbb73-7814-4946-8c0a-323d304dd633)  
(KB2676562)  
(Kritikus)  
[Microsoft .NET-keretrendszer 3.5.1](http://www.microsoft.com/downloads/details.aspx?familyid=d04bfc77-d05f-4890-9175-27ad00e84c4a)  
(KB2656410)  
(Nincs súlyossági besorolás<sup>[2]</sup>)  
[Microsoft .NET Framework 4](http://www.microsoft.com/downloads/details.aspx?familyid=4ee3cb61-542e-4e42-aa0e-0cbf8dd89648)<sup>[1]</sup>
(KB2656405)  
(Kritikus)
</td>
<td style="border:1px solid black;">
[Microsoft .NET-keretrendszer 3.5.1](http://www.microsoft.com/downloads/details.aspx?familyid=cd42511f-788c-4473-84cc-19bb1623e337)  
(KB2604114)  
(Kritikus)  
[Microsoft .NET Framework 4](http://www.microsoft.com/downloads/details.aspx?familyid=38b389d8-d534-4b0a-8dd4-b72a5ce7c4e8)<sup>[1]</sup>
(KB2604121)  
(Kritikus)
</td>
<td style="border:1px solid black;">
[Windows 7 x64-alapú rendszerekhez](http://www.microsoft.com/downloads/details.aspx?familyid=e89fb3f1-44cb-4fc0-bbc2-8e94d6933322)  
(KB2688338)  
(Fontos)
</td>
<td style="border:1px solid black;">
[Windows 7 x64-alapú rendszerekhez](http://www.microsoft.com/downloads/details.aspx?familyid=dfa13df5-9e4e-4cf6-b56d-af7db0a0f5ea)  
(KB2690533)  
(Fontos)
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
Windows 7 x64 alapú rendszerekhez, Service Pack 1
</td>
<td style="border:1px solid black;">
[Windows 7 x64 alapú rendszerekhez, Service Pack 1](http://www.microsoft.com/downloads/details.aspx?familyid=7aa0b61b-b42c-4d60-8a7f-c61cbd25d6d9)  
(KB2658846)  
(Fontos)  
[Windows 7 x64 alapú rendszerekhez, Service Pack 1](http://www.microsoft.com/downloads/details.aspx?familyid=fa38b001-eef8-4153-b077-ea524e8a1e18)  
(KB2659262)  
(Fontos)  
[Windows 7 x64 alapú rendszerekhez, Service Pack 1](http://www.microsoft.com/downloads/details.aspx?familyid=7e551e0f-3f02-49ee-a5a1-8a7480722a6b)  
(KB2660649)  
(Fontos)  
[Windows 7 x64 alapú rendszerekhez, Service Pack 1](http://www.microsoft.com/downloads/details.aspx?familyid=c09cbb73-7814-4946-8c0a-323d304dd633)  
(KB2676562)  
(Kritikus)  
[Microsoft .NET-keretrendszer 3.5.1](http://www.microsoft.com/downloads/details.aspx?familyid=c06506e6-5838-4bba-9b12-b54dfa30a944)  
(KB2656411)  
(Nincs súlyossági besorolás<sup>[2]</sup>)  
[Microsoft .NET Framework 4](http://www.microsoft.com/downloads/details.aspx?familyid=4ee3cb61-542e-4e42-aa0e-0cbf8dd89648)<sup>[1]</sup>
(KB2656405)  
(Kritikus)
</td>
<td style="border:1px solid black;">
[Microsoft .NET-keretrendszer 3.5.1](http://www.microsoft.com/downloads/details.aspx?familyid=85e0f8be-cdc7-464b-be43-da23d82b3486)  
(KB2604115)  
(Kritikus)  
[Microsoft .NET Framework 4](http://www.microsoft.com/downloads/details.aspx?familyid=38b389d8-d534-4b0a-8dd4-b72a5ce7c4e8)<sup>[1]</sup>
(KB2604121)  
(Kritikus)
</td>
<td style="border:1px solid black;">
[Windows 7 x64 alapú rendszerekhez, Service Pack 1](http://www.microsoft.com/downloads/details.aspx?familyid=e89fb3f1-44cb-4fc0-bbc2-8e94d6933322)  
(KB2688338)  
(Fontos)
</td>
<td style="border:1px solid black;">
[Windows 7 x64 alapú rendszerekhez, Service Pack 1](http://www.microsoft.com/downloads/details.aspx?familyid=dfa13df5-9e4e-4cf6-b56d-af7db0a0f5ea)  
(KB2690533)  
(Fontos)
</td>
</tr>
<tr>
<th colspan="5">
Windows Server 2008 R2
</th>
</tr>
<tr>
<td style="border:1px solid black;">
**Közlemény azonosítója**
</td>
<td style="border:1px solid black;">
[**MS12-034**](http://go.microsoft.com/fwlink/?linkid=251038)
</td>
<td style="border:1px solid black;">
[**MS12-035**](http://go.microsoft.com/fwlink/?linkid=246970)
</td>
<td style="border:1px solid black;">
[**MS12-032**](http://go.microsoft.com/fwlink/?linkid=246964)
</td>
<td style="border:1px solid black;">
[**MS12-033**](http://go.microsoft.com/fwlink/?linkid=247902)
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
[**Fontos**](http://go.microsoft.com/fwlink/?linkid=21140)
</td>
<td style="border:1px solid black;">
[**Fontos**](http://go.microsoft.com/fwlink/?linkid=21140)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Windows Server 2008 R2 x64-alapú rendszerekhez
</td>
<td style="border:1px solid black;">
[Windows Server 2008 R2 x64-alapú rendszerekhez](http://www.microsoft.com/downloads/details.aspx?familyid=6f815b10-c60d-4e9b-8283-494036985e93)  
(KB2658846)  
(Fontos)  
[Windows Server 2008 R2 x64-alapú rendszerekhez](http://www.microsoft.com/downloads/details.aspx?familyid=34824de4-0f26-4627-8ddb-23d6b9d6671a)  
(KB2659262)  
(Fontos)  
[Windows Server 2008 R2 x64 alapú rendszerekhez](http://www.microsoft.com/downloads/details.aspx?familyid=6dab7283-81ba-4362-adb1-0db25e1f055e)\[4\]  
(KB2660649)  
(Fontos)  
[Windows Server 2008 R2 x64-alapú rendszerekhez](http://www.microsoft.com/downloads/details.aspx?familyid=1a179bf7-17fa-4dc7-b0c1-af6d911373cd)  
(KB2676562)  
(Kritikus)  
[Microsoft .NET-keretrendszer 3.5.1](http://www.microsoft.com/downloads/details.aspx?familyid=d04bfc77-d05f-4890-9175-27ad00e84c4a)  
(KB2656410)  
(Nincs súlyossági besorolás<sup>[2]</sup>)  
[Microsoft .NET Framework 4](http://www.microsoft.com/downloads/details.aspx?familyid=4ee3cb61-542e-4e42-aa0e-0cbf8dd89648)<sup>[1]</sup>
(KB2656405)  
(Kritikus)
</td>
<td style="border:1px solid black;">
[Microsoft .NET-keretrendszer 3.5.1](http://www.microsoft.com/downloads/details.aspx?familyid=cd42511f-788c-4473-84cc-19bb1623e337)  
(KB2604114)  
(Kritikus)  
[Microsoft .NET Framework 4](http://www.microsoft.com/downloads/details.aspx?familyid=38b389d8-d534-4b0a-8dd4-b72a5ce7c4e8)<sup>[1]</sup>
(KB2604121)  
(Kritikus)
</td>
<td style="border:1px solid black;">
[Windows Server 2008 R2 x64-alapú rendszerekhez](http://www.microsoft.com/downloads/details.aspx?familyid=08ba4320-6c47-4f82-a54f-61a32629b985)  
(KB2688338)  
(Fontos)
</td>
<td style="border:1px solid black;">
[Windows Server 2008 R2 x64-alapú rendszerekhez](http://www.microsoft.com/downloads/details.aspx?familyid=095c20b3-8e6c-4846-9ba1-6ce0af5e9850)  
(KB2690533)  
(Fontos)
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
Windows Server 2008 R2 x64-alapú rendszerekhez, Service Pack 1
</td>
<td style="border:1px solid black;">
[Windows Server 2008 R2 x64-alapú rendszerekhez, Service Pack 1](http://www.microsoft.com/downloads/details.aspx?familyid=6f815b10-c60d-4e9b-8283-494036985e93)  
(KB2658846)  
(Fontos)  
[Windows Server 2008 R2 x64-alapú rendszerekhez, Service Pack 1](http://www.microsoft.com/downloads/details.aspx?familyid=34824de4-0f26-4627-8ddb-23d6b9d6671a)  
(KB2659262)  
(Fontos)  
[Windows Server 2008 R2 x64 alapú rendszerekhez, Service Pack 1](http://www.microsoft.com/downloads/details.aspx?familyid=6dab7283-81ba-4362-adb1-0db25e1f055e)\[4\]  
(KB2660649)  
(Fontos)  
[Windows Server 2008 R2 x64-alapú rendszerekhez, Service Pack 1](http://www.microsoft.com/downloads/details.aspx?familyid=1a179bf7-17fa-4dc7-b0c1-af6d911373cd)  
(KB2676562)  
(Kritikus)  
[Microsoft .NET-keretrendszer 3.5.1](http://www.microsoft.com/downloads/details.aspx?familyid=c06506e6-5838-4bba-9b12-b54dfa30a944)  
(KB2656411)  
(Nincs súlyossági besorolás<sup>[2]</sup>)  
[Microsoft .NET Framework 4](http://www.microsoft.com/downloads/details.aspx?familyid=4ee3cb61-542e-4e42-aa0e-0cbf8dd89648)<sup>[1]</sup>
(KB2656405)  
(Kritikus)
</td>
<td style="border:1px solid black;">
[Microsoft .NET-keretrendszer 3.5.1](http://www.microsoft.com/downloads/details.aspx?familyid=85e0f8be-cdc7-464b-be43-da23d82b3486)  
(KB2604115)  
(Kritikus)  
[Microsoft .NET Framework 4](http://www.microsoft.com/downloads/details.aspx?familyid=38b389d8-d534-4b0a-8dd4-b72a5ce7c4e8)<sup>[1]</sup>
(KB2604121)  
(Kritikus)
</td>
<td style="border:1px solid black;">
[Windows Server 2008 R2 x64-alapú rendszerekhez, Service Pack 1](http://www.microsoft.com/downloads/details.aspx?familyid=08ba4320-6c47-4f82-a54f-61a32629b985)  
(KB2688338)  
(Fontos)
</td>
<td style="border:1px solid black;">
[Windows Server 2008 R2 x64-alapú rendszerekhez, Service Pack 1](http://www.microsoft.com/downloads/details.aspx?familyid=095c20b3-8e6c-4846-9ba1-6ce0af5e9850)  
(KB2690533)  
(Fontos)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Windows Server 2008 R2 Itanium-alapú rendszerekhez
</td>
<td style="border:1px solid black;">
[Windows Server 2008 R2 Itanium-alapú rendszerekhez](http://www.microsoft.com/downloads/details.aspx?familyid=b9172218-8a3f-4b0f-a14d-64db3778f4cc)  
(KB2658846)  
(Fontos)  
[Windows Server 2008 R2 Itanium-alapú rendszerekhez](http://www.microsoft.com/downloads/details.aspx?familyid=d9abec73-150e-40cf-a108-1d8ee89aac92)  
(KB2659262)  
(Fontos)  
[Windows Server 2008 R2 Itanium-alapú rendszerekhez](http://www.microsoft.com/downloads/details.aspx?familyid=e075c03e-91db-4974-a6ea-8edeba583293)  
(KB2676562)  
(Kritikus)
</td>
<td style="border:1px solid black;">
[Microsoft .NET-keretrendszer 3.5.1](http://www.microsoft.com/downloads/details.aspx?familyid=cd42511f-788c-4473-84cc-19bb1623e337)  
(KB2604114)  
(Kritikus)  
[Microsoft .NET Framework 4](http://www.microsoft.com/downloads/details.aspx?familyid=38b389d8-d534-4b0a-8dd4-b72a5ce7c4e8)<sup>[1]</sup>
(KB2604121)  
(Kritikus)
</td>
<td style="border:1px solid black;">
[Windows Server 2008 R2 Itanium-alapú rendszerekhez](http://www.microsoft.com/downloads/details.aspx?familyid=34643abe-2905-4ac1-a5f3-3f6ea8724b7a)  
(KB2688338)  
(Fontos)
</td>
<td style="border:1px solid black;">
[Windows Server 2008 R2 Itanium-alapú rendszerekhez](http://www.microsoft.com/downloads/details.aspx?familyid=9b66a74a-7022-49ac-89da-8c9ab8105812)  
(KB2690533)  
(Fontos)
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
Windows Server 2008 R2 Itanium alapú rendszerekhez, Service Pack 1
</td>
<td style="border:1px solid black;">
[Windows Server 2008 R2 Itanium alapú rendszerekhez, Service Pack 1](http://www.microsoft.com/downloads/details.aspx?familyid=b9172218-8a3f-4b0f-a14d-64db3778f4cc)  
(KB2658846)  
(Fontos)  
[Windows Server 2008 R2 Itanium alapú rendszerekhez, Service Pack 1](http://www.microsoft.com/downloads/details.aspx?familyid=d9abec73-150e-40cf-a108-1d8ee89aac92)  
(KB2659262)  
(Fontos)  
[Windows Server 2008 R2 Itanium alapú rendszerekhez, Service Pack 1](http://www.microsoft.com/downloads/details.aspx?familyid=e075c03e-91db-4974-a6ea-8edeba583293)  
(KB2676562)  
(Kritikus)
</td>
<td style="border:1px solid black;">
[Microsoft .NET-keretrendszer 3.5.1](http://www.microsoft.com/downloads/details.aspx?familyid=85e0f8be-cdc7-464b-be43-da23d82b3486)  
(KB2604115)  
(Kritikus)  
[Microsoft .NET Framework 4](http://www.microsoft.com/downloads/details.aspx?familyid=38b389d8-d534-4b0a-8dd4-b72a5ce7c4e8)<sup>[1]</sup>
(KB2604121)  
(Kritikus)
</td>
<td style="border:1px solid black;">
[Windows Server 2008 R2 Itanium alapú rendszerekhez, Service Pack 1](http://www.microsoft.com/downloads/details.aspx?familyid=34643abe-2905-4ac1-a5f3-3f6ea8724b7a)  
(KB2688338)  
(Fontos)
</td>
<td style="border:1px solid black;">
[Windows Server 2008 R2 Itanium alapú rendszerekhez, Service Pack 1](http://www.microsoft.com/downloads/details.aspx?familyid=9b66a74a-7022-49ac-89da-8c9ab8105812)  
(KB2690533)  
(Fontos)
</td>
</tr>
<tr>
<th colspan="5">
Kiszolgálómag-telepítési opció
</th>
</tr>
<tr>
<td style="border:1px solid black;">
**Közlemény azonosítója**
</td>
<td style="border:1px solid black;">
[**MS12-034**](http://go.microsoft.com/fwlink/?linkid=251038)
</td>
<td style="border:1px solid black;">
[**MS12-035**](http://go.microsoft.com/fwlink/?linkid=246970)
</td>
<td style="border:1px solid black;">
[**MS12-032**](http://go.microsoft.com/fwlink/?linkid=246964)
</td>
<td style="border:1px solid black;">
[**MS12-033**](http://go.microsoft.com/fwlink/?linkid=247902)
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
[**Fontos**](http://go.microsoft.com/fwlink/?linkid=21140)
</td>
<td style="border:1px solid black;">
[**Fontos**](http://go.microsoft.com/fwlink/?linkid=21140)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Windows Server 2008 32 bites rendszerekhez, Service Pack 2
</td>
<td style="border:1px solid black;">
[Windows Server 2008 32 bites rendszerekhez, Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=47a0df29-f42e-463b-9c15-a93385ff8705)  
(KB2659262)  
(Fontos)  
[Windows Server 2008 32 bites rendszerekhez, Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=728a84b9-c1b8-46e2-8365-1b542963508a)  
(KB2676562)  
(Fontos)
</td>
<td style="border:1px solid black;">
Nem érintett
</td>
<td style="border:1px solid black;">
[Windows Server 2008 32 bites rendszerekhez, Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=7ef72aab-7fd2-4330-bb6a-0c77c3943345)  
(KB2688338)  
(Fontos)
</td>
<td style="border:1px solid black;">
[Windows Server 2008 32 bites rendszerekhez, Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=46e6e960-b700-4154-b91d-aca74ea9e5df)  
(KB2690533)  
(Fontos)
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
Windows Server 2008 x64-alapú rendszerekhez, Service Pack 2
</td>
<td style="border:1px solid black;">
[Windows Server 2008 x64-alapú rendszerekhez, Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=4e6d29e1-17fc-4670-9e69-988c040f06e2)  
(KB2659262)  
(Fontos)  
[Windows Server 2008 x64-alapú rendszerekhez, Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=ab897da8-a927-42eb-87da-1e5cd820f4c0)  
(KB2676562)  
(Fontos)
</td>
<td style="border:1px solid black;">
Nem érintett
</td>
<td style="border:1px solid black;">
[Windows Server 2008 x64-alapú rendszerekhez, Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=9569d980-766d-4825-bd1c-f30c93d4b035)  
(KB2688338)  
(Fontos)
</td>
<td style="border:1px solid black;">
[Windows Server 2008 x64-alapú rendszerekhez, Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=e4ab05ae-3a1c-4d6b-8c84-1165ed741356)  
(KB2690533)  
(Fontos)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Windows Server 2008 R2 x64-alapú rendszerekhez
</td>
<td style="border:1px solid black;">
[Windows Server 2008 R2 x64-alapú rendszerekhez](http://www.microsoft.com/downloads/details.aspx?familyid=34824de4-0f26-4627-8ddb-23d6b9d6671a)  
(KB2659262)  
(Fontos)  
[Windows Server 2008 R2 x64-alapú rendszerekhez](http://www.microsoft.com/downloads/details.aspx?familyid=1a179bf7-17fa-4dc7-b0c1-af6d911373cd)  
(KB2676562)  
(Fontos)  
[Microsoft .NET-keretrendszer 3.5.1](http://www.microsoft.com/downloads/details.aspx?familyid=d04bfc77-d05f-4890-9175-27ad00e84c4a)  
(KB2656410)  
(Nincs súlyossági besorolás<sup>[2]</sup>)
</td>
<td style="border:1px solid black;">
[Microsoft .NET-keretrendszer 3.5.1](http://www.microsoft.com/downloads/details.aspx?familyid=cd42511f-788c-4473-84cc-19bb1623e337)  
(KB2604114)  
(Kritikus)
</td>
<td style="border:1px solid black;">
[Windows Server 2008 R2 x64-alapú rendszerekhez](http://www.microsoft.com/downloads/details.aspx?familyid=08ba4320-6c47-4f82-a54f-61a32629b985)  
(KB2688338)  
(Fontos)
</td>
<td style="border:1px solid black;">
[Windows Server 2008 R2 x64-alapú rendszerekhez](http://www.microsoft.com/downloads/details.aspx?familyid=095c20b3-8e6c-4846-9ba1-6ce0af5e9850)  
(KB2690533)  
(Fontos)
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
Windows Server 2008 R2 x64-alapú rendszerekhez, Service Pack 1
</td>
<td style="border:1px solid black;">
[Windows Server 2008 R2 x64-alapú rendszerekhez, Service Pack 1](http://www.microsoft.com/downloads/details.aspx?familyid=34824de4-0f26-4627-8ddb-23d6b9d6671a)  
(KB2659262)  
(Fontos)  
[Windows Server 2008 R2 x64-alapú rendszerekhez, Service Pack 1](http://www.microsoft.com/downloads/details.aspx?familyid=1a179bf7-17fa-4dc7-b0c1-af6d911373cd)  
(KB2676562)  
(Fontos)  
[Microsoft .NET-keretrendszer 3.5.1](http://www.microsoft.com/downloads/details.aspx?familyid=c06506e6-5838-4bba-9b12-b54dfa30a944)  
(KB2656411)  
(Nincs súlyossági besorolás<sup>[2]</sup>)  
[Microsoft .NET Framework 4](http://www.microsoft.com/downloads/details.aspx?familyid=4ee3cb61-542e-4e42-aa0e-0cbf8dd89648)  
(KB2656405)  
(Kritikus)
</td>
<td style="border:1px solid black;">
[Microsoft .NET-keretrendszer 3.5.1](http://www.microsoft.com/downloads/details.aspx?familyid=85e0f8be-cdc7-464b-be43-da23d82b3486)  
(KB2604115)  
(Kritikus)  
[Microsoft .NET Framework 4](http://www.microsoft.com/downloads/details.aspx?familyid=38b389d8-d534-4b0a-8dd4-b72a5ce7c4e8)<sup>[1]</sup>
(KB2604121)  
(Kritikus)
</td>
<td style="border:1px solid black;">
[Windows Server 2008 R2 x64-alapú rendszerekhez, Service Pack 1](http://www.microsoft.com/downloads/details.aspx?familyid=08ba4320-6c47-4f82-a54f-61a32629b985)  
(KB2688338)  
(Fontos)
</td>
<td style="border:1px solid black;">
[Windows Server 2008 R2 x64-alapú rendszerekhez, Service Pack 1](http://www.microsoft.com/downloads/details.aspx?familyid=095c20b3-8e6c-4846-9ba1-6ce0af5e9850)  
(KB2690533)  
(Fontos)
</td>
</tr>
</table>
 
**Megjegyzések** **az** **MS12-034 közleményhez**

<sup>[1]</sup>**A .NET Framework 4 verziója és a .NET Framework 4 verziójához tartozó ügyfélprofil.** A .NET-keretrendszer 4-es verziójú terjeszthető csomagjai két profilban érhetőek el: a .NET Framework 4 és a .NET Framework 4 verziójához tartozó ügyfélprofil. A .NET Framework 4 verziójához tartozó ügyfélprofil a .NET Framework 4 részhalmaza. Az ebben a frissítésben tárgyalt biztonsági rés egyaránt érinti a .NET Framework 4 verzióját és a .NET Framework 4 verziójához tartozó ügyfélprofilt is. További információk [A .NET keretrendszer telepítése](http://msdn.microsoft.com/en-us/library/5a4x27ek.aspx) c. MSDN cikkben.

<sup>[2]</sup>A szóban forgó szoftver frissítésére nem vonatkozik súlyossági besorolás, mert a közleményben taglalt biztonsági réssel kapcsolatban nincsenek ismert támadási módszerek. Mivel a frissítésben mélyreható védelmi módosítások is vannak, a Microsoft azt ajánlja, hogy a szoftver felhasználói telepítsék ezt a biztonsági frissítést.

<sup>[3]</sup>A frissítés csak akkor vonatkozik a Windows Server 2008 rendszerekre, ha a választható Desktop Experience funkciót telepítették és bekapcsolták. A részleteket az MS12-034 frissítésekkel kapcsolatos GYIK részében találja.

\[4\]A frissítés csak akkor vonatkozik a Windows Server 2008 R2 rendszerekre, ha a választható Ink and Handwriting Services funkció Ink Support összetevőjét telepítették és bekapcsolták. A részleteket az MS12-034 frissítésekkel kapcsolatos GYIK részében találja.

Az ugyanezen a közleményazonosító alatt található, további frissített fájlokat illetően lásd még az egyéb szoftverkategóriák részt ebben a fejezetben, **Érintett szoftverek és letöltési helyek**. Ez a közlemény több szoftverkategóriát ölel fel.

**Megjegyzés** **az** **MS12-035 közleményhez**

<sup>[1]</sup>**A .NET Framework 4 verziója és a .NET Framework 4 verziójához tartozó ügyfélprofil.** A .NET-keretrendszer 4-es verziójú terjeszthető csomagjai két profilban érhetőek el: a .NET Framework 4 és a .NET Framework 4 verziójához tartozó ügyfélprofil. A .NET Framework 4 verziójához tartozó ügyfélprofil a .NET Framework 4 részhalmaza. Az ebben a frissítésben tárgyalt biztonsági rés egyaránt érinti a .NET Framework 4 verzióját és a .NET Framework 4 verziójához tartozó ügyfélprofilt is. További információk [A .NET keretrendszer telepítése](http://msdn.microsoft.com/en-us/library/5a4x27ek.aspx) c. MSDN cikkben.

#### Microsoft Office programcsomagok és szoftverek

 
<p> </p>
<table style="border:1px solid black;">
<tr>
<th colspan="5">
Microsoft Office programcsomagok és összetevők
</th>
</tr>
<tr>
<td style="border:1px solid black;">
**Közlemény azonosítója**
</td>
<td style="border:1px solid black;">
[**MS12-029**](http://go.microsoft.com/fwlink/?linkid=248419)
</td>
<td style="border:1px solid black;">
[**MS12-034**](http://go.microsoft.com/fwlink/?linkid=251038)
</td>
<td style="border:1px solid black;">
[**MS12-030**](http://go.microsoft.com/fwlink/?linkid=238499)
</td>
<td style="border:1px solid black;">
[**MS12-031**](http://go.microsoft.com/fwlink/?linkid=248385)
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
Microsoft Office 2003 Service Pack 3
</td>
<td style="border:1px solid black;">
[Microsoft Word 2003 Service Pack 3](http://www.microsoft.com/downloads/details.aspx?familyid=9819899d-7f7f-4ddd-9fc8-816a57d2979e)  
(KB2598332)  
(Fontos)
</td>
<td style="border:1px solid black;">
[Microsoft Office 2003 Service Pack 3](http://www.microsoft.com/downloads/details.aspx?familyid=0abbf09c-8828-4524-8b38-e34faefa2ae4)  
(KB2598253)  
(Fontos)
</td>
<td style="border:1px solid black;">
[Microsoft Excel 2003 Service Pack 3](http://www.microsoft.com/downloads/details.aspx?familyid=162901b1-4c1d-476f-99e9-218780897f92)  
(KB2597086)  
(Fontos)
</td>
<td style="border:1px solid black;">
Nem érintett
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
Microsoft Office 2007 Service Pack 2
</td>
<td style="border:1px solid black;">
[Microsoft Word 2007 Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=c6f79d01-8735-4b0f-a50b-90cde3fba4ee)<sup>[1]</sup>
(KB2596917)  
(Kritikus)
</td>
<td style="border:1px solid black;">
[Microsoft Office 2007 Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=b9a27671-883a-4ab7-b86f-99730a9af729)  
(KB2596672)  
(Fontos)  
[Microsoft Office 2007 Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=fa054591-b202-47f2-9610-f3cd288d34c0)  
(KB2596792)  
(Fontos)
</td>
<td style="border:1px solid black;">
[Microsoft Excel 2007 Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=22b9b3a6-ad09-4397-892c-2190a86baf3e)<sup>[1]</sup>
(KB2597161)  
(Fontos)  
[Microsoft Office 2007 Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=6ff6650c-eaf4-4c7d-986c-c4d9e5324dac)  
(KB2597969)  
(Fontos)
</td>
<td style="border:1px solid black;">
Nem érintett
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Microsoft Office 2007 Service Pack 3
</td>
<td style="border:1px solid black;">
[Microsoft Word 2007 Service Pack 3](http://www.microsoft.com/downloads/details.aspx?familyid=c6f79d01-8735-4b0f-a50b-90cde3fba4ee)<sup>[1]</sup>
(KB2596917)  
(Kritikus)
</td>
<td style="border:1px solid black;">
[Microsoft Office 2007 Service Pack 3](http://www.microsoft.com/downloads/details.aspx?familyid=b9a27671-883a-4ab7-b86f-99730a9af729)  
(KB2596672)  
(Fontos)  
[Microsoft Office 2007 Service Pack 3](http://www.microsoft.com/downloads/details.aspx?familyid=fa054591-b202-47f2-9610-f3cd288d34c0)  
(KB2596792)  
(Fontos)
</td>
<td style="border:1px solid black;">
[Microsoft Excel 2007 Service Pack 3](http://www.microsoft.com/downloads/details.aspx?familyid=22b9b3a6-ad09-4397-892c-2190a86baf3e)<sup>[1]</sup>
(KB2597161)  
(Fontos)  
[Microsoft Office 2007 Service Pack 3](http://www.microsoft.com/downloads/details.aspx?familyid=6ff6650c-eaf4-4c7d-986c-c4d9e5324dac)  
(KB2597969)  
(Fontos)
</td>
<td style="border:1px solid black;">
Nem érintett
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
Microsoft Office 2010 (32 bites kiadások)
</td>
<td style="border:1px solid black;">
Nem érintett
</td>
<td style="border:1px solid black;">
[Microsoft Office 2010 (32 bites kiadások)](http://www.microsoft.com/downloads/details.aspx?familyid=c355d598-ff4d-4cac-afa9-2de3236a7d71)  
(KB2589337)  
(Fontos)
</td>
<td style="border:1px solid black;">
[Microsoft Excel 2010 (32 bites kiadások)](http://www.microsoft.com/downloads/details.aspx?familyid=f537f6d0-be63-42af-8b39-fa6f38715f84)  
(KB2597166)  
(Fontos)  
[Microsoft Office 2010 (32 bites kiadások)](http://www.microsoft.com/downloads/details.aspx?familyid=2e1060fa-c43d-42df-be5f-f536d9b39ba4)  
(KB2553371)  
(Fontos)
</td>
<td style="border:1px solid black;">
Nem érintett
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Microsoft Office 2010 Service Pack 1 (32 bites kiadások)
</td>
<td style="border:1px solid black;">
Nem érintett
</td>
<td style="border:1px solid black;">
[Microsoft Office 2010 Service Pack 1 (32 bites kiadások)](http://www.microsoft.com/downloads/details.aspx?familyid=c355d598-ff4d-4cac-afa9-2de3236a7d71)  
(KB2589337)  
(Fontos)
</td>
<td style="border:1px solid black;">
[Microsoft Excel 2010 Service Pack 1 (32 bites kiadások)](http://www.microsoft.com/downloads/details.aspx?familyid=f537f6d0-be63-42af-8b39-fa6f38715f84)  
(KB2597166)  
(Fontos)  
[Microsoft Office 2010 Service Pack 1 (32 bites kiadások)](http://www.microsoft.com/downloads/details.aspx?familyid=2e1060fa-c43d-42df-be5f-f536d9b39ba4)  
(KB2553371)  
(Fontos)
</td>
<td style="border:1px solid black;">
Nem érintett
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
Microsoft Office 2010 (64 bites kiadások)
</td>
<td style="border:1px solid black;">
Nem érintett
</td>
<td style="border:1px solid black;">
[Microsoft Office 2010 (64 bites kiadások)](http://www.microsoft.com/downloads/details.aspx?familyid=91619bcc-9d5d-4011-a185-c405758782be)  
(KB2589337)  
(Fontos)
</td>
<td style="border:1px solid black;">
[Microsoft Excel 2010 (64 bites kiadások)](http://www.microsoft.com/downloads/details.aspx?familyid=123b96d9-de3f-4aab-bcf8-bf9089fef400)  
(KB2597166)  
(Fontos)  
[Microsoft Office 2010 (64 bites kiadások)](http://www.microsoft.com/downloads/details.aspx?familyid=ec4371f6-644d-430d-880f-12425f1b36d4)  
(KB2553371)  
(Fontos)
</td>
<td style="border:1px solid black;">
Nem érintett
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Microsoft Office 2010 Service Pack 1 (64 bites kiadások)
</td>
<td style="border:1px solid black;">
Nem érintett
</td>
<td style="border:1px solid black;">
[Microsoft Office 2010 Service Pack 1 (64 bites kiadások)](http://www.microsoft.com/downloads/details.aspx?familyid=91619bcc-9d5d-4011-a185-c405758782be)  
(KB2589337)  
(Fontos)
</td>
<td style="border:1px solid black;">
[Microsoft Excel 2010 Service Pack 1 (64 bites kiadások)](http://www.microsoft.com/downloads/details.aspx?familyid=123b96d9-de3f-4aab-bcf8-bf9089fef400)  
(KB2597166)  
(Fontos)  
[Microsoft Office 2010 Service Pack 1 (64 bites kiadások)](http://www.microsoft.com/downloads/details.aspx?familyid=ec4371f6-644d-430d-880f-12425f1b36d4)  
(KB2553371)  
(Fontos)
</td>
<td style="border:1px solid black;">
Nem érintett
</td>
</tr>
<tr>
<th colspan="5">
Microsoft Office for Mac
</th>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
**Közlemény azonosítója**
</td>
<td style="border:1px solid black;">
[**MS12-029**](http://go.microsoft.com/fwlink/?linkid=248419)
</td>
<td style="border:1px solid black;">
[**MS12-034**](http://go.microsoft.com/fwlink/?linkid=251038)
</td>
<td style="border:1px solid black;">
[**MS12-030**](http://go.microsoft.com/fwlink/?linkid=238499)
</td>
<td style="border:1px solid black;">
[**MS12-031**](http://go.microsoft.com/fwlink/?linkid=248385)
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
[**Fontos**](http://go.microsoft.com/fwlink/?linkid=21140)
</td>
<td style="border:1px solid black;">
Nincsenek
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
Microsoft Office 2008 for Mac
</td>
<td style="border:1px solid black;">
[Microsoft Office 2008 for Mac](http://www.microsoft.com/downloads/details.aspx?familyid=8f85fc23-480e-4835-9ce5-0aa56702ef59)  
(KB2665346)  
(Fontos)
</td>
<td style="border:1px solid black;">
Nem érintett
</td>
<td style="border:1px solid black;">
[Microsoft Office 2008 for Mac](http://www.microsoft.com/downloads/details.aspx?familyid=8f85fc23-480e-4835-9ce5-0aa56702ef59)  
(KB2665346)  
(Fontos)
</td>
<td style="border:1px solid black;">
Nem érintett
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Microsoft Office for Mac 2011
</td>
<td style="border:1px solid black;">
[Microsoft Office for Mac 2011](http://www.microsoft.com/downloads/details.aspx?familyid=5d88d3d4-89bd-44c3-9e5a-657998223e2f)  
(KB2665351)  
(Fontos)
</td>
<td style="border:1px solid black;">
Nem érintett
</td>
<td style="border:1px solid black;">
[Microsoft Office for Mac 2011](http://www.microsoft.com/downloads/details.aspx?familyid=5d88d3d4-89bd-44c3-9e5a-657998223e2f)  
(KB2665351)  
(Fontos)
</td>
<td style="border:1px solid black;">
Nem érintett
</td>
</tr>
<tr>
<th colspan="5">
Egyéb Microsoft Office szoftver
</th>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
**Közlemény azonosítója**
</td>
<td style="border:1px solid black;">
[**MS12-029**](http://go.microsoft.com/fwlink/?linkid=248419)
</td>
<td style="border:1px solid black;">
[**MS12-034**](http://go.microsoft.com/fwlink/?linkid=251038)
</td>
<td style="border:1px solid black;">
[**MS12-030**](http://go.microsoft.com/fwlink/?linkid=238499)
</td>
<td style="border:1px solid black;">
[**MS12-031**](http://go.microsoft.com/fwlink/?linkid=248385)
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
[**Fontos**](http://go.microsoft.com/fwlink/?linkid=21140)
</td>
<td style="border:1px solid black;">
[**Fontos**](http://go.microsoft.com/fwlink/?linkid=21140)
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
Nem érintett
</td>
<td style="border:1px solid black;">
[Microsoft Excel Megtekintő](http://www.microsoft.com/downloads/details.aspx?familyid=9dedfb18-a651-49f7-b1fc-78f7b6cb234a)<sup>[2]</sup>
(KB2596842)  
(Fontos)
</td>
<td style="border:1px solid black;">
Nem érintett
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Microsoft Visio Viewer 2010
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
[Microsoft Visio Viewer 2010 (32 bites kiadás)](http://www.microsoft.com/downloads/details.aspx?familyid=0d21d110-c787-49b6-8384-6eaf9da5a38f)  
(KB2597981)  
(Fontos)  
[Microsoft Visio Viewer 2010 Service Pack 1 (32 bites kiadás)](http://www.microsoft.com/downloads/details.aspx?familyid=0d21d110-c787-49b6-8384-6eaf9da5a38f)  
(KB2597981)  
(Fontos)  
[Microsoft Visio Viewer 2010 (64 bites kiadás)](http://www.microsoft.com/downloads/details.aspx?familyid=331d8247-559c-4040-bdea-84cb6fd5dee2)  
(KB2597981)  
(Fontos)  
[Microsoft Visio Viewer 2010 Service Pack 1 (64 bites kiadás)](http://www.microsoft.com/downloads/details.aspx?familyid=331d8247-559c-4040-bdea-84cb6fd5dee2)  
(KB2597981)  
(Fontos)
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
Microsoft Office Compatibility Pack Service Pack 2
</td>
<td style="border:1px solid black;">
[Microsoft Office Compatibility Pack Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=80d5a86a-33b0-4464-af76-0fe13bd07a5c)  
(KB2596880)  
(Fontos)
</td>
<td style="border:1px solid black;">
Nem érintett
</td>
<td style="border:1px solid black;">
[Microsoft Office Compatibility Pack Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=a8386ad9-635f-45a7-b33e-ac9a3ca55f82)  
(KB2597162)  
(Fontos)
</td>
<td style="border:1px solid black;">
Nem érintett
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Microsoft Office Compatibility Pack Service Pack 3
</td>
<td style="border:1px solid black;">
[Microsoft Office Compatibility Pack Service Pack 3](http://www.microsoft.com/downloads/details.aspx?familyid=80d5a86a-33b0-4464-af76-0fe13bd07a5c)  
(KB2596880)  
(Fontos)
</td>
<td style="border:1px solid black;">
Nem érintett
</td>
<td style="border:1px solid black;">
[Microsoft Office Compatibility Pack Service Pack 3](http://www.microsoft.com/downloads/details.aspx?familyid=a8386ad9-635f-45a7-b33e-ac9a3ca55f82)  
(KB2597162)  
(Fontos)
</td>
<td style="border:1px solid black;">
Nem érintett
</td>
</tr>
</table>
 
**Megjegyzés az MS12-029 közleményhez**

<sup>[1]</sup>A Microsoft Word 2007 felhasználóknak a KB2596917 frissítésen kívül a Microsoft Office kompatibilitási csomag (KB2596880) biztonsági frissítését is telepíteniük kell, hogy megvédjék rendszerüket a jelen közleményben ismertetett biztonsági rés hibáitól.

**Megjegyzések** **az** **MS12-030 közleményhez**

<sup>[1]</sup>A Microsoft Excel 2007 felhasználóinak a KB2597161 frissítésen kívül a Microsoft Office Compatibility Pack kompatibilitási csomag (KB2597162) biztonsági frissítését is telepíteniük kell, hogy megvédjék rendszerüket a jelen közleményben ismertetett biztonsági rések hibáitól.

<sup>[2]</sup>A frissítés telepítése előtt a Microsoft Excel Megtekintőt támogatott szervizcsomagszintre kell frissíteni (Excel Megtekintő 2007 Service Pack 2 vagy Excel Megtekintő 2007 Service Pack 3). A támogatott Office megjelenítőkről a [Microsoft Tudásbázis 979860](http://support.microsoft.com/kb/979860) számú cikkében talál ismertetést.

**Megjegyzés** **az** **MS12-034 közleményhez**

Az ugyanezen a közleményazonosító alatt található, további frissített fájlokat illetően lásd még az egyéb szoftverkategóriák részt ebben a fejezetben, **Érintett szoftverek és letöltési helyek**. Ez a közlemény több szoftverkategóriát ölel fel.

#### Microsoft fejlesztői eszközök és szoftverek

 
<p> </p>
<table style="border:1px solid black;">
<tr>
<th colspan="2">
Microsoft Silverlight 4
</th>
</tr>
<tr>
<td style="border:1px solid black;">
**Közlemény azonosítója**
</td>
<td style="border:1px solid black;">
[**MS12-034**](http://go.microsoft.com/fwlink/?linkid=251038)
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
Mac számítógépre telepített [Microsoft Silverlight 4](http://www.microsoft.com/downloads/details.aspx?familyid=8ea4fc68-7b03-43f6-bc41-af47e7aa8c7b) alkalmazás  
(KB2690729)  
(Kritikus)  
A [Microsoft Silverlight 4](http://www.microsoft.com/downloads/details.aspx?familyid=8ea4fc68-7b03-43f6-bc41-af47e7aa8c7b) Microsoft Windows ügyfelek minden támogatott kiadására telepített verziója esetén  
(KB2690729)  
(Kritikus)  
[Microsoft Silverlight 4](http://www.microsoft.com/downloads/details.aspx?familyid=8ea4fc68-7b03-43f6-bc41-af47e7aa8c7b)Microsoft Windows ügyfelek minden támogatott kiadására telepített verziója esetén  
(KB2690729)  
(Kritikus)
</td>
</tr>
<tr>
<th colspan="2">
Microsoft Silverlight 5
</th>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
**Közlemény azonosítója**
</td>
<td style="border:1px solid black;">
[**MS12-034**](http://go.microsoft.com/fwlink/?linkid=251038)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
**Összesített súlyossági besorolás**
</td>
<td style="border:1px solid black;">
[**Kritikus**](http://go.microsoft.com/fwlink/?linkid=21140)
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
Microsoft Silverlight 5
</td>
<td style="border:1px solid black;">
Mac számítógépre telepített [Microsoft Silverlight 5](http://www.microsoft.com/downloads/details.aspx?familyid=fb1258e2-f3df-4a3d-b809-abec619a0c63) alkalmazás  
(KB2636927)  
(Kritikus)  
A [Microsoft Silverlight 5](http://www.microsoft.com/downloads/details.aspx?familyid=fb1258e2-f3df-4a3d-b809-abec619a0c63) Microsoft Windows ügyfelek minden támogatott kiadására telepített verziója esetén  
(KB2636927)  
(Kritikus)  
A [Microsoft Silverlight 5](http://www.microsoft.com/downloads/details.aspx?familyid=fb1258e2-f3df-4a3d-b809-abec619a0c63) Microsoft Windows kiszolgálók minden támogatott kiadására telepített verziója esetén  
(KB2636927)  
(Kritikus)
</td>
</tr>
</table>
 
**Megjegyzés** **az** **MS12-034 közleményhez**

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

-   A [Tipping Point](http://www.tippingpoint.com/)[Zero Day Initiative](http://www.zerodayinitiative.com/) programjában részt vevő anonim kutató az MS12-029 közleményben ismertetett probléma jelentéséért
-   [Omair](http://krash.in/), az MS12-030 számú közleményben leírt két hiba jelentéséért
-   Omair, a [VeriSign iDefense Labs](http://labs.idefense.com/), az MS12-030 közleményben ismertetett probléma jelentéséért
-   Sean Larsson és Jun Mao, [VeriSign iDefense Labs](http://labs.idefense.com/), az MS12-030 közleményben ismertetett két probléma jelentéséért
-   A [Tipping Point](http://www.tippingpoint.com/)[Zero Day Initiative](http://www.zerodayinitiative.com/) programjában részt vevő anonim kutató az MS12-030 közleményben ismertetett probléma jelentéséért
-   Luigi Auriemma, [VeriSign iDefense Labs](http://labs.idefense.com/), az MS12-031 közleményben leírt hiba jelentéséért
-   Bojan Zdrnja, [INFIGO IS](http://www.infigo.hr/), az MS12-032 közleményben leírt hiba jelentéséért
-   Anatoliy Glagolev, [Genesys Telecommunications](http://www.genesyslab.com/) az MS12-032 közleményben leírt probléma közös megoldásában való részvételéért
-   Alin Rad Pop, [Tipping Point's](http://www.tippingpoint.com/)[Zero Day Initiative](http://www.zerodayinitiative.com/), az MS12-034 közleményben leírt probléma jelentéséért
-   Vitaliy Toropov, [Tipping Point's](http://www.tippingpoint.com/)[Zero Day Initiative](http://www.zerodayinitiative.com/), az MS12-034 közleményben leírt probléma jelentéséért
-   [Omair](http://krash.in/), az MS12-034 számú közleményben leírt hiba jelentéséért
-   A [VeriSign iDefense Labs](http://labs.idefense.com/) anonim együttműködő partnerének az MS12-034 közleményben ismertetett probléma jelentéséért
-   A [VeriSign iDefense Labs](http://labs.idefense.com/) anonim együttműködő partnerének az MS12-034 közleményben ismertetett probléma jelentéséért
-   Alex Plaskett, [MWR InfoSecurity](http://www.mwrinfosecurity.com/), az MS12-034 közleményben leírt biztonsági rés jelentéséért
-   Tarjei Mandt, [Azimuth Security](http://www.azimuthsecurity.com/), az MS12-034 közleményben leírt probléma jelentéséért
-   Nicolas Economou, [Core Security Technologies](http://www.coresecurity.com/), az MS12-034 közleményben ismertetett probléma jelentéséért
-   Geoff McDonald, Symantec, az MS12-034 közleményben ismertetett probléma jelentéséért
-   h4ckmp, az MS12-034 közleményben bemutatott probléma jelentéséért
-   James Forshaw, [Context Information Security](http://www.contextis.co.uk/), az MS12-035 közleményben ismertetett két probléma jelentéséért

#### Terméktámogatás

-   Teszteléssel állapították meg a felsorolt szoftverek egyes verzióinak érintettségét. A többi verzió támogatási életciklusa végére ért. Az egyes szoftververziók támogatási életciklusáról a [Microsoft termékek terméktámogatási életciklusát ismertető webhelyen](http://go.microsoft.com/fwlink/?linkid=21742) talál felvilágosítást.
-   Biztonsági megoldások informatikai szakemberek számára: [TechNet Security hibakeresés és támogatás](http://technet.microsoft.com/security/bb980617.aspx)
-   Segítség Windows operációs rendszert futtató számítógépének vírusok és rosszindulatú szoftverek elleni védelmében: [Vírusmegoldás és Biztonsági központ](http://support.microsoft.com/contactus/cu_sc_virsec_master)
-   Helyi támogatás országának megfelelően: [Nemzetközi támogatás](http://support.microsoft.com/common/international.aspx)

#### Felelősséget kizáró nyilatkozat

A Microsoft Tudásbázisban leírtak előzetes bejelentés nélkül változhatnak, és a cikkek tartalmáért a Microsoft nem vállal garanciát. A Microsoft egyben elhárít minden kifejezett és értelemszerű garanciát, beleértve az eladhatóságra és az adott célra való alkalmasságra vonatkozó garanciát is. A Microsoft Corporation vagy annak szállítói semmilyen körülmények között nem tehetők felelőssé közvetlen, közvetett, eseti, ok-okozati vagy különleges kárért (beleértve az elmaradt hasznot is), még akkor sem, ha a Microsoft Corporation vagy szállítói tudatában voltak a kár lehetséges voltának. Egyes államok törvényi szabályozása nem teszi lehetővé a véletlen vagy ok-okozati károkért vállalt felelősség korlátozását vagy kizárását, így ezekben az államokban az ez a felelősségkizárás nincs érvényben.

#### Verziók

-   1.0 verzió (2012. május 8.): Összefoglaló közlemény közzététele.
-   1.1 verzió (2012. május 9.): Frissítettük a CVE-2012-1847 címet a **Kihasználhatósági információk** részben.
-   2.0 verzió (2012. május 11.): Az MS12-035 közleményben szereplő, a Windows Server 2003 Service Pack 2 kivételével a Microsoft .NET-keretrendszer 1.1 Service Pack 1 változatát tartalmazó minden támogatott rendszerre vonatkozó biztonsági frissítés számát KB2656353-re javítottuk. A biztonsági frissítéshez kapcsolódó fájlok nem változtak. Azoknak a felhasználóknak, akik már telepítették frissítést, nincs további teendőjük
-   2.1 verzió (2012. május 22.): Az MS12-034 esetén lábjegyzetek kerültek be a KB2660649 biztonsági frissítéshez a Windows Server 2008 és Windows Server 2008 R2 szoftverekkel kapcsolatban. A biztonsági frissítés fájljai nem változtak. Azoknak a felhasználóknak, akik már telepítették frissítést, nincs további teendőjük

*Built at 2014-04-18T01:50:00Z-07:00*
