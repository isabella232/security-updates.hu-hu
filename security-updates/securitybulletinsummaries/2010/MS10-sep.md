---
TOCTitle: 'MS10-SEP'
Title: 'Microsoft biztonsági közlemény - összefoglalás, 2010. szeptember'
ms:assetid: 'ms10-sep'
ms:contentKeyID: 61227749
ms:mtpsurl: 'https://technet.microsoft.com/hu-HU/library/ms10-sep(v=Security.10)'
author: SharonSears
ms.author: SharonSears
---

Security Bulletin Summary

Microsoft biztonsági közlemény - összefoglalás, 2010. szeptember
================================================================

Közzétéve: 2010. szeptember 14. | Frissítve: 2011. október 26.

**Verzió:** 6.1

Az összefoglaló a 2010. szeptemberében kiadott biztonsági közleményeket összegzi.

A 2010. szeptemberi közlemények kiadása folytán az összefoglaló a 2010. szeptember 9-én kiadott előzetes értesítés helyébe lép. További információk a biztonsági közlemények kiadásáról szóló előzetes értesítés szolgáltatásról lásd: [Előzetes értesítés a Microsoft biztonsági közleményeinek kiadásáról](http://technet.microsoft.com/security/bulletin/advance).

Ha automatikus értesítést szeretne kapni a Microsoft biztonsági közleményeinek megjelenéséről, fizessen elő a [Microsoft Technical Security Notifications](http://go.microsoft.com/fwlink/?linkid=21163) szolgáltatásra.

A közleményekkel kapcsolatos kérdések megválaszolására a Microsoft 2010. szeptember 15-én, csendes-óceáni idő szerint 11 órakor webes szemináriumot tart. [Jelentkezzen most a szeptemberi közleményeket bemutató webes szemináriumra](https://msevents.microsoft.com/cui/webcasteventdetails.aspx?eventid=1032454433&eventcategory=4&culture=en-us&countrycode=us). Ezt követően a webes szeminárium igény szerint kerül megrendezésre. További információkért látogasson el a [Microsoft biztonsági közleményeit és a webes szemináriumokat](http://technet.microsoft.com/security/bulletin/summary) bemutató oldalra.

Az összefoglaló közlemény 3.0 verzióját kiegészítő, rendkívüli biztonsági közleménnyel (MS10-070) kapcsolatos kérdések megválaszolására a Microsoft 2010. szeptember 28-án, csendes-óceáni idő szerint 13 órakor webes szemináriumot tart. [Jelentkezzen most a szeptember 28-án 13 órakor tartandó szemináriumra](https://msevents.microsoft.com/cui/eventdetail.aspx?eventid=1032464130&culture=en-us). Ezt követően a webes szeminárium igény szerint kerül megrendezésre. További információkért látogasson el a Microsoft biztonsági közleményeit és a webes szemináriumokat bemutató oldalra.

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
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=200505">MS10-061</a></td>
<td style="border:1px solid black;"><strong>A nyomtatásisor-kezelő szolgáltatás biztonsági rése távoli kódfuttatást tehet lehetővé (2347290)</strong><br />
<br />
Ez a biztonsági frissítés a Nyomtatásisor-kezelő szolgáltatás nyilvánosan jelentett biztonsági rését szünteti meg. A biztonsági rés távoli kódfuttatást tehet lehetővé, ha a támadó egy különlegesen kialakított nyomtatási kérelmet küld egy érintett rendszerre, aminek nyomtatásisor-kezelő felülete az RPC-n keresztül sebezhető. Alapesetben a nyomtatók nincsenek megosztva a jelenleg támogatott Windows operációs rendszereken.</td>
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=21140">Kritikus</a><br />
Távoli kódfuttatás</td>
<td style="border:1px solid black;">Újraindítást igényel</td>
<td style="border:1px solid black;">Microsoft Windows</td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=190884">MS10-062</a></td>
<td style="border:1px solid black;"><strong>Az MPEG-4 kodek biztonsági rése távolról történő kódfuttatást tehet lehetővé (975558)</strong><br />
<br />
A biztonsági frissítés az MPEG-4 kodek közvetlenül jelentett biztonsági rését szünteti meg. A biztonsági rések távoli kódfuttatást tehetnek lehetővé, ha a felhasználó megnyit egy különlegesen kialakított médiafájlt, vagy különlegesen kialakított tartalom-adatfolyamot fogad egy webhelyről, illetve bármely webes tartalmat szállító alkalmazásból. A biztonsági rést kihasználó támadó a helyi felhasználóval egyező hozzáférést nyer a rendszerhez. A kevesebb jogosultsággal bíró fiókkal rendelkező felhasználók esetében kisebb a veszélyeztetettség, mint a rendszergazdai jogosultságokkal rendelkezők esetén</td>
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=21140">Kritikus</a><br />
Távoli kódfuttatás</td>
<td style="border:1px solid black;">Esetleg újra kell indítani a rendszert</td>
<td style="border:1px solid black;">Microsoft Windows</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=200378">MS10-063</a></td>
<td style="border:1px solid black;"><strong>A Unicode Scripts Processor biztonsági rése távolról történő kódfuttatást okozhat (2320113)</strong><br />
<br />
Ez a biztonsági frissítés a Unicode Scripts Processor közvetlenül jelentett biztonsági rését szünteti meg. A biztonsági rés távoli kódfuttatást tehet lehetővé, ha a felhasználó megtekint egy különlegesen kialakított dokumentumot vagy webhelyet egy olyan alkalmazással, ami támogatja a beágyazott OpenType (EOT) betűtípusokat. A biztonsági rést kihasználó támadó a helyi felhasználóval egyező hozzáférést nyer a rendszerhez. A kevesebb jogosultsággal bíró fiókkal rendelkező felhasználók esetében kisebb a veszélyeztetettség, mint a rendszergazdai jogosultságokkal rendelkezők esetén</td>
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=21140">Kritikus</a><br />
Távoli kódfuttatás</td>
<td style="border:1px solid black;">Esetleg újra kell indítani a rendszert</td>
<td style="border:1px solid black;">Microsoft Windows, Microsoft Office</td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=200727">MS10-064</a></td>
<td style="border:1px solid black;"><strong>A Microsoft Outlook biztonsági rése távoli kódfuttatást tehet lehetővé (2315011)</strong><br />
<br />
Ez a biztonsági frissítés egy közvetlenül jelzett biztonsági rést szüntet meg. A biztonsági rés lehetővé teheti a távoli kódfuttatást, ha a felhasználó megnyit vagy előnézetben megtekint egy speciálisan kialakított e-mail üzenetet a Microsoft Outlook azon érintett verziójával, ami az Exchange szerverhez Online módban csatlakozik. A biztonsági rést kihasználó támadó a helyi felhasználóval egyező hozzáférést nyer a rendszerhez. A kevesebb jogosultsággal bíró fiókkal rendelkező felhasználók esetében kisebb a veszélyeztetettség, mint a rendszergazdai jogosultságokkal rendelkezők esetén</td>
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=21140">Kritikus</a><br />
Távoli kódfuttatás</td>
<td style="border:1px solid black;">Esetleg újra kell indítani a rendszert</td>
<td style="border:1px solid black;">Microsoft Office</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=199537">MS10-065</a></td>
<td style="border:1px solid black;"><strong>A Microsoft</strong> <strong>Internet Information Services (IIS) biztonsági rése távolról történő kódfuttatást tehet lehetővé (2267960)</strong><br />
<br />
A biztonsági frissítés kettő közvetlenül és egy nyilvánosan jelentett biztonsági rést szüntet meg az Internet Information Services (IIS) programban. A biztonsági rések közül a legsúlyosabbak távoli kódfuttatást tehetnek lehetővé, ha az ügyfél egy különlegesen kialakított HTTP kérelmet küld a szerverre. Ha egy támadó kihasználja a biztonsági rést, teljes mértékben átveheti a rendszer irányítását.</td>
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=21140">Fontos</a><br />
Távoli kódfuttatás</td>
<td style="border:1px solid black;">Esetleg újra kell indítani a rendszert</td>
<td style="border:1px solid black;">Microsoft Windows</td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=197105">MS10-066</a></td>
<td style="border:1px solid black;"><strong>A Távoli eljáráshívás (RPC) biztonsági rése távoli kódfuttatást tehet lehetővé (982802)</strong><br />
<br />
A biztonsági frissítés a Microsoft Windows közvetlenül jelentett biztonsági rését szünteti meg. A biztonsági frissítés a Windows XP és Windows Server 2003 összes támogatott kiadására nézve Fontos besorolású. A Windows Vista, Windows Server 2008, Windows 7 és Windows Server 2008 R2 támogatott kiadásait nem érinti a biztonsági rés okozta probléma.<br />
<br />
A biztonsági rés távolról történő kódfuttatást tehet lehetővé, ha a támadó speciálisan kialakított RPC választ küld az ügyfél által kezdeményezett RPC kérelemre. Ha egy támadó kihasználja a biztonsági rést, távolról mesterséges kódot futtathat és teljes mértékben átveheti az érintett rendszer irányítását. A támadónak meg kell győznie a felhasználót, hogy kezdeményezzen RPC kapcsolatot a támadó irányítása alatt álló rosszindulatú kiszolgálóval. A támadó távolról nem tudja kihasználni ezt a biztonsági rést a felhasználó közreműködése nélkül.</td>
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=21140">Fontos</a><br />
Távoli kódfuttatás</td>
<td style="border:1px solid black;">Újraindítást igényel</td>
<td style="border:1px solid black;">Microsoft Windows</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=197102">MS10-067</a></td>
<td style="border:1px solid black;"><strong>A WordPad szövegkonverterek biztonsági rése távolról történő programkódfuttatást tehet lehetővé (2259922)</strong><br />
<br />
A biztonsági frissítés a Microsoft Windows közvetlenül jelentett biztonsági rését szünteti meg. A biztonsági frissítés a Windows XP és Windows Server 2003 összes támogatott kiadására nézve Fontos besorolású. A Windows Vista, Windows Server 2008, Windows 7 és Windows Server 2008 R2 támogatott kiadásait nem érinti a biztonsági rés okozta probléma.<br />
<br />
A biztonsági rés távoli kódvégrehajtást tehet lehetővé, ha a felhasználó megnyit egy speciálisan kialakított fájlt a WordPad-del. A biztonsági rést kihasználó támadó a helyi felhasználóval egyező hozzáférést nyer a rendszerhez. A kevesebb jogosultsággal bíró fiókkal rendelkező felhasználók esetében kisebb a veszélyeztetettség, mint a rendszergazdai jogosultságokkal rendelkezők esetén</td>
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=21140">Fontos</a><br />
Távoli kódfuttatás</td>
<td style="border:1px solid black;">Esetleg újra kell indítani a rendszert</td>
<td style="border:1px solid black;">Microsoft Windows</td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=190509">MS10-068</a></td>
<td style="border:1px solid black;"><strong>A helyi biztonsági szervezet szolgáltatás (LSASS) biztonsági rése szolgáltatásmegtagadást okozhat (983539)</strong><br />
<br />
A biztonsági frissítés az Active Directory, az Alkalmazásmódú Active Directory (ADAM) és az Active Directory Lightweight Directory-szolgáltatás (AD LDS) közvetlenül jelentett biztonsági rését szünteti meg. A biztonsági rés lehetővé teheti a jogok kiterjesztését, ha egy hitelesített támadó elküld egy speciálisan kialakított Lightweight Directory elérési protokoll (LDAP) üzenetet egy figyelő LSASS-kiszolgálóra. Ennek a biztonsági résnek a sikeres kihasználásához a támadónak felhasználói fiókkal kell rendelkeznie a megcélzott Windows tartományban. A támadónak nem kell azonban munkaállomásával csatlakoznia a Windows tartományhoz.</td>
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=21140">Fontos</a><br />
Jogok kiterjesztése</td>
<td style="border:1px solid black;">Újraindítást igényel</td>
<td style="border:1px solid black;">Microsoft Windows</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=197093">MS10-069</a></td>
<td style="border:1px solid black;"><strong>A Windows futásidejű ügyfélkiszolgáló alrendszerének biztonsági rése jogok kiterjesztését teheti lehetővé (2121546)</strong><br />
<br />
A biztonsági frissítés a Microsoft Windows közvetlenül jelentett biztonsági rését szünteti meg. A biztonsági frissítés a Windows XP és Windows Server 2003 összes támogatott kiadására nézve Fontos besorolású. A Windows Vista, Windows Server 2008, Windows 7 és Windows Server 2008 R2 támogatott kiadásait nem érinti a biztonsági rés okozta probléma.<br />
<br />
A biztonsági rés lehetővé teheti jogok terjesztését, ha a támadó belép egy érintett rendszerbe, aminek területbeállítási konfigurációja kínai, japán vagy koreai. A biztonsági rést sikeresen kihasználó támadó programokat telepíthet, illetve adatokat tekinthet meg, módosíthat és törölhet, de korlátozás nélküli jogosultságokkal rendelkező új fiókokat is létrehozhat.</td>
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=21140">Fontos</a><br />
Jogok kiterjesztése</td>
<td style="border:1px solid black;">Újraindítást igényel</td>
<td style="border:1px solid black;">Microsoft Windows</td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=202409">MS10-070</a></td>
<td style="border:1px solid black;"><strong>Az ASP.NET biztonsági rése adatokhoz való illetéktelen hozzáférést tehet lehetővé (2418042)</strong><br />
<br />
A biztonsági frissítés az ASP.NET nyilvánosan jelentett biztonsági rését szünteti meg. A biztonsági rés adatokhoz való illetéktelen hozzáférést okozhat. A biztonsági rést sikeresen kihasználó támadó elolvashatja a kiszolgáló által titkosított adatokat, például a nézetállapotot. A biztonsági rés az adatok módosítására is használható, amit sikeresen kihasználva a támadó visszafejtheti és módosíthatja a kiszolgáló által titkosított adatokat. A biztonsági rés fájltartalomhoz történő hozzáférésre vonatkozó része a Microsoft .NET-keretrendszer 3.5 Service Pack 1 előtti verzióit nem érinti.</td>
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=21140">Fontos</a><br />
Adatokhoz való illetéktelen hozzáférés</td>
<td style="border:1px solid black;">Esetleg újra kell indítani a rendszert</td>
<td style="border:1px solid black;">Microsoft Windows, Microsoft .NET Framework</td>
</tr>
</tbody>
</table>
  
Kihasználhatósági információk  
-----------------------------
  
<span></span>
A következő táblázat az adott hónapban megoldott biztonsági rések kihasználhatósági jellemzőit ismerteti. A biztonsági rések a kihasználhatósági kockázat, majd a CVE azonosító szerint vannak felsorolva. Csak a kritikus és fontos besorolású biztonsági rések szerepelnek.
  
**A táblázat használata**
  
A táblázat segítségével meghatározható annak valószínűsége, hogy a biztonsági közlemény kiadását követő 30 napon belül a telepíteni szükséges biztonsági frissítésekre működő rosszindulatú programkódot jelentetnek meg. A telepítés fontossági sorrendjének megállapításához az adott konfigurációnak megfelelően tekintse át az alábbi értékeléseket. A minősítések jelentéséről és meghatározásuk módjáról a [Microsoft kihasználhatósági információk](http://technet.microsoft.com/en-us/security/cc998259.aspx) című rész tartalmaz bővebb információt.
  
| Közlemény azonosítója                                     | A biztonsági rés címe                                                              | CVE-azonosító                                                                    | Kihasználhatósági információk értékelése                                                                                 | Fontos megjegyzések                                                                                       |  
|-----------------------------------------------------------|------------------------------------------------------------------------------------|----------------------------------------------------------------------------------|--------------------------------------------------------------------------------------------------------------------------|-----------------------------------------------------------------------------------------------------------|  
| [MS10-062](http://go.microsoft.com/fwlink/?linkid=190884) | MPEG-4 kodek biztonsági rése                                                       | [CVE-2010-0818](http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2010-0818) | [**1**](http://technet.microsoft.com/en-us/security/cc998259.aspx) - Valószínűleg konzisztens rosszindulatú programkód   | A kódfuttatás kevésbé valószínű Windows Vista rendszerben. Ez a kiegészítő halommegoldásoknak köszönhető. |  
| [MS10-068](http://go.microsoft.com/fwlink/?linkid=190509) | LSASS halomtúlcsordulást okozó biztonsági rése                                     | [CVE-2010-0820](http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2010-0820) | [**1**](http://technet.microsoft.com/en-us/security/cc998259.aspx) - Valószínűleg konzisztens rosszindulatú programkód   | (Nincs)                                                                                                   |  
| [MS10-069](http://go.microsoft.com/fwlink/?linkid=197093) | A CSRSS jogok helyi kiterjesztését eredményező biztonsági rése                     | [CVE-2010-1891](http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2010-1891) | [**1**](http://technet.microsoft.com/en-us/security/cc998259.aspx) - Valószínűleg konzisztens rosszindulatú programkód   | (Nincs)                                                                                                   |  
| [MS10-067](http://go.microsoft.com/fwlink/?linkid=197102) | A WordPad Word 97 szövegkonverter okozta memóriameghibásodás miatti biztonsági rés | [CVE-2010-2563](http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2010-2563) | [**1**](http://technet.microsoft.com/en-us/security/cc998259.aspx) - Valószínűleg konzisztens rosszindulatú programkód   | (Nincs)                                                                                                   |  
| [MS10-066](http://go.microsoft.com/fwlink/?linkid=197105) | Az RPC memóriameghibásodást okozó biztonsági rése                                  | [CVE-2010-2567](http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2010-2567) | [**1**](http://technet.microsoft.com/en-us/security/cc998259.aspx) - Valószínűleg konzisztens rosszindulatú programkód   | (Nincs)                                                                                                   |  
| [MS10-061](http://go.microsoft.com/fwlink/?linkid=200505) | A nyomtatásisor-kezelő megszemélyesítési biztonsági rése                           | [CVE-2010-2729](http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2010-2729) | [**1**](http://technet.microsoft.com/en-us/security/cc998259.aspx) - Valószínűleg konzisztens rosszindulatú programkód   | **A biztonsági rést jelenleg internetszerte kihasználják**                                                |  
| [MS10-070](http://go.microsoft.com/fwlink/?linkid=202409) | ASP.NET „padding oracle” biztonsági rése                                           | [CVE-2010-3332](http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2010-3332) | [**1**](http://technet.microsoft.com/en-us/security/cc998259.aspx) - Valószínűleg konzisztens rosszindulatú programkód   | **A biztonsági rést jelenleg internetszerte kihasználják**                                                |  
| [MS10-065](http://go.microsoft.com/fwlink/?linkid=199537) | Címtár hitelesítést megkerülő biztonsági rés                                       | [CVE-2010-2731](http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2010-2731) | [**1**](http://technet.microsoft.com/en-us/security/cc998259.aspx) - Valószínűleg konzisztens rosszindulatú programkód   | **A biztonsági rés nyilvánosságra került**                                                                |  
| [MS10-063](http://go.microsoft.com/fwlink/?linkid=200378) | A Uniscribe betűtípus-elemző memória-meghibásodás okozta biztonsági rése           | [CVE-2010-2738](http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2010-2738) | [**1**](http://technet.microsoft.com/en-us/security/cc998259.aspx) - Valószínűleg konzisztens rosszindulatú programkód   | (Nincs)                                                                                                   |  
| [MS10-064](http://go.microsoft.com/fwlink/?linkid=200727) | Az Outlook Halommemórián alapuló puffertúlcsordulási biztonsági rése               | [CVE-2010-2728](http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2010-2728) | [**2**](http://technet.microsoft.com/en-us/security/cc998259.aspx) - Valószínűleg inkonzisztens rosszindulatú programkód | (Nincs)                                                                                                   |  
| [MS10-065](http://go.microsoft.com/fwlink/?linkid=199537) | Kérelemfejléc puffertúlcsordulási biztonsági rése                                  | [CVE-2010-2730](http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2010-2730) | [**2**](http://technet.microsoft.com/en-us/security/cc998259.aspx) - Valószínűleg inkonzisztens rosszindulatú programkód | (Nincs)                                                                                                   |  
| [MS10-065](http://go.microsoft.com/fwlink/?linkid=199537) | IIS ismételt paraméter kérelem szolgáltatásmegtagadási biztonsági rés              | [CVE-2010-1899](http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2010-1899) | [**3**](http://technet.microsoft.com/en-us/security/cc998259.aspx) - Nem valószínű működő rosszindulatú programkód       | A hiba csak szolgáltatásmegtagadást okoz                                                                  |
  
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
Windows XP  
</th>
</tr>
<tr>
<td style="border:1px solid black;">
**Közlemény** **azonosítója**
</td>
<td style="border:1px solid black;">
[**MS10-061**](http://go.microsoft.com/fwlink/?linkid=200505)
</td>
<td style="border:1px solid black;">
[**MS10-062**](http://go.microsoft.com/fwlink/?linkid=190884)
</td>
<td style="border:1px solid black;">
[**MS10-063**](http://go.microsoft.com/fwlink/?linkid=200378)
</td>
<td style="border:1px solid black;">
[**MS10-065**](http://go.microsoft.com/fwlink/?linkid=199537)
</td>
<td style="border:1px solid black;">
[**MS10-066**](http://go.microsoft.com/fwlink/?linkid=197105)
</td>
<td style="border:1px solid black;">
[**MS10-067**](http://go.microsoft.com/fwlink/?linkid=197102)
</td>
<td style="border:1px solid black;">
[**MS10-068**](http://go.microsoft.com/fwlink/?linkid=190509)
</td>
<td style="border:1px solid black;">
[**MS10-069**](http://go.microsoft.com/fwlink/?linkid=197093)
</td>
<td style="border:1px solid black;">
[**MS10-070**](http://go.microsoft.com/fwlink/?linkid=202409)
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
</tr>
<tr>
<td style="border:1px solid black;">
Windows XP Service Pack 3
</td>
<td style="border:1px solid black;">
[Windows XP Service Pack 3](http://www.microsoft.com/downloads/details.aspx?familyid=93faba6b-0a85-4acc-b527-a012bbf56b13)  
(Kritikus)
</td>
<td style="border:1px solid black;">
[Windows XP Service Pack 3](http://www.microsoft.com/downloads/details.aspx?familyid=2084a01c-2a91-4650-8665-7053015f2083)  
(Kritikus)
</td>
<td style="border:1px solid black;">
[Windows XP Service Pack 3](http://www.microsoft.com/downloads/details.aspx?familyid=a1d47f30-c1fc-4b9d-8829-3bad1224006a)  
(KB981322)  
(Kritikus)
</td>
<td style="border:1px solid black;">
IIS ASP:  
[Internet Information Services 5.1](http://www.microsoft.com/downloads/details.aspx?familyid=555864c3-9114-4988-8526-7bf545a27706)  
(KB2124261)  
(Fontos)  
IIS hitelesítés:  
[Internet Information Services 5.1](http://www.microsoft.com/downloads/details.aspx?familyid=ae55787e-4a5c-48d5-aedf-0abada514938)  
(KB2290570)  
(Fontos)
</td>
<td style="border:1px solid black;">
[Windows XP Service Pack 3](http://www.microsoft.com/downloads/details.aspx?familyid=7ad0f2cf-03dc-49a0-a16e-17fed0c01cc6)  
(Fontos)
</td>
<td style="border:1px solid black;">
[Windows XP Service Pack 3](http://www.microsoft.com/downloads/details.aspx?familyid=fc4369ec-864a-42ae-a850-b006872241fe)  
(Fontos)
</td>
<td style="border:1px solid black;">
[Alkalmazásmódú Active Directory (ADAM)](http://www.microsoft.com/downloads/details.aspx?familyid=6554f98f-4dc5-4784-b92c-b0aae1fa22ca)  
(KB982000)  
(Fontos)
</td>
<td style="border:1px solid black;">
[Windows XP Service Pack 3](http://www.microsoft.com/downloads/details.aspx?familyid=20091358-7127-4ace-bf96-4319461ad305)  
(Fontos)
</td>
<td style="border:1px solid black;">
[Microsoft .NET-keretrendszer 1.1 Service Pack 1](http://www.microsoft.com/downloads/details.aspx?familyid=a7990e61-21fd-4942-9dfe-af7961cb0282)  
(KB2416447)  
(Fontos)  
[Microsoft .NET-keretrendszer 2.0 Service Pack 2 és Microsoft .NET-keretrendszer 3.5 Service Pack 1](http://www.microsoft.com/downloads/details.aspx?familyid=3d31fd37-eb58-4169-b6b9-4cf854524e46)  
(KB2418241)  
(Fontos)  
[Microsoft .NET-keretrendszer 3.5](http://www.microsoft.com/downloads/details.aspx?familyid=d284237b-e4d9-460a-98f0-7a18252f5780)  
(KB2416468)  
(Fontos)  
[Microsoft .NET-keretrendszer 3.5](http://www.microsoft.com/downloads/details.aspx?familyid=00d95a85-f3e8-464d-a10c-85c6d91b4aae)  
(KB2418240)  
(Fontos)  
[Microsoft .NET-keretrendszer 3.5 Service Pack 1](http://www.microsoft.com/downloads/details.aspx?familyid=ae42d6cc-6d4e-425a-9b4f-379f66fc506a)  
(KB2416473)  
(Fontos)  
[Microsoft .NET-keretrendszer 4.0](http://www.microsoft.com/downloads/details.aspx?familyid=6ce703b7-08a5-4eff-a062-d5dc720908f6)<sup>[1]</sup>
(KB2416472)  
(Fontos)
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
Windows XP Professional x64 Edition Service Pack 2
</td>
<td style="border:1px solid black;">
[Windows XP Professional x64 Edition Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=9f7f3737-056d-44bd-b644-51093b5b501b)  
(Kritikus)
</td>
<td style="border:1px solid black;">
[Windows XP Professional x64 Edition Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=284a0e80-fd03-4909-b354-0478f04585a1)  
(Kritikus)
</td>
<td style="border:1px solid black;">
[Windows XP Professional x64 Edition Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=b27f310f-6ecc-4abb-8944-9fc24c66e077)  
(KB981322)  
(Kritikus)
</td>
<td style="border:1px solid black;">
IIS ASP:  
[Internet Information Services 6.0](http://www.microsoft.com/downloads/details.aspx?familyid=0b28bfac-783d-4c89-988b-4123c0343855)  
(KB2124261)  
(Fontos)
</td>
<td style="border:1px solid black;">
[Windows XP Professional x64 Edition Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=3349b12b-621e-48bc-9c57-489c7a56920d)  
(Fontos)
</td>
<td style="border:1px solid black;">
[Windows XP Professional x64 Edition Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=7567986a-261d-4def-9fa5-c667994c7844)  
(Fontos)
</td>
<td style="border:1px solid black;">
[Alkalmazásmódú Active Directory (ADAM)](http://www.microsoft.com/downloads/details.aspx?familyid=5bc00f9a-3028-4c9d-be06-f2b78fa444c4)  
(KB982000)  
(Fontos)
</td>
<td style="border:1px solid black;">
[Windows XP Professional x64 Edition Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=107eb958-b60f-40ae-a785-5d5b4d13d8c6)  
(Fontos)
</td>
<td style="border:1px solid black;">
[Microsoft .NET-keretrendszer 1.1 Service Pack 1](http://www.microsoft.com/downloads/details.aspx?familyid=a7990e61-21fd-4942-9dfe-af7961cb0282)  
(KB2416447)  
(Fontos)  
[Microsoft .NET-keretrendszer 2.0 Service Pack 2 és Microsoft .NET-keretrendszer 3.5 Service Pack 1](http://www.microsoft.com/downloads/details.aspx?familyid=3d31fd37-eb58-4169-b6b9-4cf854524e46)  
(KB2418241)  
(Fontos)  
[Microsoft .NET-keretrendszer 3.5](http://www.microsoft.com/downloads/details.aspx?familyid=d284237b-e4d9-460a-98f0-7a18252f5780)  
(KB2416468)  
(Fontos)  
[Microsoft .NET-keretrendszer 3.5](http://www.microsoft.com/downloads/details.aspx?familyid=00d95a85-f3e8-464d-a10c-85c6d91b4aae)  
(KB2418240)  
(Fontos)  
[Microsoft .NET-keretrendszer 3.5 Service Pack 1](http://www.microsoft.com/downloads/details.aspx?familyid=ae42d6cc-6d4e-425a-9b4f-379f66fc506a)  
(KB2416473)  
(Fontos)  
[Microsoft .NET-keretrendszer 4.0](http://www.microsoft.com/downloads/details.aspx?familyid=6ce703b7-08a5-4eff-a062-d5dc720908f6)<sup>[1]</sup>
(KB2416472)  
(Fontos)
</td>
</tr>
<tr>
<th colspan="10">
Windows Server 2003
</th>
</tr>
<tr>
<td style="border:1px solid black;">
**Közlemény azonosítója**
</td>
<td style="border:1px solid black;">
[**MS10-061**](http://go.microsoft.com/fwlink/?linkid=200505)
</td>
<td style="border:1px solid black;">
[**MS10-062**](http://go.microsoft.com/fwlink/?linkid=190884)
</td>
<td style="border:1px solid black;">
[**MS10-063**](http://go.microsoft.com/fwlink/?linkid=200378)
</td>
<td style="border:1px solid black;">
[**MS10-065**](http://go.microsoft.com/fwlink/?linkid=199537)
</td>
<td style="border:1px solid black;">
[**MS10-066**](http://go.microsoft.com/fwlink/?linkid=197105)
</td>
<td style="border:1px solid black;">
[**MS10-067**](http://go.microsoft.com/fwlink/?linkid=197102)
</td>
<td style="border:1px solid black;">
[**MS10-068**](http://go.microsoft.com/fwlink/?linkid=190509)
</td>
<td style="border:1px solid black;">
[**MS10-069**](http://go.microsoft.com/fwlink/?linkid=197093)
</td>
<td style="border:1px solid black;">
[**MS10-070**](http://go.microsoft.com/fwlink/?linkid=202409)
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
</tr>
<tr>
<td style="border:1px solid black;">
Windows Server 2003 Service Pack 2
</td>
<td style="border:1px solid black;">
[Windows Server 2003 Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=3d79680b-c071-462f-9cea-551fbd42edf0)  
(Fontos)
</td>
<td style="border:1px solid black;">
[Windows Server 2003 Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=0a942985-081f-455c-bf9d-4345392c91b0)  
(Kritikus)
</td>
<td style="border:1px solid black;">
[Windows Server 2003 Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=7ff7de2f-3e37-4aff-a8e4-5ed21b83575c)  
(KB981322)  
(Kritikus)
</td>
<td style="border:1px solid black;">
IIS ASP:  
[Internet Information Services 6.0](http://www.microsoft.com/downloads/details.aspx?familyid=29e6cf4f-446b-461c-82f7-cfa8478cf739)  
(KB2124261)  
(Fontos)
</td>
<td style="border:1px solid black;">
[Windows Server 2003 Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=f8b3004b-07db-4638-a9b7-224ff829081c)  
(Fontos)
</td>
<td style="border:1px solid black;">
[Windows Server 2003 Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=3290e7ee-1e4a-464c-abfd-17fc4108601e)  
(Fontos)
</td>
<td style="border:1px solid black;">
[Active Directory](http://www.microsoft.com/downloads/details.aspx?familyid=3fe6e78c-c60a-4903-9273-27b37e129f0a)  
(KB981550)  
(Fontos)  
[Alkalmazásmódú Active Directory (ADAM)](http://www.microsoft.com/downloads/details.aspx?familyid=c42731f1-6393-42ed-b59f-5310c832fdc4)  
(KB982000)  
(Fontos)
</td>
<td style="border:1px solid black;">
[Windows Server 2003 Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=fd46ba66-8ca1-4aa2-b91b-9e5861a173f7)  
(Fontos)
</td>
<td style="border:1px solid black;">
[Microsoft .NET-keretrendszer 1.1 Service Pack 1](http://www.microsoft.com/downloads/details.aspx?familyid=71f0daad-e2df-421c-9818-58e1e40cdb65)  
(KB2416451)  
(Fontos)  
[Microsoft .NET-keretrendszer 2.0 Service Pack 2 és Microsoft .NET-keretrendszer 3.5 Service Pack 1](http://www.microsoft.com/downloads/details.aspx?familyid=3d31fd37-eb58-4169-b6b9-4cf854524e46)  
(KB2418241)  
(Fontos)  
[Microsoft .NET-keretrendszer 3.5](http://www.microsoft.com/downloads/details.aspx?familyid=d284237b-e4d9-460a-98f0-7a18252f5780)  
(KB2416468)  
(Fontos)  
[Microsoft .NET-keretrendszer 3.5](http://www.microsoft.com/downloads/details.aspx?familyid=00d95a85-f3e8-464d-a10c-85c6d91b4aae)  
(KB2418240)  
(Fontos)  
[Microsoft .NET-keretrendszer 3.5 Service Pack 1](http://www.microsoft.com/downloads/details.aspx?familyid=ae42d6cc-6d4e-425a-9b4f-379f66fc506a)  
(KB2416473)  
(Fontos)  
[Microsoft .NET-keretrendszer 4.0](http://www.microsoft.com/downloads/details.aspx?familyid=6ce703b7-08a5-4eff-a062-d5dc720908f6)<sup>[1]</sup>
(KB2416472)  
(Fontos)
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
Windows Server 2003 x64 Edition Service Pack 2
</td>
<td style="border:1px solid black;">
[Windows Server 2003 x64 Edition Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=073b3305-4a81-4ef8-b6aa-e53b31a936b4)  
(Fontos)
</td>
<td style="border:1px solid black;">
[Windows Server 2003 x64 Edition Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=284a0e80-fd03-4909-b354-0478f04585a1)  
(Kritikus)
</td>
<td style="border:1px solid black;">
[Windows Server 2003 x64 Edition Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=8382c1f2-e16d-475c-a8a0-e378696808f1)  
(KB981322)  
(Kritikus)
</td>
<td style="border:1px solid black;">
IIS ASP:  
[Internet Information Services 6.0](http://www.microsoft.com/downloads/details.aspx?familyid=750e4a79-11bf-4726-9eb4-5dd3d029a717)  
(KB2124261)  
(Fontos)
</td>
<td style="border:1px solid black;">
[Windows Server 2003 x64 Edition Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=612b2096-bd82-47ca-8b99-454c2f158d39)  
(Fontos)
</td>
<td style="border:1px solid black;">
[Windows Server 2003 x64 Edition Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=b21570cc-4f90-4ed8-b901-a34584d44a63)  
(Fontos)
</td>
<td style="border:1px solid black;">
[Active Directory](http://www.microsoft.com/downloads/details.aspx?familyid=22412eed-33cd-4dfc-8ef7-b74dcd7c5faf)  
(KB981550)  
(Fontos)  
[Alkalmazásmódú Active Directory (ADAM)](http://www.microsoft.com/downloads/details.aspx?familyid=79fb639d-2cc1-4bea-9df6-c67ed95890e3)  
(KB982000)  
(Fontos)
</td>
<td style="border:1px solid black;">
[Windows Server 2003 x64 Edition Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=ff5976e0-579c-4e6e-a225-c0d3913cdc85)  
(Fontos)
</td>
<td style="border:1px solid black;">
[Microsoft .NET-keretrendszer 1.1 Service Pack 1](http://www.microsoft.com/downloads/details.aspx?familyid=a7990e61-21fd-4942-9dfe-af7961cb0282)  
(KB2416447)  
(Fontos)  
[Microsoft .NET-keretrendszer 2.0 Service Pack 2 és Microsoft .NET-keretrendszer 3.5 Service Pack 1](http://www.microsoft.com/downloads/details.aspx?familyid=3d31fd37-eb58-4169-b6b9-4cf854524e46)  
(KB2418241)  
(Fontos)  
[Microsoft .NET-keretrendszer 3.5](http://www.microsoft.com/downloads/details.aspx?familyid=d284237b-e4d9-460a-98f0-7a18252f5780)  
(KB2416468)  
(Fontos)  
[Microsoft .NET-keretrendszer 3.5](http://www.microsoft.com/downloads/details.aspx?familyid=00d95a85-f3e8-464d-a10c-85c6d91b4aae)  
(KB2418240)  
(Fontos)  
[Microsoft .NET-keretrendszer 3.5 Service Pack 1](http://www.microsoft.com/downloads/details.aspx?familyid=ae42d6cc-6d4e-425a-9b4f-379f66fc506a)  
(KB2416473)  
(Fontos)  
[Microsoft .NET-keretrendszer 4.0](http://www.microsoft.com/downloads/details.aspx?familyid=6ce703b7-08a5-4eff-a062-d5dc720908f6)<sup>[1]</sup>
(KB2416472)  
(Fontos)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Windows Server 2003 SP2 Itanium-alapú rendszerekhez
</td>
<td style="border:1px solid black;">
[Windows Server 2003 SP2 Itanium-alapú rendszerekhez](http://www.microsoft.com/downloads/details.aspx?familyid=ca35a520-c4da-41bb-abcc-d5bc534ff19a)  
(Fontos)
</td>
<td style="border:1px solid black;">
Nem érintett
</td>
<td style="border:1px solid black;">
[Windows Server 2003 SP2 Itanium-alapú rendszerekhez](http://www.microsoft.com/downloads/details.aspx?familyid=be7b3310-ffb7-4528-9c9e-aebe14d264d6)  
(KB981322)  
(Kritikus)
</td>
<td style="border:1px solid black;">
IIS ASP:  
[Internet Information Services 6.0](http://www.microsoft.com/downloads/details.aspx?familyid=f6841057-1745-44e9-a16a-c180dd941ddf)  
(KB2124261)  
(Fontos)
</td>
<td style="border:1px solid black;">
[Windows Server 2003 SP2 Itanium-alapú rendszerekhez](http://www.microsoft.com/downloads/details.aspx?familyid=1f04f151-330a-4b6c-826e-76def35daa73)  
(Fontos)
</td>
<td style="border:1px solid black;">
[Windows Server 2003 SP2 Itanium-alapú rendszerekhez](http://www.microsoft.com/downloads/details.aspx?familyid=c9c4427d-54c8-4f3c-9a94-818196cd5180)  
(Fontos)
</td>
<td style="border:1px solid black;">
[Active Directory](http://www.microsoft.com/downloads/details.aspx?familyid=cab75c8a-0d12-4a91-82b2-9f9b70610f67)  
(KB981550)  
(Fontos)
</td>
<td style="border:1px solid black;">
[Windows Server 2003 SP2 Itanium-alapú rendszerekhez](http://www.microsoft.com/downloads/details.aspx?familyid=e450ca08-1d75-4419-ad9f-c5e5efb55cd5)  
(Fontos)
</td>
<td style="border:1px solid black;">
[Microsoft .NET-keretrendszer 1.1 Service Pack 1](http://www.microsoft.com/downloads/details.aspx?familyid=a7990e61-21fd-4942-9dfe-af7961cb0282)  
(KB2416447)  
(Fontos)  
[Microsoft .NET-keretrendszer 2.0 Service Pack 2 és Microsoft .NET-keretrendszer 3.5 Service Pack 1](http://www.microsoft.com/downloads/details.aspx?familyid=3d31fd37-eb58-4169-b6b9-4cf854524e46)  
(KB2418241)  
(Fontos)  
[Microsoft .NET-keretrendszer 3.5](http://www.microsoft.com/downloads/details.aspx?familyid=d284237b-e4d9-460a-98f0-7a18252f5780)  
(KB2416468)  
(Fontos)  
[Microsoft .NET-keretrendszer 3.5](http://www.microsoft.com/downloads/details.aspx?familyid=00d95a85-f3e8-464d-a10c-85c6d91b4aae)  
(KB2418240)  
(Fontos)  
[Microsoft .NET-keretrendszer 3.5 Service Pack 1](http://www.microsoft.com/downloads/details.aspx?familyid=ae42d6cc-6d4e-425a-9b4f-379f66fc506a)  
(KB2416473)  
(Fontos)  
[Microsoft .NET-keretrendszer 4.0](http://www.microsoft.com/downloads/details.aspx?familyid=6ce703b7-08a5-4eff-a062-d5dc720908f6)<sup>[1]</sup>
(KB2416472)  
(Fontos)
</td>
</tr>
<tr>
<th colspan="10">
Windows Vista
</th>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
**Közlemény azonosítója**
</td>
<td style="border:1px solid black;">
[**MS10-061**](http://go.microsoft.com/fwlink/?linkid=200505)
</td>
<td style="border:1px solid black;">
[**MS10-062**](http://go.microsoft.com/fwlink/?linkid=190884)
</td>
<td style="border:1px solid black;">
[**MS10-063**](http://go.microsoft.com/fwlink/?linkid=200378)
</td>
<td style="border:1px solid black;">
[**MS10-065**](http://go.microsoft.com/fwlink/?linkid=199537)
</td>
<td style="border:1px solid black;">
[**MS10-066**](http://go.microsoft.com/fwlink/?linkid=197105)
</td>
<td style="border:1px solid black;">
[**MS10-067**](http://go.microsoft.com/fwlink/?linkid=197102)
</td>
<td style="border:1px solid black;">
[**MS10-068**](http://go.microsoft.com/fwlink/?linkid=190509)
</td>
<td style="border:1px solid black;">
[**MS10-069**](http://go.microsoft.com/fwlink/?linkid=197093)
</td>
<td style="border:1px solid black;">
[**MS10-070**](http://go.microsoft.com/fwlink/?linkid=202409)
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
[Windows Vista Service Pack 1 és Windows Vista Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=028977fd-0f39-42d4-9fee-0d90a2931cfd)  
(Fontos)
</td>
<td style="border:1px solid black;">
[Windows Vista Service Pack 1 és Windows Vista Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=84629c25-7827-40c1-86fb-7ffa247202a0)  
(Kritikus)
</td>
<td style="border:1px solid black;">
[Windows Vista Service Pack 1 és Windows Vista Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=ac1b0260-3802-45d4-985e-ac827d784e4f)  
(KB981322)  
(Kritikus)
</td>
<td style="border:1px solid black;">
IIS ASP:  
[Internet Information Services 7.0](http://www.microsoft.com/downloads/details.aspx?familyid=75059175-9c59-45d5-81ce-09b964640e5f)  
(KB2124261)  
(Fontos)
</td>
<td style="border:1px solid black;">
Nem érintett
</td>
<td style="border:1px solid black;">
Nem érintett
</td>
<td style="border:1px solid black;">
Csak Windows Vista Service Pack 2:  
[Active Directory Lightweight Directory-szolgáltatás (AD LDS)](http://www.microsoft.com/downloads/details.aspx?familyid=853a71f3-fb0d-43af-a2b8-45bf8ca1a588)  
(KB981550)  
(Fontos)
</td>
<td style="border:1px solid black;">
Nem érintett
</td>
<td style="border:1px solid black;">
[Microsoft .NET-keretrendszer 1.1 Service Pack 1](http://www.microsoft.com/downloads/details.aspx?familyid=a7990e61-21fd-4942-9dfe-af7961cb0282)  
(KB2416447)  
(Fontos)  
[Microsoft .NET-keretrendszer 3.5](http://www.microsoft.com/downloads/details.aspx?familyid=00d95a85-f3e8-464d-a10c-85c6d91b4aae)  
(KB2418240)  
(Fontos)  
[Microsoft .NET-keretrendszer 3.5 Service Pack 1](http://www.microsoft.com/downloads/details.aspx?familyid=ae42d6cc-6d4e-425a-9b4f-379f66fc506a)  
(KB2416473)  
(Fontos)  
[Microsoft .NET-keretrendszer 4.0](http://www.microsoft.com/downloads/details.aspx?familyid=6ce703b7-08a5-4eff-a062-d5dc720908f6)<sup>[1]</sup>
(KB2416472)  
(Fontos)  
Csak Windows Vista Service Pack 1:  
[Microsoft .NET Framework 2.0 Service Pack 1 és Microsoft .NET Framework 3.5](http://www.microsoft.com/downloads/details.aspx?familyid=7ad59265-9dca-4731-ac09-46c162c1832a)  
(KB2416469)  
(Fontos)  
Csak Windows Vista Service Pack 1:  
[Microsoft .NET-keretrendszer 2.0 Service Pack 2 és Microsoft .NET-keretrendszer 3.5 Service Pack 1](http://www.microsoft.com/downloads/details.aspx?familyid=ac1c77df-34d5-48d4-9a9d-33dc017ffe93)  
(KB2416474)  
(Fontos)  
Csak Windows Vista Service Pack 2:  
[Microsoft .NET-keretrendszer 2.0 Service Pack 2, Microsoft .NET-keretrendszer 3.5 és Microsoft .NET-keretrendszer 3.5 Service Pack 1](http://www.microsoft.com/downloads/details.aspx?familyid=45aa5666-3454-443c-a224-2076215fef04)  
(KB2416470)  
(Fontos)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Windows Vista x64 Edition Service Pack 1 és Windows Vista x64 Edition Service Pack 2
</td>
<td style="border:1px solid black;">
[Windows Vista x64 Edition Service Pack 1 és Windows Vista x64 Edition Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=c68b9337-883d-4e98-ba0a-90b5cad46184)  
(Fontos)
</td>
<td style="border:1px solid black;">
[Windows Vista x64 Edition Service Pack 1 és Windows Vista x64 Edition Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=36e2a74b-e5c6-47d5-9cd9-b9171be63c7d)  
(Kritikus)
</td>
<td style="border:1px solid black;">
[Windows Vista x64 Edition Service Pack 1 és Windows Vista x64 Edition Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=ebfdcd6d-413e-4359-8863-e992327a607f)  
(KB981322)  
(Kritikus)
</td>
<td style="border:1px solid black;">
IIS ASP:  
[Internet Information Services 7.0](http://www.microsoft.com/downloads/details.aspx?familyid=9864c590-10a7-4971-a717-924ed0d6cace)  
(KB2124261)  
(Fontos)
</td>
<td style="border:1px solid black;">
Nem érintett
</td>
<td style="border:1px solid black;">
Nem érintett
</td>
<td style="border:1px solid black;">
Csak Windows Vista x64 Edition Service Pack 2:  
[Active Directory Lightweight Directory-szolgáltatás (AD LDS)](http://www.microsoft.com/downloads/details.aspx?familyid=566f468b-22b6-400a-a656-ae64cfcb52df)  
(KB981550)  
(Fontos)
</td>
<td style="border:1px solid black;">
Nem érintett
</td>
<td style="border:1px solid black;">
[Microsoft .NET-keretrendszer 1.1 Service Pack 1](http://www.microsoft.com/downloads/details.aspx?familyid=a7990e61-21fd-4942-9dfe-af7961cb0282)  
(KB2416447)  
(Fontos)  
[Microsoft .NET-keretrendszer 3.5](http://www.microsoft.com/downloads/details.aspx?familyid=00d95a85-f3e8-464d-a10c-85c6d91b4aae)  
(KB2418240)  
(Fontos)  
[Microsoft .NET-keretrendszer 3.5 Service Pack 1](http://www.microsoft.com/downloads/details.aspx?familyid=ae42d6cc-6d4e-425a-9b4f-379f66fc506a)  
(KB2416473)  
(Fontos)  
[Microsoft .NET-keretrendszer 4.0](http://www.microsoft.com/downloads/details.aspx?familyid=6ce703b7-08a5-4eff-a062-d5dc720908f6)<sup>[1]</sup>
(KB2416472)  
(Fontos)  
Csak Windows Vista x64 Edition Service Pack 1:  
[Microsoft .NET Framework 2.0 Service Pack 1 és Microsoft .NET Framework 3.5](http://www.microsoft.com/downloads/details.aspx?familyid=7ad59265-9dca-4731-ac09-46c162c1832a)  
(KB2416469)  
(Fontos)  
Csak Windows Vista x64 Edition Service Pack 1:  
[Microsoft .NET-keretrendszer 2.0 Service Pack 2 és Microsoft .NET-keretrendszer 3.5 Service Pack 1](http://www.microsoft.com/downloads/details.aspx?familyid=ac1c77df-34d5-48d4-9a9d-33dc017ffe93)  
(KB2416474)  
(Fontos)  
Csak Windows Vista x64 Edition Service Pack 2:  
[Microsoft .NET-keretrendszer 2.0 Service Pack 2, Microsoft .NET-keretrendszer 3.5 és Microsoft .NET-keretrendszer 3.5 Service Pack 1](http://www.microsoft.com/downloads/details.aspx?familyid=45aa5666-3454-443c-a224-2076215fef04)  
(KB2416470)  
(Fontos)
</td>
</tr>
<tr>
<th colspan="10">
Windows Server 2008
</th>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
**Közlemény azonosítója**
</td>
<td style="border:1px solid black;">
[**MS10-061**](http://go.microsoft.com/fwlink/?linkid=200505)
</td>
<td style="border:1px solid black;">
[**MS10-062**](http://go.microsoft.com/fwlink/?linkid=190884)
</td>
<td style="border:1px solid black;">
[**MS10-063**](http://go.microsoft.com/fwlink/?linkid=200378)
</td>
<td style="border:1px solid black;">
[**MS10-065**](http://go.microsoft.com/fwlink/?linkid=199537)
</td>
<td style="border:1px solid black;">
[**MS10-066**](http://go.microsoft.com/fwlink/?linkid=197105)
</td>
<td style="border:1px solid black;">
[**MS10-067**](http://go.microsoft.com/fwlink/?linkid=197102)
</td>
<td style="border:1px solid black;">
[**MS10-068**](http://go.microsoft.com/fwlink/?linkid=190509)
</td>
<td style="border:1px solid black;">
[**MS10-069**](http://go.microsoft.com/fwlink/?linkid=197093)
</td>
<td style="border:1px solid black;">
[**MS10-070**](http://go.microsoft.com/fwlink/?linkid=202409)
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
Windows Server 2008 32 bites rendszerekhez és Windows Server 2008 32 bites rendszerekhez, Service Pack 2
</td>
<td style="border:1px solid black;">
[Windows Server 2008 32 bites rendszerekhez és Windows Server 2008 32 bites rendszerekhez, Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=e2e788de-8400-4bf6-b96b-a915154aa20a)\*  
(Fontos)
</td>
<td style="border:1px solid black;">
[Windows Server 2008 32 bites rendszerekhez és Windows Server 2008 32 bites rendszerekhez Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=fdfc393e-a54d-44dd-ba45-c2a550ffd2a1)\*\*  
(Kritikus)
</td>
<td style="border:1px solid black;">
[Windows Server 2008 32 bites rendszerekhez és Windows Server 2008 32 bites rendszerekhez, Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=b679fe0c-5498-4fc5-84c8-0cd24b625907)\*  
(KB981322)  
(Kritikus)
</td>
<td style="border:1px solid black;">
IIS ASP:  
[Internet Information Services 7.0](http://www.microsoft.com/downloads/details.aspx?familyid=d798dc8e-ae64-4a1d-abda-f58cf69779d8)\*  
(KB2124261)  
(Fontos)
</td>
<td style="border:1px solid black;">
Nem érintett
</td>
<td style="border:1px solid black;">
Nem érintett
</td>
<td style="border:1px solid black;">
[Active Directory and Active Directory Lightweight Directory-szolgáltatás (AD LDS)](http://www.microsoft.com/downloads/details.aspx?familyid=1452befe-b7b8-4131-b36f-dded2bd16d5e)\*  
(KB981550)  
(Fontos)
</td>
<td style="border:1px solid black;">
Nem érintett
</td>
<td style="border:1px solid black;">
[Microsoft .NET Framework 1.1 Service Pack 1](http://www.microsoft.com/downloads/details.aspx?familyid=a7990e61-21fd-4942-9dfe-af7961cb0282)\*\*  
(KB2416447)  
(Fontos)  
[Microsoft .NET-keretrendszer 3.5](http://www.microsoft.com/downloads/details.aspx?familyid=00d95a85-f3e8-464d-a10c-85c6d91b4aae)\*\*  
(KB2418240)  
(Fontos)  
[Microsoft .NET-keretrendszer 3.5 Service Pack 1](http://www.microsoft.com/downloads/details.aspx?familyid=ae42d6cc-6d4e-425a-9b4f-379f66fc506a)\*\*  
(KB2416473)  
(Fontos)  
[Microsoft .NET-keretrendszer 4.0](http://www.microsoft.com/downloads/details.aspx?familyid=6ce703b7-08a5-4eff-a062-d5dc720908f6)\*\*<sup>[1]</sup>
(KB2416472)  
(Fontos)  
Csak Windows Server 2008 32 bites rendszerekhez:  
[Microsoft .NET Framework 2.0 Service Pack 1 és Microsoft .NET Framework 3.5](http://www.microsoft.com/downloads/details.aspx?familyid=7ad59265-9dca-4731-ac09-46c162c1832a)\*\*  
(KB2416469)  
(Fontos)  
Csak Windows Server 2008 32 bites rendszerekhez:  
[Microsoft .NET-keretrendszer 2.0 Service Pack 2 és Microsoft .NET-keretrendszer 3.5 Service Pack 1](http://www.microsoft.com/downloads/details.aspx?familyid=ac1c77df-34d5-48d4-9a9d-33dc017ffe93)\*\*  
(KB2416474)  
(Fontos)  
Csak Windows Server 2008 32 bites rendszerekhez Service Pack 2\* esetén:  
[Microsoft .NET-keretrendszer 2.0 Service Pack 2, Microsoft .NET-keretrendszer 3.5 és Microsoft .NET-keretrendszer 3.5 Service Pack 1](http://www.microsoft.com/downloads/details.aspx?familyid=45aa5666-3454-443c-a224-2076215fef04)\*\*  
(KB2416470)  
(Fontos)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Windows Server 2008 x64-alapú rendszerekhez és Windows Server 2008 x64-alapú rendszerekhez, Service Pack 2
</td>
<td style="border:1px solid black;">
[Windows Server 2008 x64 alapú rendszerekhez és Windows Server 2008 x64 alapú rendszerekhez, Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=e08d4f49-5a13-4e1d-b0a7-27b314c2edb5)\*  
(Fontos)
</td>
<td style="border:1px solid black;">
[Windows Server 2008 x64 alapú rendszerekhez és Windows Server 2008 x64 alapú rendszerekhez Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=1b7af424-6286-4a80-827c-c4df4f92fe43)\*\*  
(Kritikus)
</td>
<td style="border:1px solid black;">
[Windows Server 2008 x64 alapú rendszerekhez és Windows Server 2008 x64 alapú rendszerekhez, Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=e1b38b87-24f6-4aaa-afa9-40f4015d6694)\*  
(KB981322)  
(Kritikus)
</td>
<td style="border:1px solid black;">
IIS ASP:  
[Internet Information Services 7.0](http://www.microsoft.com/downloads/details.aspx?familyid=e29f01dc-b00d-4c12-a13e-63aa0b09d919)\*  
(KB2124261)  
(Fontos)
</td>
<td style="border:1px solid black;">
Nem érintett
</td>
<td style="border:1px solid black;">
Nem érintett
</td>
<td style="border:1px solid black;">
[Active Directory and Active Directory Lightweight Directory-szolgáltatás (AD LDS)](http://www.microsoft.com/downloads/details.aspx?familyid=38eb875f-1869-401b-b7d3-9f18f4ba4f24)\*  
(KB981550)  
(Fontos)
</td>
<td style="border:1px solid black;">
Nem érintett
</td>
<td style="border:1px solid black;">
[Microsoft .NET Framework 1.1 Service Pack 1](http://www.microsoft.com/downloads/details.aspx?familyid=a7990e61-21fd-4942-9dfe-af7961cb0282)\*\*  
(KB2416447)  
(Fontos)  
[Microsoft .NET-keretrendszer 3.5](http://www.microsoft.com/downloads/details.aspx?familyid=00d95a85-f3e8-464d-a10c-85c6d91b4aae)\*\*  
(KB2418240)  
(Fontos)  
[Microsoft .NET-keretrendszer 3.5 Service Pack 1](http://www.microsoft.com/downloads/details.aspx?familyid=ae42d6cc-6d4e-425a-9b4f-379f66fc506a)\*\*  
(KB2416473)  
(Fontos)  
[Microsoft .NET-keretrendszer 4.0](http://www.microsoft.com/downloads/details.aspx?familyid=6ce703b7-08a5-4eff-a062-d5dc720908f6)\*\*<sup>[1]</sup>
(KB2416472)  
(Fontos)  
Csak Windows Server 2008 x64 alapú rendszerekhez:  
[Microsoft .NET Framework 2.0 Service Pack 1 és Microsoft .NET Framework 3.5](http://www.microsoft.com/downloads/details.aspx?familyid=7ad59265-9dca-4731-ac09-46c162c1832a)\*\*  
(KB2416469)  
(Fontos)  
Csak Windows Server 2008 x64 alapú rendszerekhez:  
[Microsoft .NET-keretrendszer 2.0 Service Pack 2 és Microsoft .NET-keretrendszer 3.5 Service Pack 1](http://www.microsoft.com/downloads/details.aspx?familyid=ac1c77df-34d5-48d4-9a9d-33dc017ffe93)\*\*  
(KB2416474)  
(Fontos)  
Csak Windows Server 2008 x64 alapú rendszerekhez, Service Pack 2:  
[Microsoft .NET-keretrendszer 2.0 Service Pack 2, Microsoft .NET-keretrendszer 3.5 és Microsoft .NET-keretrendszer 3.5 Service Pack 1](http://www.microsoft.com/downloads/details.aspx?familyid=45aa5666-3454-443c-a224-2076215fef04)\*\*  
(KB2416470)  
(Fontos)  
Csak Windows Server 2008 x64 alapú rendszerekhez, Service Pack 2:  
[Microsoft .NET-keretrendszer 3.5](http://www.microsoft.com/downloads/details.aspx?familyid=00d95a85-f3e8-464d-a10c-85c6d91b4aae)\*\*  
(KB2418240)  
(Fontos)
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
Windows Server 2008 Itanium-alapú rendszerekhez és Windows Server 2008 Itanium-alapú rendszerekhez, Service Pack 2
</td>
<td style="border:1px solid black;">
[Windows Server 2008 Itanium-alapú rendszerekhez és Windows Server 2008 Itanium-alapú rendszerekhez, Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=098537d5-bf6e-4e04-ad33-1cde697e062f)  
(Fontos)
</td>
<td style="border:1px solid black;">
Nem érintett
</td>
<td style="border:1px solid black;">
[Windows Server 2008 Itanium-alapú rendszerekhez és Windows Server 2008 Itanium-alapú rendszerekhez, Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=ceb856e8-f4a6-4229-bd26-b1a763d7d443)  
(KB981322)  
(Kritikus)
</td>
<td style="border:1px solid black;">
IIS ASP:  
[Internet Information Services 7.0](http://www.microsoft.com/downloads/details.aspx?familyid=d595c8d2-90b1-46e4-bb9f-60efd0bf3a02)  
(KB2124261)  
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
[Microsoft .NET-keretrendszer 1.1 Service Pack 1](http://www.microsoft.com/downloads/details.aspx?familyid=a7990e61-21fd-4942-9dfe-af7961cb0282)  
(KB2416447)  
(Fontos)  
[Microsoft .NET-keretrendszer 3.5 Service Pack 1](http://www.microsoft.com/downloads/details.aspx?familyid=ae42d6cc-6d4e-425a-9b4f-379f66fc506a)  
(KB2416473)  
(Fontos)  
[Microsoft .NET-keretrendszer 4.0](http://www.microsoft.com/downloads/details.aspx?familyid=6ce703b7-08a5-4eff-a062-d5dc720908f6)<sup>[1]</sup>
(KB2416472)  
(Fontos)  
Csak Windows Server 2008 Itanium alapú rendszerekhez:  
[Microsoft .NET Framework 2.0 Service Pack 1 és Microsoft .NET Framework 3.5](http://www.microsoft.com/downloads/details.aspx?familyid=7ad59265-9dca-4731-ac09-46c162c1832a)  
(KB2416469)  
(Fontos)  
Csak Windows Server 2008 Itanium alapú rendszerekhez:  
[Microsoft .NET-keretrendszer 2.0 Service Pack 2 és Microsoft .NET-keretrendszer 3.5 Service Pack 1](http://www.microsoft.com/downloads/details.aspx?familyid=ac1c77df-34d5-48d4-9a9d-33dc017ffe93)  
(KB2416474)  
(Fontos)  
Csak Windows Server 2008 Itanium alapú rendszerekhez, Service Pack 2:  
[Microsoft .NET-keretrendszer 2.0 Service Pack 2, Microsoft .NET-keretrendszer 3.5 és Microsoft .NET-keretrendszer 3.5 Service Pack 1](http://www.microsoft.com/downloads/details.aspx?familyid=45aa5666-3454-443c-a224-2076215fef04)  
(KB2416470)  
(Fontos)
</td>
</tr>
<tr>
<th colspan="10">
Windows 7
</th>
</tr>
<tr>
<td style="border:1px solid black;">
**Közlemény azonosítója**
</td>
<td style="border:1px solid black;">
[**MS10-061**](http://go.microsoft.com/fwlink/?linkid=200505)
</td>
<td style="border:1px solid black;">
[**MS10-062**](http://go.microsoft.com/fwlink/?linkid=190884)
</td>
<td style="border:1px solid black;">
[**MS10-063**](http://go.microsoft.com/fwlink/?linkid=200378)
</td>
<td style="border:1px solid black;">
[**MS10-065**](http://go.microsoft.com/fwlink/?linkid=199537)
</td>
<td style="border:1px solid black;">
[**MS10-066**](http://go.microsoft.com/fwlink/?linkid=197105)
</td>
<td style="border:1px solid black;">
[**MS10-067**](http://go.microsoft.com/fwlink/?linkid=197102)
</td>
<td style="border:1px solid black;">
[**MS10-068**](http://go.microsoft.com/fwlink/?linkid=190509)
</td>
<td style="border:1px solid black;">
[**MS10-069**](http://go.microsoft.com/fwlink/?linkid=197093)
</td>
<td style="border:1px solid black;">
[**MS10-070**](http://go.microsoft.com/fwlink/?linkid=202409)
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
Windows 7 32 bites rendszerekhez
</td>
<td style="border:1px solid black;">
[Windows 7 32 bites rendszerekhez](http://www.microsoft.com/downloads/details.aspx?familyid=34619e9e-1f00-40e4-be6f-5bbf5e3c801b)  
(Fontos)
</td>
<td style="border:1px solid black;">
Nem érintett
</td>
<td style="border:1px solid black;">
Nem érintett
</td>
<td style="border:1px solid black;">
IIS ASP:  
[Internet Information Services 7.5](http://www.microsoft.com/downloads/details.aspx?familyid=5b2d42da-4dbc-4fbb-be22-09ca7dec5aa3)  
(KB2124261)  
(Fontos)  
IIS FastCGI:  
[Internet Information Services 7.5](http://www.microsoft.com/downloads/details.aspx?familyid=c843afd9-b6f2-48de-91cc-1c0d481c2be4)  
(KB2271195)  
(Fontos)
</td>
<td style="border:1px solid black;">
Nem érintett
</td>
<td style="border:1px solid black;">
Nem érintett
</td>
<td style="border:1px solid black;">
[Active Directory Lightweight Directory-szolgáltatás (AD LDS)](http://www.microsoft.com/downloads/details.aspx?familyid=454fc025-bfa2-4552-9522-3585f523ecb2)  
(KB981550)  
(Fontos)
</td>
<td style="border:1px solid black;">
Nem érintett
</td>
<td style="border:1px solid black;">
[Microsoft .NET-keretrendszer 3.5.1](http://www.microsoft.com/downloads/details.aspx?familyid=5e7dcf51-74f1-43cc-aece-0cd5df05ddb7)  
(KB2416471)  
(Fontos)  
[Microsoft .NET-keretrendszer 4.0](http://www.microsoft.com/downloads/details.aspx?familyid=6ce703b7-08a5-4eff-a062-d5dc720908f6)<sup>[1]</sup>
(KB2416472)  
(Fontos)
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
Windows 7 32 bites rendszerekhez, Service Pack 1
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
[Microsoft .NET-keretrendszer 4.0](http://www.microsoft.com/downloads/details.aspx?familyid=6ce703b7-08a5-4eff-a062-d5dc720908f6)<sup>[1]</sup>
(KB2416472)  
(Fontos)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Windows 7 x64-alapú rendszerekhez
</td>
<td style="border:1px solid black;">
[Windows 7 x64-alapú rendszerekhez](http://www.microsoft.com/downloads/details.aspx?familyid=dbb747a5-658d-44cf-bd49-425d1700157f)  
(Fontos)
</td>
<td style="border:1px solid black;">
Nem érintett
</td>
<td style="border:1px solid black;">
Nem érintett
</td>
<td style="border:1px solid black;">
IIS ASP:  
[Internet Information Services 7.5](http://www.microsoft.com/downloads/details.aspx?familyid=66b64374-95e4-4b99-80e6-98dc63cd272b)  
(KB2124261)  
(Fontos)  
IIS FastCGI:  
[Internet Information Services 7.5](http://www.microsoft.com/downloads/details.aspx?familyid=5f0c0454-cbb6-47ed-9227-98aa45b8cbdb)  
(KB2271195)  
(Fontos)
</td>
<td style="border:1px solid black;">
Nem érintett
</td>
<td style="border:1px solid black;">
Nem érintett
</td>
<td style="border:1px solid black;">
[Active Directory Lightweight Directory-szolgáltatás (AD LDS)](http://www.microsoft.com/downloads/details.aspx?familyid=b15ad533-3cf1-4dcf-847c-05ebffb84e26)  
(KB981550)  
(Fontos)
</td>
<td style="border:1px solid black;">
Nem érintett
</td>
<td style="border:1px solid black;">
[Microsoft .NET-keretrendszer 3.5.1](http://www.microsoft.com/downloads/details.aspx?familyid=5e7dcf51-74f1-43cc-aece-0cd5df05ddb7)  
(KB2416471)  
(Fontos)  
[Microsoft .NET-keretrendszer 4.0](http://www.microsoft.com/downloads/details.aspx?familyid=6ce703b7-08a5-4eff-a062-d5dc720908f6)<sup>[1]</sup>
(KB2416472) (Fontos)
</td>
</tr>
<tr class="alternateRow">
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
[Microsoft .NET-keretrendszer 4.0](http://www.microsoft.com/downloads/details.aspx?familyid=6ce703b7-08a5-4eff-a062-d5dc720908f6)<sup>[1]</sup>
(KB2416472) (Fontos)
</td>
</tr>
<tr>
<th colspan="10">
Windows Server 2008 R2
</th>
</tr>
<tr>
<td style="border:1px solid black;">
**Közlemény azonosítója**
</td>
<td style="border:1px solid black;">
[**MS10-061**](http://go.microsoft.com/fwlink/?linkid=200505)
</td>
<td style="border:1px solid black;">
[**MS10-062**](http://go.microsoft.com/fwlink/?linkid=190884)
</td>
<td style="border:1px solid black;">
[**MS10-063**](http://go.microsoft.com/fwlink/?linkid=200378)
</td>
<td style="border:1px solid black;">
[**MS10-065**](http://go.microsoft.com/fwlink/?linkid=199537)
</td>
<td style="border:1px solid black;">
[**MS10-066**](http://go.microsoft.com/fwlink/?linkid=197105)
</td>
<td style="border:1px solid black;">
[**MS10-067**](http://go.microsoft.com/fwlink/?linkid=197102)
</td>
<td style="border:1px solid black;">
[**MS10-068**](http://go.microsoft.com/fwlink/?linkid=190509)
</td>
<td style="border:1px solid black;">
[**MS10-069**](http://go.microsoft.com/fwlink/?linkid=197093)
</td>
<td style="border:1px solid black;">
[**MS10-070**](http://go.microsoft.com/fwlink/?linkid=202409)
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
Windows Server 2008 R2 x64-alapú rendszerekhez
</td>
<td style="border:1px solid black;">
[Windows Server 2008 R2 x64 alapú rendszerekhez](http://www.microsoft.com/downloads/details.aspx?familyid=11e20088-1be2-4166-9c97-234b7e9f1c4f)\*  
(Fontos)
</td>
<td style="border:1px solid black;">
Nem érintett
</td>
<td style="border:1px solid black;">
Nem érintett
</td>
<td style="border:1px solid black;">
IIS ASP:  
[Internet Information Services 7.5](http://www.microsoft.com/downloads/details.aspx?familyid=21458cce-f67e-4e95-a067-8311afefc261)\*  
(KB2124261)  
(Fontos)  
IIS FastCGI:  
[Internet Information Services 7.5](http://www.microsoft.com/downloads/details.aspx?familyid=9578b1de-f2c1-4b37-9d82-69e929cab6f3)\*  
(KB2271195)  
(Fontos)
</td>
<td style="border:1px solid black;">
Nem érintett
</td>
<td style="border:1px solid black;">
Nem érintett
</td>
<td style="border:1px solid black;">
[Active Directory and Active Directory Lightweight Directory-szolgáltatás (AD LDS)](http://www.microsoft.com/downloads/details.aspx?familyid=54f36389-8be4-4a0c-9640-dc32addac9d7)\*  
(KB981550)  
(Fontos)
</td>
<td style="border:1px solid black;">
Nem érintett
</td>
<td style="border:1px solid black;">
[Microsoft .NET Framework 3.5.1](http://www.microsoft.com/downloads/details.aspx?familyid=5e7dcf51-74f1-43cc-aece-0cd5df05ddb7)\*  
(KB2416471)  
(Fontos)  
[Microsoft .NET-keretrendszer 4.0](http://www.microsoft.com/downloads/details.aspx?familyid=6ce703b7-08a5-4eff-a062-d5dc720908f6)<sup>[1]</sup>
(KB2416472)  
(Fontos)
</td>
</tr>
<tr class="alternateRow">
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
[Microsoft .NET-keretrendszer 4.0](http://www.microsoft.com/downloads/details.aspx?familyid=6ce703b7-08a5-4eff-a062-d5dc720908f6)\*<sup>[1]</sup>
(KB2416472)  
(Fontos)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Windows Server 2008 R2 Itanium-alapú rendszerekhez
</td>
<td style="border:1px solid black;">
[Windows Server 2008 R2 Itanium-alapú rendszerekhez](http://www.microsoft.com/downloads/details.aspx?familyid=d8c635f8-8978-44bf-b457-e07368f08ef4)  
(Fontos)
</td>
<td style="border:1px solid black;">
Nem érintett
</td>
<td style="border:1px solid black;">
Nem érintett
</td>
<td style="border:1px solid black;">
IIS ASP:  
[Internet Information Services 7.5](http://www.microsoft.com/downloads/details.aspx?familyid=3b8f3fd1-1ef4-4e9f-9bce-0c68f10519d1)  
(KB2124261)  
(Fontos)  
IIS FastCGI:  
[Internet Information Services 7.5](http://www.microsoft.com/downloads/details.aspx?familyid=21adf80d-267f-47cd-9c03-4b4854ba159f)  
(KB2271195)  
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
[Microsoft .NET-keretrendszer 3.5.1](http://www.microsoft.com/downloads/details.aspx?familyid=5e7dcf51-74f1-43cc-aece-0cd5df05ddb7)  
(KB2416471)  
(Fontos)  
[Microsoft .NET-keretrendszer 4.0](http://www.microsoft.com/downloads/details.aspx?familyid=6ce703b7-08a5-4eff-a062-d5dc720908f6)<sup>[1]</sup>
(KB2416472)  
(Fontos)
</td>
</tr>
<tr class="alternateRow">
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
[Microsoft .NET-keretrendszer 4.0](http://www.microsoft.com/downloads/details.aspx?familyid=6ce703b7-08a5-4eff-a062-d5dc720908f6)<sup>[1]</sup>
(KB2416472)  
(Fontos)
</td>
</tr>
</table>
 
**Megjegyzések a Windows Server 2008 és Windows Server 2008 R2 rendszerhez**

**\*Érinti a kiszolgálómag telepítését.** Ez a frissítés ugyanolyan biztonsági besorolás mellett, a megadottak szerint érvényes az Windows Server 2008 és a Windows Server 2008 R2 összes támogatott kiadására, függetlenül attól, hogy a kiszolgálómag-telepítési opcióval telepítették-e. Erről a telepítési opcióról bővebben a [Kiszolgálómag-telepítés kezelése](http://technet.microsoft.com/en-us/library/ee441255(ws.10).aspx) és [Kiszolgálómag-telepítés szervizelése](http://technet.microsoft.com/en-us/library/ff698994(ws.10).aspx) TechNet cikkekben olvashat. A kiszolgálómag-telepítési opció nem vonatkozik a Windows Server 2008 és a Windows Server 2008 R2 bizonyos kiadásaira; lásd: [A kiszolgálómag-telepítési opciók összehasonlítása](http://www.microsoft.com/windowsserver2008/en/us/compare-core-installation.aspx).

**\*\*A kiszolgálómag-telepítés nem érintett.** A frissítésben tárgyalt biztonsági rések nem érintik a jelzett módon a Windows Server 2008 támogatott kiadásait, amennyiben a telepítés a kiszolgálómag-telepítési opció használatával történt. Erről a telepítési opcióról bővebben a [Kiszolgálómag-telepítés kezelése](http://technet.microsoft.com/en-us/library/ee441255(ws.10).aspx) és [Kiszolgálómag-telepítés szervizelése](http://technet.microsoft.com/en-us/library/ff698994(ws.10).aspx) TechNet cikkekben olvashat. A kiszolgálómag-telepítési opció nem vonatkozik a Windows Server 2008 és a Windows Server 2008 R2 bizonyos kiadásaira; lásd: [A kiszolgálómag-telepítési opciók összehasonlítása](http://www.microsoft.com/windowsserver2008/en/us/compare-core-installation.aspx).

**Megjegyzés az MS10-063 közleményhez**

Az ugyanezen a közleményazonosító alatt található, további frissített fájlokat illetően lásd még az egyéb szoftverkategóriák részt ebben a fejezetben, Érintett szoftverek és letöltési helyek. Ez a közlemény több szoftverkategóriát ölel fel.

**Megjegyzés az MS10-070 közleményhez**

<sup>[1]</sup>**A .NET-keretrendszer 4.0 verziójához tartozó ügyfélprofil nem érintett.** A .NET-keretrendszer 4-es verziójú terjeszthető csomagjai két profilban érhetőek el: a .NET-keretrendszer 4.0 és a .NET-keretrendszer 4.0 verziójához tartozó ügyfélprofil. A .NET-keretrendszer 4.0 verziójához tartozó ügyfélprofil része a .NET-keretrendszer 4.0 verziójának. A jelen frissítés csupán a .NET-keretrendszer 4.0 verzióját érinti, a .NET-keretrendszer 4.0 verziójához tartozó ügyfélprofilt nem. Bővebb tájékoztatást itt talál: [A .NET-keretrendszer telepítése](http://msdn.microsoft.com/en-us/library/5a4x27ek.aspx).

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
[**MS10-063**](http://go.microsoft.com/fwlink/?linkid=200378)
</td>
<td style="border:1px solid black;">
[**MS10-064**](http://go.microsoft.com/fwlink/?linkid=200727)
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
[**Kritikus**](http://go.microsoft.com/fwlink/?linkid=21140)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Microsoft Office XP Service Pack 3
</td>
<td style="border:1px solid black;">
[Microsoft Office XP Service Pack 3](http://www.microsoft.com/downloads/details.aspx?familyid=0b56f85f-d39b-410a-857a-799a5d714de7)  
(KB2288608)  
(Fontos)
</td>
<td style="border:1px solid black;">
[Microsoft Outlook 2002 Service Pack 3](http://www.microsoft.com/downloads/details.aspx?familyid=d5e85841-9dea-4776-9e0e-3cd272066f37)  
(KB2293422)  
(Kritikus)
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
Microsoft Office 2003 Service Pack 3
</td>
<td style="border:1px solid black;">
[Microsoft Office 2003 Service Pack 3](http://www.microsoft.com/downloads/details.aspx?familyid=bb7783b1-b396-4254-b317-f2292b305cfc)  
(KB2288613)  
(Fontos)
</td>
<td style="border:1px solid black;">
[Microsoft Outlook 2003 Service Pack 3](http://www.microsoft.com/downloads/details.aspx?familyid=ec8ed81e-05d0-4c20-b5fb-ebc72230a8bd)  
(KB2293428)  
(Fontos)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Microsoft Office 2007 Service Pack 2
</td>
<td style="border:1px solid black;">
[Microsoft Office 2007 Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=44c5bccf-66dd-4796-9089-e6171d8c9785)  
(KB2288621)  
(Fontos)
</td>
<td style="border:1px solid black;">
[Microsoft Outlook 2007 Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=6009d507-135c-4ce8-a830-925134f214dc)  
(KB2288953)  
(Fontos)
</td>
</tr>
</table>
 
**Megjegyzés az MS10-063 közleményhez**

Az ugyanezen a közleményazonosító alatt található, további frissített fájlokat illetően lásd még az egyéb szoftverkategóriák részt ebben a fejezetben, Érintett szoftverek és letöltési helyek. Ez a közlemény több szoftverkategóriát ölel fel.

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

-   Sergey Golovanov, Alexander Gostev, Maxim Golovkin és Alexey Monastyrsky a [Kaspersky Lab](http://www.kaspersky.com/), valamint Vitaly Kiktenko és Alexander Saprykin a [Design and Test Lab](http://www.dnt-lab.com/) munkatársai az MS10-061 közleményben leírt probléma jelentéséért
-   Liam O Morchu, [Symantec](http://www.symantec.com/index.jsp), az MS10-061 közleményben leírt probléma jelentéséért
-   Matthew Watchinski, [Sourcefire VRT](http://www.sourcefire.com/services/sf_vrt.html), az MS10-062 közleményben leírt probléma jelentéséért
-   Carsten Book, , az MS10-063 közleményben bemutatott probléma jelentéséért
-   Marc Schoenefeld, Red Hat Security Response Team, az MS10-063 számú közleményben bemutatott probléma jelentéséért
-   Carsten H. Eiram, [Secunia](http://secunia.com/), a CVE-2010-2738 biztonsági rés MS10-063 közleményben szereplő Kihasználhatósági információinak módosításához vezető bejelentéséért
-   Dyon Balding, [Secunia](http://secunia.com/), az MS10-064 közleményben leírt probléma jelentéséért.
-   Jinsik Shim az MS10-065 közleményben leírt probléma jelentéséért
-   Travis Raybold, Rubicon West, az MS10-065 közleményben leírt probléma jelentéséért
-   Yamata Li, [Palo Alto Networks](http://www.paloaltonetworks.com/), az MS10-066 közleményben leírt probléma jelentéséért
-   S0lute of [iDefense Labs](http://labs.idefense.com/) az MS10-067 közleményben leírt probléma jelentéséért
-   [IBM Japan](http://www.ibm.com/jp/ja/) az MS10-069 közleményben leírt probléma jelentéséért

#### Terméktámogatás

-   Teszteléssel állapították meg a felsorolt szoftverek egyes verzióinak érintettségét. A többi verzió támogatási életciklusa végére ért. Az egyes szoftververziók támogatási életciklusáról a [Microsoft termékek terméktámogatási életciklusát ismertető webhelyen](http://go.microsoft.com/fwlink/?linkid=21742) talál felvilágosítást.
-   Az Amerikai Egyesült Államokban és Kanada területén élő ügyfelek technikai támogatást kérhetnek a [biztonsági támogatás szolgáltatójától](http://go.microsoft.com/fwlink/?linkid=21131) vagy az 1-866-PCSAFETY telefonszámon. A biztonsági frissítésekkel kapcsolatos hívások ingyenesek. Az elérhető támogatási lehetőségekről további információt talál a [Microsoft segítségnyújtással és támogatással foglalkozó webhelyén](http://support.microsoft.com/).
-   Más országokban a helyi Microsoft-képviseletek nyújtanak támogatást. A biztonsági frissítésekkel kapcsolatos hívások ingyenesek. A [nemzetközi támogatási webhely](http://go.microsoft.com/fwlink/?linkid=21155) felvilágosítást nyújt arról, támogatási kérdéseivel hogyan fordulhat a Microsofthoz.

#### Felelősséget kizáró nyilatkozat

A Microsoft Tudásbázisban leírtak előzetes bejelentés nélkül változhatnak, és a cikkek tartalmáért a Microsoft nem vállal garanciát. A Microsoft egyben elhárít minden kifejezett és értelemszerű garanciát, beleértve az eladhatóságra és az adott célra való alkalmasságra vonatkozó garanciát is. A Microsoft Corporation vagy annak szállítói semmilyen körülmények között nem tehetők felelőssé közvetlen, közvetett, eseti, ok-okozati vagy különleges kárért (beleértve az elmaradt hasznot is), még akkor sem, ha a Microsoft Corporation vagy szállítói tudatában voltak a kár lehetséges voltának. Egyes államok törvényi szabályozása nem teszi lehetővé a véletlen vagy ok-okozati károkért vállalt felelősség korlátozását vagy kizárását, így ezekben az államokban az ez a felelősségkizárás nincs érvényben.

#### Verziók

-   1.0 verzió (2010. szeptember 14.): Összefoglaló közlemény közzététele.
-   2.0 verzió (2010. szeptember 22.): A Kihasználhatósági információk értékelésének minősítése a CVE-2010-2738 biztonsági rés esetében nőtt, a CVE-2010-2730 biztonsági rés esetében csökkent, a CVE-2010-0818 biztonsági rés esetében pedig megváltozott a Kihasználhatósági információkhoz tartozó fontos megjegyzés.
-   3.0 verzió (2010. szeptember 28.): Megjelent a Microsoft MS10-070 biztonsági közleménye: Az ASP.NET biztonsági rése adatokhoz való illetéktelen hozzáférést tehet lehetővé (2418042). A soron kívüli biztonsági frissítés webes szemináriumokra vonatkozó hivatkozással is kiegészült.
-   4.0 verzió (2010. szeptember 30.): A közlemény frissített összefoglalója arról tájékoztat, hogy az MS10-070 közleményhez tartozó frissítések már minden terjesztési csatornán elérhetők, beleértve a Windows Update és Microsoft Update szolgáltatásokat is. Ezenfelül módosultak az MS10-070 közleményhez tartozó KB2418240, KB2418241, KB2416470 és KB2416474 frissítések részletei is.
-   4.1 verzió (2010. november 3.): Az MS10-070 közlemény érintett szoftvereket tartalmazó táblázata egy megjegyzéssel bővült, amely egyértelműsíti, hogy a .NET-keretrendszer 4.0 verziójához tartozó ügyfélprofil nem érintett.
-   5.0 verzió (2010. december 14.): A frissített biztonsági közlemény tájékoztat a.NET Framework 4.0 (KB2416472) verzióhoz az MS10-070 keretében elérhető új frissítőcsomagokról. Ezek egy olyan telepítési hiba kijavítására szolgálnak, amely akadályozhatja más frissítések és/vagy termékek sikeres telepítését. A rendszer frissítését már elvégzett felhasználóknak több tennivalójuk nincsen.
-   6.0 verzió (2011. február 22.): Az MS10-070 közlemény frissítésében közölt észlelési módosítás folytán a rendszer felajánlja a Microsoft .NET-keretrendszer 4.0 (KB2416472) frissítőcsomagjait a Microsoft .NET-keretrendszer 4.0 verzióját telepítő felhasználók számára, akik korábban már telepítették a Windows 7 32 bites rendszerekhez Service Pack 1, Windows 7 x64 alapú rendszerekhez Service Pack 1, Windows Server 2008 R2 x64 alapú rendszerekhez Service Pack 1, illetve a Windows Server 2008 R2 Itanium alapú rendszerekhez Service Pack 1 operációs rendszert. A rendszer frissítését már elvégzett felhasználóknak több tennivalójuk nincsen.
-   6.1 verzió (2011. október 26.): Az MS10-070 közleménnyel kapcsolatban javították a .NET Framework 4 keretrendszerhez tartozó kiszolgálómag-telepítés alkalmazhatóságát a Windows Server 2008 R2 x64 alapú rendszerekhez operációs rendszeren.

*Built at 2014-04-18T01:50:00Z-07:00*
