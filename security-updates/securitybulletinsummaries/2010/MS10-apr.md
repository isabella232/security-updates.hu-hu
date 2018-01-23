---
TOCTitle: 'MS10-APR'
Title: 'Microsoft biztonsági közlemény - összefoglalás, április 2010'
ms:assetid: 'ms10-apr'
ms:contentKeyID: 61227738
ms:mtpsurl: 'https://technet.microsoft.com/hu-HU/library/ms10-apr(v=Security.10)'
---

Security Bulletin Summary

Microsoft biztonsági közlemény - összefoglalás, április 2010
============================================================

Közzétéve: 2010. április 13. | Frissítve: 2010. július 13.

**Verzió:** 4.0

Az összefoglaló a 2010 áprilisában kiadott biztonsági közleményeket összegzi.

A 2010. áprilisi közlemények kiadása folytán az összefoglaló a 2010. április 8-án kiadott előzetes értesítés helyébe lép. A biztonsági közlemények kiadásáról szóló előzetes értesítés szolgáltatásról itt olvashat bővebben: [Előzetes értesítés a Microsoft biztonsági közleményeinek kiadásáról](http://technet.microsoft.com/security/bulletin/advance).

Ha automatikus értesítést szeretne kapni a Microsoft biztonsági közleményeinek megjelenéséről, fizessen elő a [Microsoft Technical Security Notifications](http://go.microsoft.com/fwlink/?linkid=21163) szolgáltatásra.

A közleményekkel kapcsolatos kérdések megválaszolására a Microsoft 2010. április 14-én, csendes-óceáni idő szerint 11 órakor webes szemináriumot tart. Jelentkezzen most az [áprilisi közleményeket bemutató webes szemináriumra](http://msevents.microsoft.com/cui/webcasteventdetails.aspx?eventid=1032427721&eventcategory=4&culture=en-us&countrycode=us). Ezt követően a webes szeminárium igény szerint kerül megrendezésre. További információkért látogasson el a [Microsoft biztonsági közleményeit és a webes szemináriumokat](http://technet.microsoft.com/security/bulletin/summary)bemutató oldalra.

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
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=184933">MS10-019</a></td>
<td style="border:1px solid black;"><strong>A Windows biztonsági rései távoli programkódfuttatásra adhatnak lehetőséget (981210)</strong><br />
<br />
A frissítés két közvetlenül jelentett, távoli kódfuttatásra lehetőséget adó biztonsági rést szüntet meg a Windows Authenticode alapú hitelesítésénél. A biztonsági rést kihasználó támadó teljes mértékben átveheti az érintett rendszer irányítását. Ezt követően a támadó programokat telepíthet, illetve adatokat tekinthet meg, módosíthat és törölhet, de korlátozás nélküli jogosultságokkal rendelkező új fiókokat is létrehozhat.</td>
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=21140">Kritikus</a><br />
Távoli kódfuttatás</td>
<td style="border:1px solid black;">Újraindítást igényel</td>
<td style="border:1px solid black;">Microsoft Windows</td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=184663">MS10-020</a></td>
<td style="border:1px solid black;"><strong>Az SMB ügyfélgépén a biztonsági rések távolról történő kódfuttatást tesznek lehetővé (980232)</strong><br />
<br />
Ez a biztonsági frissítés egy nyilvánosságra került és több közvetlenül jelentett biztonsági rést szüntet meg a Microsoft Windows alkalmazásban. A biztonsági rések távolról történő programkódfuttatást tehetnek lehetővé, ha a támadó speciálisan kialakított SMB választ küld az ügyfél által kezdeményezett SMB kérelemre. A biztonsági rések kihasználásához a támadónak meg kell győzni a felhasználót, hogy SMB kapcsolatot kezdeményezzen egy speciálisan kialakított SMB kiszolgálóval.</td>
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=21140">Kritikus</a><br />
Távoli kódfuttatás</td>
<td style="border:1px solid black;">Újraindítást igényel</td>
<td style="border:1px solid black;">Microsoft Windows</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=185146">MS10-025</a></td>
<td style="border:1px solid black;"><strong>A Microsoft Windows Media Services biztonsági rése távolról történő kódfuttatást tesz lehetővé (980858)</strong><br />
<br />
A biztonsági frissítés a Microsoft Windows 2000 Server rendszeren futó Windows Media Services alkalmazás közvetlenül jelentett biztonsági rését hárítja el. A biztonsági rés távoli kódfuttatást okozhat, ha a támadó speciálisan létrehozott forgalmiadat-csomagot küld a Windows Media Services alkalmazást futtató Microsoft Windows 2000 Server rendszerre. A tűzfalakra vonatkozó gyakorlati tanácsok, valamint a szabványos alapértelmezett tűzfal-konfigurációk segítséget nyújtanak a hálózatot érő, a szervezet határain kívülről eredő támadások kivédésében. Gyakorlati tanácsként azt javasoljuk, hogy az internetkapcsolattal rendelkező számítógépeken a lehető legkevesebb port legyen megnyitva. A Microsoft Windows 2000 Server rendszeren futó Windows Media Services opcionális összetevőnek számít, és alapértelmezésben nincs telepítve.</td>
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=21140">Kritikus</a><br />
Távoli kódfuttatás</td>
<td style="border:1px solid black;">Esetleg újra kell indítani a rendszert</td>
<td style="border:1px solid black;">Microsoft Windows</td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=184752">MS10-026</a></td>
<td style="border:1px solid black;"><strong>A Microsoft MPEG Layer-3 kodekek távoli kódfuttatást okozhatnak (977816)</strong><br />
<br />
A biztonsági frissítés a Microsoft MPEG Layer-3 audiokodekek egy közvetlenül jelentett biztonsági rését szünteti meg. A biztonsági rés távoli kódvégrehajtást tehet lehetővé, ha a felhasználó megnyit egy speciálisan kialakított AVI fájlt, amely MPEG Layer-3 audiofolyamot tartalmaz. Ha valamely felhasználó felügyeleti jogosultságokkal bejelentkezett a rendszerbe, akkor a biztonsági rést kihasználó támadó teljes mértékben átveheti az irányítást a számítógép felett, Ezt követően a támadó programokat telepíthet, illetve adatokat tekinthet meg, módosíthat és törölhet, de korlátozás nélküli jogosultságokkal rendelkező új fiókokat is létrehozhat. A kevesebb jogosultsággal bíró fiókkal rendelkező felhasználók esetében kisebb a veszélyeztetettség, mint a rendszergazdai jogosultságokkal rendelkezők esetén</td>
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=21140">Kritikus</a><br />
Távoli kódfuttatás</td>
<td style="border:1px solid black;">Esetleg újra kell indítani a rendszert</td>
<td style="border:1px solid black;">Microsoft Windows</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=184071">MS10-027</a></td>
<td style="border:1px solid black;"><strong>A Windows Media Player biztonsági rése, amely távoli programkódfuttatást tesz lehetővé (979402)</strong><br />
<br />
A biztonsági frissítés a Windows Media Player közvetlenül jelentett biztonsági rését szünteti meg. A biztonsági rés távolról történő programkódfuttatást tehet lehetővé, ha a Windows Media Player egy rosszindulatú webhelyen tárolt, speciálisan kialakított médiatartalmat nyit meg. A biztonsági rést kihasználó támadó a helyi felhasználóval egyező hozzáférést nyer a rendszerhez. A kevesebb jogosultsággal bíró fiókkal rendelkező felhasználók esetében kisebb a veszélyeztetettség, mint a rendszergazdai jogosultságokkal rendelkezők esetén</td>
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=21140">Kritikus</a><br />
Távoli kódfuttatás</td>
<td style="border:1px solid black;">Esetleg újra kell indítani a rendszert</td>
<td style="border:1px solid black;">Microsoft Windows</td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=184814">MS10-021</a></td>
<td style="border:1px solid black;"><strong>A Windows-kernel biztonsági rései jogok kiterjesztését tehetik lehetővé (979683)</strong><br />
<br />
A biztonsági frissítés a Microsoft Windows néhány, közvetlenül jelentett biztonsági rését szünteti meg. A biztonsági rések legsúlyosabbika jogok kiterjesztését teheti lehetővé, ha a támadó helyben bejelentkezett, és ott különlegesen kialakított alkalmazást futtatott. A támadónak a biztonsági rések kihasználásához érvényes bejelentkezési adatokkal kell rendelkeznie, és képesnek kell lennie helyileg bejelentkezni a rendszerbe. Névtelen felhasználók nem tudják távolról kiaknázni ezeket a biztonsági réseket.</td>
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=21140">Fontos</a><br />
Jogok kiterjesztése</td>
<td style="border:1px solid black;">Újraindítást igényel</td>
<td style="border:1px solid black;">Microsoft Windows</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=184779">MS10-022</a></td>
<td style="border:1px solid black;"><strong>A VBScript biztonsági rése távolról történő kódfuttatást tehet lehetővé (981169)</strong><br />
<br />
A biztonsági frissítés a Microsoft Windows rendszeren futó VBScript alkalmazás távolról történő kódfuttatást lehetővé tevő, nyilvánosan jelentett biztonsági rését szünteti meg. Ez a biztonsági frissítés Microsoft Windows 2000, Windows XP és Windows Server 2003 esetén Fontos besorolású. Windows Server 2008, Windows Vista, Windows 7 és Windows Server 2008 R2 esetén a fenyegetett kód nem használható ki, de mivel a kód jelen van, a frissítés lényeges biztonsági intézkedésnek minősül, noha nem rendelkezik súlyossági besorolással.<br />
<br />
A biztonsági rés távoli kódfuttatást tesz lehetővé, ha egy rosszindulatú webhelyen speciálisan kialakított párbeszédpanel jelenik meg egy webhelyen és a felhasználó megnyomja az F1 gombot, ekkor ugyanis a Windows Súgó rendszere a támadó által létrehozott Windows alapú súgófájllal indul el. Ha valamely felhasználó felügyeleti jogosultságokkal bejelentkezett a rendszerbe, akkor a biztonsági rést kihasználó támadó teljes mértékben átveheti az irányítást a számítógép felett,</td>
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=21140">Fontos</a><br />
Távoli kódfuttatás</td>
<td style="border:1px solid black;">Esetleg újra kell indítani a rendszert</td>
<td style="border:1px solid black;">Microsoft Windows</td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=184751">MS10-023</a></td>
<td style="border:1px solid black;"><strong>A Microsoft Office Publisher biztonsági rése távoli kódfuttatást tehet lehetővé (981160)</strong><br />
<br />
A biztonsági frissítés a Microsoft Office Publisher közvetlenül a Microsoftnak jelzett biztonsági rését szünteti meg, amely távoli kódfuttatást tesz lehetővé, amennyiben a felhasználó különlegesen kialakított Publisher fájlt nyit meg. A biztonsági rést kihasználó támadó a helyi felhasználóval egyező hozzáférést nyer a rendszerhez. A kevesebb jogosultsággal bíró fiókkal rendelkező felhasználók esetében kisebb a veszélyeztetettség, mint a rendszergazdai jogosultságokkal rendelkezők esetén</td>
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=21140">Fontos</a><br />
Távoli kódfuttatás</td>
<td style="border:1px solid black;">Esetleg újra kell indítani a rendszert</td>
<td style="border:1px solid black;">Microsoft Office</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=167307">MS10-024</a></td>
<td style="border:1px solid black;"><strong>A Microsoft Exchange és a Windows SMTP Service biztonsági rései szolgáltatásmegtagadást okozhatnak (981832)</strong><br />
<br />
A biztonsági frissítés a Microsoft Exchange és a Windows SMTP Service egy nyilvánosságra került és egy közvetlenül jelentett biztonsági résének hibáját hárítja el. A legsúlyosabb biztonsági rése szolgáltatásmegtagadást tesz lehetővé, ha a támadó speciálisan kialakított DNS-választ küld az SMTP szolgáltatást futtató számítógépre. Alapértelmezés szerint az SMTP összetevő nincs telepítve a Windows Server 2003, a Windows Server 2003 x64 Edition és a Windows XP x64 Edition rendszeren.</td>
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=21140">Fontos</a><br />
Szolgáltatásmegtagadás</td>
<td style="border:1px solid black;">Újraindítást igényel</td>
<td style="border:1px solid black;">Microsoft Windows, Microsoft Exchange</td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=182935">MS10-028</a></td>
<td style="border:1px solid black;"><strong>A Microsoft Visio biztonsági rései távolról történő programkódfuttatást tehetnek lehetővé (980094)</strong><br />
<br />
Ez a biztonsági frissítés a Microsoft Office Visio két közvetlenül jelzett biztonsági rését szünteti meg. A biztonsági rések távoli kódvégrehajtást tehetnek lehetővé, amennyiben a felhasználó egy speciálisan kialakított Visio fájlt nyit meg. A biztonsági réseket kihasználó támadó a helyi felhasználóval egyező hozzáférést nyer a rendszerhez. A kevesebb jogosultsággal bíró fiókkal rendelkező felhasználók esetében kisebb a veszélyeztetettség, mint a rendszergazdai jogosultságokkal rendelkezők esetén</td>
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=21140">Fontos</a><br />
Távoli kódfuttatás</td>
<td style="border:1px solid black;">Esetleg újra kell indítani a rendszert</td>
<td style="border:1px solid black;">Microsoft Office</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=179056">MS10-029</a></td>
<td style="border:1px solid black;"><strong>A Windows ISATAP összetevő biztonsági rései tartalomhamisítást okozhat (978338)</strong><br />
<br />
A biztonsági frissítés a Microsoft Windows egy közvetlenül jelentett biztonsági rését szünteti meg. A biztonsági frissítés a Windows XP, Windows Server 2003, Windows Vista és Windows Server 2008 rendszerre nézve Mérsékelt besorolású. A Windows 7 és Windows Server 2008 R2 rendszert nem érinti a probléma, mivel ezek az operációs rendszerek tartalmazzák a biztonsági frissítésben telepített funkciót.<br />
<br />
A biztonsági rést kihasználó támadó úgy meghamisíthat egy IPv4 címet, hogy az megkerüli a forrás IPv4 címen alapuló szűrőeszközöket. A biztonsági frissítés a biztonsági rés elhárítása érdekében módosítja a bújtatott ISATAP csomagban található forrás IPv6 cím ellenőrzési módját a Windows TCP/IP kötegben.</td>
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=21140">Mérsékelt</a><br />
Tartalomhamisítás</td>
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
  
A táblázat segítségével meghatározható annak valószínűsége, hogy a biztonsági közlemény kiadását követő 30 napon belül a telepíteni szükséges biztonsági frissítésekre működő rosszindulatú programkódot jelentetnek meg. A telepítés fontossági sorrendjének megállapításához az adott konfigurációnak megfelelően tekintse át az alábbi értékeléseket. A minősítések jelentéséről és meghatározásuk módjáról a [Microsoft biztonsági rések jegyzéke](http://technet.microsoft.com/en-us/security/cc998259.aspx) tartalmaz bővebb információt.

 
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
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=184814">MS10-021</a></td>
<td style="border:1px solid black;">Windows-kernel memóriakiosztás biztonsági rése</td>
<td style="border:1px solid black;"><a href="http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2010-0236">CVE-2010-0236</a></td>
<td style="border:1px solid black;"><a href="http://technet.microsoft.com/en-us/security/cc998259.aspx"><strong>1</strong></a> - Valószínűleg konzisztens rosszindulatú programkód</td>
<td style="border:1px solid black;">(Nincs)</td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=184814">MS10-021</a></td>
<td style="border:1px solid black;">Windows-kernel szimbolikus hivatkozás létrehozásának biztonsági rése</td>
<td style="border:1px solid black;"><a href="http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2010-0237">CVE-2010-0237</a></td>
<td style="border:1px solid black;"><a href="http://technet.microsoft.com/en-us/security/cc998259.aspx"><strong>1</strong></a> - Valószínűleg konzisztens rosszindulatú programkód</td>
<td style="border:1px solid black;">(Nincs)</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=182935">MS10-028</a></td>
<td style="border:1px solid black;">Visio attribútumérvényesítési memóriameghibásodás okozta biztonsági rés</td>
<td style="border:1px solid black;"><a href="http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2010-0254">CVE-2010-0254</a></td>
<td style="border:1px solid black;"><a href="http://technet.microsoft.com/en-us/security/cc998259.aspx"><strong>1</strong></a> - Valószínűleg konzisztens rosszindulatú programkód</td>
<td style="border:1px solid black;">(Nincs)</td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=184071">MS10-027</a></td>
<td style="border:1px solid black;">A Media Player távoli programkódfuttatást lehetővé tevő biztonsági rése</td>
<td style="border:1px solid black;"><a href="http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2010-0268">CVE-2010-0268</a></td>
<td style="border:1px solid black;"><a href="http://technet.microsoft.com/en-us/security/cc998259.aspx"><strong>1</strong></a> - Valószínűleg konzisztens rosszindulatú programkód</td>
<td style="border:1px solid black;">(Nincs)</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=185146">MS10-025</a></td>
<td style="border:1px solid black;">A Media Services kötegalapú puffertúlcsordulás biztonsági rése</td>
<td style="border:1px solid black;"><a href="http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2010-0478">CVE-2010-0478</a></td>
<td style="border:1px solid black;"><a href="http://technet.microsoft.com/en-us/security/cc998259.aspx"><strong>1</strong></a> - Valószínűleg konzisztens rosszindulatú programkód</td>
<td style="border:1px solid black;">(Nincs)</td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=184751">MS10-023</a></td>
<td style="border:1px solid black;">Microsoft Office Publisher fájlkonverziós szövegdoboz-feldolgozás puffertúlcsordulási biztonsági rése</td>
<td style="border:1px solid black;"><a href="http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2010-0479">CVE-2010-0479</a></td>
<td style="border:1px solid black;"><a href="http://technet.microsoft.com/en-us/security/cc998259.aspx"><strong>1</strong></a> - Valószínűleg konzisztens rosszindulatú programkód</td>
<td style="border:1px solid black;">(Nincs)</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=184752">MS10-026</a></td>
<td style="border:1px solid black;">MPEG Layer-3 audiodekóder kötegtúlcsordulást okozó biztonsági rése</td>
<td style="border:1px solid black;"><a href="http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2010-0480">CVE-2010-0480</a></td>
<td style="border:1px solid black;"><a href="http://technet.microsoft.com/en-us/security/cc998259.aspx"><strong>1</strong></a> - Valószínűleg konzisztens rosszindulatú programkód</td>
<td style="border:1px solid black;">(Nincs)</td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=184779">MS10-022</a></td>
<td style="border:1px solid black;">VBScript Súgó gombjához tartozó biztonsági rés</td>
<td style="border:1px solid black;"><a href="http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2010-0483">CVE-2010-0483</a></td>
<td style="border:1px solid black;"><a href="http://technet.microsoft.com/en-us/security/cc998259.aspx"><strong>1</strong></a> - Valószínűleg konzisztens rosszindulatú programkód<br />
<br />
Windows Server 2008, Windows 7 és Windows Server 2008 R2:<br />
<a href="http://technet.microsoft.com/en-us/security/cc998259.aspx"><strong>3</strong></a> - Nem valószínű működő rosszindulatú programkód</td>
<td style="border:1px solid black;">A biztonsági rést a<a href="http://technet.microsoft.com/security/advisory/981169">Microsoft 981169-es számú biztonsági tanácsadójában írtak szerint már nyilvánosságra hozták</a></td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=182935">MS10-028</a></td>
<td style="border:1px solid black;">A Visio indexszámítási memóriameghibásodás okozta biztonsági rés</td>
<td style="border:1px solid black;"><a href="http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2010-0256">CVE-2010-0256</a></td>
<td style="border:1px solid black;"><a href="http://technet.microsoft.com/en-us/security/cc998259.aspx"><strong>2</strong></a> - Valószínűleg inkonzisztens rosszindulatú programkód</td>
<td style="border:1px solid black;">(Nincs)</td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=184663">MS10-020</a></td>
<td style="border:1px solid black;">Az SMB ügyfél tranzakciós biztonsági rése</td>
<td style="border:1px solid black;"><a href="http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2010-0270">CVE-2010-0270</a></td>
<td style="border:1px solid black;"><a href="http://technet.microsoft.com/en-us/security/cc998259.aspx"><strong>2</strong></a> - Valószínűleg inkonzisztens rosszindulatú programkód</td>
<td style="border:1px solid black;">(Nincs)</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=184663">MS10-020</a></td>
<td style="border:1px solid black;">Az SMB ügyfél válaszelemzési biztonsági rése</td>
<td style="border:1px solid black;"><a href="http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2010-0476">CVE-2010-0476</a></td>
<td style="border:1px solid black;"><a href="http://technet.microsoft.com/en-us/security/cc998259.aspx"><strong>2</strong></a> - Valószínűleg inkonzisztens rosszindulatú programkód</td>
<td style="border:1px solid black;">(Nincs)</td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=184933">MS10-019</a></td>
<td style="border:1px solid black;">A WinVerifyTrust aláírás-érvényesíti biztonsági rése</td>
<td style="border:1px solid black;"><a href="http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2010-0486">CVE-2010-0486</a></td>
<td style="border:1px solid black;"><a href="http://technet.microsoft.com/en-us/security/cc998259.aspx"><strong>2</strong></a> - Valószínűleg inkonzisztens rosszindulatú programkód</td>
<td style="border:1px solid black;">(Nincs)</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=184933">MS10-019</a></td>
<td style="border:1px solid black;">Cabview sérülés-érvényesítési biztonsági rése</td>
<td style="border:1px solid black;"><a href="http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2010-0487">CVE-2010-0487</a></td>
<td style="border:1px solid black;"><a href="http://technet.microsoft.com/en-us/security/cc998259.aspx"><strong>2</strong></a> - Valószínűleg inkonzisztens rosszindulatú programkód</td>
<td style="border:1px solid black;">(Nincs)</td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=184663">MS10-020</a></td>
<td style="border:1px solid black;">Az SMB ügyfél hiányos válaszát eredményező biztonsági rés</td>
<td style="border:1px solid black;"><a href="http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2009-3676">CVE-2009-3676</a></td>
<td style="border:1px solid black;"><a href="http://technet.microsoft.com/en-us/security/cc998259.aspx"><strong>3</strong></a> - Nem valószínű működő rosszindulatú programkód</td>
<td style="border:1px solid black;">A biztonsági rést a<a href="http://technet.microsoft.com/security/advisory/977544">Microsoft 977544-es számú biztonsági tanácsadójában írtak szerint már nyilvánosságra hozták</a><br />
<br />
A legvalószínűbb tünet a szolgáltatásmegtagadás.</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=167307">MS10-024</a></td>
<td style="border:1px solid black;">SMTP kiszolgáló MX-rekord biztonsági rése</td>
<td style="border:1px solid black;"><a href="http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2010-0024">CVE-2010-0024</a></td>
<td style="border:1px solid black;"><a href="http://technet.microsoft.com/en-us/security/cc998259.aspx"><strong>3</strong></a> - Nem valószínű működő rosszindulatú programkód</td>
<td style="border:1px solid black;">A legvalószínűbb tünet a szolgáltatásmegtagadás.</td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=184663">MS10-020</a></td>
<td style="border:1px solid black;">Az SMB ügyfél memóriakiosztási biztonsági rése</td>
<td style="border:1px solid black;"><a href="http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2010-0269">CVE-2010-0269</a></td>
<td style="border:1px solid black;"><a href="http://technet.microsoft.com/en-us/security/cc998259.aspx"><strong>3</strong></a> - Nem valószínű működő rosszindulatú programkód</td>
<td style="border:1px solid black;">(Nincs)</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=184663">MS10-020</a></td>
<td style="border:1px solid black;">Az SMB ügyfél üzenetméret biztonsági rése</td>
<td style="border:1px solid black;"><a href="http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2010-0477">CVE-2010-0477</a></td>
<td style="border:1px solid black;"><a href="http://technet.microsoft.com/en-us/security/cc998259.aspx"><strong>3</strong></a> - Nem valószínű működő rosszindulatú programkód</td>
<td style="border:1px solid black;">A legvalószínűbb tünet a szolgáltatásmegtagadás.</td>
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
</tr>
<tr>
<th colspan="10">
Microsoft Windows 2000  
</th>
</tr>
<tr>
<td style="border:1px solid black;">
**Közlemény azonosítója**
</td>
<td style="border:1px solid black;">
[**MS10-019**](http://go.microsoft.com/fwlink/?linkid=184933)
</td>
<td style="border:1px solid black;">
[**MS10-020**](http://go.microsoft.com/fwlink/?linkid=184663)
</td>
<td style="border:1px solid black;">
[**MS10-025**](http://go.microsoft.com/fwlink/?linkid=185146)
</td>
<td style="border:1px solid black;">
[**MS10-026**](http://go.microsoft.com/fwlink/?linkid=184752)
</td>
<td style="border:1px solid black;">
[**MS10-027**](http://go.microsoft.com/fwlink/?linkid=184071)
</td>
<td style="border:1px solid black;">
[**MS10-021**](http://go.microsoft.com/fwlink/?linkid=184814)
</td>
<td style="border:1px solid black;">
[**MS10-022**](http://go.microsoft.com/fwlink/?linkid=184779)
</td>
<td style="border:1px solid black;">
[**MS10-024**](http://go.microsoft.com/fwlink/?linkid=167307)
</td>
<td style="border:1px solid black;">
[**MS10-029**](http://go.microsoft.com/fwlink/?linkid=179056)
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
Microsoft Windows 2000 Service Pack 4
</td>
<td style="border:1px solid black;">
[Authenticode 5.1 aláírás-ellenőrzés](http://www.microsoft.com/downloads/details.aspx?familyid=d7538166-35ee-4c6b-be8c-e83a1fc6cd77)  
(KB978601)  
(Kritikus)  
[Kabinetfájlnéző rendszerhéj-kiterjesztés 5.1](http://www.microsoft.com/downloads/details.aspx?familyid=13846177-f25f-4dd4-9fe9-ac43e1d4d73d)  
(KB979309)  
(Kritikus)
</td>
<td style="border:1px solid black;">
[Microsoft Windows 2000 Service Pack 4](http://www.microsoft.com/downloads/details.aspx?familyid=67ccac04-e5c8-4381-9d1a-9b676dd516a6)  
(Kritikus)
</td>
<td style="border:1px solid black;">
[Microsoft Windows 2000 Server Service Pack 4](http://www.microsoft.com/downloads/details.aspx?familyid=73b3d681-26bb-49c1-849e-1f72484cb978)  
(Kritikus)
</td>
<td style="border:1px solid black;">
[MPEG Layer-3 kodekek](http://www.microsoft.com/downloads/details.aspx?familyid=f6394fc2-b9d0-46cf-9265-a0d4aeb1448f)  
(Kritikus)
</td>
<td style="border:1px solid black;">
[Windows Media Player 9 Series](http://www.microsoft.com/downloads/details.aspx?familyid=c0b8b362-a321-4ac9-be98-15c71bb7a043)  
(Kritikus)
</td>
<td style="border:1px solid black;">
[Microsoft Windows 2000 Service Pack 4](http://www.microsoft.com/downloads/details.aspx?familyid=c5f4577e-7546-40e9-8bcd-be11c1b260a6)  
(Fontos)
</td>
<td style="border:1px solid black;">
[VBScript 5.1](http://www.microsoft.com/downloads/details.aspx?familyid=421be318-f217-4d12-b7a5-833093189073)<sup>[1]</sup>
(KB981350)  
(Fontos)  
[VBScript 5.6](http://www.microsoft.com/downloads/details.aspx?familyid=421be318-f217-4d12-b7a5-833093189073)  
(KB981350)  
(Fontos)  
[VBScript 5.7](http://www.microsoft.com/downloads/details.aspx?familyid=d5fc47a4-cecb-4817-aafb-45f335061be3)  
(KB981349)  
(Fontos)
</td>
<td style="border:1px solid black;">
[Microsoft Windows 2000 Service Pack 4](http://www.microsoft.com/downloads/details.aspx?familyid=88a0e872-01de-495b-8eec-d105a970daa7)  
(Fontos)
</td>
<td style="border:1px solid black;">
Nem érintett
</td>
</tr>
<tr>
<th colspan="10">
Windows XP
</th>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
**Közlemény azonosítója**
</td>
<td style="border:1px solid black;">
[**MS10-019**](http://go.microsoft.com/fwlink/?linkid=184933)
</td>
<td style="border:1px solid black;">
[**MS10-020**](http://go.microsoft.com/fwlink/?linkid=184663)
</td>
<td style="border:1px solid black;">
[**MS10-025**](http://go.microsoft.com/fwlink/?linkid=185146)
</td>
<td style="border:1px solid black;">
[**MS10-026**](http://go.microsoft.com/fwlink/?linkid=184752)
</td>
<td style="border:1px solid black;">
[**MS10-027**](http://go.microsoft.com/fwlink/?linkid=184071)
</td>
<td style="border:1px solid black;">
[**MS10-021**](http://go.microsoft.com/fwlink/?linkid=184814)
</td>
<td style="border:1px solid black;">
[**MS10-022**](http://go.microsoft.com/fwlink/?linkid=184779)
</td>
<td style="border:1px solid black;">
[**MS10-024**](http://go.microsoft.com/fwlink/?linkid=167307)
</td>
<td style="border:1px solid black;">
[**MS10-029**](http://go.microsoft.com/fwlink/?linkid=179056)
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
[**Mérsékelt**](http://go.microsoft.com/fwlink/?linkid=21140)
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
Windows XP Service Pack 2 és Windows XP Service Pack 3
</td>
<td style="border:1px solid black;">
[Authenticode 5.1 aláírás-ellenőrzés](http://www.microsoft.com/downloads/details.aspx?familyid=2a01ddf0-f3ea-47c8-ada2-e69f6c1b5f96)  
(KB978601)  
(Kritikus)  
[Kabinetfájlnéző rendszerhéj-kiterjesztés 6.0](http://www.microsoft.com/downloads/details.aspx?familyid=6c3ac102-2107-4726-98be-4fbf6b858bfb)  
(KB979309)  
(Kritikus)
</td>
<td style="border:1px solid black;">
[Windows XP Service Pack 2 és Windows XP Service Pack 3](http://www.microsoft.com/downloads/details.aspx?familyid=dec38c02-3d4a-41c5-8954-e57f56b8fa5b)  
(Kritikus)
</td>
<td style="border:1px solid black;">
Nem érintett
</td>
<td style="border:1px solid black;">
[MPEG Layer-3 kodekek](http://www.microsoft.com/downloads/details.aspx?familyid=b1582a74-4a7b-4540-beb1-7c89c86eae87)  
(Kritikus)
</td>
<td style="border:1px solid black;">
[Windows Media Player 9 Series Windows XP Service Pack 2 operációs rendszeren](http://www.microsoft.com/downloads/details.aspx?familyid=5c748c6d-84d1-45a9-8a33-9372eb5504d5)  
(Kritikus)  
[Windows Media Player 9 Series Windows XP Service Pack 3 operációs rendszeren](http://www.microsoft.com/downloads/details.aspx?familyid=9e4277b4-2dc5-4163-a6aa-7e07dd32b721)  
(Kritikus)
</td>
<td style="border:1px solid black;">
[Windows XP Service Pack 2 és Windows XP Service Pack 3](http://www.microsoft.com/downloads/details.aspx?familyid=142710fd-9cd4-4dd0-aaba-2aace03c008f)  
(Fontos)
</td>
<td style="border:1px solid black;">
[VBScript 5.6](http://www.microsoft.com/downloads/details.aspx?familyid=aa8ff157-a7b3-4787-80c9-5bc453f0f1c9) alkalmazás Windows XP Service Pack 2 rendszeren  
(KB981350)  
(Fontos)  
[VBScript 5.7](http://www.microsoft.com/downloads/details.aspx?familyid=cb21d276-65e9-4c8f-96e3-cf6dc36d0133)  
(KB981349)  
(Fontos)  
[VBScript 5.8](http://www.microsoft.com/downloads/details.aspx?familyid=ba7ef6e5-80ba-4281-a611-6e5be008c1b4)  
(KB981332)  
(Fontos)
</td>
<td style="border:1px solid black;">
[Windows XP Service Pack 2 és Windows XP Service Pack 3](http://www.microsoft.com/downloads/details.aspx?familyid=de447b76-ec89-426b-ac54-3ae3855d1159)  
(Fontos)
</td>
<td style="border:1px solid black;">
[Windows XP Service Pack 2 és Windows XP Service Pack 3](http://www.microsoft.com/downloads/details.aspx?familyid=9dc3e1c2-2e9d-4d86-9fce-446c409ad613)  
(Mérsékelt)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Windows XP Professional x64 Edition Service Pack 2
</td>
<td style="border:1px solid black;">
[Authenticode 5.1 aláírás-ellenőrzés](http://www.microsoft.com/downloads/details.aspx?familyid=9bbff00c-f8f4-4a44-98f2-18a868986ae1)  
(KB978601)  
(Kritikus)  
[Kabinetfájlnéző rendszerhéj-kiterjesztés 6.0](http://www.microsoft.com/downloads/details.aspx?familyid=e64e487e-2727-4396-b0c9-6eaf000214d2)  
(KB979309)  
(Kritikus)
</td>
<td style="border:1px solid black;">
[Windows XP Professional x64 Edition Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=c5a21239-a9a3-4ec5-9de8-7d2fc16fc6b8)  
(Kritikus)
</td>
<td style="border:1px solid black;">
Nem érintett
</td>
<td style="border:1px solid black;">
[MPEG Layer-3 kodekek](http://www.microsoft.com/downloads/details.aspx?familyid=8afca317-a647-44aa-a771-5d85cd5d62ea)  
(Kritikus)
</td>
<td style="border:1px solid black;">
Nem érintett
</td>
<td style="border:1px solid black;">
[Windows XP Professional x64 Edition Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=3c0cb02e-3484-4cdf-8c64-c697ad3e2889)  
(Fontos)
</td>
<td style="border:1px solid black;">
[VBScript 5.6](http://www.microsoft.com/downloads/details.aspx?familyid=896c738d-4058-440f-8d4f-16c678610cd1)  
(KB981350)  
(Fontos)  
[VBScript 5.7](http://www.microsoft.com/downloads/details.aspx?familyid=d7e8b930-8708-4f0b-b22b-961c2cbc2673)  
(KB981349)  
(Fontos)  
[VBScript 5.8](http://www.microsoft.com/downloads/details.aspx?familyid=153fd9c1-0f8e-4492-87d1-f0381e7feb23)  
(KB981332)  
(Fontos)
</td>
<td style="border:1px solid black;">
[Windows XP Professional x64 Edition Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=4f9a696d-2712-4777-a642-e78a38336e8a)  
(Fontos)
</td>
<td style="border:1px solid black;">
[Windows XP Professional x64 Edition Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=d872bd77-f491-4706-8ff5-081ac0bf3d6f)  
(Mérsékelt)
</td>
</tr>
<tr>
<th colspan="10">
Windows Server 2003
</th>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
**Közlemény azonosítója**
</td>
<td style="border:1px solid black;">
[**MS10-019**](http://go.microsoft.com/fwlink/?linkid=184933)
</td>
<td style="border:1px solid black;">
[**MS10-020**](http://go.microsoft.com/fwlink/?linkid=184663)
</td>
<td style="border:1px solid black;">
[**MS10-025**](http://go.microsoft.com/fwlink/?linkid=185146)
</td>
<td style="border:1px solid black;">
[**MS10-026**](http://go.microsoft.com/fwlink/?linkid=184752)
</td>
<td style="border:1px solid black;">
[**MS10-027**](http://go.microsoft.com/fwlink/?linkid=184071)
</td>
<td style="border:1px solid black;">
[**MS10-021**](http://go.microsoft.com/fwlink/?linkid=184814)
</td>
<td style="border:1px solid black;">
[**MS10-022**](http://go.microsoft.com/fwlink/?linkid=184779)
</td>
<td style="border:1px solid black;">
[**MS10-024**](http://go.microsoft.com/fwlink/?linkid=167307)
</td>
<td style="border:1px solid black;">
[**MS10-029**](http://go.microsoft.com/fwlink/?linkid=179056)
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
Nincsenek
</td>
<td style="border:1px solid black;">
[**Kritikus**](http://go.microsoft.com/fwlink/?linkid=21140)
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
[**Mérsékelt**](http://go.microsoft.com/fwlink/?linkid=21140)
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
Windows Server 2003 Service Pack 2
</td>
<td style="border:1px solid black;">
[Authenticode 5.1 aláírás-ellenőrzés](http://www.microsoft.com/downloads/details.aspx?familyid=0e7e3deb-f078-4953-9642-675ec69267f2)  
(KB978601)  
(Kritikus)  
[Kabinetfájlnéző rendszerhéj-kiterjesztés 6.0](http://www.microsoft.com/downloads/details.aspx?familyid=7ae9b1d0-0dbe-4abd-b315-10cea4ceccd7)  
(KB979309)  
(Kritikus)
</td>
<td style="border:1px solid black;">
[Windows Server 2003 Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=1189304f-d626-426d-960c-a86dc2d2b528)  
(Kritikus)
</td>
<td style="border:1px solid black;">
Nem érintett
</td>
<td style="border:1px solid black;">
[MPEG Layer-3 kodekek](http://www.microsoft.com/downloads/details.aspx?familyid=9f89746c-181e-4177-a851-ec1826e78b6d)  
(Kritikus)
</td>
<td style="border:1px solid black;">
Nem érintett
</td>
<td style="border:1px solid black;">
[Windows Server 2003 Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=0a7ea2d0-61ce-4b68-ad82-d917b1a56f9d)  
(Fontos)
</td>
<td style="border:1px solid black;">
[VBScript 5.6](http://www.microsoft.com/downloads/details.aspx?familyid=28b035b8-d56e-4e93-b811-9a82cf1d4ba9)  
(KB981350)  
(Fontos)  
[VBScript 5.7](http://www.microsoft.com/downloads/details.aspx?familyid=a142a553-85fc-40e0-9426-8d58f6a4333c)  
(KB981349)  
(Fontos)  
[VBScript 5.8](http://www.microsoft.com/downloads/details.aspx?familyid=72754e1b-3d09-4b9d-8794-689c45a37f66)  
(KB981332)  
(Fontos)
</td>
<td style="border:1px solid black;">
[Windows Server 2003 Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=f781e9e4-87d4-4243-9d44-256424d75fec)  
(Fontos)
</td>
<td style="border:1px solid black;">
[Windows Server 2003 Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=cd007a6c-04b3-490c-aff4-d5af3e69d477)  
(Mérsékelt)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Windows Server 2003 x64 Edition Service Pack 2
</td>
<td style="border:1px solid black;">
[Authenticode 5.1 aláírás-ellenőrzés](http://www.microsoft.com/downloads/details.aspx?familyid=99a3f6da-728f-421c-ab41-c4c4751934a4)  
(KB978601)  
(Kritikus)  
[Kabinetfájlnéző rendszerhéj-kiterjesztés 6.0](http://www.microsoft.com/downloads/details.aspx?familyid=1709fd4e-d7c6-4cbb-8b71-a96b8d6eee58)  
(KB979309)  
(Kritikus)
</td>
<td style="border:1px solid black;">
[Windows Server 2003 x64 Edition Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=52e4f66b-b76c-46a1-aeff-74efa21fc743)  
(Kritikus)
</td>
<td style="border:1px solid black;">
Nem érintett
</td>
<td style="border:1px solid black;">
[MPEG Layer-3 kodekek](http://www.microsoft.com/downloads/details.aspx?familyid=b97e7ea1-a163-4ce4-8cbc-5f933773c4b2)  
(Kritikus)
</td>
<td style="border:1px solid black;">
Nem érintett
</td>
<td style="border:1px solid black;">
[Windows Server 2003 x64 Edition Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=1fc66f54-260a-4219-a0b4-056ba9dd0abe)  
(Fontos)
</td>
<td style="border:1px solid black;">
[VBScript 5.6](http://www.microsoft.com/downloads/details.aspx?familyid=339ddf48-8949-4857-9ef6-1ddcc7c5f8b8)  
(KB981350)  
(Fontos)  
[VBScript 5.7](http://www.microsoft.com/downloads/details.aspx?familyid=a489b4e3-78d2-411b-b27c-5987b8fc91d1)  
(KB981349)  
(Fontos)  
[VBScript 5.8](http://www.microsoft.com/downloads/details.aspx?familyid=72c3013b-f72f-422b-8a89-2246dea4b378)  
(KB981332)  
(Fontos)
</td>
<td style="border:1px solid black;">
[Windows Server 2003 x64 Edition Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=644ff070-237b-4a73-b2e2-9fffdafa3927)  
(Fontos)
</td>
<td style="border:1px solid black;">
[Windows Server 2003 x64 Edition Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=19cfddfe-e8da-4564-9730-babfae4a3ebb)  
(Mérsékelt)
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
Windows Server 2003 SP2 Itanium alapú rendszerekhez
</td>
<td style="border:1px solid black;">
[Authenticode 5.1 aláírás-ellenőrzés](http://www.microsoft.com/downloads/details.aspx?familyid=06832599-1e9b-4792-8c7b-7b5b3a3d6277)  
(KB978601)  
(Kritikus)  
[Kabinetfájlnéző rendszerhéj-kiterjesztés 6.0](http://www.microsoft.com/downloads/details.aspx?familyid=811a2b28-655d-4b5d-821e-5a90d556dba3)  
(KB979309)  
(Kritikus)
</td>
<td style="border:1px solid black;">
[Windows Server 2003 SP2 javítócsomaggal Itanium alapú rendszerekhez](http://www.microsoft.com/downloads/details.aspx?familyid=b2b6d8b1-63cc-459c-b5fa-1355386273c8)  
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
[Windows Server 2003 SP2 javítócsomaggal Itanium alapú rendszerekhez](http://www.microsoft.com/downloads/details.aspx?familyid=8dcb8be8-fb78-4518-aa7e-f8b17f7dfb86)  
(Fontos)
</td>
<td style="border:1px solid black;">
[VBScript 5.6](http://www.microsoft.com/downloads/details.aspx?familyid=9a8bee82-5f7f-490e-a1eb-481f6d4fc4f5)  
(KB981350)  
(Fontos)  
[VBScript 5.7](http://www.microsoft.com/downloads/details.aspx?familyid=7d542ac6-8a5b-4dd7-8688-2b5feb563636)  
(KB981349)  
(Fontos)
</td>
<td style="border:1px solid black;">
[Windows Server 2003 SP2 javítócsomaggal Itanium alapú rendszerekhez](http://www.microsoft.com/downloads/details.aspx?familyid=56c8238d-8b04-4aa5-8719-40550cd7325c)  
(Fontos)
</td>
<td style="border:1px solid black;">
[Windows Server 2003 SP2 javítócsomaggal Itanium alapú rendszerekhez](http://www.microsoft.com/downloads/details.aspx?familyid=916f1b09-e79e-4347-9fbc-c0cf07de397d)  
(Mérsékelt)
</td>
</tr>
<tr>
<th colspan="10">
Windows Vista
</th>
</tr>
<tr>
<td style="border:1px solid black;">
**Közlemény azonosítója**
</td>
<td style="border:1px solid black;">
[**MS10-019**](http://go.microsoft.com/fwlink/?linkid=184933)
</td>
<td style="border:1px solid black;">
[**MS10-020**](http://go.microsoft.com/fwlink/?linkid=184663)
</td>
<td style="border:1px solid black;">
[**MS10-025**](http://go.microsoft.com/fwlink/?linkid=185146)
</td>
<td style="border:1px solid black;">
[**MS10-026**](http://go.microsoft.com/fwlink/?linkid=184752)
</td>
<td style="border:1px solid black;">
[**MS10-027**](http://go.microsoft.com/fwlink/?linkid=184071)
</td>
<td style="border:1px solid black;">
[**MS10-021**](http://go.microsoft.com/fwlink/?linkid=184814)
</td>
<td style="border:1px solid black;">
[**MS10-022**](http://go.microsoft.com/fwlink/?linkid=184779)
</td>
<td style="border:1px solid black;">
[**MS10-024**](http://go.microsoft.com/fwlink/?linkid=167307)
</td>
<td style="border:1px solid black;">
[**MS10-029**](http://go.microsoft.com/fwlink/?linkid=179056)
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
<td style="border:1px solid black;">
Nincsenek
</td>
<td style="border:1px solid black;">
[**Mérsékelt**](http://go.microsoft.com/fwlink/?linkid=21140)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Windows Vista, Windows Vista Service Pack 1 és Windows Vista Service Pack 2
</td>
<td style="border:1px solid black;">
[Authenticode 6.0 aláírás-ellenőrzés](http://www.microsoft.com/downloads/details.aspx?familyid=a52225a7-6005-4f2b-8291-db20558f23f8)  
(KB978601  
(Kritikus)  
[Kabinetfájlnéző rendszerhéj-kiterjesztés 6.0](http://www.microsoft.com/downloads/details.aspx?familyid=6145e2b2-36fd-4360-bd5b-2bd11890fc52)  
(KB979309)  
(Kritikus)
</td>
<td style="border:1px solid black;">
[Windows Vista, Windows Vista Service Pack 1, és Windows Vista Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=25eeaeb3-c0a3-4a02-9912-acd0342648ba)  
(Kritikus)
</td>
<td style="border:1px solid black;">
Nem érintett
</td>
<td style="border:1px solid black;">
[MPEG Layer-3 kodekek](http://www.microsoft.com/downloads/details.aspx?familyid=0e7140bb-42d3-48b3-9f4b-d55b17770de8)  
(Fontos)
</td>
<td style="border:1px solid black;">
Nem érintett
</td>
<td style="border:1px solid black;">
[Windows Vista](http://www.microsoft.com/downloads/details.aspx?familyid=86d7b054-af4f-4d8a-9873-cb5246466374)  
(Fontos)  
[Windows Vista Service Pack 1 és Windows Vista Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=86d7b054-af4f-4d8a-9873-cb5246466374)  
(Mérsékelt)
</td>
<td style="border:1px solid black;">
[VBScript 5.7](http://www.microsoft.com/downloads/details.aspx?familyid=ee5c42c6-16bb-48bf-95c2-c188bb17d04b)  
(KB981349)  
(Nincs súlyossági besorolás<sup>[2]</sup>)  
[VBScript 5.8](http://www.microsoft.com/downloads/details.aspx?familyid=f2a37dbf-4a95-4e8d-a474-ecacd9aee690)  
(KB981332)  
(Nincs súlyossági besorolás<sup>[2]</sup>)
</td>
<td style="border:1px solid black;">
Nem érintett
</td>
<td style="border:1px solid black;">
[Windows Vista, Windows Vista Service Pack 1, és Windows Vista Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=196055a6-15d1-4da8-b33d-501e69bf5176)  
(Mérsékelt)
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
Windows Vista x64 Edition, Windows Vista x64 Edition Service Pack 1 és Windows Vista x64 Edition Service Pack 2
</td>
<td style="border:1px solid black;">
[Authenticode 6.0 aláírás-ellenőrzés](http://www.microsoft.com/downloads/details.aspx?familyid=9ba7468c-23a4-4994-9a5a-22e96ef586f3)  
(KB978601)  
(Kritikus)  
[Kabinetfájlnéző rendszerhéj-kiterjesztés 6.0](http://www.microsoft.com/downloads/details.aspx?familyid=5b7efa82-0feb-413a-9f8e-212e7432cd99)  
(KB979309)  
(Kritikus)
</td>
<td style="border:1px solid black;">
[Windows Vista x64 Edition, Windows Vista x64 Edition Service Pack 1 és Windows Vista x64 Edition Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=394c1caa-97e4-47a3-9aac-a4a88508bd31)  
(Kritikus)
</td>
<td style="border:1px solid black;">
Nem érintett
</td>
<td style="border:1px solid black;">
[MPEG Layer-3 kodekek](http://www.microsoft.com/downloads/details.aspx?familyid=b885aef4-3a5d-4c3e-bef6-5efef2965752)  
(Fontos)
</td>
<td style="border:1px solid black;">
Nem érintett
</td>
<td style="border:1px solid black;">
[Windows Vista x64 Edition](http://www.microsoft.com/downloads/details.aspx?familyid=7c84aa24-6331-427a-969c-27f7d39db3d7)  
(Fontos)  
[Windows Vista x64 Edition Service Pack 1 és Windows Vista x64 Edition Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=7c84aa24-6331-427a-969c-27f7d39db3d7)  
(Mérsékelt)
</td>
<td style="border:1px solid black;">
[VBScript 5.7](http://www.microsoft.com/downloads/details.aspx?familyid=ea5c5e9c-0ecd-47bc-912d-5adc00d1aa21)  
(KB981349)  
(Nincs súlyossági besorolás<sup>[2]</sup>)  
[VBScript 5.8](http://www.microsoft.com/downloads/details.aspx?familyid=79093796-4ea9-4c6c-92cc-3fd63c5db918)  
(KB981332)  
(Nincs súlyossági besorolás<sup>[2]</sup>)
</td>
<td style="border:1px solid black;">
Nem érintett
</td>
<td style="border:1px solid black;">
[Windows Vista x64 Edition, Windows Vista x64 Edition Service Pack 1 és Windows Vista x64 Edition Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=7c1d1622-1b67-438d-aae4-1a3954974a36)  
(Mérsékelt)
</td>
</tr>
<tr>
<th colspan="10">
Windows Server 2008
</th>
</tr>
<tr>
<td style="border:1px solid black;">
**Közlemény azonosítója**
</td>
<td style="border:1px solid black;">
[**MS10-019**](http://go.microsoft.com/fwlink/?linkid=184933)
</td>
<td style="border:1px solid black;">
[**MS10-020**](http://go.microsoft.com/fwlink/?linkid=184663)
</td>
<td style="border:1px solid black;">
[**MS10-025**](http://go.microsoft.com/fwlink/?linkid=185146)
</td>
<td style="border:1px solid black;">
[**MS10-026**](http://go.microsoft.com/fwlink/?linkid=184752)
</td>
<td style="border:1px solid black;">
[**MS10-027**](http://go.microsoft.com/fwlink/?linkid=184071)
</td>
<td style="border:1px solid black;">
[**MS10-021**](http://go.microsoft.com/fwlink/?linkid=184814)
</td>
<td style="border:1px solid black;">
[**MS10-022**](http://go.microsoft.com/fwlink/?linkid=184779)
</td>
<td style="border:1px solid black;">
[**MS10-024**](http://go.microsoft.com/fwlink/?linkid=167307)
</td>
<td style="border:1px solid black;">
[**MS10-029**](http://go.microsoft.com/fwlink/?linkid=179056)
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
Nincsenek
</td>
<td style="border:1px solid black;">
[**Mérsékelt**](http://go.microsoft.com/fwlink/?linkid=21140)
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
</tr>
<tr>
<td style="border:1px solid black;">
Windows Server 2008 32 bites rendszerekhez és Windows Server 2008 32 bites rendszerekhez, Service Pack 2
</td>
<td style="border:1px solid black;">
[Authenticode 6.0 aláírás-ellenőrzés\*](http://www.microsoft.com/downloads/details.aspx?familyid=97ffeec8-8b6d-4a30-97b0-4bff2ba5e91d)  
(KB978601)  
(Kritikus)  
[Kabinetfájlnéző rendszerhéj-kiterjesztés 6.0](http://www.microsoft.com/downloads/details.aspx?familyid=f111735b-68b0-4bcc-9dd8-818a5eca3400)  
(KB979309)  
(Kritikus)
</td>
<td style="border:1px solid black;">
[Windows Server 2008 32 bites rendszerekhez és Windows Server 2008 32 bites rendszerekhez, Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=51c9c420-4507-4911-a8f5-82331a696882)\*  
(Kritikus)
</td>
<td style="border:1px solid black;">
Nem érintett
</td>
<td style="border:1px solid black;">
[MPEG Layer-3 kodekek](http://www.microsoft.com/downloads/details.aspx?familyid=8e9c04c9-898f-4ed2-949d-f4343cc0d9f6)\*\*  
(Kritikus)
</td>
<td style="border:1px solid black;">
Nem érintett
</td>
<td style="border:1px solid black;">
[Windows Server 2008 32 bites rendszerekhez és Windows Server 2008 32 bites rendszerekhez, Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=25e3ce7f-53a0-4049-a65c-011d2143c4c2)\*  
(Mérsékelt)
</td>
<td style="border:1px solid black;">
[VBScript 5.7](http://www.microsoft.com/downloads/details.aspx?familyid=dbe89813-0a45-463b-928c-1e58f7bb596a)\*\*  
(KB981349)  
(Nincs súlyossági besorolás<sup>[2]</sup>)  
[VBScript 5.8](http://www.microsoft.com/downloads/details.aspx?familyid=527d6376-efc9-436b-835b-219d38bb28f0)\*\*  
(KB981332)  
(Nincs súlyossági besorolás<sup>[2]</sup>)
</td>
<td style="border:1px solid black;">
[Windows Server 2008 32 bites rendszerekhez és Windows Server 2008 32 bites rendszerekhez Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=e29ead69-000a-4982-a25c-f3981eda381a)\*\*  
(Fontos)
</td>
<td style="border:1px solid black;">
[Windows Server 2008 32 bites rendszerekhez és Windows Server 2008 32 bites rendszerekhez, Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=61ece7bc-e9fa-4ede-ba7d-9e5a4c64b9be)\*  
(Mérsékelt)
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
Windows Server 2008 x64 alapú rendszerekhez és Windows Server 2008 x64 alapú rendszerekhez, Service Pack 2
</td>
<td style="border:1px solid black;">
[Authenticode 6.0 aláírás-ellenőrzés\*](http://www.microsoft.com/downloads/details.aspx?familyid=49f9f740-023a-4291-becf-838a1d282321)  
(KB978601)  
(Kritikus)  
[Kabinetfájlnéző rendszerhéj-kiterjesztés 6.0](http://www.microsoft.com/downloads/details.aspx?familyid=91c08251-0085-44cb-9e9c-9a1a84374caf)  
(KB979309)  
(Kritikus)
</td>
<td style="border:1px solid black;">
[Windows Server 2008 x64 alapú rendszerekhez és Windows Server 2008 x64 alapú rendszerekhez, Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=61c26a1f-c885-4474-9843-204c41628889)\*  
(Kritikus)
</td>
<td style="border:1px solid black;">
Nem érintett
</td>
<td style="border:1px solid black;">
[MPEG Layer-3 kodekek](http://www.microsoft.com/downloads/details.aspx?familyid=d6f2e1ae-48d3-4d2c-b329-32cff00afee5)\*\*  
(Kritikus)
</td>
<td style="border:1px solid black;">
Nem érintett
</td>
<td style="border:1px solid black;">
[Windows Server 2008 x64 alapú rendszerekhez és Windows Server 2008 x64 alapú rendszerekhez, Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=8b99e54d-955b-4a06-9a04-b2f4596efd72)\*  
(Mérsékelt)
</td>
<td style="border:1px solid black;">
[VBScript 5.7](http://www.microsoft.com/downloads/details.aspx?familyid=9db62357-557d-40cd-9826-b7baa6c9de65)\*\*  
(KB981349)  
(Nincs súlyossági besorolás<sup>[2]</sup>)  
[VBScript 5.8](http://www.microsoft.com/downloads/details.aspx?familyid=0c384dbc-21b7-4cbc-b68f-ced971d9b791)\*\*  
(KB981332)  
(Nincs súlyossági besorolás<sup>[2]</sup>)
</td>
<td style="border:1px solid black;">
[Windows Server 2008 x64 alapú rendszerekhez és Windows Server 2008 x64 alapú rendszerekhez Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=8f922e64-e3a6-46fe-9a81-b2813ea6a330)\*\*  
(Fontos)
</td>
<td style="border:1px solid black;">
[Windows Server 2008 x64 alapú rendszerekhez és Windows Server 2008 x64 alapú rendszerekhez, Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=72e7c7ea-55ef-457b-a03a-49aa9dea2e84)\*  
(Mérsékelt)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Windows Server 2008 Itanium alapú rendszerekhez és Windows Server 2008 Itanium alapú rendszerekhez, Service Pack 2
</td>
<td style="border:1px solid black;">
[Authenticode 6.0 aláírás-ellenőrzés](http://www.microsoft.com/downloads/details.aspx?familyid=bd60779a-8bb1-4107-a344-9b09a50e96ff)  
(KB978601)  
(Kritikus)  
[Kabinetfájlnéző rendszerhéj-kiterjesztés 6.0](http://www.microsoft.com/downloads/details.aspx?familyid=eb116688-1d6e-4e20-948e-1d347af5d985)  
(KB979309)  
(Kritikus)
</td>
<td style="border:1px solid black;">
[Windows Server 2008 Itanium alapú rendszerekhez és Windows Server 2008 Itanium alapú rendszerekhez, Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=bcf8b919-08a9-487f-8dfd-3ca24328c4f3)  
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
[Windows Server 2008 Itanium alapú rendszerekhez és Windows Server 2008 Itanium alapú rendszerekhez, Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=b1f9746d-61a2-406f-b707-60646bd5b5bb)  
(Mérsékelt)
</td>
<td style="border:1px solid black;">
[VBScript 5.7](http://www.microsoft.com/downloads/details.aspx?familyid=84c5aaae-9417-42a1-834f-22c1ad46a12f)  
(KB981349)  
(Nincs súlyossági besorolás<sup>[2]</sup>)
</td>
<td style="border:1px solid black;">
Nem érintett
</td>
<td style="border:1px solid black;">
[Windows Server 2008 Itanium alapú rendszerekhez és Windows Server 2008 Itanium alapú rendszerekhez, Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=8c48302c-a1d6-41bc-ad24-7ce7332d4842)  
(Mérsékelt)
</td>
</tr>
<tr>
<th colspan="10">
Windows 7
</th>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
**Közlemény azonosítója**
</td>
<td style="border:1px solid black;">
[**MS10-019**](http://go.microsoft.com/fwlink/?linkid=184933)
</td>
<td style="border:1px solid black;">
[**MS10-020**](http://go.microsoft.com/fwlink/?linkid=184663)
</td>
<td style="border:1px solid black;">
[**MS10-025**](http://go.microsoft.com/fwlink/?linkid=185146)
</td>
<td style="border:1px solid black;">
[**MS10-026**](http://go.microsoft.com/fwlink/?linkid=184752)
</td>
<td style="border:1px solid black;">
[**MS10-027**](http://go.microsoft.com/fwlink/?linkid=184071)
</td>
<td style="border:1px solid black;">
[**MS10-021**](http://go.microsoft.com/fwlink/?linkid=184814)
</td>
<td style="border:1px solid black;">
[**MS10-022**](http://go.microsoft.com/fwlink/?linkid=184779)
</td>
<td style="border:1px solid black;">
[**MS10-024**](http://go.microsoft.com/fwlink/?linkid=167307)
</td>
<td style="border:1px solid black;">
[**MS10-029**](http://go.microsoft.com/fwlink/?linkid=179056)
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
Nincsenek
</td>
<td style="border:1px solid black;">
Nincsenek
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
<td style="border:1px solid black;">
Nincsenek
</td>
<td style="border:1px solid black;">
Nincsenek
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
Windows 7 32 bites rendszerekhez
</td>
<td style="border:1px solid black;">
[Authenticode 6.1 aláírás-ellenőrzés](http://www.microsoft.com/downloads/details.aspx?familyid=8d4a6c65-e171-4570-8f3f-118f06910baf)  
(KB978601)  
(Kritikus)  
[Kabinetfájlnéző rendszerhéj-kiterjesztés 6.1](http://www.microsoft.com/downloads/details.aspx?familyid=f0dbac52-0f0e-40bc-9371-17fa594424d5)  
(KB979309)  
(Kritikus)
</td>
<td style="border:1px solid black;">
[Windows 7 32 bites rendszerekhez](http://www.microsoft.com/downloads/details.aspx?familyid=389184c5-9001-497d-bdf4-81f97ecb617f)  
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
[Windows 7 32 bites rendszerekhez](http://www.microsoft.com/downloads/details.aspx?familyid=ff58d80c-33ce-4d9e-aaa5-0b1841458931)  
(Mérsékelt)
</td>
<td style="border:1px solid black;">
[VBScript 5.8](http://www.microsoft.com/downloads/details.aspx?familyid=c3f76835-0053-4e53-a451-14255e7a4fc0)  
(KB981332)  
(Nincs súlyossági besorolás<sup>[2]</sup>)
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
Windows 7 x64 alapú rendszerekhez
</td>
<td style="border:1px solid black;">
[Authenticode 6.1 aláírás-ellenőrzés](http://www.microsoft.com/downloads/details.aspx?familyid=cf8c6721-05c2-4680-93b4-be36f09c6d15)  
(KB978601)  
(Kritikus)  
[Kabinetfájlnéző rendszerhéj-kiterjesztés 6.1](http://www.microsoft.com/downloads/details.aspx?familyid=b23efe7d-bca4-4d49-9104-6ae39dc5daa9)  
(KB979309)  
(Kritikus)
</td>
<td style="border:1px solid black;">
[Windows 7 x64 alapú rendszerekhez](http://www.microsoft.com/downloads/details.aspx?familyid=f3495dae-71f3-421d-a191-d26965f26ad1)  
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
[Windows 7 x64 alapú rendszerekhez](http://www.microsoft.com/downloads/details.aspx?familyid=7f1dc055-2ec9-407a-9e69-da12338587e3)  
(Mérsékelt)
</td>
<td style="border:1px solid black;">
[VBScript 5.8](http://www.microsoft.com/downloads/details.aspx?familyid=998164b7-4b8c-468b-8d39-f242633c8838)  
(KB981332)  
(Nincs súlyossági besorolás<sup>[2]</sup>)
</td>
<td style="border:1px solid black;">
Nem érintett
</td>
<td style="border:1px solid black;">
Nem érintett
</td>
</tr>
<tr>
<th colspan="10">
Windows Server 2008 R2
</th>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
**Közlemény azonosítója**
</td>
<td style="border:1px solid black;">
[**MS10-019**](http://go.microsoft.com/fwlink/?linkid=184933)
</td>
<td style="border:1px solid black;">
[**MS10-020**](http://go.microsoft.com/fwlink/?linkid=184663)
</td>
<td style="border:1px solid black;">
[**MS10-025**](http://go.microsoft.com/fwlink/?linkid=185146)
</td>
<td style="border:1px solid black;">
[**MS10-026**](http://go.microsoft.com/fwlink/?linkid=184752)
</td>
<td style="border:1px solid black;">
[**MS10-027**](http://go.microsoft.com/fwlink/?linkid=184071)
</td>
<td style="border:1px solid black;">
[**MS10-021**](http://go.microsoft.com/fwlink/?linkid=184814)
</td>
<td style="border:1px solid black;">
[**MS10-022**](http://go.microsoft.com/fwlink/?linkid=184779)
</td>
<td style="border:1px solid black;">
[**MS10-024**](http://go.microsoft.com/fwlink/?linkid=167307)
</td>
<td style="border:1px solid black;">
[**MS10-029**](http://go.microsoft.com/fwlink/?linkid=179056)
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
Nincsenek
</td>
<td style="border:1px solid black;">
Nincsenek
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
<td style="border:1px solid black;">
[**Fontos**](http://go.microsoft.com/fwlink/?linkid=21140)
</td>
<td style="border:1px solid black;">
Nincsenek
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
Windows Server 2008 R2 x64 alapú rendszerekhez
</td>
<td style="border:1px solid black;">
[Authenticode 6.1 aláírás-ellenőrzés\*](http://www.microsoft.com/downloads/details.aspx?familyid=94dfdaae-8464-4de6-a401-7eb70b3bb34f)  
(KB978601)  
(Kritikus)  
[Kabinetfájlnéző rendszerhéj-kiterjesztés 6.1](http://www.microsoft.com/downloads/details.aspx?familyid=a2979c02-2a80-4b84-bf6c-4798064bdf28)  
(KB979309)  
(Kritikus)
</td>
<td style="border:1px solid black;">
[Windows Server 2008 R2 x64 alapú rendszerekhez](http://www.microsoft.com/downloads/details.aspx?familyid=cd1a046e-915d-4904-b753-5a24be10c504)\*  
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
[Windows Server 2008 R2 x64 alapú rendszerekhez](http://www.microsoft.com/downloads/details.aspx?familyid=28389c1d-2a12-4bef-a59b-726bb6449c8b)\*  
(Mérsékelt)
</td>
<td style="border:1px solid black;">
[VBScript 5.8](http://www.microsoft.com/downloads/details.aspx?familyid=c4039d40-a0c7-4183-ab50-04f690d1c5dc)\*\*  
(KB981332)  
(Nincs súlyossági besorolás<sup>[2]</sup>)
</td>
<td style="border:1px solid black;">
[Windows Server 2008 R2 x64 alapú rendszerekhez](http://www.microsoft.com/downloads/details.aspx?familyid=eb27cd2b-d514-4405-8650-259a42e35155)\*\*  
(Fontos)
</td>
<td style="border:1px solid black;">
Nem érintett
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Windows Server 2008 R2 Itanium alapú rendszerekhez
</td>
<td style="border:1px solid black;">
[Authenticode 6.1 aláírás-ellenőrzés](http://www.microsoft.com/downloads/details.aspx?familyid=40f622d2-48e7-4eb2-9430-bbd218cb5208)  
(KB978601)  
(Kritikus)  
[Kabinetfájlnéző rendszerhéj-kiterjesztés 6.1](http://www.microsoft.com/downloads/details.aspx?familyid=5e416d4b-5de7-4688-80c6-245de159e0ce)  
(KB979309)  
(Kritikus)
</td>
<td style="border:1px solid black;">
[Windows Server 2008 R2 Itanium alapú rendszerekhez](http://www.microsoft.com/downloads/details.aspx?familyid=541e9e2f-ec1d-42b2-aae5-481c0d435169)  
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
[Windows Server 2008 R2 Itanium alapú rendszerekhez](http://www.microsoft.com/downloads/details.aspx?familyid=d4ea3984-5183-47f1-814e-29cb6c90ae06)  
(Mérsékelt)
</td>
<td style="border:1px solid black;">
[VBScript 5.8](http://www.microsoft.com/downloads/details.aspx?familyid=8174463c-5c5e-4095-90c8-fd1e898d4ba5)  
(KB981332)  
(Nincs súlyossági besorolás<sup>[2]</sup>)
</td>
<td style="border:1px solid black;">
Nem érintett
</td>
<td style="border:1px solid black;">
Nem érintett
</td>
</tr>
</table>
 
**Megjegyzések a Windows Server 2008 és Windows Server 2008 R2 rendszerhez**

**\*A kiszolgálómag telepítését érinti.** Ez a frissítés ugyanolyan biztonsági besorolás mellett, a megadottak szerint érvényes az Windows Server 2008 és a Windows Server 2008 R2 összes támogatott kiadására, függetlenül attól, hogy a kiszolgálómag-telepítési opcióval telepítették-e. Erről a telepítési opcióról bővebben a [Kiszolgálómag](http://msdn.microsoft.com/en-us/library/ms723891(vs.85).aspx) és a [Kiszolgálómag a Windows Server 2008 R2 rendszerhez](http://msdn.microsoft.com/en-us/library/ee391631(vs.85).aspx) MSDN-cikkekben olvashat. A kiszolgálómag-telepítési opció nem vonatkozik a Windows Server 2008 és a Windows Server 2008 R2 bizonyos kiadásaira; lásd: [A kiszolgálómag-telepítési opciók összehasonlítása](http://www.microsoft.com/windowsserver2008/en/us/compare-core-installation.aspx).

**\*\*A kiszolgálómag-telepítés nem érintett.** A frissítésben tárgyalt biztonsági rések nem érintik a jelzett módon a Windows Server 2008 és a Windows Server 2008 R2 támogatott kiadásait, amennyiben a telepítés a kiszolgálómag-telepítési opció használatával történt. Erről a telepítési opcióról bővebben a [Kiszolgálómag](http://msdn.microsoft.com/en-us/library/ms723891(vs.85).aspx) és a [Kiszolgálómag a Windows Server 2008 R2 rendszerhez](http://msdn.microsoft.com/en-us/library/ee391631(vs.85).aspx) MSDN-cikkekben olvashat. A kiszolgálómag-telepítési opció nem vonatkozik a Windows Server 2008 és a Windows Server 2008 R2 bizonyos kiadásaira; lásd: [A kiszolgálómag-telepítési opciók összehasonlítása](http://www.microsoft.com/windowsserver2008/en/us/compare-core-installation.aspx).

**Megjegyzések az MS10-022 számú közleményhez**

<sup>[1]</sup>A biztonsági frissítés a telepített VBScript 5.1 verziót VBScript 5.6 verzióra frissíti.

<sup>[2]</sup>A súlyossági besorolás nem vonatkozik erre a frissítésre, mivel a tárgyalt biztonsági rés nem érinti ezt a szoftvert. Ennek ellenére a jövőben felfedezett esetleges új támadási pontok elleni mélyreható védekezési lépésként a Microsoft azt javasolja, hogy a szoftver felhasználói alkalmazzák ezt a biztonsági frissítést.

**Megjegyzések az MS10-024. számú közleményhez**

Az ugyanezen a közlemény azonosító alatt található, további frissített fájlokat illetően lásd még az egyéb szoftverkategóriák részt ebben a fejezetben, **Érintett szoftverek és letöltési helyek**. Ez a közlemény több szoftverkategóriát ölel fel.

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
Microsoft Office programcsomagok, rendszerek és összetevők
</th>
</tr>
<tr>
<td style="border:1px solid black;">
**Közlemény azonosítója**
</td>
<td style="border:1px solid black;">
[**MS10-023**](http://go.microsoft.com/fwlink/?linkid=184751)
</td>
<td style="border:1px solid black;">
[**MS10-028**](http://go.microsoft.com/fwlink/?linkid=182935)
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
Microsoft Office XP
</td>
<td style="border:1px solid black;">
[Microsoft Office Publisher 2002 Service Pack 3](http://www.microsoft.com/downloads/details.aspx?familyid=943b3830-70d5-46c5-bffc-1b494434b5f7)  
(KB980466)  
(Fontos)
</td>
<td style="border:1px solid black;">
[Microsoft Office Visio 2002 Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=2d563cbc-d8f7-486b-8c54-25d168085376)  
(KB979364)  
(Fontos)
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
Microsoft Office 2003
</td>
<td style="border:1px solid black;">
[Microsoft Office Publisher 2003 Service Pack 3](http://www.microsoft.com/downloads/details.aspx?familyid=7c2f4610-77bb-4d72-847b-1a06c523b137)  
(KB980469)  
(Fontos)
</td>
<td style="border:1px solid black;">
[Microsoft Office Visio 2003 Service Pack 3](http://www.microsoft.com/downloads/details.aspx?familyid=803a7ea0-a9da-46dd-9548-0177d3774be7)  
(KB979356)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
2007 Microsoft Office rendszer
</td>
<td style="border:1px solid black;">
[Microsoft Office Publisher 2007 Service Pack 1 és Microsoft Office Publisher 2007 Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=10ca2f71-0ab2-4344-b7fd-bbbd6a783a96)  
(KB980470)  
(Fontos)
</td>
<td style="border:1px solid black;">
[Microsoft Office Visio 2007 Service Pack 1 és Microsoft Office Visio 2007 Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=56fe020f-4444-4a43-aa98-e99a622f6a69)  
(KB979365)  
(Fontos)
</td>
</tr>
</table>
 

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
Microsoft Exchange Server
</th>
</tr>
<tr>
<td style="border:1px solid black;">
**Közlemény azonosítója**
</td>
<td style="border:1px solid black;">
[**MS10-024**](http://go.microsoft.com/fwlink/?linkid=167307)
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
Microsoft Exchange Server 2000
</td>
<td style="border:1px solid black;">
[Microsoft Exchange Server 2000 Service Pack 3](http://www.microsoft.com/downloads/details.aspx?familyid=e47c90a0-c9c8-43b7-bec7-34107ddde294)  
(KB976703)  
(Mérsékelt)
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
Microsoft Exchange Server 2003
</td>
<td style="border:1px solid black;">
[Microsoft Exchange Server 2003 Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=bc8391f8-5335-496b-ad4c-bae38509be4a)  
(KB976702)  
(Fontos)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Microsoft Exchange Server 2007
</td>
<td style="border:1px solid black;">
[Microsoft Exchange Server 2007 Service Pack 1 x64 alapú rendszerekhez](http://www.microsoft.com/downloads/details.aspx?familyid=6a894b4e-12b6-4a91-9555-d813956b6aac)  
(KB981407)  
(Nincs súlyossági besorolás<sup>[1]</sup>)  
[Microsoft Exchange Server 2007 Service Pack 2 x64 alapú rendszerekhez](http://www.microsoft.com/downloads/details.aspx?familyid=b8f7f872-16d5-49d6-9867-adc01351c06f)  
(KB981383)  
(Nincs súlyossági besorolás<sup>[1]</sup>)
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
Microsoft Exchange Server 2010
</td>
<td style="border:1px solid black;">
[Microsoft Exchange Server 2010 x64 alapú rendszerekhez](http://www.microsoft.com/downloads/details.aspx?familyid=7dcf2390-dff7-4e3a-acca-03f4d43fb79a)  
(KB981401)  
(Nincs súlyossági besorolás<sup>[1]</sup>)
</td>
</tr>
</table>
 
**Megjegyzések az MS10-024. számú közleményhez**

<sup>[1]</sup>A súlyossági besorolás nem vonatkozik erre a frissítésre, mivel a tárgyalt biztonsági rés nem érinti ezt a szoftvert. A Microsoft azonban javasolja, hogy a szoftverfelhasználók alkalmazzák a frissítést, amely hatékony védelmi frissítés révén kiegészítő forrásport-entrópiát társít az SMTP szolgáltatás által kezdeményezett DNS tranzakciókhoz.

Az ugyanezen a közlemény azonosító alatt található, további frissített fájlokat illetően lásd még az egyéb szoftverkategóriák részt ebben a fejezetben, **Érintett szoftverek és letöltési helyek**. Ez a közlemény több szoftverkategóriát ölel fel.

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

-   Mark Rabinovich,[Visuality Systems Ltd](http://www.visualitynq.com/)., az MS10-020 közleményben leírt probléma jelentéséért
-   Laurent Gaffié, [stratsec](http://www.stratsec.net/), az MS10-020 közleményben bemutatott három probléma jelentéséért
-   Matthew 'j00ru' Jurczyk és Gynvael Coldwind, [Hispasec](http://www.hispasec.com/)[Virustotal](http://www.virustotal.com/), az MS10-021 közleményben ismertetett hat probléma jelentéséért
-   Tavis Ormandy, [Google Inc.](http://www.google.com/), az MS10-021 közleményben bemutatott két probléma jelentéséért
-   Martin Tofall, [Obsidium Software](http://www.obsidium.de/), az MS10-021 közleményben leírt probléma jelentéséért
-   Lionel d'Hauenens, a [Tipping Point](http://www.tippingpoint.com/)[Zero Day Initiative](http://www.zerodayinitiative.com/) program munkatársa, az MS10-023 közleményben leírt egyik probléma jelentéséért
-   Fabien Perigaud, [CERT-LEXSI](http://cert.lexsi.com/), MS10-025 közleményben leírt probléma jelentéséért
-   Fabien Perigaud, [CERT-LEXSI](http://cert.lexsi.com/), [VUPEN Vulnerability Research Team](http://www.vupen.com/), valamint a Vulnerability Research Team, [TELUS Security Labs](http://telussecuritylabs.com/), [Core Security Technologies](http://www.coresecurity.com/) és az [NSFOCUS Security Team](http://www.nsfocus.com/), az együttműködésért, és az MS10-025 eredeti biztonsági frissítésével kapcsolatos minőségi probléma részletezéséért
-   Yamata Li ([Palo Alto Networks](http://www.paloaltonetworks.com/)) az MS10-026 közleményben ismertetett probléma jelentéséért
-   A [Tipping Point](http://www.tippingpoint.com/) és [Zero Day Initiative](http://www.zerodayinitiative.com/) programban résztvevő anonim kutató, az MS10-027 közleményben leírt egyik probléma jelentéséért
-   Bing Liu, [Fortinet FortiGuard Labs](http://www.fortiguard.com/), az MS10-028 közleményben ismertetett két probléma jelentéséért
-   Gabi Nakibly, National EW Research & Simulation Center, Rafael, az MS10-029 közleményben leírt probléma jelentéséért

#### Terméktámogatás

-   Teszteléssel állapították meg a felsorolt szoftverek egyes verzióinak érintettségét. A többi verzió támogatási életciklusa végére ért. Az egyes szoftververziók támogatási életciklusáról a [Microsoft termékek terméktámogatási életciklusát ismertető webhelyen](http://go.microsoft.com/fwlink/?linkid=21742) talál felvilágosítást.
-   Az Amerikai Egyesült Államokban és Kanada területén élő ügyfelek technikai támogatást kérhetnek a [biztonsági támogatás szolgáltatójától](http://go.microsoft.com/fwlink/?linkid=21131) vagy az 1-866-PCSAFETY telefonszámon. A biztonsági frissítésekkel kapcsolatos hívások ingyenesek. Az elérhető támogatási lehetőségekről további információt talál a [Microsoft segítségnyújtással és támogatással foglalkozó webhelyén](http://support.microsoft.com/).
-   Más országokban a helyi Microsoft-képviseletek nyújtanak támogatást. A biztonsági frissítésekkel kapcsolatos hívások ingyenesek. A [nemzetközi támogatási webhely](http://go.microsoft.com/fwlink/?linkid=21155) felvilágosítást nyújt arról, támogatási kérdéseivel hogyan fordulhat a Microsofthoz.

#### Felelősséget kizáró nyilatkozat

A Microsoft Tudásbázisban leírtak előzetes bejelentés nélkül változhatnak, és a cikkek tartalmáért a Microsoft nem vállal garanciát. A Microsoft egyben elhárít minden kifejezett és értelemszerű garanciát, beleértve az eladhatóságra és az adott célra való alkalmasságra vonatkozó garanciát is. A Microsoft Corporation vagy annak szállítói semmilyen körülmények között nem tehetők felelőssé közvetlen, közvetett, eseti, ok-okozati vagy különleges kárért (beleértve az elmaradt hasznot is), még akkor sem, ha a Microsoft Corporation vagy szállítói tudatában voltak a kár lehetséges voltának. Egyes államok törvényi szabályozása nem teszi lehetővé a véletlen vagy ok-okozati károkért vállalt felelősség korlátozását vagy kizárását, így ezekben az államokban az ez a felelősségkizárás nincs érvényben.

#### Verziók

-   1.0 verzió (2010. április 13.): Összefoglaló közlemény közzététele.
-   1.1 verzió (2010. április 14.): Az MS10-025 **összefoglaló részében** javítottuk az újraindítás feltételeit. Módosult a kiszolgálómaggal kapcsolatos tájékoztatás a Windows Server 2008 és Windows Server 2008 R2 rendszer vonatkozásában; csak az MS10-019 közlemény KB978601 frissítését kell alkalmazni.
-   2.0 verzió (2010. április 21.): A frissítés tájékoztatja a felhasználókat, hogy az eredeti biztonsági frissítés (MS10-025) nem védte a rendszerüket a jelen közleményben leírt biztonsági réstől. A Microsoft javasolja az MS10-025 közleményben tárgyalt megoldások valamelyikének alkalmazását az érintett rendszerek védelme érdekében, addig is, amíg ki nem adják az új biztonsági frissítést.
-   3.0 verzió (2010. április 27.): Az MS10-025 közleményhez újra kiadott biztonsági frissítést kínál fel.
-   4.0 verzió (2010. július 13.): A javított közlemény a Windows Server 2008 és a Windows Server 2008 R2 rendszerekhez tartalmaz ismételten kiadott biztonsági frissítést az MS10-024 közlemény vonatkozásában.

*Built at 2014-04-18T01:50:00Z-07:00*
