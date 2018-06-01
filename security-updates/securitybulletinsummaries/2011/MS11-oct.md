---
TOCTitle: 'MS11-OCT'
Title: 'A Microsoft biztonsági közleményei – összefoglalás, 2011. október'
ms:assetid: 'ms11-oct'
ms:contentKeyID: 61227760
ms:mtpsurl: 'https://technet.microsoft.com/hu-HU/library/ms11-oct(v=Security.10)'
author: SharonSears
ms.author: SharonSears
---

Security Bulletin Summary

A Microsoft biztonsági közleményei – összefoglalás, 2011. október
=================================================================

Közzétéve: 2011. október 11. | Frissítve: 2011. október 26.

**Verzió:** 1.1

Az összefoglaló a 2011 októberében kiadott biztonsági közleményeket összegzi.

A 2011. októberi biztonsági közlemények kiadása folytán az összefoglaló a 2011. október 6-án kiadott előzetes értesítés helyébe lép. További információk a biztonsági közlemények kiadásáról szóló előzetes értesítés szolgáltatásról lásd: [Előzetes értesítés a Microsoft biztonsági közleményeinek kiadásáról](http://go.microsoft.com/fwlink/?linkid=217213).

Ha automatikus értesítést szeretne kapni a Microsoft biztonsági közleményeinek megjelenéséről, fizessen elő a [Microsoft Technical Security Notifications](http://go.microsoft.com/fwlink/?linkid=21163) szolgáltatásra.

A közleményekkel kapcsolatos kérdések megválaszolására a Microsoft 2011. október 12-én, csendes-óceáni idő szerint 11 órakor webes szemináriumot tart. [Jelentkezzen most az októberi közleményeket bemutató webes szemináriumra](https://msevents.microsoft.com/cui/eventdetail.aspx?eventid=1032487956). Ezt követően a webes szeminárium igény szerint kerül megrendezésre. További információkért látogasson el a [Microsoft biztonsági közleményeit és a webes szemináriumokat](http://go.microsoft.com/fwlink/?linkid=217214) bemutató oldalra.

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
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=227075">MS11-078</a></td>
<td style="border:1px solid black;"><strong>A .NET-keretrendszer és a Microsoft Silverlight biztonsági rése távoli programkódfuttatást tehet lehetővé (2604930)</strong><br />
<br />
A biztonsági frissítés a Microsoft .NET-keretrendszer és a Microsoft Silverlight közvetlenül jelzett biztonsági rését szünteti meg. A biztonsági rés távoli kódfuttatást tehet lehetővé az ügyfélrendszereken, ha a felhasználó különlegesen kialakított weboldalt tekint meg az XAML böngészőalkalmazások (XBAP alkalmazások) vagy Silverlight alkalmazások futtatására alkalmas böngészőben. A kevesebb jogosultsággal bíró fiókkal rendelkező felhasználók esetében kisebb a veszélyeztetettség, mint a rendszergazdai jogosultságokkal rendelkezők esetén A biztonsági rések IIS szolgáltatást futtató kiszolgálórendszereken is lehetővé tehetik a távoli kódfuttatást, ha az adott kiszolgálón engedélyezett az ASP.NET oldalak feldolgozása, és a támadó sikeresen feltölt egy különlegesen kialakított ASP.NET oldalt a kiszolgálóra, és végrehajtja, mint az a webes tárolási forgatókönyv esetében történik. A biztonsági rés a Windows .NET alkalmazásokban is kihasználható a kódműködési biztonsági (CAS) korlátozások megkerülésére.</td>
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=21140">Kritikus</a><br />
Távoli kódfuttatás</td>
<td style="border:1px solid black;">Esetleg újra kell indítani a rendszert</td>
<td style="border:1px solid black;">Microsoft .NET-keretrendszer, Microsoft Silverlight</td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=226382">MS11-081</a></td>
<td style="border:1px solid black;"><strong>Összesítő biztonsági frissítés az Internet Explorer programhoz (2586448)</strong><br />
<br />
Ez a biztonsági frissítés az Internet Explorer nyolc közvetlenül jelzett biztonsági rését szünteti meg. A súlyosabb biztonsági rések távoli kódfuttatást tesznek lehetővé, amennyiben a felhasználó speciálisan kialakított weboldalt tekint meg az Internet Explorer alkalmazással. A biztonsági rések valamelyikét sikeresen kihasználó támadó a helyi felhasználóval egyező hozzáférést nyer a rendszerhez. A kevesebb jogosultsággal bíró fiókkal rendelkező felhasználók esetében kisebb a veszélyeztetettség, mint a rendszergazdai jogosultságokkal rendelkezők esetén</td>
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=21140">Kritikus</a><br />
Távoli kódfuttatás</td>
<td style="border:1px solid black;">Újraindítást igényel</td>
<td style="border:1px solid black;">Microsoft Windows,<br />
Internet Explorer</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=221538">MS11-075</a></td>
<td style="border:1px solid black;"><strong>A Microsoft Active Accessibility biztonsági rése távoli kódfuttatást tehet lehetővé (2623699)</strong><br />
<br />
A biztonsági frissítés a Microsoft Active Accessibility összetevő közvetlenül jelentett biztonsági rését szünteti meg. A támadó a biztonsági résen keresztül távoli kódfuttatást tud elérni, ha rá tudja venni a felhasználót, hogy nyisson meg egy megbízható fájlt, amely azonos hálózati meghajtón található, mint a különlegesen kialakított dinamikus csatolású függvénytár (DLL) fájl. Ezután a megbízható fájl megnyitása közben a Microsoft Active Accessibility összetevő megpróbálhatja betölteni a DLL-fájlt és végrehajtani az abban található kódot. A sikeres támadáshoz a felhasználónak egy nem megbízhatónak ítélt távoli fájlrendszerre vagy WebDAV megosztásra kell ellátogatnia, majd onnan dokumentumot megnyitnia, amelyet ezt követően a biztonsági rés által érintett alkalmazás betölt.</td>
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=21140">Fontos</a><br />
Távoli kódfuttatás</td>
<td style="border:1px solid black;">Újraindítást igényel</td>
<td style="border:1px solid black;">Microsoft Windows</td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=227073">MS11-076</a></td>
<td style="border:1px solid black;"><strong>A Windows Media Center biztonsági rése távoli programkódfuttatásra adhat lehetőséget (2604926)</strong><br />
<br />
A biztonsági frissítés a Windows Media Center nyilvánosan jelentett biztonsági rését szünteti meg. A támadó a biztonsági résen keresztül távoli kódfuttatást tud elérni, ha rá tudja venni a felhasználót, hogy nyisson meg egy megbízható fájlt, amely azonos hálózati meghajtón található, mint a különlegesen kialakított dinamikus csatolású függvénytár (DLL) fájl. Ezután a megbízható fájl megnyitásakor a Windows Media Center megpróbálhatja betölteni a DLL-fájlt, és végrehajtani az abban található kódot. A támadás sikerességéhez a felhasználónak nem megbízható távoli fájlrendszert vagy WebDAV megosztást kell meglátogatnia, és ott egy megbízható fájlt kell megnyitnia.</td>
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=21140">Fontos</a><br />
Távoli kódfuttatás</td>
<td style="border:1px solid black;">Esetleg újra kell indítani a rendszert</td>
<td style="border:1px solid black;">Microsoft Windows</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=225915">MS11-077</a></td>
<td style="border:1px solid black;"><strong>A kernelmódú Windows illesztőprogramok biztonsági rései távoli programkódfuttatásra adhatnak lehetőséget (2567053)</strong><br />
<br />
Ez a biztonsági frissítés a Microsoft Windows négy közvetlenül jelzett biztonsági rését szünteti meg. A biztonsági rések közül a legsúlyosabbak távoli kódfuttatást tehetnek lehetővé, ha a felhasználó különlegesen kialakított betűkészletfájlt (például .fon fájlt) nyit meg hálózati megosztásról, UNC vagy WebDAV helyről, illetve e-mail mellékletből. A távoli támadás sikerességéhez a felhasználónak meg kell látogatnia egy nem megbízható távoli fájlrendszert vagy WebDAV megosztást, és meg kell nyitnia a különlegesen kialakított betűkészletfájlt, vagy e-mail mellékletből kell megnyitnia a fájlt.</td>
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=21140">Fontos</a><br />
Távoli kódfuttatás</td>
<td style="border:1px solid black;">Újraindítást igényel</td>
<td style="border:1px solid black;">Microsoft Windows</td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=217472">MS11-079</a></td>
<td style="border:1px solid black;"><strong>A Microsoft Forefront Unified Access Gateway biztonsági rései távolról történő programkódfuttatást okozhatnak (2544641)</strong><br />
<br />
A biztonsági frissítés a Forefront Unified Access Gateway (UAG) öt, közvetlenül jelzett biztonsági rését szünteti meg. A legsúlyosabb besorolású biztonsági rések távoli kódfuttatást tehetnek lehetővé, ha a felhasználó egy speciálisan kialakított URL-címen látogat el az érintett webhelyek egyikére. A támadónak ugyanakkor nincs semmilyen lehetősége arra, hogy a felhasználót egy ilyen webhely megnyitására kényszerítse. Ehelyett a támadóknak az adott webhelyre kell csábítaniuk a felhasználókat. Ezt rendszerint úgy érik el, hogy ráveszik őket arra, hogy kattintsanak rá egy e-mailben lévő hivatkozásra vagy azonnali üzenetkezelőben megjelenő kérésre.</td>
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=21140">Fontos</a><br />
Távoli kódfuttatás</td>
<td style="border:1px solid black;">Esetleg újra kell indítani a rendszert</td>
<td style="border:1px solid black;">Microsoft Forefront United Access Gateway</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=227486">MS11-080</a></td>
<td style="border:1px solid black;"><strong>A kiegészítő funkció-illesztőprogramban lévő biztonsági rés a jogok kiterjesztését teheti lehetővé (2592799)</strong><br />
<br />
Ez a biztonsági frissítés megszünteti a Microsoft Windows kiegészítő funkció-illesztőprogramjában (AFD) a közvetlenül jelzett biztonsági rést. A biztonsági rés jogok kiterjesztését teheti lehetővé, ha a támadó bejelentkezik a felhasználó rendszerére, és ott speciálisan kialakított alkalmazást futtat. A támadónak a biztonsági rés kihasználásához érvényes bejelentkezési adatokkal kell rendelkeznie, és képesnek kell lennie helyileg bejelentkezni a rendszerbe.</td>
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=21140">Fontos</a><br />
Jogok kiterjesztése</td>
<td style="border:1px solid black;">Újraindítást igényel</td>
<td style="border:1px solid black;">Microsoft Windows</td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=228596">MS11-082</a></td>
<td style="border:1px solid black;"><strong>A Host Integration Server szolgáltatásmegtagadást lehetővé tévő biztonsági rései (2607670)</strong><br />
<br />
A biztonsági frissítés a Host Integration Server két, nyilvánosan jelentett biztonsági rését szünteti meg. A biztonsági rések szolgáltatásmegtagadást tehetnek lehetővé, ha a távoli támadó speciálisan kialakított hálózati csomagot küld az 1478. UDP-portot vagy az 1477. és 1478. TCP-portot figyelő Host Integration Server alkalmazásnak. A tűzfalakra vonatkozó gyakorlati tanácsok, valamint a szabványos alapértelmezett tűzfal-konfigurációk segítséget nyújthatnak a hálózatot érő, a szervezet határain kívülről eredő támadások kivédésében. Gyakorlati tanácsként azt javasoljuk, hogy az internetkapcsolattal rendelkező számítógépeken a lehető legkevesebb port legyen megnyitva. Ebben az esetben a Host Integration Server portokat le kell tiltani az internetről.</td>
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=21140">Fontos</a><br />
Szolgáltatásmegtagadás</td>
<td style="border:1px solid black;">Esetleg újra kell indítani a rendszert</td>
<td style="border:1px solid black;">Microsoft Host Integration Server</td>
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
<th style="border:1px solid black;" >Kódfuttatás kihasználhatóságának felmérése a legújabb szoftvereknél</th>
<th style="border:1px solid black;" >Kódfuttatás kihasználhatóságának felmérése a korábbi szoftvereknél</th>
<th style="border:1px solid black;" >Szolgáltatásmegtagadás kihasználhatóságának felmérése</th>
<th style="border:1px solid black;" >Fontos megjegyzések</th>
</tr>
</thead>
<tbody>
<tr class="odd">
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=221538">MS11-075</a></td>
<td style="border:1px solid black;">Active Accessibility nem biztonságos betöltése miatti biztonsági rés</td>
<td style="border:1px solid black;"><a href="http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2011-1247">CVE-2011-1247</a></td>
<td style="border:1px solid black;"><a href="http://technet.microsoft.com/en-us/security/cc998259.aspx">2</a> - Valószínűleg inkonzisztens rosszindulatú programkód</td>
<td style="border:1px solid black;"><a href="http://technet.microsoft.com/en-us/security/cc998259.aspx">1</a> - Valószínűleg konzisztens rosszindulatú programkód</td>
<td style="border:1px solid black;">Nem érintett</td>
<td style="border:1px solid black;">(Nincs)</td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=227073">MS11-076</a></td>
<td style="border:1px solid black;">Media Center nem biztonságos betöltése miatti biztonsági rés</td>
<td style="border:1px solid black;"><a href="http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2011-2009">CVE-2011-2009</a></td>
<td style="border:1px solid black;"><a href="http://technet.microsoft.com/en-us/security/cc998259.aspx">1</a> - Valószínűleg konzisztens rosszindulatú programkód</td>
<td style="border:1px solid black;"><a href="http://technet.microsoft.com/en-us/security/cc998259.aspx">1</a> - Valószínűleg konzisztens rosszindulatú programkód</td>
<td style="border:1px solid black;">Nem érintett</td>
<td style="border:1px solid black;">A biztonsági rés nyilvánosságra került.</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=225915">MS11-077</a></td>
<td style="border:1px solid black;">A Win32k Null mutatójának visszakeresési biztonsági rése</td>
<td style="border:1px solid black;"><a href="http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2011-1985">CVE-2011-1985</a></td>
<td style="border:1px solid black;"><a href="http://technet.microsoft.com/en-us/security/cc998259.aspx">1</a> - Valószínűleg konzisztens rosszindulatú programkód</td>
<td style="border:1px solid black;"><a href="http://technet.microsoft.com/en-us/security/cc998259.aspx">1</a> - Valószínűleg konzisztens rosszindulatú programkód</td>
<td style="border:1px solid black;">Állandó</td>
<td style="border:1px solid black;">(Nincs)</td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=225915">MS11-077</a></td>
<td style="border:1px solid black;">Font függvénytár nem biztonságos betöltése miatti biztonsági rés</td>
<td style="border:1px solid black;"><a href="http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2011-2003">CVE-2011-2003</a></td>
<td style="border:1px solid black;"><a href="http://technet.microsoft.com/en-us/security/cc998259.aspx">1</a> - Valószínűleg konzisztens rosszindulatú programkód</td>
<td style="border:1px solid black;"><a href="http://technet.microsoft.com/en-us/security/cc998259.aspx">1</a> - Valószínűleg konzisztens rosszindulatú programkód</td>
<td style="border:1px solid black;">Ideiglenes</td>
<td style="border:1px solid black;">(Nincs)</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=225915">MS11-077</a></td>
<td style="border:1px solid black;">A Win32k használat utáni felszabadítás miatti biztonsági rése</td>
<td style="border:1px solid black;"><a href="http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2011-2011">CVE-2011-2011</a></td>
<td style="border:1px solid black;"><a href="http://technet.microsoft.com/en-us/security/cc998259.aspx">2</a> - Valószínűleg inkonzisztens rosszindulatú programkód</td>
<td style="border:1px solid black;"><a href="http://technet.microsoft.com/en-us/security/cc998259.aspx">2</a> - Valószínűleg inkonzisztens rosszindulatú programkód</td>
<td style="border:1px solid black;">Állandó</td>
<td style="border:1px solid black;">(Nincs)</td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=227075">MS11-078</a></td>
<td style="border:1px solid black;">A .NET-keretrendszer osztályöröklést okozó biztonsági rése</td>
<td style="border:1px solid black;"><a href="http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2011-1253">CVE-2011-1253</a></td>
<td style="border:1px solid black;"><a href="http://technet.microsoft.com/en-us/security/cc998259.aspx">3</a> - Nem valószínű működő rosszindulatú programkód</td>
<td style="border:1px solid black;"><a href="http://technet.microsoft.com/en-us/security/cc998259.aspx">1</a> - Valószínűleg konzisztens rosszindulatú programkód</td>
<td style="border:1px solid black;">Nem érintett</td>
<td style="border:1px solid black;">(Nincs)</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=217472">MS11-079</a></td>
<td style="border:1px solid black;">ExcelTable válasz szétválasztás kiszolgáló XSS miatti biztonsági rése</td>
<td style="border:1px solid black;"><a href="http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2011-1895">CVE-2011-1895</a></td>
<td style="border:1px solid black;"><a href="http://technet.microsoft.com/en-us/security/cc998259.aspx">1</a> - Valószínűleg konzisztens rosszindulatú programkód</td>
<td style="border:1px solid black;"><a href="http://technet.microsoft.com/en-us/security/cc998259.aspx">1</a> - Valószínűleg konzisztens rosszindulatú programkód</td>
<td style="border:1px solid black;">Nem érintett</td>
<td style="border:1px solid black;">Adatokhoz való illetéktelen hozzáférés a közleményben ismertetett egyes platformokon</td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=217472">MS11-079</a></td>
<td style="border:1px solid black;">ExcelTable tükröződő XSS miatti biztonsági rése</td>
<td style="border:1px solid black;"><a href="http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2011-1896">CVE-2011-1896</a></td>
<td style="border:1px solid black;"><a href="http://technet.microsoft.com/en-us/security/cc998259.aspx">1</a> - Valószínűleg konzisztens rosszindulatú programkód</td>
<td style="border:1px solid black;"><a href="http://technet.microsoft.com/en-us/security/cc998259.aspx">1</a> - Valószínűleg konzisztens rosszindulatú programkód</td>
<td style="border:1px solid black;">Nem érintett</td>
<td style="border:1px solid black;">Adatokhoz való illetéktelen hozzáférés a közleményben ismertetett egyes platformokon</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=217472">MS11-079</a></td>
<td style="border:1px solid black;">Alapértelmezett tükröződő XSS miatti biztonsági rése</td>
<td style="border:1px solid black;"><a href="http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2011-1897">CVE-2011-1897</a></td>
<td style="border:1px solid black;"><a href="http://technet.microsoft.com/en-us/security/cc998259.aspx">1</a> - Valószínűleg konzisztens rosszindulatú programkód</td>
<td style="border:1px solid black;"><a href="http://technet.microsoft.com/en-us/security/cc998259.aspx">1</a> - Valószínűleg konzisztens rosszindulatú programkód</td>
<td style="border:1px solid black;">Nem érintett</td>
<td style="border:1px solid black;">Adatokhoz való illetéktelen hozzáférés a közleményben ismertetett egyes platformokon</td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=217472">MS11-079</a></td>
<td style="border:1px solid black;">A Poisoned Cup alkalmazás távoli programkódfuttatást lehetővé tevő biztonsági rése</td>
<td style="border:1px solid black;"><a href="http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2011-1969">CVE-2011-1969</a></td>
<td style="border:1px solid black;"><a href="http://technet.microsoft.com/en-us/security/cc998259.aspx">1</a> - Valószínűleg konzisztens rosszindulatú programkód</td>
<td style="border:1px solid black;"><a href="http://technet.microsoft.com/en-us/security/cc998259.aspx">1</a> - Valószínűleg konzisztens rosszindulatú programkód</td>
<td style="border:1px solid black;">Nem érintett</td>
<td style="border:1px solid black;">(Nincs)</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=217472">MS11-079</a></td>
<td style="border:1px solid black;">Üres munkamenet cookie összeomlás biztonsági rése</td>
<td style="border:1px solid black;"><a href="http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2011-2012">CVE-2011-2012</a></td>
<td style="border:1px solid black;">Nem érintett</td>
<td style="border:1px solid black;">Nem érintett</td>
<td style="border:1px solid black;">Állandó</td>
<td style="border:1px solid black;">Ez a biztonsági rés szolgáltatásmegtagadást okoz</td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=227486">MS11-080</a></td>
<td style="border:1px solid black;">A kiegészítő funkció-illesztőprogram jogok kiterjesztését lehetővé tévő biztonsági rése</td>
<td style="border:1px solid black;"><a href="http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2011-2005">CVE-2011-2005</a></td>
<td style="border:1px solid black;">Nem érintett</td>
<td style="border:1px solid black;"><a href="http://technet.microsoft.com/en-us/security/cc998259.aspx">1</a> - Valószínűleg konzisztens rosszindulatú programkód</td>
<td style="border:1px solid black;">Nem érintett</td>
<td style="border:1px solid black;">(Nincs)</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=226382">MS11-081</a></td>
<td style="border:1px solid black;">Görgetési esemény távoli programkódfuttatást lehetővé tevő biztonsági rése</td>
<td style="border:1px solid black;"><a href="http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2011-1993">CVE-2011-1993</a></td>
<td style="border:1px solid black;"><a href="http://technet.microsoft.com/en-us/security/cc998259.aspx">1</a> - Valószínűleg konzisztens rosszindulatú programkód</td>
<td style="border:1px solid black;"><a href="http://technet.microsoft.com/en-us/security/cc998259.aspx">1</a> - Valószínűleg konzisztens rosszindulatú programkód</td>
<td style="border:1px solid black;">Ideiglenes</td>
<td style="border:1px solid black;">(Nincs)</td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=226382">MS11-081</a></td>
<td style="border:1px solid black;">OLEAuto32.dll távoli programkódfuttatást lehetővé tevő biztonsági rése</td>
<td style="border:1px solid black;"><a href="http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2011-1995">CVE-2011-1995</a></td>
<td style="border:1px solid black;"><a href="http://technet.microsoft.com/en-us/security/cc998259.aspx">1</a> - Valószínűleg konzisztens rosszindulatú programkód</td>
<td style="border:1px solid black;"><a href="http://technet.microsoft.com/en-us/security/cc998259.aspx">1</a> - Valószínűleg konzisztens rosszindulatú programkód</td>
<td style="border:1px solid black;">Ideiglenes</td>
<td style="border:1px solid black;">(Nincs)</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=226382">MS11-081</a></td>
<td style="border:1px solid black;">Beállításelem távoli programkódfuttatást lehetővé tevő biztonsági rése</td>
<td style="border:1px solid black;"><a href="http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2011-1996">CVE-2011-1996</a></td>
<td style="border:1px solid black;">Nem érintett</td>
<td style="border:1px solid black;"><a href="http://technet.microsoft.com/en-us/security/cc998259.aspx">1</a> - Valószínűleg konzisztens rosszindulatú programkód</td>
<td style="border:1px solid black;">Ideiglenes</td>
<td style="border:1px solid black;">(Nincs)</td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=226382">MS11-081</a></td>
<td style="border:1px solid black;">nLoad (betöltési) művelet távoli programkódfuttatást lehetővé tevő biztonsági rése</td>
<td style="border:1px solid black;"><a href="http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2011-1997">CVE-2011-1997</a></td>
<td style="border:1px solid black;">Nem érintett</td>
<td style="border:1px solid black;"><a href="http://technet.microsoft.com/en-us/security/cc998259.aspx">1</a> - Valószínűleg konzisztens rosszindulatú programkód</td>
<td style="border:1px solid black;">Ideiglenes</td>
<td style="border:1px solid black;">(Nincs)</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=226382">MS11-081</a></td>
<td style="border:1px solid black;">Jscript9.dll távoli programkódfuttatást lehetővé tevő biztonsági rése</td>
<td style="border:1px solid black;"><a href="http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2011-1998">CVE-2011-1998</a></td>
<td style="border:1px solid black;"><a href="http://technet.microsoft.com/en-us/security/cc998259.aspx">1</a> - Valószínűleg konzisztens rosszindulatú programkód</td>
<td style="border:1px solid black;">Nem érintett</td>
<td style="border:1px solid black;">Ideiglenes</td>
<td style="border:1px solid black;">(Nincs)</td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=226382">MS11-081</a></td>
<td style="border:1px solid black;">Kiválasztáselem távoli programkódfuttatást lehetővé tevő biztonsági rése</td>
<td style="border:1px solid black;"><a href="http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2011-1999">CVE-2011-1999</a></td>
<td style="border:1px solid black;">Nem érintett</td>
<td style="border:1px solid black;"><a href="http://technet.microsoft.com/en-us/security/cc998259.aspx">2</a> - Valószínűleg inkonzisztens rosszindulatú programkód</td>
<td style="border:1px solid black;">Ideiglenes</td>
<td style="border:1px solid black;">(Nincs)</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=226382">MS11-081</a></td>
<td style="border:1px solid black;">Body elem távoli programkódfuttatást lehetővé tevő biztonsági rése</td>
<td style="border:1px solid black;"><a href="http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2011-2000">CVE-2011-2000</a></td>
<td style="border:1px solid black;"><a href="http://technet.microsoft.com/en-us/security/cc998259.aspx">1</a> - Valószínűleg konzisztens rosszindulatú programkód</td>
<td style="border:1px solid black;"><a href="http://technet.microsoft.com/en-us/security/cc998259.aspx">1</a> - Valószínűleg konzisztens rosszindulatú programkód</td>
<td style="border:1px solid black;">Ideiglenes</td>
<td style="border:1px solid black;">(Nincs)</td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=226382">MS11-081</a></td>
<td style="border:1px solid black;">Virtuális függvénytábla sérülés távoli programkódfuttatást lehetővé tevő biztonsági rése</td>
<td style="border:1px solid black;"><a href="http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2011-2001">CVE-2011-2001</a></td>
<td style="border:1px solid black;"><a href="http://technet.microsoft.com/en-us/security/cc998259.aspx">1</a> - Valószínűleg konzisztens rosszindulatú programkód</td>
<td style="border:1px solid black;"><a href="http://technet.microsoft.com/en-us/security/cc998259.aspx">1</a> - Valószínűleg konzisztens rosszindulatú programkód</td>
<td style="border:1px solid black;">Ideiglenes</td>
<td style="border:1px solid black;">(Nincs)</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=228596">MS11-082</a></td>
<td style="border:1px solid black;">A DoS végtelen ciklus snabase.exe alkalmazásában okozott biztonsági rése</td>
<td style="border:1px solid black;"><a href="http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2011-2007">CVE-2011-2007</a></td>
<td style="border:1px solid black;">Nem érintett</td>
<td style="border:1px solid black;">Nem érintett</td>
<td style="border:1px solid black;">Állandó</td>
<td style="border:1px solid black;">Ez a biztonsági rés szolgáltatásmegtagadást okoz.<br />
<br />
A biztonsági rés nyilvánosságra került.</td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=228596">MS11-082</a></td>
<td style="border:1px solid black;">Nem lefoglalt DoS memória hozzáférésének biztonsági rése</td>
<td style="border:1px solid black;"><a href="http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2011-2008">CVE-2011-2008</a></td>
<td style="border:1px solid black;">Nem érintett</td>
<td style="border:1px solid black;">Nem érintett</td>
<td style="border:1px solid black;">Állandó</td>
<td style="border:1px solid black;">Ez a biztonsági rés szolgáltatásmegtagadást okoz.<br />
<br />
A biztonsági rés nyilvánosságra került.</td>
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
</tr>
<tr>
<th colspan="7">
Windows XP
</th>
</tr>
<tr>
<td style="border:1px solid black;">
**Közlemény azonosítója**
</td>
<td style="border:1px solid black;">
[**MS11-078**](http://go.microsoft.com/fwlink/?linkid=227075)
</td>
<td style="border:1px solid black;">
[**MS11-081**](http://go.microsoft.com/fwlink/?linkid=226382)
</td>
<td style="border:1px solid black;">
[**MS11-075**](http://go.microsoft.com/fwlink/?linkid=221538)
</td>
<td style="border:1px solid black;">
[**MS11-076**](http://go.microsoft.com/fwlink/?linkid=227073)
</td>
<td style="border:1px solid black;">
[**MS11-077**](http://go.microsoft.com/fwlink/?linkid=225915)
</td>
<td style="border:1px solid black;">
[**MS11-080**](http://go.microsoft.com/fwlink/?linkid=227486)
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
</tr>
<tr>
<td style="border:1px solid black;">
Windows XP Service Pack 3
</td>
<td style="border:1px solid black;">
[Microsoft .NET-keretrendszer 1.0 Service Pack 3](http://www.microsoft.com/downloads/details.aspx?familyid=a54a7ad5-0504-4cc6-9eca-ba9f31c35a17)  
(KB2572066)  
(csak Media Center Edition 2005 és Tablet PC Edition 2005)  
(Kritikus)  
[Microsoft .NET-keretrendszer 1.1 Service Pack 1](http://www.microsoft.com/downloads/details.aspx?familyid=6100e577-deb5-4395-b851-e19e0ca79507)  
(KB2572067)  
(Kritikus)  
[Microsoft .NET-keretrendszer 2.0 Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=719b3da5-52ca-4d56-a2c5-69711039e59d)  
(KB2572073)  
(Kritikus)  
[Microsoft .NET Framework 4](http://www.microsoft.com/downloads/details.aspx?familyid=770e7b58-6544-4f59-9893-b3eadf6d6c8a)<sup>[1]</sup>
(KB2572078)  
(Kritikus)
</td>
<td style="border:1px solid black;">
[Internet Explorer 6](http://www.microsoft.com/downloads/details.aspx?familyid=822f91f5-bf92-42c4-ad33-b971be37d772)  
(Kritikus)  
[Internet Explorer 7](http://www.microsoft.com/downloads/details.aspx?familyid=e942554d-6cb6-4e48-a876-3470671a95a2)  
(Kritikus)  
[Internet Explorer 8](http://www.microsoft.com/downloads/details.aspx?familyid=a911b5b0-5e46-4a37-83e7-595e20585c56)  
(Kritikus)
</td>
<td style="border:1px solid black;">
[Windows XP Service Pack 3](http://www.microsoft.com/downloads/details.aspx?familyid=96af60b9-4b8d-4a9b-b125-10775bb48252)  
(KB2564958)  
(Fontos)
</td>
<td style="border:1px solid black;">
Nem érintett
</td>
<td style="border:1px solid black;">
[Windows XP Service Pack 3](http://www.microsoft.com/downloads/details.aspx?familyid=9157e677-ab3f-44b0-9735-192bc7421ba7)  
(Fontos)
</td>
<td style="border:1px solid black;">
[Windows XP Service Pack 3](http://www.microsoft.com/downloads/details.aspx?familyid=f1b2dceb-5bef-4522-9001-8dff0545d805)  
(Fontos)
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
Windows XP Professional x64 Edition Service Pack 2
</td>
<td style="border:1px solid black;">
[Microsoft .NET-keretrendszer 1.1 Service Pack 1](http://www.microsoft.com/downloads/details.aspx?familyid=6100e577-deb5-4395-b851-e19e0ca79507)  
(KB2572067)  
(Kritikus)  
[Microsoft .NET-keretrendszer 2.0 Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=719b3da5-52ca-4d56-a2c5-69711039e59d)  
(KB2572073)  
(Kritikus)  
[Microsoft .NET Framework 4](http://www.microsoft.com/downloads/details.aspx?familyid=770e7b58-6544-4f59-9893-b3eadf6d6c8a)<sup>[1]</sup>
(KB2572078)  
(Kritikus)
</td>
<td style="border:1px solid black;">
[Internet Explorer 6](http://www.microsoft.com/downloads/details.aspx?familyid=6260318c-e579-4cdf-93e3-4608892bc79e)  
(Kritikus)  
[Internet Explorer 7](http://www.microsoft.com/downloads/details.aspx?familyid=f04ad852-1418-4fc4-bd57-f47895bbf3a8)  
(Kritikus)  
[Internet Explorer 8](http://www.microsoft.com/downloads/details.aspx?familyid=67ebf641-1341-4642-96ba-bab5446d7b5d)  
(Kritikus)
</td>
<td style="border:1px solid black;">
[Windows XP Professional x64 Edition Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=c8fcf427-17d0-4caa-b406-50703f980862)  
(KB2564958)  
(Fontos)
</td>
<td style="border:1px solid black;">
Nem érintett
</td>
<td style="border:1px solid black;">
[Windows XP Professional x64 Edition Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=0f2444ac-61bd-47cf-9c1e-da86a2b0cfb5)  
(Fontos)
</td>
<td style="border:1px solid black;">
[Windows XP Professional x64 Edition Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=9a37864e-8543-4c52-aa73-e3c190860d76)  
(Fontos)
</td>
</tr>
<tr>
<th colspan="7">
Windows Server 2003
</th>
</tr>
<tr>
<td style="border:1px solid black;">
**Közlemény azonosítója**
</td>
<td style="border:1px solid black;">
[**MS11-078**](http://go.microsoft.com/fwlink/?linkid=227075)
</td>
<td style="border:1px solid black;">
[**MS11-081**](http://go.microsoft.com/fwlink/?linkid=226382)
</td>
<td style="border:1px solid black;">
[**MS11-075**](http://go.microsoft.com/fwlink/?linkid=221538)
</td>
<td style="border:1px solid black;">
[**MS11-076**](http://go.microsoft.com/fwlink/?linkid=227073)
</td>
<td style="border:1px solid black;">
[**MS11-077**](http://go.microsoft.com/fwlink/?linkid=225915)
</td>
<td style="border:1px solid black;">
[**MS11-080**](http://go.microsoft.com/fwlink/?linkid=227486)
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
[**Fontos**](http://go.microsoft.com/fwlink/?linkid=21140)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Windows Server 2003 Service Pack 2
</td>
<td style="border:1px solid black;">
[Microsoft .NET-keretrendszer 1.1 Service Pack 1](http://www.microsoft.com/downloads/details.aspx?familyid=b968b0bd-577b-4ea2-a192-a80fe7c20791)  
(KB2572069)  
(Kritikus)  
[Microsoft .NET-keretrendszer 2.0 Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=719b3da5-52ca-4d56-a2c5-69711039e59d)  
(KB2572073)  
(Kritikus)  
[Microsoft .NET Framework 4](http://www.microsoft.com/downloads/details.aspx?familyid=770e7b58-6544-4f59-9893-b3eadf6d6c8a)<sup>[1]</sup>
(KB2572078)  
(Kritikus)
</td>
<td style="border:1px solid black;">
[Internet Explorer 6](http://www.microsoft.com/downloads/details.aspx?familyid=172c55f3-6249-4ba3-a4a4-677a03262ff3)  
(Mérsékelt)  
[Internet Explorer 7](http://www.microsoft.com/downloads/details.aspx?familyid=6ffbdb93-7b92-4197-bb6c-5c305e8072a8)  
(Mérsékelt)  
[Internet Explorer 8](http://www.microsoft.com/downloads/details.aspx?familyid=14ef20d4-3530-49b2-91b7-d278d9098023)  
(Mérsékelt)
</td>
<td style="border:1px solid black;">
[Windows Server 2003 Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=09e178f8-2bd2-46e1-b975-4938ee1f304d)  
(KB2564958)  
(Fontos)
</td>
<td style="border:1px solid black;">
Nem érintett
</td>
<td style="border:1px solid black;">
[Windows Server 2003 Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=3bd62bf6-3400-4c03-95fe-148112b341e8)  
(Fontos)
</td>
<td style="border:1px solid black;">
[Windows Server 2003 Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=29228167-b811-43d7-b4a0-91e385b598a5)  
(Fontos)
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
Windows Server 2003 x64 Edition Service Pack 2
</td>
<td style="border:1px solid black;">
[Microsoft .NET-keretrendszer 1.1 Service Pack 1](http://www.microsoft.com/downloads/details.aspx?familyid=6100e577-deb5-4395-b851-e19e0ca79507)  
(KB2572067)  
(Kritikus)  
[Microsoft .NET-keretrendszer 2.0 Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=719b3da5-52ca-4d56-a2c5-69711039e59d)  
(KB2572073)  
(Kritikus)  
[Microsoft .NET Framework 4](http://www.microsoft.com/downloads/details.aspx?familyid=770e7b58-6544-4f59-9893-b3eadf6d6c8a)<sup>[1]</sup>
(KB2572078)  
(Kritikus)
</td>
<td style="border:1px solid black;">
[Internet Explorer 6](http://www.microsoft.com/downloads/details.aspx?familyid=f5a0a8db-34d4-4f0a-ab6b-7b2fb420ab91)  
(Mérsékelt)  
[Internet Explorer 7](http://www.microsoft.com/downloads/details.aspx?familyid=7379b3bf-6af0-43cb-bf8b-505e8563fc84)  
(Mérsékelt)  
[Internet Explorer 8](http://www.microsoft.com/downloads/details.aspx?familyid=b35c95f5-30b0-43a9-aa6a-6db63cab0dcb)  
(Mérsékelt)
</td>
<td style="border:1px solid black;">
[Windows Server 2003 x64 Edition Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=9b8030db-1f47-4666-8cb5-1c56577f2340)  
(KB2564958)  
(Fontos)
</td>
<td style="border:1px solid black;">
Nem érintett
</td>
<td style="border:1px solid black;">
[Windows Server 2003 x64 Edition Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=b73f4e87-9655-46d5-beb2-ea245dcd280d)  
(Fontos)
</td>
<td style="border:1px solid black;">
[Windows Server 2003 x64 Edition Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=0816d729-6769-4ca6-a14e-71750eca8d29)  
(Fontos)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Windows Server 2003 SP2 Itanium-alapú rendszerekhez
</td>
<td style="border:1px solid black;">
[Microsoft .NET-keretrendszer 1.1 Service Pack 1](http://www.microsoft.com/downloads/details.aspx?familyid=6100e577-deb5-4395-b851-e19e0ca79507)  
(KB2572067)  
(Kritikus)  
[Microsoft .NET-keretrendszer 2.0 Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=719b3da5-52ca-4d56-a2c5-69711039e59d)  
(KB2572073)  
(Kritikus)  
[Microsoft .NET Framework 4](http://www.microsoft.com/downloads/details.aspx?familyid=770e7b58-6544-4f59-9893-b3eadf6d6c8a)<sup>[1]</sup>
(KB2572078)  
(Kritikus)
</td>
<td style="border:1px solid black;">
[Internet Explorer 6](http://www.microsoft.com/downloads/details.aspx?familyid=5825cb4a-47d5-423f-b4c5-2d0fc50856c0)  
(Mérsékelt)  
[Internet Explorer 7](http://www.microsoft.com/downloads/details.aspx?familyid=11c4878e-df58-4369-b9c0-cb0a230c92dd)  
(Mérsékelt)
</td>
<td style="border:1px solid black;">
[Windows Server 2003 SP2 Itanium-alapú rendszerekhez](http://www.microsoft.com/downloads/details.aspx?familyid=82653b8c-0e58-440d-9702-8847f599caed)  
(KB2605295)  
(Fontos)
</td>
<td style="border:1px solid black;">
Nem érintett
</td>
<td style="border:1px solid black;">
[Windows Server 2003 SP2 Itanium-alapú rendszerekhez](http://www.microsoft.com/downloads/details.aspx?familyid=a618cc19-5ebc-462e-a518-d9bfe41ed98e)  
(Fontos)
</td>
<td style="border:1px solid black;">
[Windows Server 2003 SP2 Itanium-alapú rendszerekhez](http://www.microsoft.com/downloads/details.aspx?familyid=42465652-2664-4fd5-9a22-ae847b08e7c8)  
(Fontos)
</td>
</tr>
<tr>
<th colspan="7">
Windows Vista
</th>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
**Közlemény azonosítója**
</td>
<td style="border:1px solid black;">
[**MS11-078**](http://go.microsoft.com/fwlink/?linkid=227075)
</td>
<td style="border:1px solid black;">
[**MS11-081**](http://go.microsoft.com/fwlink/?linkid=226382)
</td>
<td style="border:1px solid black;">
[**MS11-075**](http://go.microsoft.com/fwlink/?linkid=221538)
</td>
<td style="border:1px solid black;">
[**MS11-076**](http://go.microsoft.com/fwlink/?linkid=227073)
</td>
<td style="border:1px solid black;">
[**MS11-077**](http://go.microsoft.com/fwlink/?linkid=225915)
</td>
<td style="border:1px solid black;">
[**MS11-080**](http://go.microsoft.com/fwlink/?linkid=227486)
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
<td style="border:1px solid black;">
[**Fontos**](http://go.microsoft.com/fwlink/?linkid=21140)
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
[Microsoft .NET-keretrendszer 1.1 Service Pack 1](http://www.microsoft.com/downloads/details.aspx?familyid=6100e577-deb5-4395-b851-e19e0ca79507)  
(KB2572067)  
(Kritikus)  
[Microsoft .NET-keretrendszer 2.0 Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=7c27128d-eaf9-4416-b8b1-9edab9102feb)  
(KB2572075)  
(Kritikus)  
[Microsoft .NET Framework 4](http://www.microsoft.com/downloads/details.aspx?familyid=770e7b58-6544-4f59-9893-b3eadf6d6c8a)<sup>[1]</sup>
(KB2572078)  
(Kritikus)
</td>
<td style="border:1px solid black;">
[Internet Explorer 7](http://www.microsoft.com/downloads/details.aspx?familyid=630335ac-5a30-46b4-acc1-c4d8bd289668)  
(Kritikus)  
[Internet Explorer 8](http://www.microsoft.com/downloads/details.aspx?familyid=76c8124e-81b9-4a6a-bd53-fbdaf45189aa)  
(Kritikus)  
[Internet Explorer 9](http://www.microsoft.com/downloads/details.aspx?familyid=7de276a3-a20d-49de-82b0-51cb22ad73af)  
(Kritikus)
</td>
<td style="border:1px solid black;">
[Windows Vista Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=96b089c0-a2e7-44cb-9fc4-9569b3993afa)  
(KB2564958)  
(Fontos)
</td>
<td style="border:1px solid black;">
[Windows Vista Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=44f7f10b-86ff-470f-996a-d4aa51c4d18f)  
(KB2579686)  
(Fontos)  
[Windows Media Center TV Pack for Windows Vista (32 bites kiadások](http://www.microsoft.com/downloads/details.aspx?familyid=60e50f72-4001-423c-831c-8ff1f1b8f090))<sup>[1]</sup>
(KB2579692)  
(Fontos)
</td>
<td style="border:1px solid black;">
[Windows Vista Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=ff53d01b-97b7-40d2-af88-4978f1099a7c)  
(Fontos)
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
[Microsoft .NET-keretrendszer 1.1 Service Pack 1](http://www.microsoft.com/downloads/details.aspx?familyid=6100e577-deb5-4395-b851-e19e0ca79507)  
(KB2572067)  
(Kritikus)  
[Microsoft .NET-keretrendszer 2.0 Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=7c27128d-eaf9-4416-b8b1-9edab9102feb)  
(KB2572075)  
(Kritikus)  
[Microsoft .NET Framework 4](http://www.microsoft.com/downloads/details.aspx?familyid=770e7b58-6544-4f59-9893-b3eadf6d6c8a)<sup>[1]</sup>
(KB2572078)  
(Kritikus)
</td>
<td style="border:1px solid black;">
[Internet Explorer 7](http://www.microsoft.com/downloads/details.aspx?familyid=9aabd7a2-0b2f-4c42-a9cf-2ec69ae6b82d)  
(Kritikus)  
[Internet Explorer 8](http://www.microsoft.com/downloads/details.aspx?familyid=3454940c-acc2-4e09-8154-075b4be1b697)  
(Kritikus)  
[Internet Explorer 9](http://www.microsoft.com/downloads/details.aspx?familyid=3df0c31b-344a-4163-93d2-79df1653b339)  
(Kritikus)
</td>
<td style="border:1px solid black;">
[Windows Vista x64 Edition Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=b79a389c-8340-4dd2-9ab1-a0943c5a220f)  
(KB2564958)  
(Fontos)
</td>
<td style="border:1px solid black;">
[Windows Vista x64 Edition Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=cbb66cd7-2688-410f-8a03-fd28e6ef5b01)  
(KB2579686)  
(Fontos)  
[Windows Media Center TV Pack for Windows Vista (64 bites kiadások](http://www.microsoft.com/downloads/details.aspx?familyid=371c7dab-5aa6-4502-80ee-ae69b736b972))<sup>[1]</sup>
(KB2579692)  
(Fontos)
</td>
<td style="border:1px solid black;">
[Windows Vista x64 Edition Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=47322e11-f1cf-4f70-b939-8cac9bbfc2bc)  
(Fontos)
</td>
<td style="border:1px solid black;">
Nem érintett
</td>
</tr>
<tr>
<th colspan="7">
Windows Server 2008
</th>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
**Közlemény azonosítója**
</td>
<td style="border:1px solid black;">
[**MS11-078**](http://go.microsoft.com/fwlink/?linkid=227075)
</td>
<td style="border:1px solid black;">
[**MS11-081**](http://go.microsoft.com/fwlink/?linkid=226382)
</td>
<td style="border:1px solid black;">
[**MS11-075**](http://go.microsoft.com/fwlink/?linkid=221538)
</td>
<td style="border:1px solid black;">
[**MS11-076**](http://go.microsoft.com/fwlink/?linkid=227073)
</td>
<td style="border:1px solid black;">
[**MS11-077**](http://go.microsoft.com/fwlink/?linkid=225915)
</td>
<td style="border:1px solid black;">
[**MS11-080**](http://go.microsoft.com/fwlink/?linkid=227486)
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
Nincsenek
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
Windows Server 2008 32 bites rendszerekhez, Service Pack 2
</td>
<td style="border:1px solid black;">
[Microsoft .NET Framework 1.1 Service Pack 1](http://www.microsoft.com/downloads/details.aspx?familyid=6100e577-deb5-4395-b851-e19e0ca79507)\*\*  
(KB2572067)  
(Kritikus)  
[Microsoft .NET-keretrendszer 2.0 Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=7c27128d-eaf9-4416-b8b1-9edab9102feb)\*\*  
(KB2572075)  
(Kritikus)  
[Microsoft .NET Framework 4](http://www.microsoft.com/downloads/details.aspx?familyid=770e7b58-6544-4f59-9893-b3eadf6d6c8a)\*\*<sup>[1]</sup>
(KB2572078)  
(Kritikus)
</td>
<td style="border:1px solid black;">
[Internet Explorer 7](http://www.microsoft.com/downloads/details.aspx?familyid=5660e23c-13a3-4275-ac69-38f03f17491a)\*\*  
(Mérsékelt)  
[Internet Explorer 8](http://www.microsoft.com/downloads/details.aspx?familyid=bd144435-1afd-4d6e-a100-fbd613eee409)\*\*  
(Mérsékelt)  
[Internet Explorer 9](http://www.microsoft.com/downloads/details.aspx?familyid=1a7f9855-20ce-4fe0-a903-bd1f145075df)\*\*  
(Mérsékelt)
</td>
<td style="border:1px solid black;">
[Windows Server 2008 32 bites rendszerekhez, Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=7cd1ecec-8a3f-4cb2-833c-a177c9602ff5)\*  
(KB2564958)  
(Fontos)
</td>
<td style="border:1px solid black;">
Nem érintett
</td>
<td style="border:1px solid black;">
[Windows Server 2008 32 bites rendszerekhez, Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=7c7498ee-eba4-44fd-8846-0b2e96c96705)\*  
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
[Microsoft .NET Framework 1.1 Service Pack 1](http://www.microsoft.com/downloads/details.aspx?familyid=6100e577-deb5-4395-b851-e19e0ca79507)\*\*  
(KB2572067)  
(Kritikus)  
[Microsoft .NET-keretrendszer 2.0 Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=7c27128d-eaf9-4416-b8b1-9edab9102feb)\*\*  
(KB2572075)  
(Kritikus)  
[Microsoft .NET Framework 4](http://www.microsoft.com/downloads/details.aspx?familyid=770e7b58-6544-4f59-9893-b3eadf6d6c8a)\*\*<sup>[1]</sup>
(KB2572078)  
(Kritikus)
</td>
<td style="border:1px solid black;">
[Internet Explorer 7](http://www.microsoft.com/downloads/details.aspx?familyid=415b1c59-f3dc-4f4f-b2eb-68692d6efc05)\*\*  
(Mérsékelt)  
[Internet Explorer 8](http://www.microsoft.com/downloads/details.aspx?familyid=b0c4949f-bce0-4255-a5f2-cf5ecf7416da)\*\*  
(Mérsékelt)  
[Internet Explorer 9](http://www.microsoft.com/downloads/details.aspx?familyid=28a09e42-5865-48b2-af26-ebc8162c3286)\*\*  
(Mérsékelt)
</td>
<td style="border:1px solid black;">
[Windows Server 2008 x64 alapú rendszerekhez, Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=456e450c-3928-4130-8127-e4d3f482c1ca)\*  
(KB2564958)  
(Fontos)
</td>
<td style="border:1px solid black;">
Nem érintett
</td>
<td style="border:1px solid black;">
[Windows Server 2008 x64 alapú rendszerekhez, Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=40386742-f397-402e-8810-63d3d6ba12a6)\*  
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
[Microsoft .NET-keretrendszer 1.1 Service Pack 1](http://www.microsoft.com/downloads/details.aspx?familyid=6100e577-deb5-4395-b851-e19e0ca79507)  
(KB2572067)  
(Kritikus)  
[Microsoft .NET-keretrendszer 2.0 Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=7c27128d-eaf9-4416-b8b1-9edab9102feb)  
(KB2572075)  
(Kritikus)  
[Microsoft .NET Framework 4](http://www.microsoft.com/downloads/details.aspx?familyid=770e7b58-6544-4f59-9893-b3eadf6d6c8a)<sup>[1]</sup>
(KB2572078)  
(Kritikus)
</td>
<td style="border:1px solid black;">
[Internet Explorer 7](http://www.microsoft.com/downloads/details.aspx?familyid=31e68c7f-4db5-463f-a315-92f574af080b)  
(Mérsékelt)
</td>
<td style="border:1px solid black;">
[Windows Server 2008 Itanium-alapú rendszerekhez, Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=2e9930d3-ba13-446d-bfa0-60720c48203b)  
(KB2564958)  
(Fontos)
</td>
<td style="border:1px solid black;">
Nem érintett
</td>
<td style="border:1px solid black;">
[Windows Server 2008 Itanium-alapú rendszerekhez, Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=3633402b-96cb-4f36-b137-d07d1baf28c7)  
(Fontos)
</td>
<td style="border:1px solid black;">
Nem érintett
</td>
</tr>
<tr>
<th colspan="7">
Windows 7
</th>
</tr>
<tr>
<td style="border:1px solid black;">
**Közlemény azonosítója**
</td>
<td style="border:1px solid black;">
[**MS11-078**](http://go.microsoft.com/fwlink/?linkid=227075)
</td>
<td style="border:1px solid black;">
[**MS11-081**](http://go.microsoft.com/fwlink/?linkid=226382)
</td>
<td style="border:1px solid black;">
[**MS11-075**](http://go.microsoft.com/fwlink/?linkid=221538)
</td>
<td style="border:1px solid black;">
[**MS11-076**](http://go.microsoft.com/fwlink/?linkid=227073)
</td>
<td style="border:1px solid black;">
[**MS11-077**](http://go.microsoft.com/fwlink/?linkid=225915)
</td>
<td style="border:1px solid black;">
[**MS11-080**](http://go.microsoft.com/fwlink/?linkid=227486)
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
<td style="border:1px solid black;">
[**Fontos**](http://go.microsoft.com/fwlink/?linkid=21140)
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
Csak Windows 7 32 bites rendszerekhez:  
[Microsoft .NET-keretrendszer 3.5.1](http://www.microsoft.com/downloads/details.aspx?familyid=81be7ff1-3ba2-430c-9edf-619cc246daf2)  
(KB2572076)  
(Kritikus)  
Csak Windows 7 32 bites rendszerekhez, Service Pack 1:  
[Microsoft .NET-keretrendszer 3.5.1](http://www.microsoft.com/downloads/details.aspx?familyid=98403988-7438-4260-95b5-a4796dbe0618)  
(KB2572077)  
(Kritikus)  
[Microsoft .NET Framework 4](http://www.microsoft.com/downloads/details.aspx?familyid=770e7b58-6544-4f59-9893-b3eadf6d6c8a)<sup>[1]</sup>
(KB2572078)  
(Kritikus)
</td>
<td style="border:1px solid black;">
[Internet Explorer 8](http://www.microsoft.com/downloads/details.aspx?familyid=4de175be-bbb7-4912-ba4e-d6fe96606c9e)  
(Kritikus)  
[Internet Explorer 9](http://www.microsoft.com/downloads/details.aspx?familyid=b49876c7-7c65-4b6d-be9a-9f18be23037b)  
(Kritikus)
</td>
<td style="border:1px solid black;">
[Windows 7 32 bites rendszerekhez és Windows 7 32 bites rendszerekhez Service Pack 1](http://www.microsoft.com/downloads/details.aspx?familyid=02d28e59-b38f-433a-a568-e86f9d43dd42)  
(KB2564958)  
(Fontos)
</td>
<td style="border:1px solid black;">
[Windows 7 32 bites rendszerekhez és Windows 7 32 bites rendszerekhez Service Pack 1](http://www.microsoft.com/downloads/details.aspx?familyid=76fcf0ec-9062-4090-acb2-401355341a2b)  
(KB2579686)  
(Fontos)
</td>
<td style="border:1px solid black;">
[Windows 7 32 bites rendszerekhez és Windows 7 32 bites rendszerekhez Service Pack 1](http://www.microsoft.com/downloads/details.aspx?familyid=9e40bc26-f77f-4b57-9b3d-9d053c19ac56)  
(Fontos)
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
Csak Windows 7 x64 alapú rendszerekhez:  
[Microsoft .NET-keretrendszer 3.5.1](http://www.microsoft.com/downloads/details.aspx?familyid=81be7ff1-3ba2-430c-9edf-619cc246daf2)  
(KB2572076)  
(Kritikus)  
Csak Windows 7 x64-alapú rendszerekhez, Service Pack 1:  
[Microsoft .NET-keretrendszer 3.5.1](http://www.microsoft.com/downloads/details.aspx?familyid=98403988-7438-4260-95b5-a4796dbe0618)  
(KB2572077)  
(Kritikus)  
[Microsoft .NET Framework 4](http://www.microsoft.com/downloads/details.aspx?familyid=770e7b58-6544-4f59-9893-b3eadf6d6c8a)<sup>[1]</sup>
(KB2572078)  
(Kritikus)
</td>
<td style="border:1px solid black;">
[Internet Explorer 8](http://www.microsoft.com/downloads/details.aspx?familyid=16fd238e-6f65-4d38-88ae-2689817588e1)  
(Kritikus)  
[Internet Explorer 9](http://www.microsoft.com/downloads/details.aspx?familyid=cc0773f2-6099-4d55-9971-ee6546369c7f)  
(Kritikus)
</td>
<td style="border:1px solid black;">
[Windows 7 x64 alapú rendszerekhez és Windows 7 x64 alapú rendszerekhez Service Pack 1](http://www.microsoft.com/downloads/details.aspx?familyid=904dec69-e8b9-4b23-a5ea-d3e7e9b9df07)  
(KB2564958)  
(Fontos)
</td>
<td style="border:1px solid black;">
[Windows 7 x64 alapú rendszerekhez és Windows 7 x64 alapú rendszerekhez Service Pack 1](http://www.microsoft.com/downloads/details.aspx?familyid=78c099b7-4bcb-4da7-8967-512c6541c541)  
(KB2579686)  
(Fontos)
</td>
<td style="border:1px solid black;">
[Windows 7 x64 alapú rendszerekhez és Windows 7 x64 alapú rendszerekhez Service Pack 1](http://www.microsoft.com/downloads/details.aspx?familyid=219554e6-eb5a-42d0-90c0-42b4d0772cfd)  
(Fontos)
</td>
<td style="border:1px solid black;">
Nem érintett
</td>
</tr>
<tr>
<th colspan="7">
Windows Server 2008 R2
</th>
</tr>
<tr>
<td style="border:1px solid black;">
**Közlemény azonosítója**
</td>
<td style="border:1px solid black;">
[**MS11-078**](http://go.microsoft.com/fwlink/?linkid=227075)
</td>
<td style="border:1px solid black;">
[**MS11-081**](http://go.microsoft.com/fwlink/?linkid=226382)
</td>
<td style="border:1px solid black;">
[**MS11-075**](http://go.microsoft.com/fwlink/?linkid=221538)
</td>
<td style="border:1px solid black;">
[**MS11-076**](http://go.microsoft.com/fwlink/?linkid=227073)
</td>
<td style="border:1px solid black;">
[**MS11-077**](http://go.microsoft.com/fwlink/?linkid=225915)
</td>
<td style="border:1px solid black;">
[**MS11-080**](http://go.microsoft.com/fwlink/?linkid=227486)
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
Nincsenek
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Windows Server 2008 R2 x64 alapú rendszerekhez és Windows Server 2008 R2 x64 alapú rendszerekhez Service Pack 1
</td>
<td style="border:1px solid black;">
Csak Windows Server 2008 R2 x64 alapú rendszerekhez:  
[Microsoft .NET Framework 3.5.1](http://www.microsoft.com/downloads/details.aspx?familyid=81be7ff1-3ba2-430c-9edf-619cc246daf2)\*  
(KB2572076)  
(Kritikus)  
Csak Windows Server 2008 R2 x64 alapú rendszerekhez:  
[Microsoft .NET Framework 4](http://www.microsoft.com/downloads/details.aspx?familyid=770e7b58-6544-4f59-9893-b3eadf6d6c8a)<sup>[1]</sup>
(KB2572078)  
(Kritikus)  
Csak Windows Server 2008 R2 x64-alapú rendszerekhez, Service Pack 1:  
[Microsoft .NET Framework 3.5.1](http://www.microsoft.com/downloads/details.aspx?familyid=98403988-7438-4260-95b5-a4796dbe0618)\*  
(KB2572077)  
(Kritikus)  
Csak Windows Server 2008 R2 x64-alapú rendszerekhez, Service Pack 1:  
[Microsoft .NET Framework 4](http://www.microsoft.com/downloads/details.aspx?familyid=770e7b58-6544-4f59-9893-b3eadf6d6c8a)\*<sup>[1]</sup>
(KB2572078)  
(Kritikus)
</td>
<td style="border:1px solid black;">
[Internet Explorer 8](http://www.microsoft.com/downloads/details.aspx?familyid=8435781e-0f77-41d0-abb9-9b70f5b02d33)\*\*  
(Mérsékelt)  
[Internet Explorer 9](http://www.microsoft.com/downloads/details.aspx?familyid=646a9a56-c343-45cb-a255-303602aa5a64)\*\*  
(Mérsékelt)
</td>
<td style="border:1px solid black;">
[Windows Server 2008 R2 x64 alapú rendszerekhez és Windows Server 2008 R2 x64 alapú rendszerekhez Service Pack 1](http://www.microsoft.com/downloads/details.aspx?familyid=c7bd50b7-03f1-4ea4-ad71-d428822c62f8)\*  
(KB2564958)  
(Fontos)
</td>
<td style="border:1px solid black;">
Nem érintett
</td>
<td style="border:1px solid black;">
[Windows Server 2008 R2 x64 alapú rendszerekhez és Windows Server 2008 R2 x64 alapú rendszerekhez Service Pack 1](http://www.microsoft.com/downloads/details.aspx?familyid=39bd4cfb-fe61-41b8-a5a2-73a9e720fc72)\*  
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
Csak Windows Server 2008 R2 Itanium-alapú rendszerekhez:  
[Microsoft .NET-keretrendszer 3.5.1](http://www.microsoft.com/downloads/details.aspx?familyid=81be7ff1-3ba2-430c-9edf-619cc246daf2)  
(KB2572076)  
(Kritikus)  
Csak Windows Server 2008 R2 Itanium-alapú rendszerekhez, Service Pack 1:  
[Microsoft .NET-keretrendszer 3.5.1](http://www.microsoft.com/downloads/details.aspx?familyid=98403988-7438-4260-95b5-a4796dbe0618)  
(KB2572077)  
(Kritikus)  
[Microsoft .NET Framework 4](http://www.microsoft.com/downloads/details.aspx?familyid=770e7b58-6544-4f59-9893-b3eadf6d6c8a)<sup>[1]</sup>
(KB2572078)  
(Kritikus)
</td>
<td style="border:1px solid black;">
[Internet Explorer 8](http://www.microsoft.com/downloads/details.aspx?familyid=2676597e-c1d4-4397-8dc4-515ce3d0c5fd)  
(Mérsékelt)
</td>
<td style="border:1px solid black;">
[Windows Server 2008 R2 Itanium alapú rendszerekhez és Windows Server 2008 R2 Itanium alapú rendszerekhez Service Pack 1](http://www.microsoft.com/downloads/details.aspx?familyid=aa816682-9652-433c-b1b4-5d0bc17b6a87)  
(KB2564958)  
(Fontos)
</td>
<td style="border:1px solid black;">
Nem érintett
</td>
<td style="border:1px solid black;">
[Windows Server 2008 R2 Itanium alapú rendszerekhez és Windows Server 2008 R2 Itanium alapú rendszerekhez Service Pack 1](http://www.microsoft.com/downloads/details.aspx?familyid=0d35c6d0-6d2d-42bf-a97f-4c5e01b1937e)  
(Fontos)
</td>
<td style="border:1px solid black;">
Nem érintett
</td>
</tr>
</table>
 
**Megjegyzések** **a Windows Server 2008 és Windows Server 2008 R2 rendszerhez**

**\*Érinti a kiszolgálómag telepítését.** Ez a frissítés ugyanolyan biztonsági besorolás mellett, a megadottak szerint érvényes az Windows Server 2008 és a Windows Server 2008 R2 összes támogatott kiadására, függetlenül attól, hogy a kiszolgálómag-telepítési opcióval telepítették-e. Erről a telepítési opcióról bővebben a [Kiszolgálómag-telepítés kezelése](http://technet.microsoft.com/en-us/library/ee441255(ws.10).aspx) és [Kiszolgálómag-telepítés szervizelése](http://technet.microsoft.com/en-us/library/ff698994(ws.10).aspx) TechNet cikkekben olvashat. A kiszolgálómag-telepítési opció nem vonatkozik a Windows Server 2008 és a Windows Server 2008 R2 bizonyos kiadásaira; lásd: [A kiszolgálómag-telepítési opciók összehasonlítása](http://www.microsoft.com/windowsserver2008/en/us/compare-core-installation.aspx).

**\*\*A kiszolgálómag-telepítés nem érintett.** A frissítésben tárgyalt biztonsági rések nem érintik a jelzett módon a Windows Server 2008 és a Windows Server 2008 R2 támogatott kiadásait, amennyiben a telepítés a kiszolgálómag-telepítési opció használatával történt. Erről a telepítési opcióról bővebben a [Kiszolgálómag-telepítés kezelése](http://technet.microsoft.com/en-us/library/ee441255(ws.10).aspx) és [Kiszolgálómag-telepítés szervizelése](http://technet.microsoft.com/en-us/library/ff698994(ws.10).aspx) TechNet cikkekben olvashat. A kiszolgálómag-telepítési opció nem vonatkozik a Windows Server 2008 és a Windows Server 2008 R2 bizonyos kiadásaira; lásd: [A kiszolgálómag-telepítési opciók összehasonlítása](http://www.microsoft.com/windowsserver2008/en/us/compare-core-installation.aspx).

**Megjegyzés az MS11-078 számú közleményhez**

<sup>[1]</sup>**A .NET Framework 4 verziója és a .NET Framework 4 verziójához tartozó ügyfélprofil.** A .NET-keretrendszer 4-es verziójú terjeszthető csomagjai két profilban érhetőek el: a .NET Framework 4 és a .NET Framework 4 verziójához tartozó ügyfélprofil. A .NET Framework 4 verziójához tartozó ügyfélprofil a .NET Framework 4 részhalmaza. Az ebben a frissítésben tárgyalt biztonsági rés egyaránt érinti a .NET Framework 4 verzióját és a .NET Framework 4 verziójához tartozó ügyfélprofilt is. További információk [A .NET keretrendszer telepítése](http://msdn.microsoft.com/en-us/library/5a4x27ek.aspx) c. MSDN cikkben.

Az ugyanezen a közleményazonosító alatt található, további frissített fájlokat illetően lásd még az egyéb szoftverkategóriák részt ebben a fejezetben, **Érintett szoftverek és letöltési helyek**. Ez a közlemény több szoftverkategóriát ölel fel.

**Megjegyzés az MS11-076 számú közleményhez**

<sup>[1]</sup>A Windows Media Center TV Pack for Windows Vista kizárólag az eredeti berendezésgyártótól (OEM) beszerzett Windows Vista Home Premium és Ultimate kiadásaihoz érhető el, opcionális összetevőként. Ha telepítette x64-alapú rendszerére ezt az opcionális összetevőt, mindkét elérhető frissítést telepítse. A bevett gyakorlat azt mutatja, hogy érdemes előbb telepíteni az operációs rendszer frissítését (KB2579686), és csak azután a Windows Media Center TV Pack frissítését (KB2579692). A Media Center TV Pack alkalmazást 32-bites rendszerre telepítő felhasználóknak kizárólag a KB2579692 számú frissítést kell telepíteniük.

#### Microsoft Server Software

 
<p> </p>
<table style="border:1px solid black;">
<tr>
<th colspan="2">
Microsoft Host Integration Server
</th>
</tr>
<tr>
<td style="border:1px solid black;">
**Közlemény azonosítója**
</td>
<td style="border:1px solid black;">
[**MS11-082**](http://go.microsoft.com/fwlink/?linkid=228596)
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
Microsoft Host Integration Server 2004
</td>
<td style="border:1px solid black;">
[Microsoft Host Integration Server 2004 SP1](http://www.microsoft.com/downloads/details.aspx?familyid=b7536139-63ea-482a-8d1c-0faad1fcfaa4)  
(KB2578757)  
(Fontos)
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
Microsoft Host Integration Server 2006
</td>
<td style="border:1px solid black;">
[Microsoft Host Integration Server 2006 Service Pack 1](http://www.microsoft.com/downloads/details.aspx?familyid=3bc0c89c-56b2-4463-b671-2a58bed9667b)  
(KB2579597)  
(Fontos)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Microsoft Host Integration Server 2009
</td>
<td style="border:1px solid black;">
[Microsoft Host Integration Server 2009](http://www.microsoft.com/downloads/details.aspx?familyid=28716ed4-f215-4c69-b6b8-63fbeecefc5b)  
(KB2579598)  
(Fontos)
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
Microsoft Host Integration Server 2010
</td>
<td style="border:1px solid black;">
[Microsoft Host Integration Server 2010](http://www.microsoft.com/downloads/details.aspx?familyid=dbbd67d8-68aa-424d-8eaf-a273a71624d1)  
(KB2579599)  
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
[**MS11-078**](http://go.microsoft.com/fwlink/?linkid=227075)
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
Microsoft Silverlight 4
</td>
<td style="border:1px solid black;">
Mac számítógépre telepített [Microsoft Silverlight 4](http://www.microsoft.com/downloads/details.aspx?familyid=8bde4992-bdf7-4345-835a-4e1fbfcd8c5f) alkalmazás  
(KB2617986)  
A [Microsoft Silverlight 4](http://www.microsoft.com/downloads/details.aspx?familyid=8bde4992-bdf7-4345-835a-4e1fbfcd8c5f) Microsoft Windows ügyfelek minden támogatott kiadására telepített verziója esetén  
(KB2617986)  
[Microsoft Silverlight 4](http://www.microsoft.com/downloads/details.aspx?familyid=8bde4992-bdf7-4345-835a-4e1fbfcd8c5f)Microsoft Windows ügyfelek minden támogatott kiadására telepített verziója esetén\*\*  
(KB2617986)
</td>
</tr>
</table>
 
**Megjegyzések** **az MS11-078 számú közleményhez**

**\*\*A kiszolgálómag-telepítés nem érintett.** A frissítésben tárgyalt biztonsági rések nem érintik a jelzett módon a Windows Server 2008 és a Windows Server 2008 R2 támogatott kiadásait, amennyiben a telepítés a kiszolgálómag-telepítési opció használatával történt. Erről a telepítési opcióról bővebben a [Kiszolgálómag-telepítés kezelése](http://technet.microsoft.com/en-us/library/ee441255(ws.10).aspx) és [Kiszolgálómag-telepítés szervizelése](http://technet.microsoft.com/en-us/library/ff698994(ws.10).aspx) TechNet cikkekben olvashat. A kiszolgálómag-telepítési opció nem vonatkozik a Windows Server 2008 és a Windows Server 2008 R2 bizonyos kiadásaira; lásd: [A kiszolgálómag-telepítési opciók összehasonlítása](http://www.microsoft.com/windowsserver2008/en/us/compare-core-installation.aspx).

Az ugyanezen a közleményazonosító alatt található, további frissített fájlokat illetően lásd még az egyéb szoftverkategóriák részt ebben a fejezetben, **Érintett szoftverek és letöltési helyek**. Ez a közlemény több szoftverkategóriát ölel fel.

#### Microsoft távelérési szoftver

 
<p> </p>
<table style="border:1px solid black;">
<tr>
<th colspan="2">
Microsoft Forefront Unified Access Gateway
</th>
</tr>
<tr>
<td style="border:1px solid black;">
**Közlemény azonosítója**
</td>
<td style="border:1px solid black;">
[**MS11-079**](http://go.microsoft.com/fwlink/?linkid=217472)
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
Microsoft Forefront Unified Access Gateway
</td>
<td style="border:1px solid black;">
[Microsoft Forefront Unified Access Gateway 2010](http://www.microsoft.com/downloads/details.aspx?familyid=770ad8ba-4d9a-404e-9515-6ed1e41682df)<sup>[1]</sup>
(KB2522482)  
(Fontos)  
[Microsoft Forefront Unified Access Gateway 2010 Update 1](http://www.microsoft.com/downloads/details.aspx?familyid=b0de8d20-9c25-41c0-9c02-d263b9ed22fa)<sup>[1]</sup>
(KB2522483)  
(Fontos)  
[Microsoft Forefront Unified Access Gateway 2010 Update 2](http://www.microsoft.com/downloads/details.aspx?familyid=166bdfcb-5088-4471-9d51-a3071ac13b73)<sup>[1]</sup>
(KB2522484)  
(Fontos)  
[Microsoft Forefront Unified Access Gateway 2010 Service Pack 1](http://www.microsoft.com/downloads/details.aspx?familyid=8b6ad2ae-e168-45d9-bd3f-5590e0cbd2b5)<sup>[1]</sup>
(KB2522485)  
(Fontos)
</td>
</tr>
</table>
 
**Megjegyzés az** **MS11-079** közleményhez

<sup>[1]</sup>Ez a frissítés kizárólag a Microsoft letöltő központból érhető el.

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

Az alkalmazások működése érdekében a frissítések gyakran írnak ugyanazokba a fájlokba, illetve regisztrációs bejegyzésekbe. Ez inkompatibilitást okozhat, és növelheti a biztonsági frissítések központi telepítésére használt időt. A Windows frissítések és az alkalmazásoknak való megfelelőség tesztelése és ellenőrzése egyszerűsíthető az [Update Compatibility Evaluator](http://technet2.microsoft.com/windowsvista/en/library/4279e239-37a4-44aa-aec5-4e70fe39f9de1033.mspx?mfr=true) összetevőivel, amelyek az [Application Compatibility Toolkit](http://www.microsoft.com/downloads/details.aspx?familyid=24da89e9-b581-47b0-b45e-492dd6da2971&displaylang=hu) alkalmazáskompatibilitási eszközkészletben megtalálhatók.

Az Application Compatibility Toolkit (ACT) tartalmazza a Microsoft Windows Vista, a Windows Update, a Microsoft Security Update vagy a Windows Internet Explorer új verziójának központi telepítése előtt az alkalmazáskompatibilitási problémák kiértékeléséhez és enyhítéséhez szükséges eszközöket és dokumentációt.

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

-   [Mila Parkour](http://contagiodump.com), valamint Anshul Kothari és Nishant Kaushik, [Adobe Systems, Inc.](http://www.adobe.com), az MS11-075 közleményben bemutatott probléma jelentéséért
-   Andrei Lutas, [BitDefender](http://www.bitdefender.com/), az MS11-077 közleményben ismertetett probléma jelentéséért
-   Tarjei Mandt, [Norman](http://www.norman.com/), az MS11-077 számú közleményben bemutatott probléma jelentéséért
-   Maik Wellmann, az MS11-077 közleményben ismertetett probléma jelentéséért
-   Will Dorman, [CERT/CC,](http://www.cert.org/) az MS11-077 közleményben ismertetett probléma jelentéséért
-   A [Beyond Security SecuriTeam Secure Disclosure](http://www.beyondsecurity.com/ssd.html) programjában részt vevő anonim kutató, az MS11-078 közleményben ismertetett probléma jelentéséért
-   [Tenable Network Security](http://www.tenable.com/), az MS11-079 közleményben ismertetett három probléma jelentéséért
-   Elisabeth Demeter, [SEC Consult Unternehmensberatung GmbH](http://www.sec-consult.com/), az MS11-079 közleményben ismertetett probléma jelentéséért
-   Bo Zhou, [National University of Defense Technology](http://www.nudt.edu.cn/), az MS11-080 közleményben ismertetett probléma jelentéséért
-   Vishwas Sharma, McAfee Labs, az MS11-081 közleményben bemutatott probléma jelentéséért
-   David Bloom, [Greplin](https://www.greplin.com), az MS11-081 közleményben bemutatott két probléma jelentéséért
-   Ivan Fratric, a [TippingPoint](http://www.tippingpoint.com)[Zero Day Initiative](http://www.zerodayinitiative.com/) programjával együttműködésben, az MS11-081 közleményben ismertetett két probléma jelentéséért
-   [GWSlabs](http://www.gwslabs.com), [VeriSign iDefense Labs](http://labs.idefense.com), az MS11-081 közleményben ismertetett probléma jelentéséért
-   Sebastian Apelt, a [TippingPoint](http://www.tippingpoint.com)[Zero Day Initiative](http://www.zerodayinitiative.com/) programjával együttműködésben, az MS11-081 közleményben ismertetett probléma jelentéséért
-   A [Tipping Point](http://www.tippingpoint.com)[Zero Day Initiative](http://www.zerodayinitiative.com/) programjában részt vevő anonim kutató, az MS11-081 közleményben ismertetett probléma jelentéséért
-   Eduardo Vela Nava, [Google Inc.](http://www.google.com), és David Bloom, [Greplin](https://www.greplin.com), az MS11-081 közleményben ismertetett mélyreható biztonsági megoldásokkal kapcsolatos együttműködésért
-   [Soroush Dalili](http://www.secproject.com), az MS11-081 közleményben ismertetett mélyreható biztonsági megoldásokkal kapcsolatos együttműködésért
-   Billy Rios, [Google Inc.](http://www.google.com), az MS11-081 közleményben ismertetett mélyreható biztonsági megoldásokkal kapcsolatos együttműködésért

#### Terméktámogatás

-   Teszteléssel állapították meg a felsorolt szoftverek egyes verzióinak érintettségét. A többi verzió támogatási életciklusa végére ért. Az egyes szoftververziók támogatási életciklusáról a [Microsoft termékek terméktámogatási életciklusát ismertető webhelyen](http://go.microsoft.com/fwlink/?linkid=21742) talál felvilágosítást.
-   Az Amerikai Egyesült Államokban és Kanada területén élő ügyfelek technikai támogatást kérhetnek a [biztonsági támogatás szolgáltatójától](http://go.microsoft.com/fwlink/?linkid=21131) vagy az 1-866-PCSAFETY telefonszámon. A biztonsági frissítésekkel kapcsolatos hívások ingyenesek. Az elérhető támogatási lehetőségekről további információt talál a [Microsoft segítségnyújtással és támogatással foglalkozó webhelyén](http://support.microsoft.com/).
-   Más országokban a helyi Microsoft-képviseletek nyújtanak támogatást. A biztonsági frissítésekkel kapcsolatos hívások ingyenesek. A [nemzetközi támogatási webhely](http://go.microsoft.com/fwlink/?linkid=21155) felvilágosítást nyújt arról, támogatási kérdéseivel hogyan fordulhat a Microsofthoz.

#### Felelősséget kizáró nyilatkozat

A Microsoft Tudásbázisban leírtak előzetes bejelentés nélkül változhatnak, és a cikkek tartalmáért a Microsoft nem vállal garanciát. A Microsoft egyben elhárít minden kifejezett és értelemszerű garanciát, beleértve az eladhatóságra és az adott célra való alkalmasságra vonatkozó garanciát is. A Microsoft Corporation vagy annak szállítói semmilyen körülmények között nem tehetők felelőssé közvetlen, közvetett, eseti, ok-okozati vagy különleges kárért (beleértve az elmaradt hasznot is), még akkor sem, ha a Microsoft Corporation vagy szállítói tudatában voltak a kár lehetséges voltának. Egyes államok törvényi szabályozása nem teszi lehetővé a véletlen vagy ok-okozati károkért vállalt felelősség korlátozását vagy kizárását, így ezekben az államokban az ez a felelősségkizárás nincs érvényben.

#### Verziók

-   1.0 verzió (2011. október 11.): Összefoglaló közlemény közzététele.
-   1.1 verzió (2011. október 26.): Az MS11-078 közleménnyel kapcsolatban javították a .NET Framework 4 keretrendszerhez tartozó kiszolgálómag-telepítés alkalmazhatóságát a Windows Server 2008 R2 x64 alapú rendszerekhez operációs rendszeren.

*Built at 2014-04-18T01:50:00Z-07:00*
