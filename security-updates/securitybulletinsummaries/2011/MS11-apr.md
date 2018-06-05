---
TOCTitle: 'MS11-APR'
Title: 'A Microsoft biztonsági közleményei - összefoglalás, 2011. április'
ms:assetid: 'ms11-apr'
ms:contentKeyID: 61227750
ms:mtpsurl: 'https://technet.microsoft.com/hu-HU/library/ms11-apr(v=Security.10)'
author: SharonSears
ms.author: SharonSears
---

Security Bulletin Summary

A Microsoft biztonsági közleményei - összefoglalás, 2011. április
=================================================================

Közzétéve: 2011. április 12. | Frissítve: 2011. október 26.

**Verzió:** 6.1

Az összefoglaló a 2011 áprilisában kiadott biztonsági közleményeket összegzi.

A 2011. áprilisi biztonsági közlemények kiadása folytán az összefoglaló a 2011. április 7-én kiadott előzetes értesítés helyébe lép. A biztonsági közlemények kiadásáról szóló előzetes értesítés szolgáltatásról itt olvashat bővebben: [Előzetes értesítés a Microsoft biztonsági közleményeinek kiadásáról](http://technet.microsoft.com/security/bulletin/advance).

Ha automatikus értesítést szeretne kapni a Microsoft biztonsági közleményeinek megjelenéséről, fizessen elő a [Microsoft Technical Security Notifications](http://go.microsoft.com/fwlink/?linkid=21163) szolgáltatásra.

A közleményekkel kapcsolatos kérdések megválaszolására a Microsoft 2011. április 13-án, csendes-óceáni idő szerint 11 órakor webes szemináriumot tart. Jelentkezzen most az [áprilisi közleményeket bemutató webes szemináriumra](https://msevents.microsoft.com/cui/webcasteventdetails.aspx?culture=en-us&eventid=1032455069&eventcategory=4). Ezt követően a webes szeminárium igény szerint kerül megrendezésre. További információkért látogasson el a [Microsoft biztonsági közleményeit és a webes szemináriumokat](http://technet.microsoft.com/security/bulletin/summary) bemutató oldalra.

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
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=214126">MS11-018</a></td>
<td style="border:1px solid black;"><strong>Összesítő biztonsági frissítés az Internet Explorer programhoz (2497640)</strong><br />
<br />
A biztonsági frissítés négy közvetlenül és egy nyilvánosan jelentett biztonsági rést szüntet meg az Internet Explorer programban. A biztonsági frissítés az Internet Explorer 6, az Internet Explorer 7 és az Internet Explorer 8 Windows ügyfeleken futó verzióira nézve Kritikus, az Internet Explorer 6, az Internet Explorer 7 és az Internet Explorer 8 Windows kiszolgálókon futó verzióira nézve pedig Mérsékelt besorolású. A biztonsági rések az Internet Explorer 9 alkalmazást nem érintik.<br />
<br />
A súlyosabb biztonsági rések távoli kódfuttatást tesznek lehetővé, amennyiben a felhasználó speciálisan kialakított weboldalt tekint meg az Internet Explorer alkalmazással. A biztonsági rések valamelyikét sikeresen kihasználó támadó a helyi felhasználóval egyező hozzáférést nyer a rendszerhez. A kevesebb jogosultsággal bíró fiókkal rendelkező felhasználók esetében kisebb a veszélyeztetettség, mint a rendszergazdai jogosultságokkal rendelkezők esetén</td>
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=21140">Kritikus</a><br />
Távoli kódfuttatás</td>
<td style="border:1px solid black;">Újraindítást igényel</td>
<td style="border:1px solid black;">Microsoft Windows,<br />
Internet Explorer</td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=212314">MS11-019</a></td>
<td style="border:1px solid black;"><strong>Az SMB ügyfélgépén a biztonsági rések távolról történő kódfuttatást tesznek lehetővé (2511455)</strong><br />
<br />
Ez a biztonsági frissítés egy nyilvánosságra került és egy közvetlenül jelentett biztonsági rést szüntet meg a Microsoft Windows rendszerben. A biztonsági rések közül a súlyosabbak távolról történő programkódfuttatást tehetnek lehetővé, ha a támadó speciálisan kialakított SMB választ küld az ügyfél által kezdeményezett SMB kérelemre. A biztonsági rés kihasználásához a támadónak meg kell győzni a felhasználót, hogy SMB kapcsolatot kezdeményezzen egy speciálisan kialakított SMB kiszolgálóval.</td>
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=21140">Kritikus</a><br />
Távoli kódfuttatás</td>
<td style="border:1px solid black;">Újraindítást igényel</td>
<td style="border:1px solid black;">Microsoft Windows</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=212236">MS11-020</a></td>
<td style="border:1px solid black;"><strong>Az SMB ügyfélgépén a biztonsági rés távolról történő kódfuttatást tehet lehetővé (2508429)</strong><br />
<br />
A biztonsági frissítés a Microsoft Windows közvetlenül jelentett biztonsági rését szünteti meg. A biztonsági rés távoli kódfuttatást tehet lehetővé, ha a támadó speciálisan kialakított SMB-csomagot hoz létre, és azt elküldi az érintett számítógépre. A tűzfalakra vonatkozó gyakorlati tanácsok, valamint a szabványos alapértelmezett tűzfal-konfigurációk segítséget nyújtanak a hálózatot érő, a szervezet határain kívülről érkező, a biztonsági réseket kihasználni próbáló támadások kivédésében.</td>
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=21140">Kritikus</a><br />
Távoli kódfuttatás</td>
<td style="border:1px solid black;">Újraindítást igényel</td>
<td style="border:1px solid black;">Microsoft Windows</td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=214005">MS11-027</a></td>
<td style="border:1px solid black;"><strong>Összesítő biztonsági frissítés az ActiveX-tiltóbitekhez (2508272)</strong><br />
<br />
A biztonsági frissítés kettő közvetlenül és egy nyilvánosan jelentett biztonsági rést szüntet meg a Microsoft szoftverekben. A biztonsági rések távoli kódvégrehajtást tehetnek lehetővé, ha a felhasználó egy olyan különlegesen kialakított weblapot tekint meg, amely speciális ActiveX-vezérlőt aktivál az Internet Explorer segítségével. A kevesebb jogosultsággal bíró fiókkal rendelkező felhasználók esetében kisebb a veszélyeztetettség, mint a rendszergazdai jogosultságokkal rendelkezők esetén A frissítés három, külső cég által gyártott ActiveX-vezérlőhöz is tartalmaz tiltóbiteket.</td>
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=21140">Kritikus</a><br />
Távoli kódfuttatás</td>
<td style="border:1px solid black;">Esetleg újra kell indítani a rendszert</td>
<td style="border:1px solid black;">Microsoft Windows</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=207931">MS11-028</a></td>
<td style="border:1px solid black;"><strong>A .NET-keretrendszer biztonsági rése távoli programkódfuttatást tehet lehetővé (2484015)</strong><br />
<br />
A biztonsági frissítés a Microsoft .NET Framework nyilvánosan jelentett biztonsági rését szünteti meg. A biztonsági rés távoli kódfuttatást tehet lehetővé az ügyfélrendszereken, ha a felhasználó különlegesen kialakított weboldalt tekint meg az XAML böngészőalkalmazások (XBAP alkalmazások) futtatására alkalmas böngészőben. A kevesebb jogosultsággal bíró fiókkal rendelkező felhasználók esetében kisebb a veszélyeztetettség, mint a rendszergazdai jogosultságokkal rendelkezők esetén A biztonsági rések IIS szolgáltatást futtató kiszolgálórendszereken is lehetővé tehetik a távoli kódfuttatást, ha az adott kiszolgálón engedélyezett az ASP.NET oldalak feldolgozása, és a támadó sikeresen feltölt egy különlegesen kialakított ASP.NET oldalt a kiszolgálóra, és végrehajtja, mint az a webes tárolási forgatókönyv esetében történik. A biztonsági rés a Windows .NET alkalmazásokban is kihasználható a kódműködési biztonsági (CAS) korlátozások megkerülésére.</td>
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=21140">Kritikus</a><br />
Távoli kódfuttatás</td>
<td style="border:1px solid black;">Esetleg újra kell indítani a rendszert</td>
<td style="border:1px solid black;">Microsoft Windows</td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=208524">MS11-029</a></td>
<td style="border:1px solid black;"><strong>A GDI+ biztonsági rése távolról történő kódfuttatást tehet lehetővé (2489979)</strong><br />
<br />
A biztonsági frissítés a Microsoft Windows GDI+ közvetlenül jelentett biztonsági rését szünteti meg. A biztonsági rés távoli kódvégrehajtást tehet lehetővé, amennyiben a felhasználó különlegesen kialakított képfájlt tekintett meg az érintett alkalmazás segítségével, vagy különleges tartalomnak helyet adó weboldalra látogatott el. A kevesebb jogosultsággal bíró fiókkal rendelkező felhasználók esetében kisebb a veszélyeztetettség, mint a rendszergazdai jogosultságokkal rendelkezők esetén</td>
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=21140">Kritikus</a><br />
Távoli kódfuttatás</td>
<td style="border:1px solid black;">Esetleg újra kell indítani a rendszert</td>
<td style="border:1px solid black;">Microsoft Windows,<br />
Microsoft Office</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=212595">MS11-030</a></td>
<td style="border:1px solid black;"><strong>A DNS-címfeloldás biztonsági rése távoli kódfuttatást tesz lehetővé (2509553)</strong><br />
<br />
A biztonsági frissítés a Windows DNS-címfeloldás közvetlenül jelentett biztonsági rését szünteti meg. A biztonsági rés távoli kódvégrehajtást tehet lehetővé, ha a támadó hozzáférést szerez a hálózathoz, majd egyedi programot hoz létre, és azzal küld különlegesen kialakított LLMNR-szórásos lekérdezéseket a célrendszerekre. A tűzfalakra vonatkozó gyakorlati tanácsok, valamint a szabványos alapértelmezett tűzfal-konfigurációk segítséget nyújtanak a hálózatot érő, a szervezet határain kívülről eredő támadások kivédésében. Gyakorlati tanácsként azt javasoljuk, hogy az internetkapcsolattal rendelkező számítógépeken a lehető legkevesebb port legyen megnyitva. Ebben az esetben az LLMNR portokat le kell tiltani az internetről.</td>
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=21140">Kritikus</a><br />
Távoli kódfuttatás</td>
<td style="border:1px solid black;">Újraindítást igényel</td>
<td style="border:1px solid black;">Microsoft Windows</td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=212243">MS11-031</a></td>
<td style="border:1px solid black;"><strong>A JScript és VBScript parancsértelmezők biztonsági</strong> <strong>rése távoli kódfuttatást tehet lehetővé (2514666)</strong><br />
<br />
A biztonsági frissítés a JScript és VBScript parancsértelmezők közvetlenül jelentett biztonsági rését szünteti meg. A biztonsági rés távoli kódvégrehajtást tehet lehetővé, ha a felhasználó különlegesen kialakított weboldalt tekint meg. A támadónak nincs lehetősége arra, hogy a felhasználót a webhely megnyitására kényszerítse. Ehelyett a támadóknak az adott webhelyre kell csábítaniuk a felhasználókat. Ezt rendszerint úgy érik el, hogy ráveszik őket arra, hogy kattintsanak rá egy e-mailben lévő hivatkozásra vagy azonnali üzenetkezelőben megjelenő kérésre.</td>
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=21140">Kritikus</a><br />
Távoli kódfuttatás</td>
<td style="border:1px solid black;">Esetleg újra kell indítani a rendszert</td>
<td style="border:1px solid black;">Microsoft Windows</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=212224">MS11-032</a></td>
<td style="border:1px solid black;"><strong>Az OpenType Compact Font Format (CFF) illesztőprogramjának biztonsági rése távolról történő kódfuttatást tehet lehetővé (2507618)</strong><br />
<br />
A biztonsági frissítés az OpenType Compact Font Format (CFF) illesztőprogram egy közvetlenül jelentett biztonsági rését szünteti meg. A biztonsági rés távoli kódfuttatást tehet lehetővé, ha a felhasználó speciálisan kialakított CFF betűtípussal megjelenített tartalmat tekint meg. A támadóknak nem áll módjukban a felhasználókat rákényszeríteni a speciálisan kialakított tartalom megtekintésére. Ehelyett a támadóknak az adott webhelyre kell csábítaniuk a felhasználókat. Ezt rendszerint úgy érik el, hogy ráveszik őket arra, hogy kattintsanak rá egy e-mailben lévő hivatkozásra vagy azonnali üzenetkezelőben megjelenő kérésre.</td>
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=21140">Kritikus</a><br />
Távoli kódfuttatás</td>
<td style="border:1px solid black;">Újraindítást igényel</td>
<td style="border:1px solid black;">Microsoft Windows</td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=210121">MS11-021</a></td>
<td style="border:1px solid black;"><strong>A Microsoft Excel biztonsági rései távolról történő kódfuttatást tehetnek lehetővé (2489279)</strong><br />
<br />
Ez a biztonsági frissítés a Microsoft Office kilenc, közvetlenül jelzett biztonsági rését szünteti meg. A biztonsági rések távoli kódvégrehajtást tehetnek lehetővé, amennyiben a felhasználó egy speciálisan kialakított Excel fájlt nyit meg. A biztonsági rések valamelyikét sikeresen kihasználó támadó a bejelentkezett felhasználóval egyező hozzáférést nyer a rendszerhez. A kevesebb jogosultsággal bíró fiókkal rendelkező felhasználók esetében kisebb a veszélyeztetettség, mint a rendszergazdai jogosultságokkal rendelkezők esetén</td>
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=21140">Fontos</a><br />
Távoli kódfuttatás</td>
<td style="border:1px solid black;">Esetleg újra kell indítani a rendszert</td>
<td style="border:1px solid black;">Microsoft Office</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=210727">MS11-022</a></td>
<td style="border:1px solid black;"><strong>A Microsoft PowerPoint biztonsági rései távoli kódfuttatást tehetnek lehetővé (2489283)</strong><br />
<br />
A biztonsági frissítés a Microsoft PowerPoint három, közvetlenül jelentett biztonsági rését szünteti meg. A biztonsági rések távoli kódvégrehajtást tehetnek lehetővé, amennyiben a felhasználó egy speciálisan kialakított PowerPoint fájlt nyit meg. A biztonsági rések valamelyikét sikeresen kihasználó támadó a helyi felhasználóval egyező hozzáférést nyer a rendszerhez. A kevesebb jogosultsággal bíró fiókkal rendelkező felhasználók esetében kisebb a veszélyeztetettség, mint a rendszergazdai jogosultságokkal rendelkezők esetén A PowerPoint 2010 programhoz tartozó, a <a href="http://support.microsoft.com/kb/2501584">Microsoft Tudásbázis 2501584. számú cikkében</a> elérhető, „A szerkesztés letiltása védett nézetben a PowerPoint 2010 alkalmazásban” című automatizált <strong>Microsoft Fix it</strong> megoldás védelmet nyújt a CVE-2011-0655 és CVE-2011-0656 közleményekben ismertetett biztonsági rések kihasználásával végrehajtható támadások ellen.</td>
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=21140">Fontos</a><br />
Távoli kódfuttatás</td>
<td style="border:1px solid black;">Esetleg újra kell indítani a rendszert</td>
<td style="border:1px solid black;">Microsoft Office,<br />
Microsoft Server Software</td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=210206">MS11-023</a></td>
<td style="border:1px solid black;"><strong>A Microsoft Office biztonsági rései távolról történő programkódfuttatást tehetnek lehetővé (2489293)</strong><br />
<br />
Ez a biztonsági frissítés egy nyilvánosságra került és egy közvetlenül jelentett biztonsági rést szüntet meg a Microsoft Office programban. A támadó a biztonsági réseken keresztül távoli kódfuttatást tud elérni, ha rá tudja venni a felhasználót, hogy nyisson meg egy különlegesen kialakított Office-fájlt vagy egy különlegesen kialakított objektumtárfájllal azonos hálózati meghajtón található normál Office-fájlt. A biztonsági rések valamelyikét sikeresen kihasználó támadó a bejelentkezett felhasználóéval megegyező hozzáférést nyer a rendszerhez. A kevesebb jogosultsággal bíró fiókkal rendelkező felhasználók esetében kisebb a veszélyeztetettség, mint a rendszergazdai jogosultságokkal rendelkezők esetén</td>
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=21140">Fontos</a><br />
Távoli kódfuttatás</td>
<td style="border:1px solid black;">Esetleg újra kell indítani a rendszert</td>
<td style="border:1px solid black;">Microsoft Office</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=212226">MS11-024</a></td>
<td style="border:1px solid black;"><strong>A Windows Faxfedőlap-szerkesztő biztonsági rései távoli programkódfuttatást tehetnek lehetővé (2527308)</strong><br />
<br />
A biztonsági frissítés a Microsoft Windows két, nyilvánosan jelentett biztonsági rését szünteti meg. A biztonsági rések távoli kódvégrehajtást tehetnek lehetővé, ha a felhasználó speciálisan kialakított faxfedőlapfájlt (.cov) nyit meg a Windows Faxfedőlap-szerkesztővel. A biztonsági rések valamelyikét sikeresen kihasználó támadó a bejelentkezett felhasználóval egyező hozzáférést nyer a rendszerhez. A kevesebb jogosultsággal bíró fiókkal rendelkező felhasználók esetében kisebb a veszélyeztetettség, mint a rendszergazdai jogosultságokkal rendelkezők esetén</td>
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=21140">Fontos</a><br />
Távoli kódfuttatás</td>
<td style="border:1px solid black;">Esetleg újra kell indítani a rendszert</td>
<td style="border:1px solid black;">Microsoft Windows</td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=209720">MS11-025</a></td>
<td style="border:1px solid black;"><strong>A Microsoft Foundation Class (MFC) objektumtár</strong> <strong>biztonsági rése távoli programkódfuttatást tehet lehetővé (2500212)</strong><br />
<br />
A biztonsági frissítés a Microsoft Foundation Class (MFC) objektumtárral készített egyes alkalmazásokban jelentkező, nyilvánosan jelentett biztonsági rést szüntet meg. A biztonsági rés távolról történő programkódfuttatást tehet lehetővé, ha a felhasználó az érintett alkalmazással társított olyan érvényes fájlt nyit meg, amely egy különlegesen kialakított objektumtárfájllal azonos hálózati mappában található. A sikeres támadáshoz a felhasználónak egy nem megbízhatónak ítélt távoli fájlrendszerre vagy WebDAV megosztásra kell ellátogatnia, majd onnan dokumentumot megnyitnia, amelyet ezt követően az érintett alkalmazás betölt.</td>
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=21140">Fontos</a><br />
Távoli kódfuttatás</td>
<td style="border:1px solid black;">Esetleg újra kell indítani a rendszert</td>
<td style="border:1px solid black;">Microsoft fejlesztői eszközök és szoftver</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=212523">MS11-026</a></td>
<td style="border:1px solid black;"><strong>Az MHTML szabvány biztonsági rése adatokhoz való illetéktelen hozzáférést tehet lehetővé (2503658)</strong><br />
<br />
A biztonsági frissítés az MHTML protokollkezelő nyilvánosan jelentett biztonsági rését szünteti meg a Microsoft Windows rendszerekben. A biztonsági rés információfelfedést tehet lehetővé, ha a felhasználó különlegesen kialakított weboldalt tekint meg. Webalapú támadás esetén a webhely a biztonsági rés kihasználására alkalmas, speciálisan kialakított hivatkozást tartalmazhat. A támadónak rá kell vennie a felhasználót a webhely megtekintésére és a különlegesen kialakított hivatkozás megnyitására.</td>
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=21140">Fontos</a><br />
Adatokhoz való illetéktelen hozzáférés</td>
<td style="border:1px solid black;">Újraindítást igényel</td>
<td style="border:1px solid black;">Microsoft Windows</td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=208110">MS11-033</a></td>
<td style="border:1px solid black;"><strong>A WordPad szövegkonverterek biztonsági rése távolról történő programkódfuttatást tehet lehetővé (2485663)</strong><br />
<br />
A biztonsági frissítés a Microsoft Windows közvetlenül jelentett biztonsági rését szünteti meg. A biztonsági frissítés a Windows XP és Windows Server 2003 összes támogatott kiadására nézve Fontos besorolású. A Windows Vista, Windows Server 2008, Windows 7 és Windows Server 2008 R2 támogatott kiadásait nem érinti a biztonsági rés okozta probléma.<br />
<br />
A biztonsági rés távoli kódvégrehajtást tehet lehetővé, ha a felhasználó megnyit egy speciálisan kialakított fájlt a WordPad-del. A biztonsági rést kihasználó támadó a helyi felhasználóval egyező hozzáférést nyer a rendszerhez. A kevesebb jogosultsággal bíró fiókkal rendelkező felhasználók esetében kisebb a veszélyeztetettség, mint a rendszergazdai jogosultságokkal rendelkezők esetén</td>
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=21140">Fontos</a><br />
Távoli kódfuttatás</td>
<td style="border:1px solid black;">Esetleg újra kell indítani a rendszert</td>
<td style="border:1px solid black;">Microsoft Windows</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=211826">MS11-034</a></td>
<td style="border:1px solid black;"><strong>A Windows kernelmódú illesztőprogramjainak biztonsági rései jogok kiterjesztéséhez vezethetnek (2506223)</strong><br />
<br />
A biztonsági frissítés a Microsoft Windows harminc közvetlenül jelzett biztonsági rését szünteti meg. A biztonsági rések jogok kiterjesztését tehetik lehetővé, ha a támadó helyben bejelentkezett, és ott különlegesen kialakított alkalmazást futtatott. A támadónak a biztonsági rések kihasználásához érvényes bejelentkezési adatokkal kell rendelkeznie, és képesnek kell lennie helyileg bejelentkezni a rendszerbe. Névtelen felhasználók nem tudják távolról kiaknázni ezeket a biztonsági réseket.</td>
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
A következő táblázat az adott hónapban megoldott biztonsági rések kihasználhatósági jellemzőit ismerteti. A biztonsági rések a kihasználhatósági kockázat, majd a CVE azonosító szerint vannak felsorolva. Csak a kritikus és fontos besorolású biztonsági rések szerepelnek.
  
**A táblázat használata**
  
A táblázat segítségével meghatározható annak valószínűsége, hogy a biztonsági közlemény kiadását követő 30 napon belül a telepíteni szükséges biztonsági frissítésekre működő rosszindulatú programkódot jelentetnek meg. A telepítés fontossági sorrendjének megállapításához az adott konfigurációnak megfelelően tekintse át az alábbi értékeléseket. A minősítések jelentéséről és meghatározásuk módjáról a [Microsoft kihasználhatósági információk](http://technet.microsoft.com/en-us/security/cc998259.aspx) című rész tartalmaz bővebb információt.

 
<p> </p>
<table style="border:1px solid black;">
<thead>
<tr class="header">
<th style="border:1px solid black;" >Közlemény azonosítója</th>
<th style="border:1px solid black;" >A biztonsági rés címe</th>
<th style="border:1px solid black;" >CVE-azonosító</th>
<th style="border:1px solid black;" >Kihasználhatósági információk értékelése</th>
<th style="border:1px solid black;" >Fontos megjegyzések</th>
</tr>
</thead>
<tbody>
<tr class="odd">
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=209720">MS11-025</a></td>
<td style="border:1px solid black;">Az MFC nem biztonságos függvénytárbetöltése miatti biztonsági rés</td>
<td style="border:1px solid black;"><a href="http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2010-3190">CVE-2010-3190</a></td>
<td style="border:1px solid black;"><a href="http://technet.microsoft.com/en-us/security/cc998259.aspx">1</a> - Valószínűleg konzisztens rosszindulatú programkód</td>
<td style="border:1px solid black;">A biztonsági rés nyilvánosságra került</td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=207931">MS11-028</a></td>
<td style="border:1px solid black;">A .NET-keretrendszer veremsérülést okozó biztonsági rése</td>
<td style="border:1px solid black;"><a href="http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2010-3958">CVE-2010-3958</a></td>
<td style="border:1px solid black;"><a href="http://technet.microsoft.com/en-us/security/cc998259.aspx">1</a> - Valószínűleg konzisztens rosszindulatú programkód</td>
<td style="border:1px solid black;">A biztonsági rés nyilvánosságra került</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=212224">MS11-032</a></td>
<td style="border:1px solid black;">Az OpenType betűkészlet veremtúlcsordulást okozó biztonsági rése</td>
<td style="border:1px solid black;"><a href="http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2011-0034">CVE-2011-0034</a></td>
<td style="border:1px solid black;"><a href="http://technet.microsoft.com/en-us/security/cc998259.aspx">1</a> - Valószínűleg konzisztens rosszindulatú programkód</td>
<td style="border:1px solid black;">(Nincs)</td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=208524">MS11-029</a></td>
<td style="border:1px solid black;">A GDI+ egészszám-túlcsordulást okozó biztonsági rése</td>
<td style="border:1px solid black;"><a href="http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2011-0041">CVE-2011-0041</a></td>
<td style="border:1px solid black;"><a href="http://technet.microsoft.com/en-us/security/cc998259.aspx">1</a> - Valószínűleg konzisztens rosszindulatú programkód</td>
<td style="border:1px solid black;">(Nincs)</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=214126">MS11-018</a></td>
<td style="border:1px solid black;">Az elrendezéskezelés memóriameghibásodást okozó biztonsági rése</td>
<td style="border:1px solid black;"><a href="http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2011-0094">CVE-2011-0094</a></td>
<td style="border:1px solid black;"><a href="http://technet.microsoft.com/en-us/security/cc998259.aspx">1</a> - Valószínűleg konzisztens rosszindulatú programkód</td>
<td style="border:1px solid black;"><strong>A biztonsági rést korlátozott számú</strong> <strong>, célzott támadás során használják ki</strong></td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=210121">MS11-021</a></td>
<td style="border:1px solid black;">Az Excel alkalmazás egészszám-túlcsordulást okozó biztonsági rése</td>
<td style="border:1px solid black;"><a href="http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2011-0097">CVE-2011-0097</a></td>
<td style="border:1px solid black;"><a href="http://technet.microsoft.com/en-us/security/cc998259.aspx">1</a> - Valószínűleg konzisztens rosszindulatú programkód</td>
<td style="border:1px solid black;">(Nincs)</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=210121">MS11-021</a></td>
<td style="border:1px solid black;">Az Excel alkalmazás halomtúlcsordulást okozó biztonsági rése</td>
<td style="border:1px solid black;"><a href="http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2011-0098">CVE-2011-0098</a></td>
<td style="border:1px solid black;"><a href="http://technet.microsoft.com/en-us/security/cc998259.aspx">1</a> - Valószínűleg konzisztens rosszindulatú programkód</td>
<td style="border:1px solid black;">(Nincs)</td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=210121">MS11-021</a></td>
<td style="border:1px solid black;">Az Excel-bejegyzések elemzésének WriteAV biztonsági rése</td>
<td style="border:1px solid black;"><a href="http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2011-0101">CVE-2011-0101</a></td>
<td style="border:1px solid black;"><a href="http://technet.microsoft.com/en-us/security/cc998259.aspx">1</a> - Valószínűleg konzisztens rosszindulatú programkód</td>
<td style="border:1px solid black;">(Nincs)</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=210206">MS11-023</a></td>
<td style="border:1px solid black;">Office-összetevő nem biztonságos függvénytár betöltése miatti biztonsági rése</td>
<td style="border:1px solid black;"><a href="http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2011-0107">CVE-2011-0107</a></td>
<td style="border:1px solid black;"><a href="http://technet.microsoft.com/en-us/security/cc998259.aspx">1</a> - Valószínűleg konzisztens rosszindulatú programkód</td>
<td style="border:1px solid black;">A biztonsági rés nyilvánosságra került</td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=214126">MS11-018</a></td>
<td style="border:1px solid black;">Az MSHTML memóriameghibásodást okozó biztonsági rése</td>
<td style="border:1px solid black;"><a href="http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2011-0346">CVE-2011-0346</a></td>
<td style="border:1px solid black;"><a href="http://technet.microsoft.com/en-us/security/cc998259.aspx">1</a> - Valószínűleg konzisztens rosszindulatú programkód</td>
<td style="border:1px solid black;">A biztonsági rés nyilvánosságra került</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=212314">MS11-019</a></td>
<td style="border:1px solid black;">Az SMB ügyfél válaszelemzési biztonsági rése</td>
<td style="border:1px solid black;"><a href="http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2011-0660">CVE-2011-0660</a></td>
<td style="border:1px solid black;"><a href="http://technet.microsoft.com/en-us/security/cc998259.aspx">1</a> - Valószínűleg konzisztens rosszindulatú programkód</td>
<td style="border:1px solid black;">(Nincs)</td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=212236">MS11-020</a></td>
<td style="border:1px solid black;">Az SMB-tranzakcióelemzés biztonsági rése</td>
<td style="border:1px solid black;"><a href="http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2011-0661">CVE-2011-0661</a></td>
<td style="border:1px solid black;"><a href="http://technet.microsoft.com/en-us/security/cc998259.aspx">1</a> - Valószínűleg konzisztens rosszindulatú programkód</td>
<td style="border:1px solid black;">(Nincs)</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=211826">MS11-034</a></td>
<td style="border:1px solid black;">A Win32k használat utáni felszabadítás miatti biztonsági rése</td>
<td style="border:1px solid black;"><a href="http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2011-0662">CVE-2011-0662</a></td>
<td style="border:1px solid black;"><a href="http://technet.microsoft.com/en-us/security/cc998259.aspx">1</a> - Valószínűleg konzisztens rosszindulatú programkód</td>
<td style="border:1px solid black;">(Nincs)</td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=211826">MS11-034</a></td>
<td style="border:1px solid black;">A Win32k használat utáni felszabadítás miatti biztonsági rése</td>
<td style="border:1px solid black;"><a href="http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2011-0665">CVE-2011-0665</a></td>
<td style="border:1px solid black;"><a href="http://technet.microsoft.com/en-us/security/cc998259.aspx">1</a> - Valószínűleg konzisztens rosszindulatú programkód</td>
<td style="border:1px solid black;">(Nincs)</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=211826">MS11-034</a></td>
<td style="border:1px solid black;">A Win32k használat utáni felszabadítás miatti biztonsági rése</td>
<td style="border:1px solid black;"><a href="http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2011-0666">CVE-2011-0666</a></td>
<td style="border:1px solid black;"><a href="http://technet.microsoft.com/en-us/security/cc998259.aspx">1</a> - Valószínűleg konzisztens rosszindulatú programkód</td>
<td style="border:1px solid black;">(Nincs)</td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=211826">MS11-034</a></td>
<td style="border:1px solid black;">A Win32k használat utáni felszabadítás miatti biztonsági rése</td>
<td style="border:1px solid black;"><a href="http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2011-0667">CVE-2011-0667</a></td>
<td style="border:1px solid black;"><a href="http://technet.microsoft.com/en-us/security/cc998259.aspx">1</a> - Valószínűleg konzisztens rosszindulatú programkód</td>
<td style="border:1px solid black;">(Nincs)</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=211826">MS11-034</a></td>
<td style="border:1px solid black;">A Win32k használat utáni felszabadítás miatti biztonsági rése</td>
<td style="border:1px solid black;"><a href="http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2011-0670">CVE-2011-0670</a></td>
<td style="border:1px solid black;"><a href="http://technet.microsoft.com/en-us/security/cc998259.aspx">1</a> - Valószínűleg konzisztens rosszindulatú programkód</td>
<td style="border:1px solid black;">(Nincs)</td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=211826">MS11-034</a></td>
<td style="border:1px solid black;">A Win32k használat utáni felszabadítás miatti biztonsági rése</td>
<td style="border:1px solid black;"><a href="http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2011-0671">CVE-2011-0671</a></td>
<td style="border:1px solid black;"><a href="http://technet.microsoft.com/en-us/security/cc998259.aspx">1</a> - Valószínűleg konzisztens rosszindulatú programkód</td>
<td style="border:1px solid black;">(Nincs)</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=211826">MS11-034</a></td>
<td style="border:1px solid black;">A Win32k használat utáni felszabadítás miatti biztonsági rése</td>
<td style="border:1px solid black;"><a href="http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2011-0672">CVE-2011-0672</a></td>
<td style="border:1px solid black;"><a href="http://technet.microsoft.com/en-us/security/cc998259.aspx">1</a> - Valószínűleg konzisztens rosszindulatú programkód</td>
<td style="border:1px solid black;">(Nincs)</td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=211826">MS11-034</a></td>
<td style="border:1px solid black;">A Win32k Null mutatójának visszakeresési biztonsági rése</td>
<td style="border:1px solid black;"><a href="http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2011-0673">CVE-2011-0673</a></td>
<td style="border:1px solid black;"><a href="http://technet.microsoft.com/en-us/security/cc998259.aspx">1</a> - Valószínűleg konzisztens rosszindulatú programkód</td>
<td style="border:1px solid black;">(Nincs)</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=211826">MS11-034</a></td>
<td style="border:1px solid black;">A Win32k használat utáni felszabadítás miatti biztonsági rése</td>
<td style="border:1px solid black;"><a href="http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2011-0674">CVE-2011-0674</a></td>
<td style="border:1px solid black;"><a href="http://technet.microsoft.com/en-us/security/cc998259.aspx">1</a> - Valószínűleg konzisztens rosszindulatú programkód</td>
<td style="border:1px solid black;">(Nincs)</td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=211826">MS11-034</a></td>
<td style="border:1px solid black;">A Win32k használat utáni felszabadítás miatti biztonsági rése</td>
<td style="border:1px solid black;"><a href="http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2011-0675">CVE-2011-0675</a></td>
<td style="border:1px solid black;"><a href="http://technet.microsoft.com/en-us/security/cc998259.aspx">1</a> - Valószínűleg konzisztens rosszindulatú programkód</td>
<td style="border:1px solid black;">(Nincs)</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=211826">MS11-034</a></td>
<td style="border:1px solid black;">A Win32k Null mutatójának visszakeresési biztonsági rése</td>
<td style="border:1px solid black;"><a href="http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2011-0676">CVE-2011-0676</a></td>
<td style="border:1px solid black;"><a href="http://technet.microsoft.com/en-us/security/cc998259.aspx">1</a> - Valószínűleg konzisztens rosszindulatú programkód</td>
<td style="border:1px solid black;">(Nincs)</td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=211826">MS11-034</a></td>
<td style="border:1px solid black;">A Win32k Null mutatójának visszakeresési biztonsági rése</td>
<td style="border:1px solid black;"><a href="http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2011-0677">CVE-2011-0677</a></td>
<td style="border:1px solid black;"><a href="http://technet.microsoft.com/en-us/security/cc998259.aspx">1</a> - Valószínűleg konzisztens rosszindulatú programkód</td>
<td style="border:1px solid black;">(Nincs)</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=210727">MS11-022</a></td>
<td style="border:1px solid black;">Az OfficeArt Atom RCE biztonsági rése</td>
<td style="border:1px solid black;"><a href="http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2011-0976">CVE-2011-0976</a></td>
<td style="border:1px solid black;"><a href="http://technet.microsoft.com/en-us/security/cc998259.aspx">1</a> - Valószínűleg konzisztens rosszindulatú programkód</td>
<td style="border:1px solid black;">(Nincs)</td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=210121">MS11-021</a></td>
<td style="border:1px solid black;">Az Excel alkalmazás tömbindexelés miatti biztonsági rése</td>
<td style="border:1px solid black;"><a href="http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2011-0978">CVE-2011-0978</a></td>
<td style="border:1px solid black;"><a href="http://technet.microsoft.com/en-us/security/cc998259.aspx">1</a> - Valószínűleg konzisztens rosszindulatú programkód</td>
<td style="border:1px solid black;">(Nincs)</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=210121">MS11-021</a></td>
<td style="border:1px solid black;">Az Excel alkalmazás kapcsolt lista meghibásodását okozó biztonsági rése</td>
<td style="border:1px solid black;"><a href="http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2011-0979">CVE-2011-0979</a></td>
<td style="border:1px solid black;"><a href="http://technet.microsoft.com/en-us/security/cc998259.aspx">1</a> - Valószínűleg konzisztens rosszindulatú programkód</td>
<td style="border:1px solid black;">(Nincs)</td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=210121">MS11-021</a></td>
<td style="border:1px solid black;">Az Excel alkalmazás értékhiányos mutató miatti biztonsági rése</td>
<td style="border:1px solid black;"><a href="http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2011-0980">CVE-2011-0980</a></td>
<td style="border:1px solid black;"><a href="http://technet.microsoft.com/en-us/security/cc998259.aspx">1</a> - Valószínűleg konzisztens rosszindulatú programkód</td>
<td style="border:1px solid black;">(Nincs)</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=211826">MS11-034</a></td>
<td style="border:1px solid black;">A Win32k Null mutatójának visszakeresési biztonsági rése</td>
<td style="border:1px solid black;"><a href="http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2011-1225">CVE-2011-1225</a></td>
<td style="border:1px solid black;"><a href="http://technet.microsoft.com/en-us/security/cc998259.aspx">1</a> - Valószínűleg konzisztens rosszindulatú programkód</td>
<td style="border:1px solid black;">(Nincs)</td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=211826">MS11-034</a></td>
<td style="border:1px solid black;">A Win32k Null mutatójának visszakeresési biztonsági rése</td>
<td style="border:1px solid black;"><a href="http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2011-1226">CVE-2011-1226</a></td>
<td style="border:1px solid black;"><a href="http://technet.microsoft.com/en-us/security/cc998259.aspx">1</a> - Valószínűleg konzisztens rosszindulatú programkód</td>
<td style="border:1px solid black;">(Nincs)</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=211826">MS11-034</a></td>
<td style="border:1px solid black;">A Win32k Null mutatójának visszakeresési biztonsági rése</td>
<td style="border:1px solid black;"><a href="http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2011-1227">CVE-2011-1227</a></td>
<td style="border:1px solid black;"><a href="http://technet.microsoft.com/en-us/security/cc998259.aspx">1</a> - Valószínűleg konzisztens rosszindulatú programkód</td>
<td style="border:1px solid black;">(Nincs)</td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=211826">MS11-034</a></td>
<td style="border:1px solid black;">A Win32k Null mutatójának visszakeresési biztonsági rése</td>
<td style="border:1px solid black;"><a href="http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2011-1228">CVE-2011-1228</a></td>
<td style="border:1px solid black;"><a href="http://technet.microsoft.com/en-us/security/cc998259.aspx">1</a> - Valószínűleg konzisztens rosszindulatú programkód</td>
<td style="border:1px solid black;">(Nincs)</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=211826">MS11-034</a></td>
<td style="border:1px solid black;">A Win32k Null mutatójának visszakeresési biztonsági rése</td>
<td style="border:1px solid black;"><a href="http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2011-1229">CVE-2011-1229</a></td>
<td style="border:1px solid black;"><a href="http://technet.microsoft.com/en-us/security/cc998259.aspx">1</a> - Valószínűleg konzisztens rosszindulatú programkód</td>
<td style="border:1px solid black;">(Nincs)</td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=211826">MS11-034</a></td>
<td style="border:1px solid black;">A Win32k Null mutatójának visszakeresési biztonsági rése</td>
<td style="border:1px solid black;"><a href="http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2011-1230">CVE-2011-1230</a></td>
<td style="border:1px solid black;"><a href="http://technet.microsoft.com/en-us/security/cc998259.aspx">1</a> - Valószínűleg konzisztens rosszindulatú programkód</td>
<td style="border:1px solid black;">(Nincs)</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=211826">MS11-034</a></td>
<td style="border:1px solid black;">A Win32k Null mutatójának visszakeresési biztonsági rése</td>
<td style="border:1px solid black;"><a href="http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2011-1231">CVE-2011-1231</a></td>
<td style="border:1px solid black;"><a href="http://technet.microsoft.com/en-us/security/cc998259.aspx">1</a> - Valószínűleg konzisztens rosszindulatú programkód</td>
<td style="border:1px solid black;">(Nincs)</td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=211826">MS11-034</a></td>
<td style="border:1px solid black;">A Win32k Null mutatójának visszakeresési biztonsági rése</td>
<td style="border:1px solid black;"><a href="http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2011-1232">CVE-2011-1232</a></td>
<td style="border:1px solid black;"><a href="http://technet.microsoft.com/en-us/security/cc998259.aspx">1</a> - Valószínűleg konzisztens rosszindulatú programkód</td>
<td style="border:1px solid black;">(Nincs)</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=211826">MS11-034</a></td>
<td style="border:1px solid black;">A Win32k Null mutatójának visszakeresési biztonsági rése</td>
<td style="border:1px solid black;"><a href="http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2011-1233">CVE-2011-1233</a></td>
<td style="border:1px solid black;"><a href="http://technet.microsoft.com/en-us/security/cc998259.aspx">1</a> - Valószínűleg konzisztens rosszindulatú programkód</td>
<td style="border:1px solid black;">(Nincs)</td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=211826">MS11-034</a></td>
<td style="border:1px solid black;">A Win32k használat utáni felszabadítás miatti biztonsági rése</td>
<td style="border:1px solid black;"><a href="http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2011-1235">CVE-2011-1235</a></td>
<td style="border:1px solid black;"><a href="http://technet.microsoft.com/en-us/security/cc998259.aspx">1</a> - Valószínűleg konzisztens rosszindulatú programkód</td>
<td style="border:1px solid black;">(Nincs)</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=211826">MS11-034</a></td>
<td style="border:1px solid black;">A Win32k használat utáni felszabadítás miatti biztonsági rése</td>
<td style="border:1px solid black;"><a href="http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2011-1236">CVE-2011-1236</a></td>
<td style="border:1px solid black;"><a href="http://technet.microsoft.com/en-us/security/cc998259.aspx">1</a> - Valószínűleg konzisztens rosszindulatú programkód</td>
<td style="border:1px solid black;">(Nincs)</td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=211826">MS11-034</a></td>
<td style="border:1px solid black;">A Win32k használat utáni felszabadítás miatti biztonsági rése</td>
<td style="border:1px solid black;"><a href="http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2011-1237">CVE-2011-1237</a></td>
<td style="border:1px solid black;"><a href="http://technet.microsoft.com/en-us/security/cc998259.aspx">1</a> - Valószínűleg konzisztens rosszindulatú programkód</td>
<td style="border:1px solid black;">(Nincs)</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=211826">MS11-034</a></td>
<td style="border:1px solid black;">A Win32k használat utáni felszabadítás miatti biztonsági rése</td>
<td style="border:1px solid black;"><a href="http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2011-1239">CVE-2011-1239</a></td>
<td style="border:1px solid black;"><a href="http://technet.microsoft.com/en-us/security/cc998259.aspx">1</a> - Valószínűleg konzisztens rosszindulatú programkód</td>
<td style="border:1px solid black;">(Nincs)</td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=211826">MS11-034</a></td>
<td style="border:1px solid black;">A Win32k használat utáni felszabadítás miatti biztonsági rése</td>
<td style="border:1px solid black;"><a href="http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2011-1240">CVE-2011-1240</a></td>
<td style="border:1px solid black;"><a href="http://technet.microsoft.com/en-us/security/cc998259.aspx">1</a> - Valószínűleg konzisztens rosszindulatú programkód</td>
<td style="border:1px solid black;">(Nincs)</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=211826">MS11-034</a></td>
<td style="border:1px solid black;">A Win32k használat utáni felszabadítás miatti biztonsági rése</td>
<td style="border:1px solid black;"><a href="http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2011-1241">CVE-2011-1241</a></td>
<td style="border:1px solid black;"><a href="http://technet.microsoft.com/en-us/security/cc998259.aspx">1</a> - Valószínűleg konzisztens rosszindulatú programkód</td>
<td style="border:1px solid black;">(Nincs)</td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=211826">MS11-034</a></td>
<td style="border:1px solid black;">A Win32k használat utáni felszabadítás miatti biztonsági rése</td>
<td style="border:1px solid black;"><a href="http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2011-1242">CVE-2011-1242</a></td>
<td style="border:1px solid black;"><a href="http://technet.microsoft.com/en-us/security/cc998259.aspx">1</a> - Valószínűleg konzisztens rosszindulatú programkód</td>
<td style="border:1px solid black;">(Nincs)</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=214126">MS11-018</a></td>
<td style="border:1px solid black;">Az objektumkezelés memóriameghibásodást okozó biztonsági rése</td>
<td style="border:1px solid black;"><a href="http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2011-1345">CVE-2011-1345</a></td>
<td style="border:1px solid black;"><a href="http://technet.microsoft.com/en-us/security/cc998259.aspx">1</a> - Valószínűleg konzisztens rosszindulatú programkód</td>
<td style="border:1px solid black;"><strong>A biztonsági rést korlátozott számú,</strong> <strong>célzott támadás során használják ki</strong></td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=208110">MS11-033</a></td>
<td style="border:1px solid black;">A WordPad szövegkonverter elemzési biztonsági rése</td>
<td style="border:1px solid black;"><a href="http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2011-0028">CVE-2011-0028</a></td>
<td style="border:1px solid black;"><a href="http://technet.microsoft.com/en-us/security/cc998259.aspx">2</a> - Valószínűleg inkonzisztens rosszindulatú programkód</td>
<td style="border:1px solid black;">(Nincs)</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=210121">MS11-021</a></td>
<td style="border:1px solid black;">Az Excel memóriameghibásodást okozó biztonsági rése</td>
<td style="border:1px solid black;"><a href="http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2011-0103">CVE-2011-0103</a></td>
<td style="border:1px solid black;"><a href="http://technet.microsoft.com/en-us/security/cc998259.aspx">2</a> - Valószínűleg inkonzisztens rosszindulatú programkód</td>
<td style="border:1px solid black;">(Nincs)</td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=210121">MS11-021</a></td>
<td style="border:1px solid black;">Az Excel alkalmazás puffertúlcsordulást okozó biztonsági rése</td>
<td style="border:1px solid black;"><a href="http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2011-0104">CVE-2011-0104</a></td>
<td style="border:1px solid black;"><a href="http://technet.microsoft.com/en-us/security/cc998259.aspx">2</a> - Valószínűleg inkonzisztens rosszindulatú programkód</td>
<td style="border:1px solid black;">(Nincs)</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=210121">MS11-021</a></td>
<td style="border:1px solid black;">Az Excel alkalmazás adatinicializálási biztonsági rése</td>
<td style="border:1px solid black;"><a href="http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2011-0105">CVE-2011-0105</a></td>
<td style="border:1px solid black;"><a href="http://technet.microsoft.com/en-us/security/cc998259.aspx">2</a> - Valószínűleg inkonzisztens rosszindulatú programkód</td>
<td style="border:1px solid black;">(Nincs)</td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=212314">MS11-019</a></td>
<td style="border:1px solid black;">A tallózó gyűjtősérülés miatti biztonsági rése</td>
<td style="border:1px solid black;"><a href="http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2011-0654">CVE-2011-0654</a></td>
<td style="border:1px solid black;"><a href="http://technet.microsoft.com/en-us/security/cc998259.aspx">2</a> - Valószínűleg inkonzisztens rosszindulatú programkód</td>
<td style="border:1px solid black;">A biztonsági rés nyilvánosságra került</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=210727">MS11-022</a></td>
<td style="border:1px solid black;">Floating Point Techno-color Time Bandit RCE biztonsági rés</td>
<td style="border:1px solid black;"><a href="http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2011-0655">CVE-2011-0655</a></td>
<td style="border:1px solid black;"><a href="http://technet.microsoft.com/en-us/security/cc998259.aspx">2</a> - Valószínűleg inkonzisztens rosszindulatú programkód</td>
<td style="border:1px solid black;">(Nincs)</td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=210727">MS11-022</a></td>
<td style="border:1px solid black;">Persist Directory RCE biztonsági rés</td>
<td style="border:1px solid black;"><a href="http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2011-0656">CVE-2011-0656</a></td>
<td style="border:1px solid black;"><a href="http://technet.microsoft.com/en-us/security/cc998259.aspx">2</a> - Valószínűleg inkonzisztens rosszindulatú programkód</td>
<td style="border:1px solid black;">(Nincs)</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=212595">MS11-030</a></td>
<td style="border:1px solid black;">A DNS-lekérdezések miatti biztonsági rés</td>
<td style="border:1px solid black;"><a href="http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2011-0657">CVE-2011-0657</a></td>
<td style="border:1px solid black;"><a href="http://technet.microsoft.com/en-us/security/cc998259.aspx">2</a> - Valószínűleg inkonzisztens rosszindulatú programkód</td>
<td style="border:1px solid black;">(Nincs)</td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=212243">MS11-031</a></td>
<td style="border:1px solid black;">A parancsfájl-memória újrakiosztása okozta biztonsági rés</td>
<td style="border:1px solid black;"><a href="http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2011-0663">CVE-2011-0663</a></td>
<td style="border:1px solid black;"><a href="http://technet.microsoft.com/en-us/security/cc998259.aspx">2</a> - Valószínűleg inkonzisztens rosszindulatú programkód</td>
<td style="border:1px solid black;">(Nincs)</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=210206">MS11-023</a></td>
<td style="border:1px solid black;">A Microsoft Office grafikus objektumának visszakeresésekor fellépő biztonsági rés</td>
<td style="border:1px solid black;"><a href="http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2011-0977">CVE-2011-0977</a></td>
<td style="border:1px solid black;"><a href="http://technet.microsoft.com/en-us/security/cc998259.aspx">2</a> - Valószínűleg inkonzisztens rosszindulatú programkód</td>
<td style="border:1px solid black;">(Nincs)</td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=211826">MS11-034</a></td>
<td style="border:1px solid black;">A Win32k használat utáni felszabadítás miatti biztonsági rése</td>
<td style="border:1px solid black;"><a href="http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2011-1234">CVE-2011-1234</a></td>
<td style="border:1px solid black;"><a href="http://technet.microsoft.com/en-us/security/cc998259.aspx">2</a> - Valószínűleg inkonzisztens rosszindulatú programkód</td>
<td style="border:1px solid black;">(Nincs)</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=212226">MS11-024</a></td>
<td style="border:1px solid black;">A Faxfedőlap-szerkesztő memóriameghibásodást okozó biztonsági rése</td>
<td style="border:1px solid black;"><a href="http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2010-3974">CVE-2010-3974</a></td>
<td style="border:1px solid black;"><a href="http://technet.microsoft.com/en-us/security/cc998259.aspx">3</a> – Nem valószínű működő rosszindulatú programkód</td>
<td style="border:1px solid black;">A biztonsági rés nyilvánosságra került</td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=212226">MS11-024</a></td>
<td style="border:1px solid black;">Faxfedőlap biztonsági rése</td>
<td style="border:1px solid black;"><a href="http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2010-4701">CVE-2010-4701</a></td>
<td style="border:1px solid black;"><a href="http://technet.microsoft.com/en-us/security/cc998259.aspx">3</a> – Nem valószínű működő rosszindulatú programkód</td>
<td style="border:1px solid black;">A biztonsági rés nyilvánosságra került</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=212523">MS11-026</a></td>
<td style="border:1px solid black;">Az MHTML Mime formátumú kérelmek miatti biztonsági rése</td>
<td style="border:1px solid black;"><a href="http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2011-0096">CVE-2011-0096</a></td>
<td style="border:1px solid black;"><a href="http://technet.microsoft.com/en-us/security/cc998259.aspx">3</a> – Nem valószínű működő rosszindulatú programkód</td>
<td style="border:1px solid black;">A biztonsági rés nyilvánosságra került<br />
<br />
A biztonsági rés illetéktelen adatelérést okoz</td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=211826">MS11-034</a></td>
<td style="border:1px solid black;">A Win32k használat utáni felszabadítás miatti biztonsági rése</td>
<td style="border:1px solid black;"><a href="http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2011-1238">CVE-2011-1238</a></td>
<td style="border:1px solid black;"><a href="http://technet.microsoft.com/en-us/security/cc998259.aspx">3</a> – Nem valószínű működő rosszindulatú programkód</td>
<td style="border:1px solid black;">(Nincs)</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=214126">MS11-018</a></td>
<td style="border:1px solid black;">A Javascript alkalmazás információfelfedést okozó biztonsági rése</td>
<td style="border:1px solid black;"><a href="http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2011-1245">CVE-2011-1245</a></td>
<td style="border:1px solid black;"><a href="http://technet.microsoft.com/en-us/security/cc998259.aspx">3</a> – Nem valószínű működő rosszindulatú programkód</td>
<td style="border:1px solid black;">A biztonsági rés illetéktelen adatelérést okoz</td>
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
**Közlemény azonosítója**
</td>
<td style="border:1px solid black;">
[**MS11-018**](http://go.microsoft.com/fwlink/?linkid=214126)
</td>
<td style="border:1px solid black;">
[**MS11-019**](http://go.microsoft.com/fwlink/?linkid=212314)
</td>
<td style="border:1px solid black;">
[**MS11-020**](http://go.microsoft.com/fwlink/?linkid=212236)
</td>
<td style="border:1px solid black;">
[**MS11-027**](http://go.microsoft.com/fwlink/?linkid=214005)
</td>
<td style="border:1px solid black;">
[**MS11-028**](http://go.microsoft.com/fwlink/?linkid=207931)
</td>
<td style="border:1px solid black;">
[**MS11-029**](http://go.microsoft.com/fwlink/?linkid=208524)
</td>
<td style="border:1px solid black;">
[**MS11-030**](http://go.microsoft.com/fwlink/?linkid=212595)
</td>
<td style="border:1px solid black;">
[**MS11-031**](http://go.microsoft.com/fwlink/?linkid=212243)
</td>
<td style="border:1px solid black;">
[**MS11-032**](http://go.microsoft.com/fwlink/?linkid=212224)
</td>
<td style="border:1px solid black;">
[**MS11-024**](http://go.microsoft.com/fwlink/?linkid=212226)
</td>
<td style="border:1px solid black;">
[**MS11-026**](http://go.microsoft.com/fwlink/?linkid=212523)
</td>
<td style="border:1px solid black;">
[**MS11-033**](http://go.microsoft.com/fwlink/?linkid=208110)
</td>
<td style="border:1px solid black;">
[**MS11-034**](http://go.microsoft.com/fwlink/?linkid=211826)
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
[**Kritikus**](http://go.microsoft.com/fwlink/?linkid=21140)
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
</tr>
<tr>
<td style="border:1px solid black;">
Windows XP Service Pack 3
</td>
<td style="border:1px solid black;">
[Internet Explorer 6](http://www.microsoft.com/downloads/details.aspx?familyid=c3a8cec0-f947-4d4e-a6ae-c7f4f1f311b0)  
(Kritikus)  
[Internet Explorer 7](http://www.microsoft.com/downloads/details.aspx?familyid=0b7d0403-8965-4c62-970c-20b561f66713)  
(Kritikus)  
[Internet Explorer 8](http://www.microsoft.com/downloads/details.aspx?familyid=689c5496-56c4-48a6-9f3d-b5f5aaf3e566)  
(Kritikus)
</td>
<td style="border:1px solid black;">
[Windows XP Service Pack 3](http://www.microsoft.com/downloads/details.aspx?familyid=f5378e7b-4619-4c42-9d9f-87b209c6d878)  
(Kritikus)
</td>
<td style="border:1px solid black;">
[Windows XP Service Pack 3](http://www.microsoft.com/downloads/details.aspx?familyid=ccb08a8a-f4d9-4320-8ffb-3fd4fe217987)  
(Kritikus)
</td>
<td style="border:1px solid black;">
[Windows XP Service Pack 3](http://www.microsoft.com/downloads/details.aspx?familyid=b031a496-aa74-4367-b2ae-24843c061745)  
(Kritikus)
</td>
<td style="border:1px solid black;">
[Microsoft .NET-keretrendszer 2.0 Service Pack 2 és Microsoft .NET-keretrendszer 3.5 Service Pack 1](http://www.microsoft.com/downloads/details.aspx?familyid=ce925e76-cb85-48f6-8c0f-e53fa2b09be6)  
(KB2446704)  
(Kritikus)  
[Microsoft .NET-keretrendszer 4.0](http://www.microsoft.com/downloads/details.aspx?familyid=91aa6772-4811-4a58-9bc0-8aa271ed99df)<sup>[1]</sup>
(KB2446708)  
(Kritikus)
</td>
<td style="border:1px solid black;">
[Windows XP Service Pack 3](http://www.microsoft.com/downloads/details.aspx?familyid=59266a9d-a319-4309-a046-7f15c6da0136)  
(KB2412687)  
(Kritikus)
</td>
<td style="border:1px solid black;">
[Windows XP Service Pack 3](http://www.microsoft.com/downloads/details.aspx?familyid=2d433adb-bcaf-4c59-9405-a4892f8ccba3)  
(Fontos)
</td>
<td style="border:1px solid black;">
[JScript 5.7 és VBScript 5.7](http://www.microsoft.com/downloads/details.aspx?familyid=637f4d4c-de07-4c6a-95f8-3bd0cbfe77b2)  
(KB2510581)  
(Kritikus)  
[JScript 5.8 és VBScript 5.8](http://www.microsoft.com/downloads/details.aspx?familyid=fbe1e7e3-1d5f-4daf-a4a5-67fe79292963)  
(KB2510531)  
(Kritikus)
</td>
<td style="border:1px solid black;">
[Windows XP Service Pack 3](http://www.microsoft.com/downloads/details.aspx?familyid=9080c5a1-e638-4047-a70a-9367f1acced7)  
(Fontos)
</td>
<td style="border:1px solid black;">
[Windows XP Service Pack 3](http://www.microsoft.com/downloads/details.aspx?familyid=50fc3869-f2fc-43c8-8049-aad62f2cb332)  
(KB2491683)  
(Fontos)  
[Windows XP Service Pack 3](http://www.microsoft.com/downloads/details.aspx?familyid=a8220a21-02fc-4ad6-988d-844276b2fd66)  
(KB2506212)  
(Fontos)
</td>
<td style="border:1px solid black;">
[Windows XP Service Pack 3](http://www.microsoft.com/downloads/details.aspx?familyid=7f0a4616-8e3e-4925-9d95-ce6e614e45ae)  
(Fontos)
</td>
<td style="border:1px solid black;">
[Windows XP Service Pack 3](http://www.microsoft.com/downloads/details.aspx?familyid=6753ca98-feb4-4c7f-9969-9294038a2bbb)  
(Fontos)
</td>
<td style="border:1px solid black;">
[Windows XP Service Pack 3](http://www.microsoft.com/downloads/details.aspx?familyid=39e55bbf-c1c5-4696-bfe7-632e997cd98e)  
(Fontos)
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
Windows XP Professional x64 Edition Service Pack 2
</td>
<td style="border:1px solid black;">
[Internet Explorer 6](http://www.microsoft.com/downloads/details.aspx?familyid=986f07ae-0fdc-4be2-8a74-5eb56d4300ef)  
(Kritikus)  
[Internet Explorer 7](http://www.microsoft.com/downloads/details.aspx?familyid=ed88f183-dd06-46f6-ae8a-a594a752f248)  
(Kritikus)  
[Internet Explorer 8](http://www.microsoft.com/downloads/details.aspx?familyid=6d3433ee-c2e1-433f-a3d9-c049d66e2190)  
(Kritikus)
</td>
<td style="border:1px solid black;">
[Windows XP Professional x64 Edition Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=c01441da-8933-4f60-923b-d9b00db8ba3d)  
(Kritikus)
</td>
<td style="border:1px solid black;">
[Windows XP Professional x64 Edition Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=7ee202da-a711-42ee-bea3-7202a70e4ea0)  
(Kritikus)
</td>
<td style="border:1px solid black;">
[Windows XP Professional x64 Edition Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=eddd2964-9765-461d-9df8-2c05402948e8)  
(Kritikus)
</td>
<td style="border:1px solid black;">
[Microsoft .NET-keretrendszer 2.0 Service Pack 2 és Microsoft .NET-keretrendszer 3.5 Service Pack 1](http://www.microsoft.com/downloads/details.aspx?familyid=ce925e76-cb85-48f6-8c0f-e53fa2b09be6)  
(KB2446704)  
(Kritikus)  
[Microsoft .NET-keretrendszer 4.0](http://www.microsoft.com/downloads/details.aspx?familyid=91aa6772-4811-4a58-9bc0-8aa271ed99df)<sup>[1]</sup>
(KB2446708)  
(Kritikus)
</td>
<td style="border:1px solid black;">
[Windows XP Professional x64 Edition Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=3797009a-b9a4-4e83-8614-e1589c8b5090)  
(KB2412687)  
(Kritikus)
</td>
<td style="border:1px solid black;">
[Windows XP Professional x64 Edition Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=29ff546e-a232-4f23-a223-c029c71ff1c6)  
(Fontos)
</td>
<td style="border:1px solid black;">
[JScript 5.6 és VBScript 5.6](http://www.microsoft.com/downloads/details.aspx?familyid=a5586246-2908-4def-9298-c16060098197)  
(KB2510587)  
(Kritikus)  
[JScript 5.7 és VBScript 5.7](http://www.microsoft.com/downloads/details.aspx?familyid=3a5f65e0-bb00-4e55-b8b5-77751349a3ec)  
(KB2510581)  
(Kritikus)  
[JScript 5.8 és VBScript 5.8](http://www.microsoft.com/downloads/details.aspx?familyid=57aa7ee2-254d-40b5-9ff0-cba969daf45a)  
(KB2510531)  
(Kritikus)
</td>
<td style="border:1px solid black;">
[Windows XP Professional x64 Edition Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=2374e09a-cb3e-4bc3-bb4b-53b611025121)  
(Fontos)
</td>
<td style="border:1px solid black;">
[Windows XP Professional x64 Edition Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=b93311b4-1b8f-478d-8833-750c5e01e6f8)  
(KB2491683)  
(Fontos)  
[Windows XP Professional x64 Edition Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=0f60fc99-cd88-4237-8b31-a4e618502f7e)  
(KB2506212)  
(Fontos)
</td>
<td style="border:1px solid black;">
[Windows XP Professional x64 Edition Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=b01fe9a5-66a4-4683-963b-e78aea214579)  
(Fontos)
</td>
<td style="border:1px solid black;">
[Windows XP Professional x64 Edition Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=3c94bc96-99ea-44a1-9052-e69de5e21f81)  
(Fontos)
</td>
<td style="border:1px solid black;">
[Windows XP Professional x64 Edition Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=83771177-284e-4918-86a9-980e8229c7c9)  
(Fontos)
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
[**MS11-018**](http://go.microsoft.com/fwlink/?linkid=214126)
</td>
<td style="border:1px solid black;">
[**MS11-019**](http://go.microsoft.com/fwlink/?linkid=212314)
</td>
<td style="border:1px solid black;">
[**MS11-020**](http://go.microsoft.com/fwlink/?linkid=212236)
</td>
<td style="border:1px solid black;">
[**MS11-027**](http://go.microsoft.com/fwlink/?linkid=214005)
</td>
<td style="border:1px solid black;">
[**MS11-028**](http://go.microsoft.com/fwlink/?linkid=207931)
</td>
<td style="border:1px solid black;">
[**MS11-029**](http://go.microsoft.com/fwlink/?linkid=208524)
</td>
<td style="border:1px solid black;">
[**MS11-030**](http://go.microsoft.com/fwlink/?linkid=212595)
</td>
<td style="border:1px solid black;">
[**MS11-031**](http://go.microsoft.com/fwlink/?linkid=212243)
</td>
<td style="border:1px solid black;">
[**MS11-032**](http://go.microsoft.com/fwlink/?linkid=212224)
</td>
<td style="border:1px solid black;">
[**MS11-024**](http://go.microsoft.com/fwlink/?linkid=212226)
</td>
<td style="border:1px solid black;">
[**MS11-026**](http://go.microsoft.com/fwlink/?linkid=212523)
</td>
<td style="border:1px solid black;">
[**MS11-033**](http://go.microsoft.com/fwlink/?linkid=208110)
</td>
<td style="border:1px solid black;">
[**MS11-034**](http://go.microsoft.com/fwlink/?linkid=211826)
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
**Összesített súlyossági besorolás**
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
[**Mérsékelt.**](http://go.microsoft.com/fwlink/?linkid=21140)
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
[**Kritikus**](http://go.microsoft.com/fwlink/?linkid=21140)
</td>
<td style="border:1px solid black;">
[**Fontos**](http://go.microsoft.com/fwlink/?linkid=21140)
</td>
<td style="border:1px solid black;">
[**Fontos**](http://go.microsoft.com/fwlink/?linkid=21140)
</td>
<td style="border:1px solid black;">
[**Alacsony**](http://go.microsoft.com/fwlink/?linkid=21140)
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
[Internet Explorer 6](http://www.microsoft.com/downloads/details.aspx?familyid=b902c58a-9e2f-4352-8d2f-fffda5344598)  
(Mérsékelt)  
[Internet Explorer 7](http://www.microsoft.com/downloads/details.aspx?familyid=5c464287-3dab-4342-a38d-a12719d3b158)  
(Mérsékelt)  
[Internet Explorer 8](http://www.microsoft.com/downloads/details.aspx?familyid=45feb35b-b24e-4160-adb0-d0b7ae530e90)  
(Mérsékelt)
</td>
<td style="border:1px solid black;">
[Windows Server 2003 Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=d46fe0bf-28c2-4696-87bc-dd3c8287fc28)  
(Kritikus)
</td>
<td style="border:1px solid black;">
[Windows Server 2003 Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=64c550d4-c927-4382-91e1-473ed6790819)  
(Kritikus)
</td>
<td style="border:1px solid black;">
[Windows Server 2003 Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=53756404-39e4-43af-81e9-81471536aa66)  
(Mérsékelt)
</td>
<td style="border:1px solid black;">
[Microsoft .NET-keretrendszer 2.0 Service Pack 2 és Microsoft .NET-keretrendszer 3.5 Service Pack 1](http://www.microsoft.com/downloads/details.aspx?familyid=ce925e76-cb85-48f6-8c0f-e53fa2b09be6)  
(KB2446704)  
(Kritikus)  
[Microsoft .NET-keretrendszer 4.0](http://www.microsoft.com/downloads/details.aspx?familyid=91aa6772-4811-4a58-9bc0-8aa271ed99df)<sup>[1]</sup>
(KB2446708)  
(Kritikus)
</td>
<td style="border:1px solid black;">
[Windows Server 2003 Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=fd284233-e177-4064-9b02-f83dcb727dbe)  
(KB2412687)  
(Kritikus)
</td>
<td style="border:1px solid black;">
[Windows Server 2003 Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=753ed6e3-df2e-4b2d-9e9f-7275cd94d214)  
(Fontos)
</td>
<td style="border:1px solid black;">
[JScript 5.6 és VBScript 5.6](http://www.microsoft.com/downloads/details.aspx?familyid=e026f2ed-8a20-4268-9b29-04a78bde1999)  
(KB2510587)  
(Kritikus)  
[JScript 5.7 és VBScript 5.7](http://www.microsoft.com/downloads/details.aspx?familyid=5b0ed0b2-07f9-43da-bb5d-5be5a45969ee)  
(KB2510581)  
(Kritikus)  
[JScript 5.8 és VBScript 5.8](http://www.microsoft.com/downloads/details.aspx?familyid=01aa2beb-9fc1-40f0-a2a4-bcd3d9cb31f8)  
(KB2510531)  
(Kritikus)
</td>
<td style="border:1px solid black;">
[Windows Server 2003 Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=5d71d3f5-fd6b-4f3b-8389-37c899748d4b)  
(Fontos)
</td>
<td style="border:1px solid black;">
[Windows Server 2003 Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=edda8cce-b764-4ef1-afbe-391fbd087362)  
(KB2491683)  
(Fontos)  
[Windows Server 2003 Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=bf084b4c-aac9-4cc6-bb30-87fc96ba9430)  
(KB2506212)  
(Fontos)
</td>
<td style="border:1px solid black;">
[Windows Server 2003 Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=0209a004-f23a-40d9-991f-864046f4605f)  
(Alacsony)
</td>
<td style="border:1px solid black;">
[Windows Server 2003 Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=9fbfc742-6c74-49a2-b3cc-e1d5d8c84b77)  
(Fontos)
</td>
<td style="border:1px solid black;">
[Windows Server 2003 Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=af320f27-bb3a-4e76-a279-4632267c8761)  
(Fontos)
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
Windows Server 2003 x64 Edition Service Pack 2
</td>
<td style="border:1px solid black;">
[Internet Explorer 6](http://www.microsoft.com/downloads/details.aspx?familyid=5d8f14d1-85cc-478f-8b50-5c355a331f59)  
(Mérsékelt)  
[Internet Explorer 7](http://www.microsoft.com/downloads/details.aspx?familyid=9d8bbea9-c456-4569-ad96-c2cd0f5fae7e)  
(Mérsékelt)  
[Internet Explorer 8](http://www.microsoft.com/downloads/details.aspx?familyid=979d2ec5-5114-4ec7-aa97-e9289c590cbb)  
(Mérsékelt)
</td>
<td style="border:1px solid black;">
[Windows Server 2003 x64 Edition Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=ca0fb4d3-7651-4760-83fa-b71c86cbe459)  
(Kritikus)
</td>
<td style="border:1px solid black;">
[Windows Server 2003 x64 Edition Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=ef62db94-4f72-4245-ac9f-6391035e2516)  
(Kritikus)
</td>
<td style="border:1px solid black;">
[Windows Server 2003 x64 Edition Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=c8d59f49-45ec-4527-b3a8-4925f710bbfd)  
(Mérsékelt)
</td>
<td style="border:1px solid black;">
[Microsoft .NET-keretrendszer 2.0 Service Pack 2 és Microsoft .NET-keretrendszer 3.5 Service Pack 1](http://www.microsoft.com/downloads/details.aspx?familyid=ce925e76-cb85-48f6-8c0f-e53fa2b09be6)  
(KB2446704)  
(Kritikus)  
[Microsoft .NET-keretrendszer 4.0](http://www.microsoft.com/downloads/details.aspx?familyid=91aa6772-4811-4a58-9bc0-8aa271ed99df)<sup>[1]</sup>
(KB2446708)  
(Kritikus)
</td>
<td style="border:1px solid black;">
[Windows Server 2003 x64 Edition Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=d5adaf4e-4cd7-42ea-8202-31b5c856f5e3)  
(KB2412687)  
(Kritikus)
</td>
<td style="border:1px solid black;">
[Windows Server 2003 x64 Edition Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=a0192dbc-4d0d-4555-9ef7-3e10209a6389)  
(Fontos)
</td>
<td style="border:1px solid black;">
[JScript 5.6 és VBScript 5.6](http://www.microsoft.com/downloads/details.aspx?familyid=83ce6c99-a57d-4ed1-972b-a6b6798e6675)  
(KB2510587)  
(Kritikus)  
[JScript 5.7 és VBScript 5.7](http://www.microsoft.com/downloads/details.aspx?familyid=af791715-77a1-405b-a69e-d63f75dd7ccd)  
(KB2510581)  
(Kritikus)  
[JScript 5.8 és VBScript 5.8](http://www.microsoft.com/downloads/details.aspx?familyid=bf0a2966-25c4-4717-bcd6-016ce610d220)  
(KB2510531)  
(Kritikus)
</td>
<td style="border:1px solid black;">
[Windows Server 2003 x64 Edition Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=3a498ff0-21d9-493a-b127-6bc20f1baf95)  
(Fontos)
</td>
<td style="border:1px solid black;">
[Windows Server 2003 x64 Edition Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=f04d939a-da11-4a9f-9e03-b6c3bf3ca58b)  
(KB2491683)  
(Fontos)  
[Windows Server 2003 x64 Edition Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=12b01f3a-ccf8-41c1-ac5a-e417a6ddbe95)  
(KB2506212)  
(Fontos)
</td>
<td style="border:1px solid black;">
[Windows Server 2003 x64 Edition Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=6c287571-54ea-4298-8b7d-b98b2c830cc3)  
(Alacsony)
</td>
<td style="border:1px solid black;">
[Windows Server 2003 x64 Edition Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=897b97b0-1bab-4b1b-b417-950fab0d4a65)  
(Fontos)
</td>
<td style="border:1px solid black;">
[Windows Server 2003 x64 Edition Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=9c95f81c-9812-4070-88d7-34422c638e42)  
(Fontos)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Windows Server 2003 SP2 Itanium-alapú rendszerekhez
</td>
<td style="border:1px solid black;">
[Internet Explorer 6](http://www.microsoft.com/downloads/details.aspx?familyid=8afe86fc-58b4-4a95-b047-c09138fa4f5e)  
(Mérsékelt)  
[Internet Explorer 7](http://www.microsoft.com/downloads/details.aspx?familyid=f1abfb48-3c8a-4b2d-b739-cc61628b387d)  
(Mérsékelt)
</td>
<td style="border:1px solid black;">
[Windows Server 2003 SP2 Itanium-alapú rendszerekhez](http://www.microsoft.com/downloads/details.aspx?familyid=87eb8b93-9829-45ec-9528-52787732044e)  
(Kritikus)
</td>
<td style="border:1px solid black;">
[Windows Server 2003 SP2 Itanium-alapú rendszerekhez](http://www.microsoft.com/downloads/details.aspx?familyid=79aeb3cd-7c73-467b-b91e-02c6ea01e911)  
(Kritikus)
</td>
<td style="border:1px solid black;">
[Windows Server 2003 SP2 Itanium-alapú rendszerekhez](http://www.microsoft.com/downloads/details.aspx?familyid=9c784734-f44f-4a3c-8223-6289f7dc2ad8)  
(Nincs súlyossági besorolás<sup>[1]</sup>)
</td>
<td style="border:1px solid black;">
[Microsoft .NET-keretrendszer 2.0 Service Pack 2 és Microsoft .NET-keretrendszer 3.5 Service Pack 1](http://www.microsoft.com/downloads/details.aspx?familyid=ce925e76-cb85-48f6-8c0f-e53fa2b09be6)  
(KB2446704)  
(Kritikus)  
[Microsoft .NET-keretrendszer 4.0](http://www.microsoft.com/downloads/details.aspx?familyid=91aa6772-4811-4a58-9bc0-8aa271ed99df)<sup>[1]</sup>
(KB2446708)  
(Kritikus)
</td>
<td style="border:1px solid black;">
[Windows Server 2003 SP2 Itanium-alapú rendszerekhez](http://www.microsoft.com/downloads/details.aspx?familyid=72a513bb-f901-4992-8562-d1afe1afec8a)  
(KB2412687)  
(Kritikus)
</td>
<td style="border:1px solid black;">
[Windows Server 2003 SP2 Itanium-alapú rendszerekhez](http://www.microsoft.com/downloads/details.aspx?familyid=f5ad6963-2d6a-4d59-9e25-4fc088647fcd)  
(Fontos)
</td>
<td style="border:1px solid black;">
[JScript 5.6 és VBScript 5.6](http://www.microsoft.com/downloads/details.aspx?familyid=b7d36bae-7ca4-4a40-9efb-13f484fa5518)  
(KB2510587)  
(Kritikus)  
[JScript 5.7 és VBScript 5.7](http://www.microsoft.com/downloads/details.aspx?familyid=3f519013-ed14-41a8-aa45-cf8b095d3152)  
(KB2510581)  
(Kritikus)
</td>
<td style="border:1px solid black;">
[Windows Server 2003 SP2 Itanium-alapú rendszerekhez](http://www.microsoft.com/downloads/details.aspx?familyid=c71f4398-2e3b-4b81-a650-8806e618db7f)  
(Fontos)
</td>
<td style="border:1px solid black;">
[Windows Server 2003 SP2 Itanium-alapú rendszerekhez](http://www.microsoft.com/downloads/details.aspx?familyid=efb575c7-3259-49b1-b59c-89d9544e37a6)  
(KB2491683)  
(Fontos)  
[Windows Server 2003 SP2 Itanium-alapú rendszerekhez](http://www.microsoft.com/downloads/details.aspx?familyid=03a7ee49-7bd6-4215-9779-1b48c10d08b9)  
(KB2506212)  
(Fontos)
</td>
<td style="border:1px solid black;">
[Windows Server 2003 SP2 Itanium-alapú rendszerekhez](http://www.microsoft.com/downloads/details.aspx?familyid=3fb450a0-d087-4f36-9301-05ffbf94cc1a)  
(Alacsony)
</td>
<td style="border:1px solid black;">
[Windows Server 2003 SP2 Itanium-alapú rendszerekhez](http://www.microsoft.com/downloads/details.aspx?familyid=ede38974-4e57-4ea1-8731-b91e96534693)  
(Fontos)
</td>
<td style="border:1px solid black;">
[Windows Server 2003 SP2 Itanium-alapú rendszerekhez](http://www.microsoft.com/downloads/details.aspx?familyid=f58cf64a-bf31-4496-be75-5775a123338b)  
(Fontos)
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
[**MS11-018**](http://go.microsoft.com/fwlink/?linkid=214126)
</td>
<td style="border:1px solid black;">
[**MS11-019**](http://go.microsoft.com/fwlink/?linkid=212314)
</td>
<td style="border:1px solid black;">
[**MS11-020**](http://go.microsoft.com/fwlink/?linkid=212236)
</td>
<td style="border:1px solid black;">
[**MS11-027**](http://go.microsoft.com/fwlink/?linkid=214005)
</td>
<td style="border:1px solid black;">
[**MS11-028**](http://go.microsoft.com/fwlink/?linkid=207931)
</td>
<td style="border:1px solid black;">
[**MS11-029**](http://go.microsoft.com/fwlink/?linkid=208524)
</td>
<td style="border:1px solid black;">
[**MS11-030**](http://go.microsoft.com/fwlink/?linkid=212595)
</td>
<td style="border:1px solid black;">
[**MS11-031**](http://go.microsoft.com/fwlink/?linkid=212243)
</td>
<td style="border:1px solid black;">
[**MS11-032**](http://go.microsoft.com/fwlink/?linkid=212224)
</td>
<td style="border:1px solid black;">
[**MS11-024**](http://go.microsoft.com/fwlink/?linkid=212226)
</td>
<td style="border:1px solid black;">
[**MS11-026**](http://go.microsoft.com/fwlink/?linkid=212523)
</td>
<td style="border:1px solid black;">
[**MS11-033**](http://go.microsoft.com/fwlink/?linkid=208110)
</td>
<td style="border:1px solid black;">
[**MS11-034**](http://go.microsoft.com/fwlink/?linkid=211826)
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
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
Windows Vista Service Pack 1 és Windows Vista Service Pack 2
</td>
<td style="border:1px solid black;">
[Internet Explorer 7](http://www.microsoft.com/downloads/details.aspx?familyid=00c3c176-feff-4022-ac4c-2d4732ca3d78)  
(Kritikus)  
[Internet Explorer 8](http://www.microsoft.com/downloads/details.aspx?familyid=5ea94705-4f76-4b0d-bbbc-afb5e75204bf)  
(Kritikus)
</td>
<td style="border:1px solid black;">
[Windows Vista Service Pack 1 és Windows Vista Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=da8dd55d-6630-484e-836c-9feeab5cc311)  
(Kritikus)
</td>
<td style="border:1px solid black;">
[Windows Vista Service Pack 1 és Windows Vista Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=d6eddff4-a242-4dec-9d84-72891db2b754)  
(Kritikus)
</td>
<td style="border:1px solid black;">
[Windows Vista Service Pack 1 és Windows Vista Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=80bf050a-9aff-4cd4-8e2f-196b0a92b1c0)  
(Kritikus)
</td>
<td style="border:1px solid black;">
Csak Windows Vista Service Pack 1:  
[Microsoft .NET-keretrendszer 2.0 Service Pack 2 és Microsoft .NET-keretrendszer 3.5 Service Pack 1](http://www.microsoft.com/downloads/details.aspx?familyid=94b6a1b3-e048-437b-a224-2a64b3735bc3)  
(KB2449741)  
(Kritikus)  
Csak Windows Vista Service Pack 2:  
[Microsoft .NET-keretrendszer 2.0 Service Pack 2 és Microsoft .NET-keretrendszer 3.5 Service Pack 1](http://www.microsoft.com/downloads/details.aspx?familyid=1407aaec-b3e0-404c-b84f-0c8e808614c4)  
(KB2449742)  
(Kritikus)  
Windows Vista Service Pack 1 és Windows Vista Service Pack 2:  
[Microsoft .NET-keretrendszer 4.0](http://www.microsoft.com/downloads/details.aspx?familyid=91aa6772-4811-4a58-9bc0-8aa271ed99df)<sup>[1]</sup>
(KB2446708)  
(Kritikus)
</td>
<td style="border:1px solid black;">
[Windows Vista Service Pack 1 és Windows Vista Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=4ff2e440-79c2-4045-b225-913d1740fdb9)  
(KB2412687)  
(Kritikus)
</td>
<td style="border:1px solid black;">
[Windows Vista Service Pack 1 és Windows Vista Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=2a17e44f-54aa-423d-b3c7-a4f404f7c28b)  
(Kritikus)
</td>
<td style="border:1px solid black;">
[JScript 5.7 és VBScript 5.7](http://www.microsoft.com/downloads/details.aspx?familyid=719e2c86-30e5-4cd5-94f4-d6de54efee5f)  
(KB2510581)  
(Kritikus)  
[JScript 5.8 és VBScript 5.8](http://www.microsoft.com/downloads/details.aspx?familyid=21decb84-75ef-4bde-a802-1e661a505e94)<sup>[1]</sup>
(KB2510531)  
(Kritikus)
</td>
<td style="border:1px solid black;">
[Windows Vista Service Pack 1 és Windows Vista Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=e7c4fc81-d1ef-4378-862b-e955d75fb2de)  
(Kritikus)
</td>
<td style="border:1px solid black;">
[Windows Vista Service Pack 1 és Windows Vista Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=11a8f240-51b3-4e31-a24a-a235179f3396)  
(KB2491683)  
(Fontos)  
[Windows Vista Service Pack 1 és Windows Vista Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=e6cba040-9d7c-4777-a2f7-e4dd11dfb845)  
(KB2506212)  
(Fontos)
</td>
<td style="border:1px solid black;">
[Windows Vista Service Pack 1 és Windows Vista Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=c8fce0fb-4c90-479b-8ce9-75e60d52d256)  
(Fontos)
</td>
<td style="border:1px solid black;">
Nem érintett
</td>
<td style="border:1px solid black;">
[Windows Vista Service Pack 1 és Windows Vista Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=b4743167-9614-445a-9e91-10efdac505a8)  
(Fontos)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Windows Vista x64 Edition Service Pack 1 és Windows Vista x64 Edition Service Pack 2
</td>
<td style="border:1px solid black;">
[Internet Explorer 7](http://www.microsoft.com/downloads/details.aspx?familyid=79f52733-44e4-47b6-86ca-1395a095b4e7)  
(Kritikus)  
[Internet Explorer 8](http://www.microsoft.com/downloads/details.aspx?familyid=bc63b233-9db0-4fb1-a61c-fa7e9e44ba10)  
(Kritikus)
</td>
<td style="border:1px solid black;">
[Windows Vista x64 Edition Service Pack 1 és Windows Vista x64 Edition Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=040f8b46-f458-4a72-a1b0-ad8a65a1194c)  
(Kritikus)
</td>
<td style="border:1px solid black;">
[Windows Vista x64 Edition Service Pack 1 és Windows Vista x64 Edition Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=2878c587-6544-40b4-9288-fc3b3ce1128d)  
(Kritikus)
</td>
<td style="border:1px solid black;">
[Windows Vista x64 Edition Service Pack 1 és Windows Vista x64 Edition Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=a81412d0-2516-4bf4-87f7-3e41ebf6b82b)  
(Kritikus)
</td>
<td style="border:1px solid black;">
Csak Windows Vista x64 Edition Service Pack 1:  
[Microsoft .NET-keretrendszer 2.0 Service Pack 2 és Microsoft .NET-keretrendszer 3.5 Service Pack 1](http://www.microsoft.com/downloads/details.aspx?familyid=94b6a1b3-e048-437b-a224-2a64b3735bc3)  
(KB2449741)  
(Kritikus)  
Csak Windows Vista x64 Edition Service Pack 2:  
[Microsoft .NET-keretrendszer 2.0 Service Pack 2 és Microsoft .NET-keretrendszer 3.5 Service Pack 1](http://www.microsoft.com/downloads/details.aspx?familyid=1407aaec-b3e0-404c-b84f-0c8e808614c4)  
(KB2449742)  
(Kritikus)  
Windows Vista x64 Edition Service Pack 1 és Windows Vista x64 Edition Service Pack 2:  
[Microsoft .NET-keretrendszer 4.0](http://www.microsoft.com/downloads/details.aspx?familyid=91aa6772-4811-4a58-9bc0-8aa271ed99df)<sup>[1]</sup>
(KB2446708)  
(Kritikus)
</td>
<td style="border:1px solid black;">
[Windows Vista x64 Edition Service Pack 1 és Windows Vista x64 Edition Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=4d826026-e62a-4cec-8682-49fbe7f65cd6)  
(KB2412687)  
(Kritikus)
</td>
<td style="border:1px solid black;">
[Windows Vista x64 Edition Service Pack 1 és Windows Vista x64 Edition Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=e708d24f-e348-4c4d-99ed-e78dd1689d01)  
(Kritikus)
</td>
<td style="border:1px solid black;">
[JScript 5.7 és VBScript 5.7](http://www.microsoft.com/downloads/details.aspx?familyid=89b9d01e-bcbc-4f2c-973b-51051494f406)  
(KB2510581)  
(Kritikus)  
[JScript 5.8 és VBScript 5.8](http://www.microsoft.com/downloads/details.aspx?familyid=d4ac199e-7bf8-4661-a4e5-c53719b2673a)<sup>[1]</sup>
(KB2510531)  
(Kritikus)
</td>
<td style="border:1px solid black;">
[Windows Vista x64 Edition Service Pack 1 és Windows Vista x64 Edition Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=8d654a78-0e4f-452c-8874-fbf478813857)  
(Kritikus)
</td>
<td style="border:1px solid black;">
[Windows Vista x64 Edition Service Pack 1 és Windows Vista x64 Edition Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=61db662e-88d7-4454-b4b7-e987728fb137)  
(KB2491683)  
(Fontos)  
[Windows Vista x64 Edition Service Pack 1 és Windows Vista x64 Edition Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=1c942282-0f80-46c1-aeef-1ef948e105a3)  
(KB2506212)  
(Fontos)
</td>
<td style="border:1px solid black;">
[Windows Vista x64 Edition Service Pack 1 és Windows Vista x64 Edition Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=7da10b64-d0a9-4e42-aa3a-87c657122a8c)  
(Fontos)
</td>
<td style="border:1px solid black;">
Nem érintett
</td>
<td style="border:1px solid black;">
[Windows Vista x64 Edition Service Pack 1 és Windows Vista x64 Edition Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=7e410d5c-b9f7-4a63-8300-36b2d57c6128)  
(Fontos)
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
[**MS11-018**](http://go.microsoft.com/fwlink/?linkid=214126)
</td>
<td style="border:1px solid black;">
[**MS11-019**](http://go.microsoft.com/fwlink/?linkid=212314)
</td>
<td style="border:1px solid black;">
[**MS11-020**](http://go.microsoft.com/fwlink/?linkid=212236)
</td>
<td style="border:1px solid black;">
[**MS11-027**](http://go.microsoft.com/fwlink/?linkid=214005)
</td>
<td style="border:1px solid black;">
[**MS11-028**](http://go.microsoft.com/fwlink/?linkid=207931)
</td>
<td style="border:1px solid black;">
[**MS11-029**](http://go.microsoft.com/fwlink/?linkid=208524)
</td>
<td style="border:1px solid black;">
[**MS11-030**](http://go.microsoft.com/fwlink/?linkid=212595)
</td>
<td style="border:1px solid black;">
[**MS11-031**](http://go.microsoft.com/fwlink/?linkid=212243)
</td>
<td style="border:1px solid black;">
[**MS11-032**](http://go.microsoft.com/fwlink/?linkid=212224)
</td>
<td style="border:1px solid black;">
[**MS11-024**](http://go.microsoft.com/fwlink/?linkid=212226)
</td>
<td style="border:1px solid black;">
[**MS11-026**](http://go.microsoft.com/fwlink/?linkid=212523)
</td>
<td style="border:1px solid black;">
[**MS11-033**](http://go.microsoft.com/fwlink/?linkid=208110)
</td>
<td style="border:1px solid black;">
[**MS11-034**](http://go.microsoft.com/fwlink/?linkid=211826)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
**Összesített súlyossági besorolás**
</td>
<td style="border:1px solid black;">
[**Mérsékelt.**](http://go.microsoft.com/fwlink/?linkid=21140)
</td>
<td style="border:1px solid black;">
[**Kritikus**](http://go.microsoft.com/fwlink/?linkid=21140)
</td>
<td style="border:1px solid black;">
[**Kritikus**](http://go.microsoft.com/fwlink/?linkid=21140)
</td>
<td style="border:1px solid black;">
[**Mérsékelt.**](http://go.microsoft.com/fwlink/?linkid=21140)
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
[**Kritikus**](http://go.microsoft.com/fwlink/?linkid=21140)
</td>
<td style="border:1px solid black;">
[**Fontos**](http://go.microsoft.com/fwlink/?linkid=21140)
</td>
<td style="border:1px solid black;">
[**Alacsony**](http://go.microsoft.com/fwlink/?linkid=21140)
</td>
<td style="border:1px solid black;">
Nincsenek
</td>
<td style="border:1px solid black;">
[**Fontos**](http://go.microsoft.com/fwlink/?linkid=21140)
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
Windows Server 2008 32 bites rendszerekhez és Windows Server 2008 32 bites rendszerekhez, Service Pack 2
</td>
<td style="border:1px solid black;">
[Internet Explorer 7](http://www.microsoft.com/downloads/details.aspx?familyid=7d8603b8-bb52-4cf6-be8b-bb3475d30fc5)\*\*  
(Mérsékelt)  
[Internet Explorer 8](http://www.microsoft.com/downloads/details.aspx?familyid=d5d76e90-1cef-47e8-9d8d-2c5a43f42ba3)\*\*  
(Mérsékelt)
</td>
<td style="border:1px solid black;">
[Windows Server 2008 32 bites rendszerekhez és Windows Server 2008 32 bites rendszerekhez, Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=f8c9390a-5ca1-492a-9e35-a516de48deb5)\*  
(Kritikus)
</td>
<td style="border:1px solid black;">
[Windows Server 2008 32 bites rendszerekhez és Windows Server 2008 32 bites rendszerekhez, Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=31c48ba9-7774-4633-862d-5c27c3703584)\*  
(Kritikus)
</td>
<td style="border:1px solid black;">
[Windows Server 2008 32 bites rendszerekhez és Windows Server 2008 32 bites rendszerekhez Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=c3247886-76d0-4292-be9d-3e9b0221c46a)\*\*  
(Mérsékelt)
</td>
<td style="border:1px solid black;">
Csak Windows Server 2008 32 bites rendszerekhez:  
[Microsoft .NET-keretrendszer 2.0 Service Pack 2 és Microsoft .NET-keretrendszer 3.5 Service Pack 1](http://www.microsoft.com/downloads/details.aspx?familyid=94b6a1b3-e048-437b-a224-2a64b3735bc3)\*\*  
(KB2449741)  
(Kritikus)  
Csak Windows Server 2008 32 bites rendszerekhez Service Pack 2\* esetén:  
[Microsoft .NET-keretrendszer 2.0 Service Pack 2 és Microsoft .NET-keretrendszer 3.5 Service Pack 1](http://www.microsoft.com/downloads/details.aspx?familyid=1407aaec-b3e0-404c-b84f-0c8e808614c4)\*\*  
(KB2449742)  
(Kritikus)  
Windows Server 2008 32 bites rendszerekhez és Windows Server 2008 32 bites rendszerekhez, Service Pack 2:  
[Microsoft .NET-keretrendszer 4.0](http://www.microsoft.com/downloads/details.aspx?familyid=91aa6772-4811-4a58-9bc0-8aa271ed99df)\*\*<sup>[1]</sup>
(KB2446708)  
(Kritikus)
</td>
<td style="border:1px solid black;">
[Windows Server 2008 32 bites rendszerekhez és Windows Server 2008 32 bites rendszerekhez, Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=fbada866-7d36-4b85-acde-fd856a998737)\*\*\*  
(KB2412687)  
(Kritikus)
</td>
<td style="border:1px solid black;">
[Windows Server 2008 32 bites rendszerekhez és Windows Server 2008 32 bites rendszerekhez, Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=9894be38-a582-4c15-ad0e-cc3afab2aebc)\*  
(Kritikus)
</td>
<td style="border:1px solid black;">
[JScript 5.7 és VBScript 5.7](http://www.microsoft.com/downloads/details.aspx?familyid=d8b33ffd-eff1-4a10-b6fc-3c8f01e0fec5)\*\*  
(KB2510581)  
(Kritikus)  
[JScript 5.8 és VBScript 5.8](http://www.microsoft.com/downloads/details.aspx?familyid=afd128ff-717f-4d98-b214-f2c28d59623d)\*\*<sup>[1]</sup>
(KB2510531)  
(Kritikus)
</td>
<td style="border:1px solid black;">
[Windows Server 2008 32 bites rendszerekhez és Windows Server 2008 32 bites rendszerekhez, Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=9105377e-83c7-4010-8fd6-26e42e98c2cc)\*  
(Kritikus)
</td>
<td style="border:1px solid black;">
[Windows Server 2008 32 bites rendszerekhez és Windows Server 2008 32 bites rendszerekhez Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=90f56368-776b-4d45-ad68-91afbd316d25)\*\*  
(KB2491683)  
(Fontos)  
[Windows Server 2008 32 bites rendszerekhez és Windows Server 2008 32 bites rendszerekhez, Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=fa972742-1166-4a9e-ab64-6a4f968f9c6d)\*  
(KB2506212)  
(Fontos)
</td>
<td style="border:1px solid black;">
[Windows Server 2008 32 bites rendszerekhez és Windows Server 2008 32 bites rendszerekhez Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=036f1285-7484-4e3b-8799-2c6c08166596)\*\*  
(Alacsony)
</td>
<td style="border:1px solid black;">
Nem érintett
</td>
<td style="border:1px solid black;">
[Windows Server 2008 32 bites rendszerekhez és Windows Server 2008 32 bites rendszerekhez, Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=c6ac26b8-8cc8-40fe-baab-22bf13df1aa8)\*  
(Fontos)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Windows Server 2008 x64-alapú rendszerekhez és Windows Server 2008 x64-alapú rendszerekhez, Service Pack 2
</td>
<td style="border:1px solid black;">
[Internet Explorer 7](http://www.microsoft.com/downloads/details.aspx?familyid=c6d58f64-bdd5-4fe6-96f4-9641b8e7b570)\*\*  
(Mérsékelt)  
[Internet Explorer 8](http://www.microsoft.com/downloads/details.aspx?familyid=51203a31-368b-4b47-96a5-9e9e5a55cd76)\*\*  
(Mérsékelt)
</td>
<td style="border:1px solid black;">
[Windows Server 2008 x64 alapú rendszerekhez és Windows Server 2008 x64 alapú rendszerekhez, Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=b0cfd5e0-6de5-4863-b5e4-b223a0e36d72)\*  
(Kritikus)
</td>
<td style="border:1px solid black;">
[Windows Server 2008 x64 alapú rendszerekhez és Windows Server 2008 x64 alapú rendszerekhez, Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=de843115-cf98-4511-aa93-f620e4572555)\*  
(Kritikus)
</td>
<td style="border:1px solid black;">
[Windows Server 2008 x64 alapú rendszerekhez és Windows Server 2008 x64 alapú rendszerekhez Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=51521b6b-94a7-4bcf-ad5f-fc304728b10f)\*\*  
(Mérsékelt)
</td>
<td style="border:1px solid black;">
Csak Windows Server 2008 x64 alapú rendszerekhez:  
[Microsoft .NET-keretrendszer 2.0 Service Pack 2 és Microsoft .NET-keretrendszer 3.5 Service Pack 1](http://www.microsoft.com/downloads/details.aspx?familyid=94b6a1b3-e048-437b-a224-2a64b3735bc3)\*\*  
(KB2449741)  
(Kritikus)  
Csak Windows Server 2008 x64 alapú rendszerekhez, Service Pack 2:  
[Microsoft .NET-keretrendszer 2.0 Service Pack 2 és Microsoft .NET-keretrendszer 3.5 Service Pack 1](http://www.microsoft.com/downloads/details.aspx?familyid=1407aaec-b3e0-404c-b84f-0c8e808614c4)\*\*  
(KB2449742)  
(Kritikus)  
Windows Server 2008 x64 alapú rendszerekhez és Windows Server 2008 x64 alapú rendszerekhez, Service Pack 2:  
[Microsoft .NET-keretrendszer 4.0](http://www.microsoft.com/downloads/details.aspx?familyid=91aa6772-4811-4a58-9bc0-8aa271ed99df)\*\*<sup>[1]</sup>
(KB2446708)  
(Kritikus)
</td>
<td style="border:1px solid black;">
[Windows Server 2008 x64-alapú rendszerekhez és Windows Server 2008 x64-alapú rendszerekhez, Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=8f4ddfcb-374d-4cad-8c61-2b988b46f628)\*\*\*  
(KB2412687)  
(Kritikus)
</td>
<td style="border:1px solid black;">
[Windows Server 2008 x64 alapú rendszerekhez és Windows Server 2008 x64 alapú rendszerekhez, Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=2d7d2021-020f-4cc9-a027-258d7e5faec9)\*  
(Kritikus)
</td>
<td style="border:1px solid black;">
[JScript 5.7 és VBScript 5.7](http://www.microsoft.com/downloads/details.aspx?familyid=6c2e6b87-afcd-461a-8a43-9a2fb277b18a)\*\*  
(KB2510581)  
(Kritikus)  
[JScript 5.8 és VBScript 5.8](http://www.microsoft.com/downloads/details.aspx?familyid=40e8beca-0b5a-43b0-98f8-b32a82ad65d6)\*\*<sup>[1]</sup>
(KB2510531)  
(Kritikus)
</td>
<td style="border:1px solid black;">
[Windows Server 2008 x64 alapú rendszerekhez és Windows Server 2008 x64 alapú rendszerekhez, Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=060e8b20-edca-4427-9d60-eb57261eb668)\*  
(Kritikus)
</td>
<td style="border:1px solid black;">
[Windows Server 2008 x64 alapú rendszerekhez és Windows Server 2008 x64 alapú rendszerekhez Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=22a001fc-5c2e-4539-85c9-0c2054a1777d)\*\*  
(KB2491683)  
(Fontos)  
[Windows Server 2008 x64 alapú rendszerekhez és Windows Server 2008 x64 alapú rendszerekhez, Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=fc250c8a-ebaf-4264-9393-dc23cc372d9f)\*  
(KB2506212)  
(Fontos)
</td>
<td style="border:1px solid black;">
[Windows Server 2008 x64 alapú rendszerekhez és Windows Server 2008 x64 alapú rendszerekhez Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=1438cec8-8dab-4510-ad75-dc6959dac0d8)\*\*  
(Alacsony)
</td>
<td style="border:1px solid black;">
Nem érintett
</td>
<td style="border:1px solid black;">
[Windows Server 2008 x64 alapú rendszerekhez és Windows Server 2008 x64 alapú rendszerekhez, Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=ac49f5d3-5e2f-4916-99be-a3254278da7e)\*  
(Fontos)
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
Windows Server 2008 Itanium-alapú rendszerekhez és Windows Server 2008 Itanium-alapú rendszerekhez, Service Pack 2
</td>
<td style="border:1px solid black;">
[Internet Explorer 7](http://www.microsoft.com/downloads/details.aspx?familyid=f6f6f22c-fc7f-4e96-b6b5-be3c1acecf6e)  
(Mérsékelt)
</td>
<td style="border:1px solid black;">
[Windows Server 2008 Itanium-alapú rendszerekhez és Windows Server 2008 Itanium-alapú rendszerekhez, Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=8eaf51cd-2f6e-4bbc-bc4f-9deed03649ac)  
(Kritikus)
</td>
<td style="border:1px solid black;">
[Windows Server 2008 Itanium-alapú rendszerekhez és Windows Server 2008 Itanium-alapú rendszerekhez, Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=b89b8e28-cd98-4bcc-8729-5e51d52d1e92)  
(Kritikus)
</td>
<td style="border:1px solid black;">
[Windows Server 2008 Itanium-alapú rendszerekhez és Windows Server 2008 Itanium-alapú rendszerekhez, Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=e7c38b0d-7240-420a-88d3-2749a40e386f)  
(Nincs súlyossági besorolás<sup>[1]</sup>)
</td>
<td style="border:1px solid black;">
Csak Windows Server 2008 Itanium alapú rendszerekhez:  
[Microsoft .NET-keretrendszer 2.0 Service Pack 2 és Microsoft .NET-keretrendszer 3.5 Service Pack 1](http://www.microsoft.com/downloads/details.aspx?familyid=94b6a1b3-e048-437b-a224-2a64b3735bc3)  
(KB2449741)  
(Kritikus)  
Csak Windows Server 2008 Itanium alapú rendszerekhez, Service Pack 2:  
[Microsoft .NET-keretrendszer 2.0 Service Pack 2 és Microsoft .NET-keretrendszer 3.5 Service Pack 1](http://www.microsoft.com/downloads/details.aspx?familyid=1407aaec-b3e0-404c-b84f-0c8e808614c4)  
(KB2449742)  
(Kritikus)  
Windows Server 2008 Itanium alapú rendszerekhez és Windows Server 2008 Itanium alapú rendszerekhez, Service Pack 2:  
[Microsoft .NET-keretrendszer 4.0](http://www.microsoft.com/downloads/details.aspx?familyid=91aa6772-4811-4a58-9bc0-8aa271ed99df)<sup>[1]</sup>
(KB2446708)  
(Kritikus)
</td>
<td style="border:1px solid black;">
[Windows Server 2008 Itanium-alapú rendszerekhez és Windows Server 2008 Itanium-alapú rendszerekhez, Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=2fd71543-0e18-4907-89b9-355d24d7db69)  
(KB2412687)  
(Kritikus)
</td>
<td style="border:1px solid black;">
[Windows Server 2008 Itanium-alapú rendszerekhez és Windows Server 2008 Itanium-alapú rendszerekhez, Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=c0275df0-10ac-4500-ab86-b7e9a34f8e1d)  
(Kritikus)
</td>
<td style="border:1px solid black;">
[JScript 5.7 és VBScript 5.7](http://www.microsoft.com/downloads/details.aspx?familyid=afb49d24-1913-4e5f-a3ea-c6c9642e2017)  
(KB2510581)  
(Kritikus)
</td>
<td style="border:1px solid black;">
[Windows Server 2008 Itanium-alapú rendszerekhez és Windows Server 2008 Itanium-alapú rendszerekhez, Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=2b8571cb-2dae-4bff-9f13-feb89840044c)  
(Kritikus)
</td>
<td style="border:1px solid black;">
[Windows Server 2008 Itanium-alapú rendszerekhez és Windows Server 2008 Itanium-alapú rendszerekhez, Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=421024f1-aa86-459e-b6de-53851a3fcba2)  
(KB2506212)  
(Fontos)
</td>
<td style="border:1px solid black;">
[Windows Server 2008 Itanium-alapú rendszerekhez és Windows Server 2008 Itanium-alapú rendszerekhez, Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=f35ecdd1-6b5c-40e7-a00b-ca083bdf5cba)  
(Alacsony)
</td>
<td style="border:1px solid black;">
Nem érintett
</td>
<td style="border:1px solid black;">
[Windows Server 2008 Itanium-alapú rendszerekhez és Windows Server 2008 Itanium-alapú rendszerekhez, Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=3b93de4f-01f4-4efd-afc1-31d87b92fad2)  
(Fontos)
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
[**MS11-018**](http://go.microsoft.com/fwlink/?linkid=214126)
</td>
<td style="border:1px solid black;">
[**MS11-019**](http://go.microsoft.com/fwlink/?linkid=212314)
</td>
<td style="border:1px solid black;">
[**MS11-020**](http://go.microsoft.com/fwlink/?linkid=212236)
</td>
<td style="border:1px solid black;">
[**MS11-027**](http://go.microsoft.com/fwlink/?linkid=214005)
</td>
<td style="border:1px solid black;">
[**MS11-028**](http://go.microsoft.com/fwlink/?linkid=207931)
</td>
<td style="border:1px solid black;">
[**MS11-029**](http://go.microsoft.com/fwlink/?linkid=208524)
</td>
<td style="border:1px solid black;">
[**MS11-030**](http://go.microsoft.com/fwlink/?linkid=212595)
</td>
<td style="border:1px solid black;">
[**MS11-031**](http://go.microsoft.com/fwlink/?linkid=212243)
</td>
<td style="border:1px solid black;">
[**MS11-032**](http://go.microsoft.com/fwlink/?linkid=212224)
</td>
<td style="border:1px solid black;">
[**MS11-024**](http://go.microsoft.com/fwlink/?linkid=212226)
</td>
<td style="border:1px solid black;">
[**MS11-026**](http://go.microsoft.com/fwlink/?linkid=212523)
</td>
<td style="border:1px solid black;">
[**MS11-033**](http://go.microsoft.com/fwlink/?linkid=208110)
</td>
<td style="border:1px solid black;">
[**MS11-034**](http://go.microsoft.com/fwlink/?linkid=211826)
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
</tr>
<tr>
<td style="border:1px solid black;">
Windows 7 32 bites rendszerekhez és Windows 7 32 bites rendszerekhez Service Pack 1
</td>
<td style="border:1px solid black;">
[Internet Explorer 8](http://www.microsoft.com/downloads/details.aspx?familyid=59676b71-8b9d-4230-a9e0-b20db3e3ec7e)  
(Kritikus)
</td>
<td style="border:1px solid black;">
[Windows 7 32 bites rendszerekhez és Windows 7 32 bites rendszerekhez Service Pack 1](http://www.microsoft.com/downloads/details.aspx?familyid=0dcba089-19f7-46ca-9e52-24eaebad4715)  
(Kritikus)
</td>
<td style="border:1px solid black;">
[Windows 7 32 bites rendszerekhez és Windows 7 32 bites rendszerekhez Service Pack 1](http://www.microsoft.com/downloads/details.aspx?familyid=d3ef905b-3584-4842-9ec2-cf3856305d49)  
(Kritikus)
</td>
<td style="border:1px solid black;">
[Windows 7 32 bites rendszerekhez és Windows 7 32 bites rendszerekhez Service Pack 1](http://www.microsoft.com/downloads/details.aspx?familyid=46510959-e4a2-4c21-b33c-fd3d97b3ac3d)  
(Kritikus)
</td>
<td style="border:1px solid black;">
Csak Windows 7 32 bites rendszerekhez:  
[Microsoft .NET-keretrendszer 3.5.1](http://www.microsoft.com/downloads/details.aspx?familyid=157aa425-953c-4fc9-ab76-4e65d4be8baa)  
(KB2446709)  
(Kritikus)  
Csak Windows 7 32 bites rendszerekhez, Service Pack 1:  
[Microsoft .NET-keretrendszer 3.5.1](http://www.microsoft.com/downloads/details.aspx?familyid=8f87b8aa-1a2a-405e-aee0-9247d553756a)  
(KB2446710)  
(Kritikus)  
Windows 7 32 bites rendszerekhez és Windows 7 32 bites rendszerekhez, Service Pack 1:  
[Microsoft .NET-keretrendszer 4.0](http://www.microsoft.com/downloads/details.aspx?familyid=91aa6772-4811-4a58-9bc0-8aa271ed99df)<sup>[1]</sup>
(KB2446708)  
(Kritikus)
</td>
<td style="border:1px solid black;">
Nem érintett
</td>
<td style="border:1px solid black;">
[Windows 7 32 bites rendszerekhez és Windows 7 32 bites rendszerekhez Service Pack 1](http://www.microsoft.com/downloads/details.aspx?familyid=8fdae09b-d1bb-4ef5-aa45-2a05f2a5e12d)  
(Kritikus)
</td>
<td style="border:1px solid black;">
[JScript 5.8 és VBScript 5.8](http://www.microsoft.com/downloads/details.aspx?familyid=17ebf291-fdae-4e78-9377-871b3103ce16)<sup>[1]</sup>
(KB2510531)  
(Kritikus)
</td>
<td style="border:1px solid black;">
[Windows 7 32 bites rendszerekhez és Windows 7 32 bites rendszerekhez Service Pack 1](http://www.microsoft.com/downloads/details.aspx?familyid=751c45ea-0943-4948-807f-8716c6ff9198)  
(Kritikus)
</td>
<td style="border:1px solid black;">
[Windows 7 32 bites rendszerekhez és Windows 7 32 bites rendszerekhez Service Pack 1](http://www.microsoft.com/downloads/details.aspx?familyid=bf762b86-b949-4e84-8ca4-93ebe669c1b8)  
(KB2491683)  
(Fontos)  
[Windows 7 32 bites rendszerekhez és Windows 7 32 bites rendszerekhez Service Pack 1](http://www.microsoft.com/downloads/details.aspx?familyid=0f5a122e-dd5e-4b08-881a-f13b38642720)  
(KB2506212)  
(Fontos)
</td>
<td style="border:1px solid black;">
[Windows 7 32 bites rendszerekhez és Windows 7 32 bites rendszerekhez Service Pack 1](http://www.microsoft.com/downloads/details.aspx?familyid=aed201c1-f1fb-4df9-8875-6f57ea0eb15b)  
(Fontos)
</td>
<td style="border:1px solid black;">
Nem érintett
</td>
<td style="border:1px solid black;">
[Windows 7 32 bites rendszerekhez és Windows 7 32 bites rendszerekhez Service Pack 1](http://www.microsoft.com/downloads/details.aspx?familyid=6e7ff003-ff3f-49bb-8e45-d869885dd8d7)  
(Fontos)
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
Windows 7 x64 alapú rendszerekhez és Windows 7 x64 alapú rendszerekhez Service Pack 1
</td>
<td style="border:1px solid black;">
[Internet Explorer 8](http://www.microsoft.com/downloads/details.aspx?familyid=3a998678-2678-489e-8711-39322663147d)  
(Kritikus)
</td>
<td style="border:1px solid black;">
[Windows 7 x64 alapú rendszerekhez és Windows 7 x64 alapú rendszerekhez Service Pack 1](http://www.microsoft.com/downloads/details.aspx?familyid=b7fd356a-56d0-4638-8901-40acfa600f25)  
(Kritikus)
</td>
<td style="border:1px solid black;">
[Windows 7 x64 alapú rendszerekhez és Windows 7 x64 alapú rendszerekhez Service Pack 1](http://www.microsoft.com/downloads/details.aspx?familyid=7ddc943b-6868-4e8f-a869-89b47133c287)  
(Kritikus)
</td>
<td style="border:1px solid black;">
[Windows 7 x64 alapú rendszerekhez és Windows 7 x64 alapú rendszerekhez Service Pack 1](http://www.microsoft.com/downloads/details.aspx?familyid=432555cf-aed8-4329-a74f-526441521082)  
(Kritikus)
</td>
<td style="border:1px solid black;">
Csak Windows 7 x64 alapú rendszerekhez:  
[Microsoft .NET-keretrendszer 3.5.1](http://www.microsoft.com/downloads/details.aspx?familyid=157aa425-953c-4fc9-ab76-4e65d4be8baa)  
(KB2446709)  
(Kritikus)  
Csak Windows 7 x64-alapú rendszerekhez, Service Pack 1:  
[Microsoft .NET-keretrendszer 3.5.1](http://www.microsoft.com/downloads/details.aspx?familyid=8f87b8aa-1a2a-405e-aee0-9247d553756a)  
(KB2446710)  
(Kritikus)  
Windows 7 x64-alapú rendszerekhez és Windows 7 x64-alapú rendszerekhez, Service Pack 1:  
[Microsoft .NET-keretrendszer 4.0](http://www.microsoft.com/downloads/details.aspx?familyid=91aa6772-4811-4a58-9bc0-8aa271ed99df)<sup>[1]</sup>
(KB2446708)  
(Kritikus)
</td>
<td style="border:1px solid black;">
Nem érintett
</td>
<td style="border:1px solid black;">
[Windows 7 x64 alapú rendszerekhez és Windows 7 x64 alapú rendszerekhez Service Pack 1](http://www.microsoft.com/downloads/details.aspx?familyid=40879dfb-efa4-41ba-8d5c-22e926a55eef)  
(Kritikus)
</td>
<td style="border:1px solid black;">
[JScript 5.8 és VBScript 5.8](http://www.microsoft.com/downloads/details.aspx?familyid=c95ad86d-da58-4d7a-9ffd-8441f92baaa5)<sup>[1]</sup>
(KB2510531)  
(Kritikus)
</td>
<td style="border:1px solid black;">
[Windows 7 x64 alapú rendszerekhez és Windows 7 x64 alapú rendszerekhez Service Pack 1](http://www.microsoft.com/downloads/details.aspx?familyid=976c882a-bc07-4128-927f-82a2df46cf45)  
(Kritikus)
</td>
<td style="border:1px solid black;">
[Windows 7 x64 alapú rendszerekhez és Windows 7 x64 alapú rendszerekhez Service Pack 1](http://www.microsoft.com/downloads/details.aspx?familyid=a6793ecf-a3f6-4989-8e4c-c5c0005f9ac4)  
(KB2491683)  
(Fontos)  
[Windows 7 x64 alapú rendszerekhez és Windows 7 x64 alapú rendszerekhez Service Pack 1](http://www.microsoft.com/downloads/details.aspx?familyid=658301f1-103a-48a2-9b67-61cf8e1dad50)  
(KB2506212)  
(Fontos)
</td>
<td style="border:1px solid black;">
[Windows 7 x64 alapú rendszerekhez és Windows 7 x64 alapú rendszerekhez Service Pack 1](http://www.microsoft.com/downloads/details.aspx?familyid=1a32bf04-7eed-4d27-a8e4-054b4a5b76cb)  
(Fontos)
</td>
<td style="border:1px solid black;">
Nem érintett
</td>
<td style="border:1px solid black;">
[Windows 7 x64 alapú rendszerekhez és Windows 7 x64 alapú rendszerekhez Service Pack 1](http://www.microsoft.com/downloads/details.aspx?familyid=0c0aef7e-501c-4ca3-ae7f-497a8c169121)  
(Fontos)
</td>
</tr>
<tr>
<th colspan="14">
Windows Server 2008 R2
</th>
</tr>
<tr>
<td style="border:1px solid black;">
**Közlemény azonosítója**
</td>
<td style="border:1px solid black;">
[**MS11-018**](http://go.microsoft.com/fwlink/?linkid=214126)
</td>
<td style="border:1px solid black;">
[**MS11-019**](http://go.microsoft.com/fwlink/?linkid=212314)
</td>
<td style="border:1px solid black;">
[**MS11-020**](http://go.microsoft.com/fwlink/?linkid=212236)
</td>
<td style="border:1px solid black;">
[**MS11-027**](http://go.microsoft.com/fwlink/?linkid=214005)
</td>
<td style="border:1px solid black;">
[**MS11-028**](http://go.microsoft.com/fwlink/?linkid=207931)
</td>
<td style="border:1px solid black;">
[**MS11-029**](http://go.microsoft.com/fwlink/?linkid=208524)
</td>
<td style="border:1px solid black;">
[**MS11-030**](http://go.microsoft.com/fwlink/?linkid=212595)
</td>
<td style="border:1px solid black;">
[**MS11-031**](http://go.microsoft.com/fwlink/?linkid=212243)
</td>
<td style="border:1px solid black;">
[**MS11-032**](http://go.microsoft.com/fwlink/?linkid=212224)
</td>
<td style="border:1px solid black;">
[**MS11-024**](http://go.microsoft.com/fwlink/?linkid=212226)
</td>
<td style="border:1px solid black;">
[**MS11-026**](http://go.microsoft.com/fwlink/?linkid=212523)
</td>
<td style="border:1px solid black;">
[**MS11-033**](http://go.microsoft.com/fwlink/?linkid=208110)
</td>
<td style="border:1px solid black;">
[**MS11-034**](http://go.microsoft.com/fwlink/?linkid=211826)
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
**Összesített súlyossági besorolás**
</td>
<td style="border:1px solid black;">
[**Mérsékelt.**](http://go.microsoft.com/fwlink/?linkid=21140)
</td>
<td style="border:1px solid black;">
[**Kritikus**](http://go.microsoft.com/fwlink/?linkid=21140)
</td>
<td style="border:1px solid black;">
[**Kritikus**](http://go.microsoft.com/fwlink/?linkid=21140)
</td>
<td style="border:1px solid black;">
[**Mérsékelt.**](http://go.microsoft.com/fwlink/?linkid=21140)
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
[**Kritikus**](http://go.microsoft.com/fwlink/?linkid=21140)
</td>
<td style="border:1px solid black;">
[**Fontos**](http://go.microsoft.com/fwlink/?linkid=21140)
</td>
<td style="border:1px solid black;">
[**Alacsony**](http://go.microsoft.com/fwlink/?linkid=21140)
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
Windows Server 2008 R2 x64 alapú rendszerekhez és Windows Server 2008 R2 x64 alapú rendszerekhez Service Pack 1
</td>
<td style="border:1px solid black;">
[Internet Explorer 8](http://www.microsoft.com/downloads/details.aspx?familyid=c7b2482b-44bf-4c01-99d8-f93868659a24)\*\*  
(Mérsékelt)
</td>
<td style="border:1px solid black;">
[Windows Server 2008 R2 x64 alapú rendszerekhez és Windows Server 2008 R2 x64 alapú rendszerekhez Service Pack 1](http://www.microsoft.com/downloads/details.aspx?familyid=27a3847b-695b-4f60-aea5-86b0dbe68945)\*  
(Kritikus)
</td>
<td style="border:1px solid black;">
[Windows Server 2008 R2 x64 alapú rendszerekhez és Windows Server 2008 R2 x64 alapú rendszerekhez Service Pack 1](http://www.microsoft.com/downloads/details.aspx?familyid=c4352802-9c5a-4c07-8303-3a4b78d3f954)\*  
(Kritikus)
</td>
<td style="border:1px solid black;">
[Windows Server 2008 R2 x64-alapú rendszerekhez és Windows Server 2008 R2 x64-alapú rendszerekhez, Service Pack 1](http://www.microsoft.com/downloads/details.aspx?familyid=e4fa8ed0-acb0-4864-be18-29a27f8501de)\*\*  
(Mérsékelt)
</td>
<td style="border:1px solid black;">
Csak Windows Server 2008 R2 x64 alapú rendszerekhez:  
[Microsoft .NET Framework 3.5.1](http://www.microsoft.com/downloads/details.aspx?familyid=157aa425-953c-4fc9-ab76-4e65d4be8baa)\*  
(KB2446709)  
(Kritikus)  
Csak Windows Server 2008 R2 x64 alapú rendszerekhez:  
[Microsoft .NET-keretrendszer 4.0](http://www.microsoft.com/downloads/details.aspx?familyid=91aa6772-4811-4a58-9bc0-8aa271ed99df)<sup>[1]</sup>
(KB2446708)  
(Kritikus)  
Csak Windows Server 2008 R2 x64-alapú rendszerekhez, Service Pack 1:  
[Microsoft .NET Framework 3.5.1](http://www.microsoft.com/downloads/details.aspx?familyid=8f87b8aa-1a2a-405e-aee0-9247d553756a)\*  
(KB2446710)  
(Kritikus)  
Csak Windows Server 2008 R2 x64-alapú rendszerekhez, Service Pack 1:  
[Microsoft .NET-keretrendszer 4.0](http://www.microsoft.com/downloads/details.aspx?familyid=91aa6772-4811-4a58-9bc0-8aa271ed99df)\*<sup>[1]</sup>
(KB2446708)  
(Kritikus)
</td>
<td style="border:1px solid black;">
Nem érintett
</td>
<td style="border:1px solid black;">
[Windows Server 2008 R2 x64 alapú rendszerekhez és Windows Server 2008 R2 x64 alapú rendszerekhez Service Pack 1](http://www.microsoft.com/downloads/details.aspx?familyid=2084c726-187e-41f9-9bea-da18f490d29e)\*  
(Kritikus)
</td>
<td style="border:1px solid black;">
[JScript 5.8 és VBScript 5.8](http://www.microsoft.com/downloads/details.aspx?familyid=aecc2c7a-285c-409d-be23-c5b4b5449496)\*\*<sup>[1]</sup>
(KB2510531)  
(Kritikus)
</td>
<td style="border:1px solid black;">
[Windows Server 2008 R2 x64 alapú rendszerekhez és Windows Server 2008 R2 x64 alapú rendszerekhez Service Pack 1](http://www.microsoft.com/downloads/details.aspx?familyid=6f2a52cc-4833-448d-becc-2eac1a447410)\*  
(Kritikus)
</td>
<td style="border:1px solid black;">
[Windows Server 2008 R2 x64-alapú rendszerekhez és Windows Server 2008 R2 x64-alapú rendszerekhez, Service Pack 1](http://www.microsoft.com/downloads/details.aspx?familyid=465c0478-6a74-4b00-8608-938cc492549f)\*\*  
(KB2491683)  
(Fontos)  
[Windows Server 2008 R2 x64 alapú rendszerekhez és Windows Server 2008 R2 x64 alapú rendszerekhez Service Pack 1](http://www.microsoft.com/downloads/details.aspx?familyid=4c5c3a0f-0672-49d0-bcbd-c7f40e11d092)\*  
(KB2506212)  
(Fontos)
</td>
<td style="border:1px solid black;">
[Windows Server 2008 R2 x64-alapú rendszerekhez és Windows Server 2008 R2 x64-alapú rendszerekhez, Service Pack 1](http://www.microsoft.com/downloads/details.aspx?familyid=665faa7e-2368-4421-9dd5-ea6df2c79498)\*\*  
(Alacsony)
</td>
<td style="border:1px solid black;">
Nem érintett
</td>
<td style="border:1px solid black;">
[Windows Server 2008 R2 x64 alapú rendszerekhez és Windows Server 2008 R2 x64 alapú rendszerekhez Service Pack 1](http://www.microsoft.com/downloads/details.aspx?familyid=2fc66224-45c6-4e8f-ad00-6a1ec30b4505)\*  
(Fontos)
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
Windows Server 2008 R2 Itanium alapú rendszerekhez és Windows Server 2008 R2 Itanium alapú rendszerekhez Service Pack 1
</td>
<td style="border:1px solid black;">
[Internet Explorer 8](http://www.microsoft.com/downloads/details.aspx?familyid=af6db318-fbec-4286-a3a7-4081620146e5)  
(Mérsékelt)
</td>
<td style="border:1px solid black;">
[Windows Server 2008 R2 Itanium alapú rendszerekhez és Windows Server 2008 R2 Itanium alapú rendszerekhez Service Pack 1](http://www.microsoft.com/downloads/details.aspx?familyid=1e7d3f21-bdbd-4826-855d-85422aa5f836)  
(Kritikus)
</td>
<td style="border:1px solid black;">
[Windows Server 2008 R2 Itanium alapú rendszerekhez és Windows Server 2008 R2 Itanium alapú rendszerekhez Service Pack 1](http://www.microsoft.com/downloads/details.aspx?familyid=0005377b-443f-44ca-a890-620b2dcea6f1)  
(Kritikus)
</td>
<td style="border:1px solid black;">
[Windows Server 2008 R2 Itanium alapú rendszerekhez és Windows Server 2008 R2 Itanium alapú rendszerekhez Service Pack 1](http://www.microsoft.com/downloads/details.aspx?familyid=d7bcf4d7-b697-4c5f-adbc-a2b3700e0ad5)  
(Mérsékelt)
</td>
<td style="border:1px solid black;">
Csak Windows Server 2008 R2 Itanium-alapú rendszerekhez:  
[Microsoft .NET-keretrendszer 3.5.1](http://www.microsoft.com/downloads/details.aspx?familyid=157aa425-953c-4fc9-ab76-4e65d4be8baa)  
(KB2446709)  
(Kritikus)  
Csak Windows Server 2008 R2 Itanium-alapú rendszerekhez, Service Pack 1:  
[Microsoft .NET-keretrendszer 3.5.1](http://www.microsoft.com/downloads/details.aspx?familyid=8f87b8aa-1a2a-405e-aee0-9247d553756a)  
(KB2446710)  
(Kritikus)  
Windows Server 2008 R2 Itanium-alapú rendszerekhez és Windows Server 2008 R2 Itanium-alapú rendszerekhez, Service Pack 1:  
[Microsoft .NET-keretrendszer 4.0](http://www.microsoft.com/downloads/details.aspx?familyid=91aa6772-4811-4a58-9bc0-8aa271ed99df)<sup>[1]</sup>
(KB2446708)  
(Kritikus)
</td>
<td style="border:1px solid black;">
Nem érintett
</td>
<td style="border:1px solid black;">
[Windows Server 2008 R2 Itanium alapú rendszerekhez és Windows Server 2008 R2 Itanium alapú rendszerekhez Service Pack 1](http://www.microsoft.com/downloads/details.aspx?familyid=34d2793e-a2cd-49f6-b524-6598ea86175f)  
(Kritikus)
</td>
<td style="border:1px solid black;">
[JScript 5.8 és VBScript 5.8](http://www.microsoft.com/downloads/details.aspx?familyid=e1bc0ed8-5a93-4d01-b407-919dfd894b5f)<sup>[1]</sup>
(KB2510531)  
(Kritikus)
</td>
<td style="border:1px solid black;">
[Windows Server 2008 R2 Itanium alapú rendszerekhez és Windows Server 2008 R2 Itanium alapú rendszerekhez Service Pack 1](http://www.microsoft.com/downloads/details.aspx?familyid=c6ca0b7c-8151-4d54-aa9b-5ec2b75d8ab6)  
(Kritikus)
</td>
<td style="border:1px solid black;">
[Windows Server 2008 R2 Itanium alapú rendszerekhez és Windows Server 2008 R2 Itanium alapú rendszerekhez Service Pack 1](http://www.microsoft.com/downloads/details.aspx?familyid=1a993f8c-d28a-4a95-a3c6-059f06e75461)  
(KB2506212)  
(Fontos)
</td>
<td style="border:1px solid black;">
[Windows Server 2008 R2 Itanium alapú rendszerekhez és Windows Server 2008 R2 Itanium alapú rendszerekhez Service Pack 1](http://www.microsoft.com/downloads/details.aspx?familyid=140ea384-2877-401f-ac3b-f84f6966e970)  
(Alacsony)
</td>
<td style="border:1px solid black;">
Nem érintett
</td>
<td style="border:1px solid black;">
[Windows Server 2008 R2 Itanium alapú rendszerekhez és Windows Server 2008 R2 Itanium alapú rendszerekhez Service Pack 1](http://www.microsoft.com/downloads/details.aspx?familyid=485ccf96-27a0-499e-9f52-2836b73d26d2)  
(Fontos)
</td>
</tr>
</table>
 
**Megjegyzések a Windows Server 2008 és Windows Server 2008 R2 rendszerhez**

**\*Érinti a kiszolgálómag telepítését.** Ez a frissítés ugyanolyan biztonsági besorolás mellett, a megadottak szerint érvényes az Windows Server 2008 és a Windows Server 2008 R2 összes támogatott kiadására, függetlenül attól, hogy a kiszolgálómag-telepítési opcióval telepítették-e. Erről a telepítési opcióról bővebben a [Kiszolgálómag-telepítés kezelése](http://technet.microsoft.com/en-us/library/ee441255(ws.10).aspx) és [Kiszolgálómag-telepítés szervizelése](http://technet.microsoft.com/en-us/library/ff698994(ws.10).aspx) TechNet cikkekben olvashat. A kiszolgálómag-telepítési opció nem vonatkozik a Windows Server 2008 és a Windows Server 2008 R2 bizonyos kiadásaira; lásd: [A kiszolgálómag-telepítési opciók összehasonlítása](http://www.microsoft.com/windowsserver2008/en/us/compare-core-installation.aspx).

**\*\*A kiszolgálómag-telepítés nem érintett.** A frissítésben tárgyalt biztonsági rések nem érintik a jelzett módon a Windows Server 2008 és a Windows Server 2008 R2 támogatott kiadásait, amennyiben a telepítés a kiszolgálómag-telepítési opció használatával történt. Erről a telepítési opcióról bővebben a [Kiszolgálómag-telepítés kezelése](http://technet.microsoft.com/en-us/library/ee441255(ws.10).aspx) és [Kiszolgálómag-telepítés szervizelése](http://technet.microsoft.com/en-us/library/ff698994(ws.10).aspx) TechNet cikkekben olvashat. A kiszolgálómag-telepítési opció nem vonatkozik a Windows Server 2008 és a Windows Server 2008 R2 bizonyos kiadásaira; lásd: [A kiszolgálómag-telepítési opciók összehasonlítása](http://www.microsoft.com/windowsserver2008/en/us/compare-core-installation.aspx).

**\*\*\*A kiszolgálómag-telepítés nem érintett.** A frissítés által javított biztonsági rések nem érintik a jelzett módon a Windows Server 2008 vagy Windows Server 2008 R2 támogatott kiadásait, ha a rendszert a kiszolgálómag-telepítés segítségével telepítették, annak dacára, hogy elképzelhető, hogy a biztonsági rés által érintett fájlok megtalálhatóak a rendszeren. Az érintett fájlokkal rendelkező felhasználóknak mégis felajánlják a frissítést, mivel a frissített fájlok újabbak (magasabb verziószámúak), mint a jelenleg a rendszeren található fájlok. Erről a telepítési opcióról bővebben a [Kiszolgálómag-telepítés kezelése](http://technet.microsoft.com/en-us/library/ee441255(ws.10).aspx) és [Kiszolgálómag-telepítés szervizelése](http://technet.microsoft.com/en-us/library/ff698994(ws.10).aspx) TechNet cikkekben olvashat. A kiszolgálómag-telepítési opció nem vonatkozik a Windows Server 2008 és a Windows Server 2008 R2 bizonyos kiadásaira; lásd: [A kiszolgálómag-telepítési opciók összehasonlítása](http://www.microsoft.com/windowsserver2008/en/us/compare-core-installation.aspx).

**Megjegyzés az MS11-027 közleményhez**

<sup>[1]</sup>Ezt az operációs rendszert nem érintik a közleményben ismertetett biztonsági rések. A rendelkezésre álló frissítés a külső gyártótól származó vezérlőkhöz állít be tiltóbiteket:

**Megjegyzés az MS11-028 közleményhez**

<sup>[1]</sup>**.érintett .NET-keretrendszer 4.0 és .NET-keretrendszer 4.0 Client Profile.** A .NET-keretrendszer 4-es verziójú terjeszthető csomagjai két profilban érhetőek el: a .NET-keretrendszer 4.0 és a .NET-keretrendszer 4.0 verziójához tartozó ügyfélprofil. A .NET-keretrendszer 4.0 verziójához tartozó ügyfélprofil része a .NET-keretrendszer 4.0 verziójának. A jelen frissítés mindkettőt, a .NET-keretrendszer 4.0 verzióját és a .NET-keretrendszer 4.0 verziójához tartozó ügyfélprofilt is érinti. Bővebb tájékoztatást itt talál: [A .NET-keretrendszer telepítése](http://msdn.microsoft.com/en-us/library/5a4x27ek.aspx).

**Megjegyzés az MS11-029 közleményhez**

Az ugyanezen a közleményazonosító alatt található, további frissített fájlokat illetően lásd még az egyéb szoftverkategóriák részt ebben a fejezetben, **Érintett szoftverek és letöltési helyek**. Ez a közlemény több szoftverkategóriát ölel fel.

**Megjegyzés az MS11-031 közleményhez**

<sup>[1]</sup>A telepített Internet Explorer 9 programmal rendelkező rendszereket a biztonsági rés nem érinti; ezeken nincs szükség a frissítésre. Azokon a rendszereken, amelyeket nem frissített az Internet Explorer 9-es verziójával, alkalmazni kell a telepített JScript és VBScript verziójának megfelelő frissítést. A rendszerre telepített JScript és VBScript verziójának meghatározásához a közleményben talál információt.

**Megjegyzés az MS11-024 közleményhez**

Ahol ugyanazon operációs rendszerhez két frissítés is elérhető, telepítse mindkét frissítést.

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
<th style="border:1px solid black;" >
</th>
<th style="border:1px solid black;" >
</th>
</tr>
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
[**MS11-029**](http://go.microsoft.com/fwlink/?linkid=208524)
</td>
<td style="border:1px solid black;">
[**MS11-021**](http://go.microsoft.com/fwlink/?linkid=210121)
</td>
<td style="border:1px solid black;">
[**MS11-022**](http://go.microsoft.com/fwlink/?linkid=210727)
</td>
<td style="border:1px solid black;">
[**MS11-023**](http://go.microsoft.com/fwlink/?linkid=210206)
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
**Összesített súlyossági** **besorolás**
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
</tr>
<tr>
<td style="border:1px solid black;">
Microsoft Office XP Service Pack 3
</td>
<td style="border:1px solid black;">
[Microsoft Office XP Service Pack 3](http://www.microsoft.com/downloads/details.aspx?familyid=6c87c2a9-3705-4680-8a9b-63b6ec83674d)  
(KB2509461)  
(Fontos)
</td>
<td style="border:1px solid black;">
[Microsoft Excel 2002 Service Pack 3](http://www.microsoft.com/downloads/details.aspx?familyid=db2c5cfe-588c-4646-b86a-3fb8248f7af4)  
(KB2466169)  
(Fontos)
</td>
<td style="border:1px solid black;">
[Microsoft PowerPoint 2002 Service Pack 3](http://www.microsoft.com/downloads/details.aspx?familyid=0d215ab6-c9be-4f43-9501-658bb7ef008e)  
(KB2464617)  
(Fontos)
</td>
<td style="border:1px solid black;">
[Microsoft Office XP Service Pack 3](http://www.microsoft.com/downloads/details.aspx?familyid=6c87c2a9-3705-4680-8a9b-63b6ec83674d)  
(KB2509461)  
(Fontos)
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
Microsoft Office 2003 Service Pack 3
</td>
<td style="border:1px solid black;">
Nem érintett
</td>
<td style="border:1px solid black;">
[Microsoft Excel 2003 Service Pack 3](http://www.microsoft.com/downloads/details.aspx?familyid=916a076d-d754-4092-b23d-c8826db7e397)  
(KB2502786)  
(Fontos)
</td>
<td style="border:1px solid black;">
[Microsoft PowerPoint 2003 Service Pack 3](http://www.microsoft.com/downloads/details.aspx?familyid=2ce8349f-79b1-41ef-a1c0-cbe40ccf9f20)  
(KB2464588)  
(Fontos)
</td>
<td style="border:1px solid black;">
[Microsoft Office 2003 Service Pack 3](http://www.microsoft.com/downloads/details.aspx?familyid=8b68cf68-1606-4649-b860-a64702c6cf33)  
(KB2509503)  
(Fontos)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Microsoft Office 2007 Service Pack 2
</td>
<td style="border:1px solid black;">
Nem érintett
</td>
<td style="border:1px solid black;">
[Microsoft Excel 2007 Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=5ae34fe0-03bd-48a9-a7ac-de8f7b1aff90)<sup>[1]</sup>
(KB2464583)  
(Fontos)
</td>
<td style="border:1px solid black;">
[Microsoft PowerPoint 2007 Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=6b2526fe-a061-4a17-992e-ac867bef130e)  
(KB2464594)  
(Fontos)
</td>
<td style="border:1px solid black;">
[Microsoft Office 2007 Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=dbba0cd4-ab72-4e2b-9524-fd6be27f0b02)  
(KB2509488)  
(Fontos)
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
[Microsoft Excel 2010 (32 bites kiadások)](http://www.microsoft.com/downloads/details.aspx?familyid=a427f0e2-b74d-4ef3-bec4-0a101d09bfa3)  
(KB2466146)  
(Fontos)
</td>
<td style="border:1px solid black;">
[Microsoft PowerPoint 2010 (32 bites kiadások)](http://www.microsoft.com/downloads/details.aspx?familyid=549ca7f0-44bf-4965-a9d2-aa5e8dac2238)  
(KB2519975)  
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
Nem érintett
</td>
<td style="border:1px solid black;">
[Microsoft Excel 2010 (64 bites kiadások)](http://www.microsoft.com/downloads/details.aspx?familyid=13dca35d-2209-4c5c-9150-d6db2bb3b496)  
(KB2466146)  
(Fontos)
</td>
<td style="border:1px solid black;">
[Microsoft PowerPoint 2010 (64 bites kiadások)](http://www.microsoft.com/downloads/details.aspx?familyid=ef62deae-2b07-41c9-a4bf-b746566e59ee)  
(KB2519975)  
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
[**MS11-029**](http://go.microsoft.com/fwlink/?linkid=208524)
</td>
<td style="border:1px solid black;">
[**MS11-021**](http://go.microsoft.com/fwlink/?linkid=210121)
</td>
<td style="border:1px solid black;">
[**MS11-022**](http://go.microsoft.com/fwlink/?linkid=210727)
</td>
<td style="border:1px solid black;">
[**MS11-023**](http://go.microsoft.com/fwlink/?linkid=210206)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
**Összesített súlyossági besorolás**
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
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
Microsoft Office 2004 for Mac
</td>
<td style="border:1px solid black;">
Nem érintett
</td>
<td style="border:1px solid black;">
[Microsoft Office 2004 for Mac](http://www.microsoft.com/downloads/details.aspx?familyid=f756d836-6ab2-4adb-9dee-6cb523d7c1f5)  
(KB2505924)  
(Fontos)
</td>
<td style="border:1px solid black;">
[Microsoft Office 2004 for Mac](http://www.microsoft.com/downloads/details.aspx?familyid=f756d836-6ab2-4adb-9dee-6cb523d7c1f5)  
(KB2505924)  
(Fontos)
</td>
<td style="border:1px solid black;">
[Microsoft Office 2004 for Mac](http://www.microsoft.com/downloads/details.aspx?familyid=f756d836-6ab2-4adb-9dee-6cb523d7c1f5)  
(KB2505924)  
(Fontos)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Microsoft Office 2008 for Mac
</td>
<td style="border:1px solid black;">
Nem érintett
</td>
<td style="border:1px solid black;">
[Microsoft Office 2008 for Mac](http://www.microsoft.com/downloads/details.aspx?familyid=84dfe3f4-a2a1-47b9-8da1-29ae67230918)  
(KB2505927)  
(Fontos)
</td>
<td style="border:1px solid black;">
[Microsoft Office 2008 for Mac](http://www.microsoft.com/downloads/details.aspx?familyid=84dfe3f4-a2a1-47b9-8da1-29ae67230918)  
(KB2505927)  
(Fontos)
</td>
<td style="border:1px solid black;">
[Microsoft Office 2008 for Mac](http://www.microsoft.com/downloads/details.aspx?familyid=84dfe3f4-a2a1-47b9-8da1-29ae67230918)  
(KB2505927)  
(Fontos)
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
Microsoft Office for Mac 2011
</td>
<td style="border:1px solid black;">
Nem érintett
</td>
<td style="border:1px solid black;">
[Microsoft Office for Mac 2011](http://www.microsoft.com/downloads/details.aspx?familyid=ef1e612f-d8e3-4628-9fe4-ad136f0debd3)  
(KB2525412)  
(Fontos)
</td>
<td style="border:1px solid black;">
[Microsoft Office for Mac 2011](http://www.microsoft.com/downloads/details.aspx?familyid=ef1e612f-d8e3-4628-9fe4-ad136f0debd3)  
(KB2525412)  
(Fontos)
</td>
<td style="border:1px solid black;">
Nem érintett
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Open XML File Format Converter for Mac
</td>
<td style="border:1px solid black;">
Nem érintett
</td>
<td style="border:1px solid black;">
[Open XML File Format Converter for Mac](http://www.microsoft.com/downloads/details.aspx?familyid=0c323a12-6385-4666-ad39-a9516a8eda14)  
(KB2505935)  
(Fontos)
</td>
<td style="border:1px solid black;">
[Open XML File Format Converter for Mac](http://www.microsoft.com/downloads/details.aspx?familyid=0c323a12-6385-4666-ad39-a9516a8eda14)  
(KB2505935)  
(Fontos)
</td>
<td style="border:1px solid black;">
[Open XML File Format Converter for Mac](http://www.microsoft.com/downloads/details.aspx?familyid=0c323a12-6385-4666-ad39-a9516a8eda14)  
(KB2505935)  
(Fontos)
</td>
</tr>
<tr>
<th colspan="5">
További Office-szoftverek
</th>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
**Közlemény azonosítója**
</td>
<td style="border:1px solid black;">
[**MS11-029**](http://go.microsoft.com/fwlink/?linkid=208524)
</td>
<td style="border:1px solid black;">
[**MS11-021**](http://go.microsoft.com/fwlink/?linkid=210121)
</td>
<td style="border:1px solid black;">
[**MS11-022**](http://go.microsoft.com/fwlink/?linkid=210727)
</td>
<td style="border:1px solid black;">
[**MS11-023**](http://go.microsoft.com/fwlink/?linkid=210206)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
**Összesített súlyossági besorolás**
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
Nincsenek
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
Microsoft Excel megjelenítő Service Pack 2
</td>
<td style="border:1px solid black;">
Nem érintett
</td>
<td style="border:1px solid black;">
[Microsoft Excel megjelenítő Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=2d75786a-2368-4ef2-970b-fa2e57d63ca9)  
(KB2466158)  
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
Microsoft PowerPoint Viewer 2007 Service Pack 2
</td>
<td style="border:1px solid black;">
Nem érintett
</td>
<td style="border:1px solid black;">
Nem érintett
</td>
<td style="border:1px solid black;">
[Microsoft PowerPoint Viewer 2007 Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=6e23d3c3-2944-42ea-80b3-0663af60d0f1)  
(KB2464623)  
(Fontos)
</td>
<td style="border:1px solid black;">
Nem érintett
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
Microsoft PowerPoint megjelenítő
</td>
<td style="border:1px solid black;">
Nem érintett
</td>
<td style="border:1px solid black;">
Nem érintett
</td>
<td style="border:1px solid black;">
[Microsoft PowerPoint megjelenítő](http://www.microsoft.com/downloads/details.aspx?familyid=44a703f5-b581-4900-bdbb-0f0e8d9bf0e6)  
(KB2519984)  
(Fontos)
</td>
<td style="border:1px solid black;">
Nem érintett
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Microsoft Office kompatibilitási csomag a Word, Excel és a PowerPoint 2007 fájlformátumokhoz Service Pack 2
</td>
<td style="border:1px solid black;">
Nem érintett
</td>
<td style="border:1px solid black;">
[Microsoft Office kompatibilitási csomag a Word, Excel és a PowerPoint 2007 fájlformátumokhoz Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=946cc611-4d75-4728-b9d3-1c8b557b02c2)  
(KB2466156)  
(Fontos)
</td>
<td style="border:1px solid black;">
[Microsoft Office kompatibilitási csomag a Word, Excel és a PowerPoint 2007 fájlformátumokhoz Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=913efc28-7deb-47b8-8c22-8eb5fc2631e4)  
(KB2464635)  
(Fontos)
</td>
<td style="border:1px solid black;">
Nem érintett
</td>
</tr>
</table>
 
**Megjegyzés az MS11-029 közleményhez**

Az ugyanezen a közleményazonosító alatt található, további frissített fájlokat illetően lásd még az egyéb szoftverkategóriák részt ebben a fejezetben, **Érintett szoftverek és letöltési helyek**. Ez a közlemény több szoftverkategóriát ölel fel.

**Megjegyzés az MS11-021 közleményhez**

<sup>[1]</sup>A Microsoft Excel 2007 Service Pack 2 felhasználóinak a KB2464583 frissítésen kívül a Word, Excel és PowerPoint 2007 fájlformátumokhoz készült Microsoft Office kompatibilitási csomag Service Pack 2 (KB2466156) biztonsági frissítését is telepíteniük kell, hogy megvédjék rendszerüket a jelen közleményben ismertetett biztonsági rések hibáitól.

**Megjegyzés az MS11-022 közleményhez**

Az ugyanezen a közleményazonosító alatt található, további frissített fájlokat illetően lásd még az egyéb szoftverkategóriák részt ebben a fejezetben, **Érintett szoftverek és letöltési helyek**. Ez a közlemény több szoftverkategóriát ölel fel.

#### Microsoft Server Software

 
<p> </p>
<table style="border:1px solid black;">
<tr class="thead">
<th style="border:1px solid black;" >
</th>
<th style="border:1px solid black;" >
</th>
</tr>
<tr>
<th colspan="2">
Microsoft Office Web Apps
</th>
</tr>
<tr>
<td style="border:1px solid black;">
**Közlemény azonosítója**
</td>
<td style="border:1px solid black;">
[**MS11-022**](http://go.microsoft.com/fwlink/?linkid=210727)
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
Microsoft Office Web Apps
</td>
<td style="border:1px solid black;">
[Microsoft PowerPoint Web App](http://www.microsoft.com/downloads/details.aspx?familyid=9847dc05-7d4a-4a64-9e6a-622d3fa171f9)  
(KB2520047)  
(Fontos)
</td>
</tr>
</table>
 
**Megjegyzés az MS11-022 közleményhez**

Az ugyanezen a közleményazonosító alatt található, további frissített fájlokat illetően lásd még az egyéb szoftverkategóriák részt ebben a fejezetben, **Érintett szoftverek és letöltési helyek**. Ez a közlemény több szoftverkategóriát ölel fel.

#### Microsoft fejlesztői eszközök és szoftver

 
<p> </p>
<table style="border:1px solid black;">
<tr class="thead">
<th style="border:1px solid black;" >
</th>
<th style="border:1px solid black;" >
</th>
</tr>
<tr>
<th colspan="2">
Microsoft Visual Studio
</th>
</tr>
<tr>
<td style="border:1px solid black;">
**Közlemény azonosítója**
</td>
<td style="border:1px solid black;">
[**MS11-025**](http://go.microsoft.com/fwlink/?linkid=209720)
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
Microsoft Visual Studio .NET 2003 Service Pack 1
</td>
<td style="border:1px solid black;">
[Microsoft Visual Studio .NET 2003 Service Pack 1](http://www.microsoft.com/downloads/details.aspx?familyid=e9501082-a651-452b-8c1a-43987ffd3102)  
(KB2465373)  
(Fontos)
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
Microsoft Visual Studio 2005 Service Pack 1
</td>
<td style="border:1px solid black;">
[Microsoft Visual Studio 2005 Service Pack 1](http://www.microsoft.com/downloads/details.aspx?familyid=ee64d83b-6c06-4ccf-b12d-99e2a7a7b18d)  
(KB2538218)  
(Fontos)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Microsoft Visual Studio 2008 Service Pack 1
</td>
<td style="border:1px solid black;">
[Microsoft Visual Studio 2008 Service Pack 1](http://www.microsoft.com/downloads/details.aspx?familyid=e6a8e024-12ee-43d5-9aae-4c721505d6df)  
(KB2538241)  
(Fontos)
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
Microsoft Visual Studio 2010 és Microsoft Visual Studio 2010 Service Pack 1
</td>
<td style="border:1px solid black;">
[Microsoft Visual Studio 2010](http://www.microsoft.com/downloads/details.aspx?familyid=7fd643a8-8e05-4d27-8853-33f79f01cb26)  
(KB2542054)  
(Fontos)  
[Microsoft Visual Studio 2010 Service Pack 1](http://www.microsoft.com/downloads/details.aspx?familyid=1a21c9db-dfa3-4a07-a1e0-89a8069b7c17)  
(KB2565057)  
(Fontos)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Microsoft Visual C++ 2005 Service Pack 1
</td>
<td style="border:1px solid black;">
[Microsoft Visual C++ 2005 Service Pack 1 Redistributable Package](http://www.microsoft.com/downloads/details.aspx?familyid=ae2e1a40-7b45-4fe9-a20f-2ed2923aca62)  
(KB2538242)  
(Fontos)
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
Microsoft Visual C++ 2008 Service Pack 1
</td>
<td style="border:1px solid black;">
[Microsoft Visual C++ 2008 Service Pack 1 Redistributable Package](http://www.microsoft.com/downloads/details.aspx?familyid=a821847e-4c44-45c0-9128-61c822bb3280)  
(KB2538243)  
(Fontos)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Microsoft Visual C++ 2010 éd Microsoft Visual C++ 2010 Service Pack 1
</td>
<td style="border:1px solid black;">
[Microsoft Visual C++ 2010 terjeszthető csomag](http://www.microsoft.com/downloads/details.aspx?familyid=fe558aed-9274-415f-8a0f-d9d8622fb35b)  
(KB2467173)  
(Fontos)  
[Microsoft Visual C++ 2010 Redistributable Package Service Pack 1](http://www.microsoft.com/downloads/details.aspx?familyid=7557d29b-731b-4abb-8815-2b87a4132efb)  
(KB2565063)  
(Fontos)
</td>
</tr>
</table>
 

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

A biztonsági frissítésnek Windows Server Update Services szolgáltatással történő központi telepítéséről a [Windows Server Update Services](http://go.microsoft.com/fwlink/?linkid=50120) webhelyen tudhat meg többet.

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

-   A [VeriSign iDefense Labs](http://labs.idefense.com/) anonim együttműködő partnerének az MS11-018 közleményben ismertetett probléma jelentéséért
-   [MITRE](http://mitre.org/), az MS11-018 közleményben ismertetett probléma közös megoldásában való részvételéért
-   Michal Zalewski, [Google Inc.](http://www.google.com/), az MS11-018 közleményben ismertetett probléma megoldásában való közreműködésért
-   David Bloom, [Google Inc.](http://www.google.com/), az MS11-018 közleményben bemutatott két probléma jelentéséért
-   Stephen Fewer, [Harmony Security](http://www.harmonysecurity.com/), a [TippingPoint](http://www.tippingpoint.com/)[Zero Day Initiative](http://www.zerodayinitiative.com/) programjával együttműködésben, az MS11-018 közleményben ismertetett probléma jelentéséért
-   Alin Rad Pop, [Secunia Research](http://secunia.com/), az MS11-021 közleményben ismertetett két probléma jelentéséért
-   Muhammad Junaid Bohio, [Telus Security Labs](http://www.telussecuritylabs.com), az MS11-021 közleményben ismertetett probléma jelentéséért
-   Aniway, a [TippingPoint](http://www.tippingpoint.com/)[Zero Day Initiativ](http://www.zerodayinitiative.com/)e programjával együttműködésben, az MS11-021 közleményben ismertetett három probléma jelentéséért
-   A [VeriSign iDefense Labs](http://labs.idefense.com/) anonim együttműködő partnerének az MS11-021 közleményben ismertetett probléma jelentéséért
-   Rodrigo Rubira Branco, a [Check Point](http://www.checkpoint.com/) biztonsági résekkel foglalkozó csoportjától (VDT), az MS11-021 közleményben ismertetett probléma jelentéséért
-   A [Tipping Point](http://www.tippingpoint.com/)[Zero Day Initiative](http://www.zerodayinitiative.com/) programjában részt vevő anonim kutató, az MS11-021 közleményben ismertetett probléma jelentéséért
-   A [Tipping Point](http://www.tippingpoint.com/)[Zero Day Initiative](http://www.zerodayinitiative.com/) programjában részt vevő anonim kutató, az MS11-021 közleményben ismertetett probléma jelentéséért
-   A [TippingPoint](http://www.tippingpoint.com/)[Zero Day Initiative](http://www.zerodayinitiative.com/) programja, az MS11-022 közleményben ismertetett három probléma jelentéséért
-   Haifei Li, [Fortinet, FortiGuard Labs](http://www.fortiguard.com/), az MS11-023 közleményben ismertetett problémák egyikének jelentéséért
-   A [Tipping Point](http://www.tippingpoint.com/)[Zero Day Initiative](http://www.zerodayinitiative.com/) programjában részt vevő anonim kutató, az MS11-023 közleményben ismertetett probléma jelentéséért
-   Carsten H. Eiram, [Secunia](http://secunia.com/), az MS11-024 közleményben említett probléma megoldásában való együttműködésért
-   A [Google Security Team](http://www.google.com/), az MS11-026 közleményben ismertetett probléma megoldásában való közreműködésért
-   Chris Ries, Carnegie Mellon University Information Security Office, az MS11-027 közleményben ismertetett probléma jelentéséért
-   RadLSneak, az [iSIGHT Partners](http://www.isightpartners.com/) Global Vulnerability Partnership programjával együttműködésben, az MS11-027 közleményben ismertetett probléma jelentéséért
-   Nicolas Joly és Chaouki Bekrar, [VUPEN Threat Protection Program](http://www.vupen.com/english/services/tpp-index.php), az MS11-029 közleményben ismertetett probléma jelentéséért
-   Neel Mehta, [Google Inc.](http://www.google.com/), az MS11-030 közleményben bemutatott probléma jelentéséért
-   [Jesse Ruderman](http://www.squarefree.com/), [Mozilla](http://www.mozilla.org/), az MS11-031 közleményben ismertetett probléma megoldásában való közreműködésért
-   Adam Twardoch, [Fontlab Ltd.](http://www.fontlab.com/), az MS11-032 közleményben bemutatott probléma jelentéséért
-   Carsten Eiram, [Secunia](http://secunia.com/), az MS11-033 közleményben leírt probléma jelentéséért
-   Tarjei Mandt, [Norman](http://www.norman.com/), az MS11-034 számú közleményben bemutatott 30 probléma jelentéséért

#### Terméktámogatás

-   Teszteléssel állapították meg a felsorolt szoftverek egyes verzióinak érintettségét. A többi verzió támogatási életciklusa végére ért. Az egyes szoftververziók támogatási életciklusáról a [Microsoft termékek terméktámogatási életciklusát ismertető webhelyen](http://go.microsoft.com/fwlink/?linkid=21742) talál felvilágosítást.
-   Az Amerikai Egyesült Államokban és Kanada területén élő ügyfelek technikai támogatást kérhetnek a [biztonsági támogatás szolgáltatójától](http://go.microsoft.com/fwlink/?linkid=21131) vagy az 1-866-PCSAFETY telefonszámon. A biztonsági frissítésekkel kapcsolatos hívások ingyenesek. Az elérhető támogatási lehetőségekről további információt talál a [Microsoft segítségnyújtással és támogatással foglalkozó webhelyén](http://support.microsoft.com/).
-   Más országokban a helyi Microsoft-képviseletek nyújtanak támogatást. A biztonsági frissítésekkel kapcsolatos hívások ingyenesek. A [nemzetközi támogatási webhely](http://go.microsoft.com/fwlink/?linkid=21155) felvilágosítást nyújt arról, támogatási kérdéseivel hogyan fordulhat a Microsofthoz.

#### Felelősséget kizáró nyilatkozat

A Microsoft Tudásbázisban leírtak előzetes bejelentés nélkül változhatnak, és a cikkek tartalmáért a Microsoft nem vállal garanciát. A Microsoft egyben elhárít minden kifejezett és értelemszerű garanciát, beleértve az eladhatóságra és az adott célra való alkalmasságra vonatkozó garanciát is. A Microsoft Corporation vagy annak szállítói semmilyen körülmények között nem tehetők felelőssé közvetlen, közvetett, eseti, ok-okozati vagy különleges kárért (beleértve az elmaradt hasznot is), még akkor sem, ha a Microsoft Corporation vagy szállítói tudatában voltak a kár lehetséges voltának. Egyes államok törvényi szabályozása nem teszi lehetővé a véletlen vagy ok-okozati károkért vállalt felelősség korlátozását vagy kizárását, így ezekben az államokban az ez a felelősségkizárás nincs érvényben.

#### Verziók

-   1.0 verzió (2011. április 12.): Összefoglaló közlemény közzététele.
-   1.1 verzió (2011. április 13.): Az MS11-019 közleménnyel kapcsolatban a biztonsági rés kihasználási lehetőségeinek pontosítása belekerült az Összefoglalásba.
-   2.0 verzió (2011. április 15.): Az MS11-032 biztonsági résnél a CVE-2011-0034 mutatót 1-es értékűre változtattuk – Valószínűleg konzisztens rosszindulatú programkód.
-   3.0 verzió (2011. április 21.): Az MS11-025 közleményhez újra kiadott biztonsági frissítést kínál fel.
-   3.1 verzió (2011. április 27.): Kiegészítettük az MS11-024 közleményben található Kihasználhatósági információkat a jelen frissítésben tárgyalt CVE-2010-4701 biztonsági réssel. A módosítás csak tájékoztató jellegű.
-   4.0 verzió (2011. május 16.): Az ismét kiadott MS11-018 közlemény ismételten felajánlja a Windows XP és Windows Server 2003 rendszeren telepített Internet Explorer 7 alkalmazás frissítését. Ez csak észlelési módosítás. A bináris fájlok nem változtak. A rendszer csak az érintett felhasználóknak ajánlja fel a frissítést. A frissítést manuálisan telepített felhasználóknak, valamint azoknak a felhasználóknak, akik az észlelési logika módosítása által nem érintett rendszereket futtattnak, semmilyen teendőjük nincsen.
-   5.0 verzió (2011. június 14.): Az MS11-025 frissítésnél ismét felajánlottuk a frissítést Microsoft Visual Studio 2005 Service Pack 1, Microsoft Visual Studio 2008 Service Pack 1, Microsoft Visual Studio 2010, Microsoft Visual C++ 2005 Service Pack 1 Redistributable Package és Microsoft Visual C++ 2008 Service Pack 1 Redistributable Package rendszerhez. Ha már telepítette rendszerére a frissítést, telepítse az új csomagokat az érintett rendszerekre.
-   6.0 verzió (2011. augusztus 9.): Az MS11-025 közlemény esetében a Microsoft Visual Studio 2010 Service Pack 1 (KB2565057) és a Microsoft Visual C++ 2010 Redistributable Package Service Pack 1 (KB2565063) felkerült az érintett szoftverek listájára.
-   6.1 verzió (2011. október 26.): Az MS11-028 közleménnyel kapcsolatban javították a .NET Framework 4 keretrendszerhez tartozó kiszolgálómag-telepítés alkalmazhatóságát a Windows Server 2008 R2 x64 alapú rendszerekhez operációs rendszeren.

*Built at 2014-04-18T01:50:00Z-07:00*
