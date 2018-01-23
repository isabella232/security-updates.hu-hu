---
TOCTitle: 'MS09-OCT'
Title: 'Microsoft biztonsági közlemény - összefoglalás, október 2009'
ms:assetid: 'ms09-oct'
ms:contentKeyID: 61227736
ms:mtpsurl: 'https://technet.microsoft.com/hu-HU/library/ms09-oct(v=Security.10)'
---

Security Bulletin Summary

Microsoft biztonsági közlemény - összefoglalás, október 2009
============================================================

Közzétéve: 2009. október 13. | Frissítve: 2010. június 22.

**Verzió:** 4.2

Az összefoglaló a 2009 októberében kiadott biztonsági közleményeket összegzi.

A 2009. októberi közlemények kiadása folytán az összefoglaló a 2009. október 8-án kiadott előzetes értesítés helyébe lép. További információkat a biztonsági közlemények kiadásáról szóló előzetes értesítési szolgáltatásról lásd: [Előzetes értesítés a Microsoft biztonsági közleményeinek kiadásáról](http://technet.microsoft.com/security/bulletin/advance).

Ha automatikus értesítést szeretne kapni a Microsoft biztonsági közleményeinek megjelenéséről, fizessen elő a [Microsoft Technical Security Notifications](http://go.microsoft.com/fwlink/?linkid=21163) szolgáltatásra.

A közleményekkel kapcsolatos kérdések megválaszolására a Microsoft 2009. október 14-én, csendes-óceáni idő szerint 11 órakor webes szemináriumot tart. [Jelentkezzen most az októberi közleményeket bemutató webes szemináriumra](http://msevents.microsoft.com/cui/eventdetail.aspx?eventid=1032407488&culture=en-us). Ezt követően a webes szeminárium igény szerint kerül megrendezésre. További információkért látogasson el a [Microsoft biztonsági közleményeit és a webes szemináriumokat](http://technet.microsoft.com/security/bulletin/summary)bemutató oldalra.

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
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=163970">MS09-050</a></td>
<td style="border:1px solid black;"><strong>Az SMBv2 távoli kódfuttatást lehetővé tévő biztonsági rései (975517)</strong><br />
<br />
Ez a biztonsági frissítés egy nyilvánosságra került és két közvetlenül jelentett biztonsági rést szüntet meg a Server Message Block 2. verzióban (SMBv2). A biztonsági rések legsúlyosabbjai távoli kódfuttatást tesznek lehetővé, ha a támadó speciálisan kialakított SMB-csomagokat küld a hálózaton keresztül a Server szolgáltatást futtató számítógépre. A tűzfalakra vonatkozó gyakorlati tanácsok, valamint a szabványos alapértelmezett tűzfal-konfigurációk segítséget nyújtanak a hálózatot érő, a szervezet határain kívülről eredő támadások kivédésében. Gyakorlati tanácsként azt javasoljuk, hogy az internetkapcsolattal rendelkező számítógépeken a lehető legkevesebb port legyen megnyitva.</td>
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=21140">Kritikus</a><br />
Távoli kódfuttatás</td>
<td style="border:1px solid black;">Újraindítást igényel</td>
<td style="border:1px solid black;">Microsoft Windows</td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=125438">MS09-051</a></td>
<td style="border:1px solid black;"><strong>A Windows Media Runtime biztonsági rései távoli programkódfuttatást tesznek lehetővé (975682)</strong><br />
<br />
Ez a biztonsági frissítés a Windows Media Runtime két közvetlenül jelzett biztonsági rését szünteti meg. A biztonsági rés távoli kódfuttatást tehet lehetővé, ha a felhasználó megnyit egy különlegesen kialakított médiafájlt, vagy különlegesen kialakított tartalom-adatfolyamot fogad egy webhelyről, illetve bármely webes tartalmat szállító alkalmazásból. A biztonsági réseket kihasználó támadó a helyi felhasználóval egyező hozzáférést nyer a rendszerhez. A kevesebb jogosultsággal bíró fiókkal rendelkező felhasználók esetében kisebb a veszélyeztetettség, mint a rendszergazdai jogosultságokkal rendelkezők esetén</td>
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=21140">Kritikus</a><br />
Távoli kódfuttatás</td>
<td style="border:1px solid black;">Esetleg újra kell indítani a rendszert</td>
<td style="border:1px solid black;">Microsoft Windows</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=163913">MS09-052</a></td>
<td style="border:1px solid black;"><strong>A Windows Media Player biztonsági rése, amely távoli programkódfuttatást tesz lehetővé (974112)</strong><br />
<br />
A biztonsági frissítés a Windows Media Player közvetlenül jelentett biztonsági rését szünteti meg. A biztonsági rés távoli kódvégrehajtást tehet lehetővé, amennyiben egy különlegesen kialakított ASD-fájlt tekintett meg a Windows Media Player 6.4 alkalmazással. A biztonsági rést kihasználó támadó a helyi felhasználóval egyező hozzáférést nyer a rendszerhez. A kevesebb jogosultsággal bíró fiókkal rendelkező felhasználók esetében kisebb a veszélyeztetettség, mint a rendszergazdai jogosultságokkal rendelkezők esetén</td>
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=21140">Kritikus</a><br />
Távoli kódfuttatás</td>
<td style="border:1px solid black;">Esetleg újra kell indítani a rendszert</td>
<td style="border:1px solid black;">Microsoft Windows</td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=163979">MS09-054</a></td>
<td style="border:1px solid black;"><strong>Összesítő biztonsági frissítés az Internet Explorer programhoz (974455)</strong><br />
<br />
A biztonsági frissítés három közvetlenül és egy nyilvánosan jelentett biztonsági rést szüntet meg az Internet Explorer programban. A biztonsági rések mindegyike távoli kódvégrehajtást tehet lehetővé, amennyiben a felhasználó egy különlegesen kialakított weboldalt tekint meg az Internet Explorer alkalmazás segítségével. A kevesebb jogosultsággal bíró fiókkal rendelkező felhasználók esetében kisebb a veszélyeztetettség, mint a rendszergazdai jogosultságokkal rendelkezők esetén A Windows megjelenítési alaprendszer (WPF) beépülő modult futtató Firefox felhasználók, akik nem tiltották le ezt a funkciót, szintén alkalmazzák a biztonsági frissítést. További információk a problémáról a HTML-összetevő kezelése okozta biztonsági rés (CVE-2009-2529) GYIK részében.</td>
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=21140">Kritikus</a><br />
Távoli kódfuttatás</td>
<td style="border:1px solid black;">Újraindítást igényel</td>
<td style="border:1px solid black;">Microsoft Windows,<br />
Internet Explorer</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><a href="http://technet.microsoft.com/security/bulletin/ms09-055">MS09-055</a></td>
<td style="border:1px solid black;"><strong>Összesítő biztonsági frissítés az ActiveX-tiltóbitekhez (973525)</strong><br />
<br />
Ez a biztonsági frissítés egy az ActiveX vezérlőkre jellemző, közvetlenül jelzett biztonsági rést tárgyal, amelyet jelenleg is kihasználnak. A Microsoft Active Template Library (ATL) sérülékeny verziójának felhasználásával összeállított ActiveX vezérlőket érintő biztonsági rés távolról történő kódfuttatást tesz lehetővé, ha a felhasználó egy különlegesen kialakított weboldalra látogat el az Internet Explorer alkalmazással és a program elindítja az ActiveX-vezérlőt. A kevesebb jogosultsággal bíró fiókkal rendelkező felhasználók esetében kisebb a veszélyeztetettség, mint a rendszergazdai jogosultságokkal rendelkezők esetén</td>
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=21140">Kritikus</a><br />
Távoli kódfuttatás</td>
<td style="border:1px solid black;">Esetleg újra kell indítani a rendszert</td>
<td style="border:1px solid black;">Microsoft Windows</td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=160633">MS09-060</a></td>
<td style="border:1px solid black;"><strong>A Microsoft Active Template Library (ATL) Microsoft Office ActiveX vezérlőinek biztonsági rései távolról történő programkódfuttatást tehetnek lehetővé (973965)</strong><br />
<br />
Ez a biztonsági frissítés több közvetlenül jelentett biztonsági rést old meg a Microsoft Office ActiveX-vezérlőkben, melyeket a Microsoft Active Template Library (ATL) érintett verziójával állítottak össze. A biztonsági rések távolról történő programkódfuttatást tehetnek lehetővé, ha a felhasználó betölt egy speciálisan kialakított összetevőt vagy vezérlőt. A kevesebb jogosultsággal bíró fiókkal rendelkező felhasználók esetében kisebb a veszélyeztetettség, mint a rendszergazdai jogosultságokkal rendelkezők esetén</td>
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=21140">Kritikus</a><br />
Távoli kódfuttatás</td>
<td style="border:1px solid black;">Esetleg újra kell indítani a rendszert</td>
<td style="border:1px solid black;">Microsoft Office</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=160527">MS09-061</a></td>
<td style="border:1px solid black;"><strong>A Microsoft .NET közös nyelvi futtató környezet biztonsági rése távoli kódfuttatást tehet lehetővé (974378)</strong><br />
<br />
Ez a biztonsági frissítés a Microsoft .NET Framework és a Microsoft Silverlight három, közvetlenül jelzett biztonsági rését szünteti meg. A biztonsági rések távoli kódfuttatást tehetnek lehetővé az ügyfélrendszereken, ha a felhasználó különlegesen kialakított weboldalt tekint meg az XAML böngészőalkalmazások (XBAP alkalmazások) vagy Silverlight alkalmazások futtatására alkalmas böngészőben, illetve ha a támadó sikeresen ráveszi a felhasználót, hogy különlegesen kialakított Microsoft .NET alkalmazást futtasson. A kevesebb jogosultsággal bíró fiókkal rendelkező felhasználók esetében kisebb a veszélyeztetettség, mint a rendszergazdai jogosultságokkal rendelkezők esetén A biztonsági rések IIS szolgáltatást futtató kiszolgálórendszereken is lehetővé tehetik a távoli kódfuttatást, ha az adott kiszolgálón engedélyezett az ASP.NET oldalak feldolgozása, és a támadó sikeresen feltölt egy különlegesen kialakított ASP.NET oldalt a kiszolgálóra, és végrehajtja, mint az a webes tárolási forgatókönyv esetében történik. A Microsoft .NET alkalmazások, Silverlight alkalmazások, XBAP-k és ASP.NET oldalak, amelyek nem rosszindulatúak, a biztonsági rés által nem érintettek.</td>
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=21140">Kritikus</a><br />
Távoli kódfuttatás</td>
<td style="border:1px solid black;">Esetleg újra kell indítani a rendszert</td>
<td style="border:1px solid black;">Microsoft Windows,<br />
Microsoft .NET-keretrendszer,<br />
Microsoft Silverlight</td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=161342">MS09-062</a></td>
<td style="border:1px solid black;"><strong>A GDI+ biztonsági rései távolról történő kódfuttatást tesznek lehetővé (957488)</strong><br />
<br />
A biztonsági frissítés a Microsoft Windows GDI+ számos, közvetlenül jelentett biztonsági rését szünteti meg. A biztonsági rések távoli kódvégrehajtást tehetnek lehetővé, amennyiben a felhasználó egy különlegesen kialakított képfájlt tekintett meg az érintett alkalmazás segítségével vagy ellátogatott a különleges tartalomnak helyet adó weboldalra. A kevesebb jogosultsággal bíró fiókkal rendelkező felhasználók esetében kisebb a veszélyeztetettség, mint a rendszergazdai jogosultságokkal rendelkezők esetén</td>
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=21140">Kritikus</a><br />
Távoli kódfuttatás</td>
<td style="border:1px solid black;">Esetleg újra kell indítani a rendszert</td>
<td style="border:1px solid black;">Microsoft Windows,<br />
Internet Explorer,<br />
Microsoft .NET-keretrendszer,<br />
Microsoft Office,<br />
Microsoft SQL Server,<br />
Microsoft fejlesztői eszközök<br />
Microsoft Forefront</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=164004">MS09-053</a></td>
<td style="border:1px solid black;"><strong>Az Internet Information Services FTP szolgáltatásának biztonsági rése távolról történő programkódfuttatást tehet lehetővé (975254)</strong><br />
<br />
A biztonsági frissítés a Microsoft Internet Information Services alkalmazás FTP szolgáltatás (IIS) 5.0, Microsoft Internet Information Services (IIS) 5.1, Microsoft Internet Information Services (IIS) 6.0 és Microsoft Internet Information Services (IIS) 7.0 két nyilvánosan feltárt biztonsági rését szünteti meg. Az IIS 7.0 esetében csak az FTP Service 6.0 érintett. A biztonsági rések távoli kódfuttatást (RCE) tehetnek lehetővé az IIS 5.0 verzión FTP szolgáltatást futtató rendszereken, vagy szolgáltatásmegtagadást (DoS) az IIS 5.0, IIS 5.1, IIS 6.0 vagy IIS 7.0 verzión FTP szolgáltatást futtató rendszereken.</td>
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=21140">Fontos</a><br />
Távoli kódfuttatás</td>
<td style="border:1px solid black;">Esetleg újra kell indítani a rendszert</td>
<td style="border:1px solid black;">Microsoft Windows</td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=163830">MS09-056</a></td>
<td style="border:1px solid black;"><strong>A Windows CryptoAPI biztonsági rései tartalomhamisítást tehetnek lehetővé (974571)</strong><br />
<br />
A biztonsági frissítés a Microsoft Windows két, nyilvánosan jelentett biztonsági rését szünteti meg. A biztonsági rések tartalomhamisítást tehetnek lehetővé, ha a támadó hozzáférést szerez a végfelhasználó hitelesítésre használt tanúsítványához.</td>
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=21140">Fontos</a><br />
Tartalomhamisítás</td>
<td style="border:1px solid black;">Újraindítást igényel</td>
<td style="border:1px solid black;">Microsoft Windows</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=163832">MS09-057</a></td>
<td style="border:1px solid black;"><strong>Az indexelő szolgáltatás biztonsági rése távoli programkódfuttatást tehet lehetővé (969059)</strong><br />
<br />
A biztonsági frissítés a Microsoft Windows közvetlenül jelentett biztonsági rését szünteti meg. A biztonsági rés lehetővé teheti a távoli kódfuttatást, ha egy támadó rosszindulatú weboldalt készít, mely indexelő szolgáltatást aktivizál az ActiveX összetevő hívása révén. Ez a hívás rosszindulatú URL-t tartalmazhat, kihasználhatja a biztonsági rést, és hozzáférést biztosíthat a támadó számára az ügyfélrendszerhez a weblapot böngésző felhasználó jogosultságaival. A kevesebb jogosultsággal bíró fiókkal rendelkező felhasználók esetében kisebb a veszélyeztetettség, mint a rendszergazdai jogosultságokkal rendelkezők esetén</td>
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=21140">Fontos</a><br />
Távoli kódfuttatás</td>
<td style="border:1px solid black;">Újraindítást igényel</td>
<td style="border:1px solid black;">Microsoft Windows</td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=162442">MS09-058</a></td>
<td style="border:1px solid black;"><strong>A Windows-kernel biztonsági rései jogok kiterjesztését tehetik lehetővé (971486)</strong><br />
<br />
A biztonsági frissítés a Windows rendszermag számos, közvetlenül jelentett biztonsági rését szünteti meg. A biztonsági rések legsúlyosabbika a jogok kiterjesztését teheti lehetővé, ha a támadó bejelentkezhet a rendszerre, és ott különlegesen kialakított alkalmazást futtatott. A támadónak bármely biztonsági rés kihasználásához érvényes bejelentkezési adatokkal kell rendelkeznie, és képesnek kell lennie helyileg bejelentkezni a rendszerbe. Névtelen felhasználók nem tudják távolról kiaknázni ezeket a biztonsági réseket.</td>
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=21140">Fontos</a><br />
Jogok kiterjesztése</td>
<td style="border:1px solid black;">Újraindítást igényel</td>
<td style="border:1px solid black;">Microsoft Windows</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=163843">MS09-059</a></td>
<td style="border:1px solid black;"><strong>Az LSASS biztonsági rése szolgáltatásmegtagadást okozhat (975467)</strong><br />
<br />
A biztonsági frissítés a Microsoft Windows közvetlenül jelentett biztonsági rését szünteti meg. A biztonsági rés szolgáltatásmegtagadást okozhat, ha a támadó rosszindulatú céllal létrehozott csomagot küld az NTLM hitelesítési folyamat során.</td>
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=21140">Fontos</a><br />
Szolgáltatásmegtagadás</td>
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
  
| Közlemény azonosítója                                               | Közlemény címe                                                                                                                                                  | CVE-azonosító                                                                    | Kihasználhatósági információk értékelése                                                                                 | Fontos megjegyzések                                                                                                                                                                                                                                                                                                                                                                              |  
|---------------------------------------------------------------------|-----------------------------------------------------------------------------------------------------------------------------------------------------------------|----------------------------------------------------------------------------------|--------------------------------------------------------------------------------------------------------------------------|--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|  
| [MS09-050](http://go.microsoft.com/fwlink/?linkid=163970)           | Az SMBv2 távoli kódfuttatást lehetővé tévő biztonsági rései (975517)                                                                                            | [CVE-2009-2526](http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2009-2526) | [**3**](http://technet.microsoft.com/en-us/security/cc998259.aspx) - Nem valószínű működő rosszindulatú programkód       | Ez a biztonsági rés korlátozott szolgáltatásmegtagadást okoz.                                                                                                                                                                                                                                                                                                                                    |  
| [MS09-050](http://go.microsoft.com/fwlink/?linkid=163970)           | Az SMBv2 távoli kódfuttatást lehetővé tévő biztonsági rései (975517)                                                                                            | [CVE-2009-2532](http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2009-2532) | [**1**](http://technet.microsoft.com/en-us/security/cc998259.aspx) - Valószínűleg konzisztens rosszindulatú programkód   | (Nincs)                                                                                                                                                                                                                                                                                                                                                                                          |  
| [MS09-050](http://go.microsoft.com/fwlink/?linkid=163970)           | Az SMBv2 távoli kódfuttatást lehetővé tévő biztonsági rései (975517)                                                                                            | [CVE-2009-3103](http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2009-3103) | [**1**](http://technet.microsoft.com/en-us/security/cc998259.aspx) - Valószínűleg konzisztens rosszindulatú programkód   | A rosszindulatú programkódot nyilvánosságra hozták.                                                                                                                                                                                                                                                                                                                                              |  
| [MS09-051](http://go.microsoft.com/fwlink/?linkid=125438)           | A Windows Media Runtime biztonsági rései távoli programkódfuttatást tesznek lehetővé (975682)                                                                   | [CVE-2009-0555](http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2009-0555) | [**1**](http://technet.microsoft.com/en-us/security/cc998259.aspx) - Valószínűleg konzisztens rosszindulatú programkód   | (Nincs)                                                                                                                                                                                                                                                                                                                                                                                          |  
| [MS09-051](http://go.microsoft.com/fwlink/?linkid=125438)           | A Windows Media Runtime biztonsági rései távoli programkódfuttatást tesznek lehetővé (975682)                                                                   | [CVE-2009-2525](http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2009-2525) | [**2**](http://technet.microsoft.com/en-us/security/cc998259.aspx) - Valószínűleg inkonzisztens rosszindulatú programkód | (Nincs)                                                                                                                                                                                                                                                                                                                                                                                          |  
| [MS09-052](http://go.microsoft.com/fwlink/?linkid=163913)           | A Windows Media Player biztonsági rése, amely távoli programkódfuttatást tesz lehetővé (974112)                                                                 | [CVE-2009-2527](http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2009-2527) | [**1**](http://technet.microsoft.com/en-us/security/cc998259.aspx) - Valószínűleg konzisztens rosszindulatú programkód   | (Nincs)                                                                                                                                                                                                                                                                                                                                                                                          |  
| [MS09-053](http://go.microsoft.com/fwlink/?linkid=164004)           | Az Internet Information Services FTP szolgáltatásának biztonsági rése távolról történő programkódfuttatást tehet lehetővé (975254)                              | [CVE-2009-2521](http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2009-2521) | [**3**](http://technet.microsoft.com/en-us/security/cc998259.aspx) - Nem valószínű működő rosszindulatú programkód       | Ez a biztonsági rés szolgáltatásmegtagadást okoz. A rosszindulatú programkódot nyilvánosságra hozták.                                                                                                                                                                                                                                                                                            |  
| [MS09-053](http://go.microsoft.com/fwlink/?linkid=164004)           | Az Internet Information Services FTP szolgáltatásának biztonsági rése távolról történő programkódfuttatást tehet lehetővé (975254)                              | [CVE-2009-3023](http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2009-3023) | [**1**](http://technet.microsoft.com/en-us/security/cc998259.aspx) - Valószínűleg konzisztens rosszindulatú programkód   | A rosszindulatú programkódot nyilvánosságra hozták.                                                                                                                                                                                                                                                                                                                                              |  
| [MS09-054](http://go.microsoft.com/fwlink/?linkid=163979)           | Összesítő biztonsági frissítés az Internet Explorer programhoz (974455)                                                                                         | [CVE-2009-1547](http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2009-1547) | [**2**](http://technet.microsoft.com/en-us/security/cc998259.aspx) - Valószínűleg inkonzisztens rosszindulatú programkód | (Nincs)                                                                                                                                                                                                                                                                                                                                                                                          |  
| [MS09-054](http://go.microsoft.com/fwlink/?linkid=163979)           | Összesítő biztonsági frissítés az Internet Explorer programhoz (974455)                                                                                         | [CVE-2009-2529](http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2009-2529) | [**1**](http://technet.microsoft.com/en-us/security/cc998259.aspx) - Valószínűleg konzisztens rosszindulatú programkód   | (Nincs)                                                                                                                                                                                                                                                                                                                                                                                          |  
| [MS09-054](http://go.microsoft.com/fwlink/?linkid=163979)           | Összesítő biztonsági frissítés az Internet Explorer programhoz (974455)                                                                                         | [CVE-2009-2530](http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2009-2530) | [**2**](http://technet.microsoft.com/en-us/security/cc998259.aspx) - Valószínűleg inkonzisztens rosszindulatú programkód | Microsoft Windows 2000 rendszereken a halomvédelem hiánya [**1**](http://technet.microsoft.com/en-us/security/cc998259.aspx)-es szintűre növeli a kihasználhatósági indexet: Valószínűleg konzisztens rosszindulatú programkód                                                                                                                                                                   |  
| [MS09-054](http://go.microsoft.com/fwlink/?linkid=163979)           | Összesítő biztonsági frissítés az Internet Explorer programhoz (974455)                                                                                         | [CVE-2009-2531](http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2009-2531) | [**2**](http://technet.microsoft.com/en-us/security/cc998259.aspx) - Valószínűleg inkonzisztens rosszindulatú programkód |                                                                                                                                                                                                                                                                                                                                                                                                  |  
| [MS09-055](http://technet.microsoft.com/security/bulletin/ms09-055) | Összesítő biztonsági frissítés az ActiveX-tiltóbitekhez (973525)                                                                                                | [CVE-2009-2493](http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2009-2493) | Nincsenek                                                                                                                | (Ezt a biztonsági rést a [júliusi közleményösszesítő](http://technet.microsoft.com/security/bulletin/ms09-jul) a kihasználhatóság szempontjából már besorolta. A biztonsági réssel először az [MS09-035](http://go.microsoft.com/fwlink/?linkid=158131) közlemény foglalkozott.) Lásd ugyanezt a CVE-számot az [MS09-060](http://go.microsoft.com/fwlink/?linkid=160633) közleményben.           |  
| [MS09-056](http://go.microsoft.com/fwlink/?linkid=163830)           | A Windows CryptoAPI biztonsági rései tartalomhamisítást tehetnek lehetővé (974571)                                                                              | [CVE-2009-2510](http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2009-2510) | [**3**](http://technet.microsoft.com/en-us/security/cc998259.aspx) - Nem valószínű működő rosszindulatú programkód       | Ez a biztonsági rés tartalomhamisításra ad lehetőséget.                                                                                                                                                                                                                                                                                                                                          |  
| [MS09-056](http://go.microsoft.com/fwlink/?linkid=163830)           | A Windows CryptoAPI biztonsági rései tartalomhamisítást tehetnek lehetővé (974571)                                                                              | [CVE-2009-2511](http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2009-2511) | [**3**](http://technet.microsoft.com/en-us/security/cc998259.aspx) - Nem valószínű működő rosszindulatú programkód       | Ez a biztonsági rés tartalomhamisításra ad lehetőséget.                                                                                                                                                                                                                                                                                                                                          |  
| [MS09-057](http://go.microsoft.com/fwlink/?linkid=163832)           | Az indexelő szolgáltatás biztonsági rése távoli programkódfuttatást tehet lehetővé (969059)                                                                     | [CVE-2009-2507](http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2009-2507) | [**2**](http://technet.microsoft.com/en-us/security/cc998259.aspx) - Valószínűleg inkonzisztens rosszindulatú programkód | (Nincs)                                                                                                                                                                                                                                                                                                                                                                                          |  
| [MS09-058](http://go.microsoft.com/fwlink/?linkid=162442)           | A Windows-kernel biztonsági rései jogok kiterjesztését tehetik lehetővé (971486)                                                                                | [CVE-2009-2515](http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2009-2515) | [**2**](http://technet.microsoft.com/en-us/security/cc998259.aspx) - Valószínűleg inkonzisztens rosszindulatú programkód | (Nincs)                                                                                                                                                                                                                                                                                                                                                                                          |  
| [MS09-058](http://go.microsoft.com/fwlink/?linkid=162442)           | A Windows-kernel biztonsági rései jogok kiterjesztését tehetik lehetővé (971486)                                                                                | [CVE-2009-2516](http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2009-2516) | [**3**](http://technet.microsoft.com/en-us/security/cc998259.aspx) - Nem valószínű működő rosszindulatú programkód       | A biztonsági rés hálózati megosztás révén történő kihasználása szolgáltatásmegtagadást, míg a helyi rendszeren keresztüli kihasználás jogok kiterjesztését eredményezheti.                                                                                                                                                                                                                       |  
| [MS09-058](http://go.microsoft.com/fwlink/?linkid=162442)           | A Windows-kernel biztonsági rései jogok kiterjesztését tehetik lehetővé (971486)                                                                                | [CVE-2009-2517](http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2009-2517) | [**3**](http://technet.microsoft.com/en-us/security/cc998259.aspx) - Nem valószínű működő rosszindulatú programkód       | Ez a biztonsági rés szolgáltatásmegtagadást okoz.                                                                                                                                                                                                                                                                                                                                                |  
| [MS09-059](http://go.microsoft.com/fwlink/?linkid=163843)           | Az LSASS biztonsági rése szolgáltatásmegtagadást okozhat (975467)                                                                                               | [CVE-2009-2524](http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2009-2524) | [**3**](http://technet.microsoft.com/en-us/security/cc998259.aspx) - Nem valószínű működő rosszindulatú programkód       | Ez a biztonsági rés korlátozott szolgáltatásmegtagadást okoz.                                                                                                                                                                                                                                                                                                                                    |  
| [MS09-060](http://go.microsoft.com/fwlink/?linkid=160633)           | A Microsoft Active Template Library (ATL) Microsoft Office ActiveX vezérlőinek biztonsági rései távolról történő programkódfuttatást tehetnek lehetővé (973965) | [CVE-2009-0901](http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2009-0901) | Nincsenek                                                                                                                | (Ezt a biztonsági rést a [júliusi közleményösszesítő](http://technet.microsoft.com/security/bulletin/ms09-jul) a kihasználhatóság szempontjából már besorolta. Ennek oka az, hogy a biztonsági rést első alkalommal az [MS09-035](http://go.microsoft.com/fwlink/?linkid=158131) közlemény orvosolta.)                                                                                           |  
| [MS09-060](http://go.microsoft.com/fwlink/?linkid=160633)           | A Microsoft Active Template Library (ATL) Microsoft Office ActiveX vezérlőinek biztonsági rései távolról történő programkódfuttatást tehetnek lehetővé (973965) | [CVE-2009-2493](http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2009-2493) | Nincsenek                                                                                                                | (Ezt a biztonsági rést a [júliusi közleményösszesítő](http://technet.microsoft.com/security/bulletin/ms09-jul) a kihasználhatóság szempontjából már besorolta. A biztonsági réssel először az [MS09-035](http://go.microsoft.com/fwlink/?linkid=158131) közlemény foglalkozott.) Lásd ugyanezt a CVE-számot az [MS09-055](http://technet.microsoft.com/security/bulletin/ms09-055) közleményben. |  
| [MS09-060](http://go.microsoft.com/fwlink/?linkid=160633)           | A Microsoft Active Template Library (ATL) Microsoft Office ActiveX vezérlőinek biztonsági rései távolról történő programkódfuttatást tehetnek lehetővé (973965) | [CVE-2009-2495](http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2009-2495) | [**3**](http://technet.microsoft.com/en-us/security/cc998259.aspx) - Nem valószínű működő rosszindulatú programkód       | A biztonsági rés illetéktelen adatelérést okoz.                                                                                                                                                                                                                                                                                                                                                  |  
| [MS09-061](http://go.microsoft.com/fwlink/?linkid=160527)           | A Microsoft .NET közös nyelvi futtató környezet biztonsági rése távoli kódfuttatást tehet lehetővé (974378)                                                     | [CVE-2009-0090](http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2009-0090) | [**1**](http://technet.microsoft.com/en-us/security/cc998259.aspx) - Valószínűleg konzisztens rosszindulatú programkód   | (Nincs)                                                                                                                                                                                                                                                                                                                                                                                          |  
| [MS09-061](http://go.microsoft.com/fwlink/?linkid=160527)           | A Microsoft .NET közös nyelvi futtató környezet biztonsági rése távoli kódfuttatást tehet lehetővé (974378)                                                     | [CVE-2009-0091](http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2009-0091) | [**1**](http://technet.microsoft.com/en-us/security/cc998259.aspx) - Valószínűleg konzisztens rosszindulatú programkód   | (Nincs)                                                                                                                                                                                                                                                                                                                                                                                          |  
| [MS09-061](http://go.microsoft.com/fwlink/?linkid=160527)           | A Microsoft .NET közös nyelvi futtató környezet biztonsági rése távoli kódfuttatást tehet lehetővé (974378)                                                     | [CVE-2009-2497](http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2009-2497) | [**1**](http://technet.microsoft.com/en-us/security/cc998259.aspx) - Valószínűleg konzisztens rosszindulatú programkód   | Az internetet érintő támadások lehetősége továbbra is fennáll.                                                                                                                                                                                                                                                                                                                                   |  
| [MS09-062](http://go.microsoft.com/fwlink/?linkid=161342)           | A GDI+ biztonsági rései távolról történő kódfuttatást tesznek lehetővé (957488)                                                                                 | [CVE-2009-2500](http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2009-2500) | [**2**](http://technet.microsoft.com/en-us/security/cc998259.aspx) - Valószínűleg inkonzisztens rosszindulatú programkód | (Nincs)                                                                                                                                                                                                                                                                                                                                                                                          |  
| [MS09-062](http://go.microsoft.com/fwlink/?linkid=161342)           | A GDI+ biztonsági rései távolról történő kódfuttatást tesznek lehetővé (957488)                                                                                 | [CVE-2009-2501](http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2009-2501) | [**2**](http://technet.microsoft.com/en-us/security/cc998259.aspx) - Valószínűleg inkonzisztens rosszindulatú programkód | (Nincs)                                                                                                                                                                                                                                                                                                                                                                                          |  
| [MS09-062](http://go.microsoft.com/fwlink/?linkid=161342)           | A GDI+ biztonsági rései távolról történő kódfuttatást tesznek lehetővé (957488)                                                                                 | [CVE-2009-2502](http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2009-2502) | [**2**](http://technet.microsoft.com/en-us/security/cc998259.aspx) - Valószínűleg inkonzisztens rosszindulatú programkód | (Nincs)                                                                                                                                                                                                                                                                                                                                                                                          |  
| [MS09-062](http://go.microsoft.com/fwlink/?linkid=161342)           | A GDI+ biztonsági rései távolról történő kódfuttatást tesznek lehetővé (957488)                                                                                 | [CVE-2009-2503](http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2009-2503) | [**1**](http://technet.microsoft.com/en-us/security/cc998259.aspx) - Valószínűleg konzisztens rosszindulatú programkód   | (Nincs)                                                                                                                                                                                                                                                                                                                                                                                          |  
| [MS09-062](http://go.microsoft.com/fwlink/?linkid=161342)           | A GDI+ biztonsági rései távolról történő kódfuttatást tesznek lehetővé (957488)                                                                                 | [CVE-2009-2504](http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2009-2504) | [**2**](http://technet.microsoft.com/en-us/security/cc998259.aspx) - Valószínűleg inkonzisztens rosszindulatú programkód | (Nincs)                                                                                                                                                                                                                                                                                                                                                                                          |  
| [MS09-062](http://go.microsoft.com/fwlink/?linkid=161342)           | A GDI+ biztonsági rései távolról történő kódfuttatást tesznek lehetővé (957488)                                                                                 | [CVE-2009-2518](http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2009-2518) | [**2**](http://technet.microsoft.com/en-us/security/cc998259.aspx) - Valószínűleg inkonzisztens rosszindulatú programkód | (Nincs)                                                                                                                                                                                                                                                                                                                                                                                          |  
| [MS09-062](http://go.microsoft.com/fwlink/?linkid=161342)           | A GDI+ biztonsági rései távolról történő kódfuttatást tesznek lehetővé (957488)                                                                                 | [CVE-2009-2528](http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2009-2528) | [**1**](http://technet.microsoft.com/en-us/security/cc998259.aspx) - Valószínűleg konzisztens rosszindulatú programkód   | (Nincs)                                                                                                                                                                                                                                                                                                                                                                                          |  
| [MS09-062](http://go.microsoft.com/fwlink/?linkid=161342)           | A GDI+ biztonsági rései távolról történő kódfuttatást tesznek lehetővé (957488)                                                                                 | [CVE-2009-3126](http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2009-3126) | [**2**](http://technet.microsoft.com/en-us/security/cc998259.aspx) - Valószínűleg inkonzisztens rosszindulatú programkód | (Nincs)                                                                                                                                                                                                                                                                                                                                                                                          |
  
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
</tr>
<tr>
<th colspan="13">
Microsoft Windows 2000  
</th>
</tr>
<tr>
<td style="border:1px solid black;">
**Közlemény azonosítója**
</td>
<td style="border:1px solid black;">
[**MS09-050**](http://go.microsoft.com/fwlink/?linkid=163970)
</td>
<td style="border:1px solid black;">
[**MS09-051**](http://go.microsoft.com/fwlink/?linkid=125438)
</td>
<td style="border:1px solid black;">
[**MS09-052**](http://go.microsoft.com/fwlink/?linkid=163913)
</td>
<td style="border:1px solid black;">
[**MS09-054**](http://go.microsoft.com/fwlink/?linkid=163979)
</td>
<td style="border:1px solid black;">
[**MS09-055**](http://technet.microsoft.com/security/bulletin/ms09-055)
</td>
<td style="border:1px solid black;">
[**MS09-061**](http://go.microsoft.com/fwlink/?linkid=160527)
</td>
<td style="border:1px solid black;">
[**MS09-062**](http://go.microsoft.com/fwlink/?linkid=161342)
</td>
<td style="border:1px solid black;">
[**MS09-053**](http://go.microsoft.com/fwlink/?linkid=164004)
</td>
<td style="border:1px solid black;">
[**MS09-056**](http://go.microsoft.com/fwlink/?linkid=163830)
</td>
<td style="border:1px solid black;">
[**MS09-057**](http://go.microsoft.com/fwlink/?linkid=163832)
</td>
<td style="border:1px solid black;">
[**MS09-058**](http://go.microsoft.com/fwlink/?linkid=162442)
</td>
<td style="border:1px solid black;">
[**MS09-059**](http://go.microsoft.com/fwlink/?linkid=163843)
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
**Összesített súlyossági besorolás**
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
[**Nincs**](http://go.microsoft.com/fwlink/?linkid=21140)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Microsoft Windows 2000 Service Pack 4
</td>
<td style="border:1px solid black;">
Nem érintett
</td>
<td style="border:1px solid black;">
[DirectShow WMA hangkodek](http://www.microsoft.com/downloads/details.aspx?familyid=4fe0dff5-04d9-4409-8d1d-52419537126b)  
(KB969878)  
(Kritikus)  
[Windows Media Audio Voice Decoder](http://www.microsoft.com/downloads/details.aspx?familyid=8f850a82-61f9-447b-a0aa-a2c192cc5d2e)  
(KB954155)  
(Kritikus)  
[Audio Compression Manager](http://www.microsoft.com/downloads/details.aspx?familyid=6dfd5405-cabe-4bd7-9330-b6bde1d99194)  
(KB975025)  
(Kritikus)
</td>
<td style="border:1px solid black;">
[Microsoft Windows Media Player 6.4](http://www.microsoft.com/downloads/details.aspx?familyid=13035ef7-7e47-487c-8b7c-7795d33ce7de)  
(Kritikus)
</td>
<td style="border:1px solid black;">
[Microsoft Internet Explorer 5.01 Service Pack 4](http://www.microsoft.com/downloads/details.aspx?familyid=26515c7b-d7a6-4405-96b5-a518dcb39d38)  
(Kritikus)  
[Microsoft Internet Explorer 6 Service Pack 1 szervizcsomaggal](http://www.microsoft.com/downloads/details.aspx?familyid=8154ba37-0fbc-4d31-9d6e-0b21586ad65a)  
(Kritikus)
</td>
<td style="border:1px solid black;">
[Microsoft Windows 2000 Service Pack 4](http://www.microsoft.com/downloads/details.aspx?familyid=edfea805-9544-4dc0-a52c-d7594205657b)  
(Kritikus)
</td>
<td style="border:1px solid black;">
[Microsoft .NET Framework 1.1 Service Pack 1](http://www.microsoft.com/downloads/details.aspx?familyid=78ac8b97-8327-4ae1-8bb0-6cf227f3968f) (KB953297)  
(Kritikus)  
[Microsoft .NET Framework 2.0 Service Pack 1](http://www.microsoft.com/downloads/details.aspx?familyid=d4a328b5-5470-46b0-86c7-cfe0e6a3ea01) (KB953300)  
(Kritikus)  
[Microsoft .NET Framework 2.0 Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=491874d4-5eea-4545-9b7d-3861857c862e) (KB974417)  
(Kritikus)
</td>
<td style="border:1px solid black;">
[Microsoft Internet Explorer 6 Service Pack 1](http://www.microsoft.com/downloads/details.aspx?familyid=f3fef608-dafb-4b37-a65a-9cc4ae8e2c4c)  
(KB958869)  
(Kritikus)  
[Microsoft .NET Framework 1.1 Service Pack 1](http://www.microsoft.com/downloads/details.aspx?familyid=ecf78619-80fa-417d-852b-1b5b2cf574e2)  
(KB971108)  
(Fontos)  
[Microsoft .NET Framework 2.0 Service Pack 1](http://www.microsoft.com/downloads/details.aspx?familyid=3e534aa8-29c2-4379-9f57-931a6ff47418)  
(KB971110)  
(Fontos)  
[Microsoft .NET Framework 2.0 Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=e6f5e730-85cc-4c08-a50d-c456b1e9f5bc)  
(KB971111)  
(Fontos)
</td>
<td style="border:1px solid black;">
[Microsoft Windows 2000 Service Pack 4](http://www.microsoft.com/downloads/details.aspx?familyid=7fecd367-aaff-458b-91bc-8925c8e57528)  
(Fontos)
</td>
<td style="border:1px solid black;">
[Microsoft Windows 2000 Service Pack 4](http://www.microsoft.com/downloads/details.aspx?familyid=52b9198d-b65f-467a-a5ab-141e23d64a86)  
(Fontos)
</td>
<td style="border:1px solid black;">
[Microsoft Windows 2000 Service Pack 4](http://www.microsoft.com/downloads/details.aspx?familyid=b34d94b5-b828-4e16-a636-04344c60d945)  
(Fontos)
</td>
<td style="border:1px solid black;">
[Microsoft Windows 2000 Service Pack 4](http://www.microsoft.com/downloads/details.aspx?familyid=bdfa6583-28a2-4d6b-91d2-157a8518b664)  
(Fontos)
</td>
<td style="border:1px solid black;">
Nem érintett
</td>
</tr>
<tr>
<th colspan="13">
Windows XP
</th>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
**Közlemény azonosítója**
</td>
<td style="border:1px solid black;">
[**MS09-050**](http://go.microsoft.com/fwlink/?linkid=163970)
</td>
<td style="border:1px solid black;">
[**MS09-051**](http://go.microsoft.com/fwlink/?linkid=125438)
</td>
<td style="border:1px solid black;">
[**MS09-052**](http://go.microsoft.com/fwlink/?linkid=163913)
</td>
<td style="border:1px solid black;">
[**MS09-054**](http://go.microsoft.com/fwlink/?linkid=163979)
</td>
<td style="border:1px solid black;">
[**MS09-055**](http://technet.microsoft.com/security/bulletin/ms09-055)
</td>
<td style="border:1px solid black;">
[**MS09-061**](http://go.microsoft.com/fwlink/?linkid=160527)
</td>
<td style="border:1px solid black;">
[**MS09-062**](http://go.microsoft.com/fwlink/?linkid=161342)
</td>
<td style="border:1px solid black;">
[**MS09-053**](http://go.microsoft.com/fwlink/?linkid=164004)
</td>
<td style="border:1px solid black;">
[**MS09-056**](http://go.microsoft.com/fwlink/?linkid=163830)
</td>
<td style="border:1px solid black;">
[**MS09-057**](http://go.microsoft.com/fwlink/?linkid=163832)
</td>
<td style="border:1px solid black;">
[**MS09-058**](http://go.microsoft.com/fwlink/?linkid=162442)
</td>
<td style="border:1px solid black;">
[**MS09-059**](http://go.microsoft.com/fwlink/?linkid=163843)
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
Windows XP Service Pack 2 és Windows XP Service Pack 3
</td>
<td style="border:1px solid black;">
Nem érintett
</td>
<td style="border:1px solid black;">
[DirectShow WMA hangkodek](http://www.microsoft.com/downloads/details.aspx?familyid=4fe0dff5-04d9-4409-8d1d-52419537126b)  
(KB969878)  
(Kritikus)  
[Windows Media Audio Voice Decoder](http://www.microsoft.com/downloads/details.aspx?familyid=4516c219-e357-485e-a52b-23dcb8ee49d8)  
(KB954155)  
(Kritikus)  
(csak Windows XP Service Pack 2 rendszerben)  
[Windows Media Audio Voice Decoder](http://www.microsoft.com/downloads/details.aspx?familyid=746d3440-5a6a-421e-9286-7b534a1dfe54)  
(KB954155)  
(Kritikus)  
(csak Windows XP Service Pack 3 rendszerben)  
[Audio Compression Manager](http://www.microsoft.com/downloads/details.aspx?familyid=6ecc7129-8caa-4daf-a8e2-8f3536225fb3)  
(KB975025)  
(Kritikus)
</td>
<td style="border:1px solid black;">
[Microsoft Windows Media Player 6.4](http://www.microsoft.com/downloads/details.aspx?familyid=b2efe1ac-d8d7-41bb-b87d-fc5e22afef0f)  
(Kritikus)
</td>
<td style="border:1px solid black;">
[Microsoft Internet Explorer 6](http://www.microsoft.com/downloads/details.aspx?familyid=9aacf890-afb4-46a7-a13f-dd9fe3c0ca4a)  
(Kritikus)  
[Windows Internet Explorer 7](http://www.microsoft.com/downloads/details.aspx?familyid=dc166dc6-577f-4d8d-94df-dd963233dd85)  
(Kritikus)  
[Windows Internet Explorer 8](http://www.microsoft.com/downloads/details.aspx?familyid=8799159d-df69-49f6-9db5-49147690ce0c)  
(Kritikus)
</td>
<td style="border:1px solid black;">
[Windows XP Service Pack 2 és Windows XP Service Pack 3](http://www.microsoft.com/downloads/details.aspx?familyid=171d43d3-669c-4923-b266-e47591833c05)  
(Kritikus)
</td>
<td style="border:1px solid black;">
[Microsoft .NET Framework 1.0 Service Pack 3](http://www.microsoft.com/downloads/details.aspx?familyid=1bc56c26-1c7c-47e3-94f4-37af7e00392c)  
(KB953295)  
(Kritikus)  
(csak Tablet PC Edition 2005 és Media Center Edition 2005)  
[Microsoft .NET Framework 1.1 Service Pack 1](http://www.microsoft.com/downloads/details.aspx?familyid=78ac8b97-8327-4ae1-8bb0-6cf227f3968f) (KB953297)  
(Kritikus)  
[Microsoft .NET Framework 2.0 Service Pack 1 és Microsoft .NET Framework 3.5](http://www.microsoft.com/downloads/details.aspx?familyid=d4a328b5-5470-46b0-86c7-cfe0e6a3ea01) (KB953300)  
(Kritikus)  
[Microsoft .NET Framework 2.0 Service Pack 2 és Microsoft .NET Framework 3.5 Service Pack 1](http://www.microsoft.com/downloads/details.aspx?familyid=491874d4-5eea-4545-9b7d-3861857c862e) (KB974417)  
(Kritikus)
</td>
<td style="border:1px solid black;">
[Windows XP Service Pack 2 és Windows XP Service Pack 3](http://www.microsoft.com/downloads/details.aspx?familyid=e2acde20-a6d3-4135-b6eb-1214f743d474)  
(Kritikus)
</td>
<td style="border:1px solid black;">
[Windows XP Service Pack 2 és Windows XP Service Pack 3](http://www.microsoft.com/downloads/details.aspx?familyid=2ae0bdd4-f8b2-420a-b1ac-d2cdaa87c828)  
(Fontos)
</td>
<td style="border:1px solid black;">
[Windows XP Service Pack 2 és Windows XP Service Pack 3](http://www.microsoft.com/downloads/details.aspx?familyid=9c5ab624-e37b-418a-a919-d8f652b15679)  
(Fontos)
</td>
<td style="border:1px solid black;">
[Windows XP Service Pack 2 és Windows XP Service Pack 3](http://www.microsoft.com/downloads/details.aspx?familyid=768fd74e-0a2f-4353-ac22-65d0d6321739)  
(Fontos)
</td>
<td style="border:1px solid black;">
[Windows XP Service Pack 2 és Windows XP Service Pack 3](http://www.microsoft.com/downloads/details.aspx?familyid=cece4c55-0756-4357-9d2d-6709e8426068)  
(Fontos)
</td>
<td style="border:1px solid black;">
[Windows XP Service Pack 2 és Windows XP Service Pack 3](http://www.microsoft.com/downloads/details.aspx?familyid=e997ea40-668e-40df-bd50-0ca53437b375)<sup>[1]</sup>
(Fontos)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Windows XP Professional x64 Edition Service Pack 2
</td>
<td style="border:1px solid black;">
Nem érintett
</td>
<td style="border:1px solid black;">
[DirectShow WMA hangkodek](http://www.microsoft.com/downloads/details.aspx?familyid=c116ae9d-e416-4b7d-be75-4b4b2ebcc33a)  
(KB969878)  
(Kritikus)  
[Windows Media Audio Voice Decoder](http://www.microsoft.com/downloads/details.aspx?familyid=4729de51-8fd8-46c6-b4ad-9c9f25202684)  
(KB954155)  
(Kritikus)  
[Windows Media Audio Voice Decoder](http://www.microsoft.com/downloads/details.aspx?familyid=fe0d51b2-345e-4eb7-a036-d8c3f6a683d2) a Windows Media Format SDK 9.5 x64 kiadásában  
(KB954155)  
(Kritikus)  
[Windows Media Audio Voice Decoder](http://www.microsoft.com/downloads/details.aspx?familyid=a866a490-6d3a-4ecd-acf4-770312ba2fd6) a Windows Media Format SDK 11 kiadásában  
(KB954155)  
(Kritikus)  
[Audio Compression Manager](http://www.microsoft.com/downloads/details.aspx?familyid=46daf7c7-1cd3-4f47-9c7a-d5eb6ea7327b)  
(KB975025)  
(Kritikus)
</td>
<td style="border:1px solid black;">
[Microsoft Windows Media Player 6.4](http://www.microsoft.com/downloads/details.aspx?familyid=a9e7dfd8-7ba1-4f14-8e60-92ef00d91467)  
(Kritikus)
</td>
<td style="border:1px solid black;">
[Microsoft Internet Explorer 6](http://www.microsoft.com/downloads/details.aspx?familyid=89a2cf2a-a7a2-4d4b-aa6f-24dde288d500)  
(Kritikus)  
[Windows Internet Explorer 7](http://www.microsoft.com/downloads/details.aspx?familyid=bd54e595-25f2-4839-a838-2a0f809bde2b)  
(Kritikus)  
[Windows Internet Explorer 8](http://www.microsoft.com/downloads/details.aspx?familyid=77b18fc2-e769-47c6-8e72-916716a49e58)  
(Kritikus)
</td>
<td style="border:1px solid black;">
[Windows XP Professional x64 Edition Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=c08623bf-94bc-4c50-8c10-f50fb8448a0b)  
(Kritikus)
</td>
<td style="border:1px solid black;">
[Microsoft .NET Framework 1.1 Service Pack 1](http://www.microsoft.com/downloads/details.aspx?familyid=78ac8b97-8327-4ae1-8bb0-6cf227f3968f) (KB953297)  
(Kritikus)  
[Microsoft .NET Framework 2.0 Service Pack 1 és Microsoft .NET Framework 3.5](http://www.microsoft.com/downloads/details.aspx?familyid=d4a328b5-5470-46b0-86c7-cfe0e6a3ea01) (KB953300)  
(Kritikus)  
[Microsoft .NET Framework 2.0 Service Pack 2 és Microsoft .NET Framework 3.5 Service Pack 1](http://www.microsoft.com/downloads/details.aspx?familyid=491874d4-5eea-4545-9b7d-3861857c862e) (KB974417)  
(Kritikus)
</td>
<td style="border:1px solid black;">
[Windows XP Professional x64 Edition Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=ad92503a-8c91-4d73-98b0-942d7961637d)  
(Kritikus)
</td>
<td style="border:1px solid black;">
[Windows XP Professional x64 Edition Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=819dd2d1-cad5-4784-9baf-185d8a76df5d)  
(Fontos)
</td>
<td style="border:1px solid black;">
[Windows XP Professional x64 Edition Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=ad29696d-4611-4a12-9dfa-74fa6866b759)  
(Fontos)
</td>
<td style="border:1px solid black;">
[Windows XP Professional x64 Edition Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=270ec100-5ba1-4f8c-aa36-105d30ad57bf)  
(Fontos)
</td>
<td style="border:1px solid black;">
[Windows XP Professional x64 Edition Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=5459b7d4-1fab-4a04-ab9d-b8323505c1e2)  
(Fontos)
</td>
<td style="border:1px solid black;">
[Windows XP Professional x64 Edition Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=17008892-7950-44c4-850d-002c8d73495f)<sup>[1]</sup>
(Fontos)
</td>
</tr>
<tr>
<th colspan="13">
Windows Server 2003
</th>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
**Közlemény azonosítója**
</td>
<td style="border:1px solid black;">
[**MS09-050**](http://go.microsoft.com/fwlink/?linkid=163970)
</td>
<td style="border:1px solid black;">
[**MS09-051**](http://go.microsoft.com/fwlink/?linkid=125438)
</td>
<td style="border:1px solid black;">
[**MS09-052**](http://go.microsoft.com/fwlink/?linkid=163913)
</td>
<td style="border:1px solid black;">
[**MS09-054**](http://go.microsoft.com/fwlink/?linkid=163979)
</td>
<td style="border:1px solid black;">
[**MS09-055**](http://technet.microsoft.com/security/bulletin/ms09-055)
</td>
<td style="border:1px solid black;">
[**MS09-061**](http://go.microsoft.com/fwlink/?linkid=160527)
</td>
<td style="border:1px solid black;">
[**MS09-062**](http://go.microsoft.com/fwlink/?linkid=161342)
</td>
<td style="border:1px solid black;">
[**MS09-053**](http://go.microsoft.com/fwlink/?linkid=164004)
</td>
<td style="border:1px solid black;">
[**MS09-056**](http://go.microsoft.com/fwlink/?linkid=163830)
</td>
<td style="border:1px solid black;">
[**MS09-057**](http://go.microsoft.com/fwlink/?linkid=163832)
</td>
<td style="border:1px solid black;">
[**MS09-058**](http://go.microsoft.com/fwlink/?linkid=162442)
</td>
<td style="border:1px solid black;">
[**MS09-059**](http://go.microsoft.com/fwlink/?linkid=163843)
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
[**Kritikus**](http://go.microsoft.com/fwlink/?linkid=21140)
</td>
<td style="border:1px solid black;">
[**Kritikus**](http://go.microsoft.com/fwlink/?linkid=21140)
</td>
<td style="border:1px solid black;">
[**Kritikus**](http://go.microsoft.com/fwlink/?linkid=21140)
</td>
<td style="border:1px solid black;">
[**Mérsékelt**](http://go.microsoft.com/fwlink/?linkid=21140)
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
<tr class="alternateRow">
<td style="border:1px solid black;">
Windows Server 2003 Service Pack 2
</td>
<td style="border:1px solid black;">
Nem érintett
</td>
<td style="border:1px solid black;">
[DirectShow WMA hangkodek](http://www.microsoft.com/downloads/details.aspx?familyid=4fe0dff5-04d9-4409-8d1d-52419537126b)  
(KB969878)  
(Kritikus)  
[Windows Media Audio Voice Decoder](http://www.microsoft.com/downloads/details.aspx?familyid=00b3cb86-c9eb-4fbe-987e-2b0d94271d87)  
(KB954155)  
(Kritikus)  
[Audio Compression Manager](http://www.microsoft.com/downloads/details.aspx?familyid=ab1803ff-2371-487f-a7b6-95747c46ba4e)  
(KB975025)  
(Kritikus)
</td>
<td style="border:1px solid black;">
[Microsoft Windows Media Player 6.4](http://www.microsoft.com/downloads/details.aspx?familyid=5f82d01c-573e-425e-b9f2-86a54f377b19)  
(Kritikus)
</td>
<td style="border:1px solid black;">
[Microsoft Internet Explorer 6](http://www.microsoft.com/downloads/details.aspx?familyid=8101625d-ee93-46e5-aec2-3bdbf2d86472)  
(Kritikus)  
[Windows Internet Explorer 7](http://www.microsoft.com/downloads/details.aspx?familyid=4647bcf1-69fb-4ad6-9e03-7bc22d8a914b)  
(Kritikus)  
[Windows Internet Explorer 8](http://www.microsoft.com/downloads/details.aspx?familyid=9eae7eca-1a6f-4397-a6e2-7dda6b9d5276)  
(Kritikus)
</td>
<td style="border:1px solid black;">
[Windows Server 2003 Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=f3249c99-82e4-45dc-a254-28e647e822c8)  
(Mérsékelt)
</td>
<td style="border:1px solid black;">
[Microsoft .NET Framework 1.1 Service Pack 1](http://www.microsoft.com/downloads/details.aspx?familyid=d1b4a58b-f0b1-4400-a6e6-0255b0513bd1) (KB953298)  
(Fontos)  
[Microsoft .NET Framework 2.0 Service Pack 1 és Microsoft .NET Framework 3.5](http://www.microsoft.com/downloads/details.aspx?familyid=d4a328b5-5470-46b0-86c7-cfe0e6a3ea01) (KB953300)  
(Fontos)  
[Microsoft .NET Framework 2.0 Service Pack 2 és Microsoft .NET Framework 3.5 Service Pack 1](http://www.microsoft.com/downloads/details.aspx?familyid=491874d4-5eea-4545-9b7d-3861857c862e) (KB974417)  
(Fontos)
</td>
<td style="border:1px solid black;">
[Windows Server 2003 Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=414466a4-39a0-476d-9a43-ae7674cbd6a0)  
(Kritikus)
</td>
<td style="border:1px solid black;">
[Windows Server 2003 Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=48256ea3-b433-4e84-9019-22300069cfc1)  
(Fontos)
</td>
<td style="border:1px solid black;">
[Windows Server 2003 Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=d170cef9-f5d2-4fcd-997b-e778ad5a6797)  
(Fontos)
</td>
<td style="border:1px solid black;">
[Windows Server 2003 Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=78072164-84d1-44da-8ede-2a9d212d47a9)  
(Fontos)
</td>
<td style="border:1px solid black;">
[Windows Server 2003 Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=1e3f3842-f8fd-4969-a2cf-706db38d7580)  
(Fontos)
</td>
<td style="border:1px solid black;">
[Windows Server 2003 Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=9dff4662-7771-4bdc-87ec-7899d79b3a55)<sup>[1]</sup>
(Fontos)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Windows Server 2003 x64 Edition Service Pack 2
</td>
<td style="border:1px solid black;">
Nem érintett
</td>
<td style="border:1px solid black;">
[DirectShow WMA hangkodek](http://www.microsoft.com/downloads/details.aspx?familyid=c116ae9d-e416-4b7d-be75-4b4b2ebcc33a)  
(KB969878)  
(Kritikus)  
[Windows Media Audio Voice Decoder](http://www.microsoft.com/downloads/details.aspx?familyid=13ba4839-7fa9-4bbb-95f6-3fafb6c49f20)  
(KB954155)  
(Kritikus)  
[Windows Media Audio Voice Decoder](http://www.microsoft.com/downloads/details.aspx?familyid=fe0d51b2-345e-4eb7-a036-d8c3f6a683d2) a Windows Media Format SDK 9.5 x64 kiadásában  
(KB954155)  
(Kritikus)  
[Audio Compression Manager](http://www.microsoft.com/downloads/details.aspx?familyid=46daf7c7-1cd3-4f47-9c7a-d5eb6ea7327b)  
(KB975025)  
(Kritikus)
</td>
<td style="border:1px solid black;">
[Microsoft Windows Media Player 6.4](http://www.microsoft.com/downloads/details.aspx?familyid=65e9036e-2e1b-40ff-a84b-c507107bcce8)  
(Kritikus)
</td>
<td style="border:1px solid black;">
[Microsoft Internet Explorer 6](http://www.microsoft.com/downloads/details.aspx?familyid=2f966053-01eb-4a23-a9d5-71deac2498ea)  
(Kritikus)  
[Windows Internet Explorer 7](http://www.microsoft.com/downloads/details.aspx?familyid=e7d77bd9-8317-42f3-9ad1-a0b8bfa65b53)  
(Kritikus)  
[Windows Internet Explorer 8](http://www.microsoft.com/downloads/details.aspx?familyid=708a549d-11fd-43bf-a6e1-309e3205d59d)  
(Kritikus)
</td>
<td style="border:1px solid black;">
[Windows Server 2003 x64 Edition Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=1ad3f7b3-58d5-4507-ae20-a265e47cee9c)  
(Mérsékelt)
</td>
<td style="border:1px solid black;">
[Microsoft .NET Framework 1.1 Service Pack 1](http://www.microsoft.com/downloads/details.aspx?familyid=78ac8b97-8327-4ae1-8bb0-6cf227f3968f) (KB953297)  
(Fontos)  
[Microsoft .NET Framework 2.0 Service Pack 1 és Microsoft .NET Framework 3.5](http://www.microsoft.com/downloads/details.aspx?familyid=d4a328b5-5470-46b0-86c7-cfe0e6a3ea01) (KB953300)  
(Fontos)  
[Microsoft .NET Framework 2.0 Service Pack 2 és Microsoft .NET Framework 3.5 Service Pack 1](http://www.microsoft.com/downloads/details.aspx?familyid=491874d4-5eea-4545-9b7d-3861857c862e) (KB974417)  
(Fontos)
</td>
<td style="border:1px solid black;">
[Windows Server 2003 x64 Edition Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=eb95e8d9-6ef5-4526-99d2-507e50de049b)  
(Kritikus)
</td>
<td style="border:1px solid black;">
[Windows Server 2003 x64 Edition Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=61bded07-201e-4815-ac1e-468bf907e063)  
(Fontos)
</td>
<td style="border:1px solid black;">
[Windows Server 2003 x64 Edition Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=d170cef9-f5d2-4fcd-997b-e778ad5a6797)  
(Fontos)
</td>
<td style="border:1px solid black;">
[Windows Server 2003 x64 Edition Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=8aa1f97d-ad53-4450-bb93-4a147dd10a87)  
(Fontos)
</td>
<td style="border:1px solid black;">
[Windows Server 2003 x64 Edition Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=95286b8d-4b53-4e6c-af59-e9e18fad3559)  
(Fontos)
</td>
<td style="border:1px solid black;">
[Windows Server 2003 x64 Edition Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=8df7a2d9-2f97-4f18-84e8-415a1632cf09)<sup>[1]</sup>
(Fontos)
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
Windows Server 2003 SP2 Itanium alapú rendszerekhez
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
[Microsoft Internet Explorer 6](http://www.microsoft.com/downloads/details.aspx?familyid=79a1a94d-3b47-47e9-9476-2f591c3f6a59)  
(Kritikus)  
[Windows Internet Explorer 7](http://www.microsoft.com/downloads/details.aspx?familyid=07e66c09-2cd7-47ba-bf87-d3da602184b4)  
(Kritikus)
</td>
<td style="border:1px solid black;">
[Windows Server 2003 SP2 javítócsomaggal Itanium alapú rendszerekhez](http://www.microsoft.com/downloads/details.aspx?familyid=575e75d9-e348-4fbb-9eaa-43240e4d715e)  
(Mérsékelt)
</td>
<td style="border:1px solid black;">
[Microsoft .NET Framework 1.1 Service Pack 1](http://www.microsoft.com/downloads/details.aspx?familyid=78ac8b97-8327-4ae1-8bb0-6cf227f3968f) (KB953297)  
(Fontos)  
[Microsoft .NET Framework 2.0 Service Pack 1 és Microsoft .NET Framework 3.5](http://www.microsoft.com/downloads/details.aspx?familyid=d4a328b5-5470-46b0-86c7-cfe0e6a3ea01) (KB953300)  
(Fontos)  
[Microsoft .NET Framework 2.0 Service Pack 2 és Microsoft .NET Framework 3.5 Service Pack 1](http://www.microsoft.com/downloads/details.aspx?familyid=491874d4-5eea-4545-9b7d-3861857c862e) (KB974417)  
(Fontos)
</td>
<td style="border:1px solid black;">
[Windows Server 2003 SP2 javítócsomaggal Itanium alapú rendszerekhez](http://www.microsoft.com/downloads/details.aspx?familyid=a678ceb9-a37a-4c29-8bd1-f209922990e5)  
(Kritikus)
</td>
<td style="border:1px solid black;">
[Windows Server 2003 SP2 javítócsomaggal Itanium alapú rendszerekhez](http://www.microsoft.com/downloads/details.aspx?familyid=b99d4d9b-e0cc-4a8c-ad99-6a53958b37c8)  
(Fontos)
</td>
<td style="border:1px solid black;">
[Windows Server 2003 SP2 javítócsomaggal Itanium alapú rendszerekhez](http://www.microsoft.com/downloads/details.aspx?familyid=2ede1eb9-7f5f-411d-bbc3-5db46d80e0bb)  
(Fontos)
</td>
<td style="border:1px solid black;">
[Windows Server 2003 SP2 javítócsomaggal Itanium alapú rendszerekhez](http://www.microsoft.com/downloads/details.aspx?familyid=fb5678b9-5ef1-42db-902e-c9ea02880e0a)  
(Fontos)
</td>
<td style="border:1px solid black;">
[Windows Server 2003 SP2 javítócsomaggal Itanium alapú rendszerekhez](http://www.microsoft.com/downloads/details.aspx?familyid=faef714b-5f46-47f2-bea7-881df05a1bc0)  
(Fontos)
</td>
<td style="border:1px solid black;">
[Windows Server 2003 SP2 Itanium alapú rendszerekhez](http://www.microsoft.com/downloads/details.aspx?familyid=83c77015-7f96-4c0d-bd56-60aef90ea2f8)<sup>[1]</sup>
(Fontos)
</td>
</tr>
<tr>
<th colspan="13">
Windows Vista
</th>
</tr>
<tr>
<td style="border:1px solid black;">
**Közlemény azonosítója**
</td>
<td style="border:1px solid black;">
[**MS09-050**](http://go.microsoft.com/fwlink/?linkid=163970)
</td>
<td style="border:1px solid black;">
[**MS09-051**](http://go.microsoft.com/fwlink/?linkid=125438)
</td>
<td style="border:1px solid black;">
[**MS09-052**](http://go.microsoft.com/fwlink/?linkid=163913)
</td>
<td style="border:1px solid black;">
[**MS09-054**](http://go.microsoft.com/fwlink/?linkid=163979)
</td>
<td style="border:1px solid black;">
[**MS09-055**](http://technet.microsoft.com/security/bulletin/ms09-055)
</td>
<td style="border:1px solid black;">
[**MS09-061**](http://go.microsoft.com/fwlink/?linkid=160527)
</td>
<td style="border:1px solid black;">
[**MS09-062**](http://go.microsoft.com/fwlink/?linkid=161342)
</td>
<td style="border:1px solid black;">
[**MS09-053**](http://go.microsoft.com/fwlink/?linkid=164004)
</td>
<td style="border:1px solid black;">
[**MS09-056**](http://go.microsoft.com/fwlink/?linkid=163830)
</td>
<td style="border:1px solid black;">
[**MS09-057**](http://go.microsoft.com/fwlink/?linkid=163832)
</td>
<td style="border:1px solid black;">
[**MS09-058**](http://go.microsoft.com/fwlink/?linkid=162442)
</td>
<td style="border:1px solid black;">
[**MS09-059**](http://go.microsoft.com/fwlink/?linkid=163843)
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
<td style="border:1px solid black;">
[**Fontos**](http://go.microsoft.com/fwlink/?linkid=21140)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Windows Vista
</td>
<td style="border:1px solid black;">
[Windows Vista, Windows Vista Service Pack 1, és Windows Vista Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=29842c0c-8930-4b5f-83c6-1a718974b63f)  
(Kritikus)
</td>
<td style="border:1px solid black;">
[Windows Media audiodekódoló](http://www.microsoft.com/downloads/details.aspx?familyid=f17ee0ea-f1e2-49f4-9f90-60296246ddfe)  
(KB954155)  
(Kritikus)
</td>
<td style="border:1px solid black;">
Nem érintett
</td>
<td style="border:1px solid black;">
[Windows Internet Explorer 7](http://www.microsoft.com/downloads/details.aspx?familyid=f6995616-2a84-4c26-9599-26f1314873ed)  
(Kritikus)  
[Windows Internet Explorer 8](http://www.microsoft.com/downloads/details.aspx?familyid=e8f6014f-950b-4e11-a105-51d298069f1a)  
(Kritikus)
</td>
<td style="border:1px solid black;">
[Windows Vista, Windows Vista Service Pack 1, és Windows Vista Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=7313c03b-8844-4086-a0cc-43dfdb3ca48c)  
(Fontos)
</td>
<td style="border:1px solid black;">
[Microsoft .NET Framework 1.1 Service Pack 1](http://www.microsoft.com/downloads/details.aspx?familyid=78ac8b97-8327-4ae1-8bb0-6cf227f3968f) (KB953297)  
(Kritikus)  
[Microsoft .NET Framework 2.0](http://www.microsoft.com/downloads/details.aspx?familyid=6f99521e-86b3-4083-9132-e5ac06d40b63) (KB974468)  
(Kritikus)  
[Microsoft .NET Framework 2.0 Service Pack 1 és Microsoft .NET Framework 3.5](http://www.microsoft.com/downloads/details.aspx?familyid=3cf329c6-6d3d-41eb-bb72-8ba241df0882) (KB974292)  
(Kritikus)  
[Microsoft .NET Framework 2.0 Service Pack 2 és Microsoft .NET Framework 3.5 Service Pack 1](http://www.microsoft.com/downloads/details.aspx?familyid=7438eb1e-6e86-4aa1-b1f4-f71a7699d233) (KB974467)  
(Kritikus)
</td>
<td style="border:1px solid black;">
[Windows Vista és Windows Vista Service Pack 1](http://www.microsoft.com/downloads/details.aspx?familyid=19aa01f3-026d-4264-85f8-216d0597969b)  
(Kritikus)
</td>
<td style="border:1px solid black;">
[Windows Vista, Windows Vista Service Pack 1, és Windows Vista Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=bb96eb1c-66a2-4276-9773-eea22179bcd4)  
(Fontos)
</td>
<td style="border:1px solid black;">
[Windows Vista, Windows Vista Service Pack 1, és Windows Vista Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=8b5a9a95-9439-40c8-acef-000b919daa04)  
(Fontos)
</td>
<td style="border:1px solid black;">
Nem érintett
</td>
<td style="border:1px solid black;">
[Windows Vista és Windows Vista Service Pack 1](http://www.microsoft.com/downloads/details.aspx?familyid=acf6f3e6-282e-4f05-9060-8d0ebb874b97)  
(Fontos)
</td>
<td style="border:1px solid black;">
[Windows Vista, Windows Vista Service Pack 1, és Windows Vista Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=04ae306b-0d0d-4767-ab54-cc11aec477ed)  
(Fontos)
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
Windows Vista Service Pack 1
</td>
<td style="border:1px solid black;">
Ugyanaz, mint fent
</td>
<td style="border:1px solid black;">
Ugyanaz, mint fent
</td>
<td style="border:1px solid black;">
Nem érintett
</td>
<td style="border:1px solid black;">
Ugyanaz, mint fent
</td>
<td style="border:1px solid black;">
Ugyanaz, mint fent
</td>
<td style="border:1px solid black;">
[Microsoft .NET Framework 1.1 Service Pack 1](http://www.microsoft.com/downloads/details.aspx?familyid=78ac8b97-8327-4ae1-8bb0-6cf227f3968f) (KB953297)  
(Kritikus)  
[Microsoft .NET Framework 2.0 Service Pack 1](http://www.microsoft.com/downloads/details.aspx?familyid=30e5410d-0942-4964-9037-52330488efda) (KB974291)  
(Kritikus)  
[Microsoft .NET Framework 2.0 Service Pack 2 és Microsoft .NET Framework 3.5 Service Pack 1](http://www.microsoft.com/downloads/details.aspx?familyid=72fe9066-2397-439d-82fb-2b7f9d2bcce8) (KB974469)  
(Kritikus)
</td>
<td style="border:1px solid black;">
Ugyanaz, mint fent
</td>
<td style="border:1px solid black;">
Ugyanaz, mint fent
</td>
<td style="border:1px solid black;">
Ugyanaz, mint fent
</td>
<td style="border:1px solid black;">
Nem érintett
</td>
<td style="border:1px solid black;">
Ugyanaz, mint fent
</td>
<td style="border:1px solid black;">
Ugyanaz, mint fent
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Windows Vista Service Pack 2
</td>
<td style="border:1px solid black;">
Ugyanaz, mint fent
</td>
<td style="border:1px solid black;">
Ugyanaz, mint fent
</td>
<td style="border:1px solid black;">
Nem érintett
</td>
<td style="border:1px solid black;">
Ugyanaz, mint fent
</td>
<td style="border:1px solid black;">
Ugyanaz, mint fent
</td>
<td style="border:1px solid black;">
[Microsoft .NET Framework 1.1 Service Pack 1](http://www.microsoft.com/downloads/details.aspx?familyid=78ac8b97-8327-4ae1-8bb0-6cf227f3968f) (KB953297)  
(Kritikus)  
[Microsoft .NET Framework 2.0 Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=614a92ee-0512-4ccc-b6b8-32ebcec8e6a4) (KB974470)  
(Kritikus)
</td>
<td style="border:1px solid black;">
Nem érintett
</td>
<td style="border:1px solid black;">
Ugyanaz, mint fent
</td>
<td style="border:1px solid black;">
Ugyanaz, mint fent
</td>
<td style="border:1px solid black;">
Nem érintett
</td>
<td style="border:1px solid black;">
[Windows Vista Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=acf6f3e6-282e-4f05-9060-8d0ebb874b97)  
(Mérsékelt)
</td>
<td style="border:1px solid black;">
Ugyanaz, mint fent
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
Windows Vista x64 Edition
</td>
<td style="border:1px solid black;">
[Windows Vista x64 Edition, Windows Vista x64 Edition Service Pack 1 és Windows Vista x64 Edition Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=62ed5d0a-5ca6-4942-80c9-7808b14cb6b5)  
(Kritikus)
</td>
<td style="border:1px solid black;">
[Windows Media audiodekódoló](http://www.microsoft.com/downloads/details.aspx?familyid=26905f12-92c7-4d45-99e7-227f03d2cb82)  
(KB954155)  
(Kritikus)
</td>
<td style="border:1px solid black;">
Nem érintett
</td>
<td style="border:1px solid black;">
[Windows Internet Explorer 7](http://www.microsoft.com/downloads/details.aspx?familyid=b3de5236-afdd-436e-8648-5382d564cc99)  
(Kritikus)  
[Windows Internet Explorer 8](http://www.microsoft.com/downloads/details.aspx?familyid=85978f28-5fc0-481b-9b03-2021c785889b)  
(Kritikus)
</td>
<td style="border:1px solid black;">
[Windows Vista x64 Edition, Windows Vista x64 Edition Service Pack 1 és Windows Vista x64 Edition Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=7216bcb1-ff16-402b-ad1b-1500d46d0157)  
(Fontos)
</td>
<td style="border:1px solid black;">
[Microsoft .NET Framework 1.1 Service Pack 1](http://www.microsoft.com/downloads/details.aspx?familyid=78ac8b97-8327-4ae1-8bb0-6cf227f3968f) (KB953297)  
(Kritikus)  
[Microsoft .NET Framework 2.0](http://www.microsoft.com/downloads/details.aspx?familyid=6f99521e-86b3-4083-9132-e5ac06d40b63) (KB974468)  
(Kritikus)  
[Microsoft .NET Framework 2.0 Service Pack 1 és Microsoft .NET Framework 3.5](http://www.microsoft.com/downloads/details.aspx?familyid=3cf329c6-6d3d-41eb-bb72-8ba241df0882) (KB974292)  
(Kritikus)  
[Microsoft .NET Framework 2.0 Service Pack 2 és Microsoft .NET Framework 3.5 Service Pack 1](http://www.microsoft.com/downloads/details.aspx?familyid=7438eb1e-6e86-4aa1-b1f4-f71a7699d233) (KB974467)  
(Kritikus)
</td>
<td style="border:1px solid black;">
[Windows Vista x64 Edition és Windows Vista x64 Edition Service Pack 1](http://www.microsoft.com/downloads/details.aspx?familyid=8f5f0c1d-1dd6-47fa-aef2-d3c96c8fc06e)  
(Kritikus)
</td>
<td style="border:1px solid black;">
[Windows Vista x64 Edition, Windows Vista x64 Edition Service Pack 1 és Windows Vista x64 Edition Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=bce096c8-833b-45c8-99cd-1280f0744f2f)  
(Fontos)
</td>
<td style="border:1px solid black;">
[Windows Vista x64 Edition, Windows Vista x64 Edition Service Pack 1 és Windows Vista x64 Edition Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=4a60f789-1a4a-49a8-8d13-fda989ed40be)  
(Fontos)
</td>
<td style="border:1px solid black;">
Nem érintett
</td>
<td style="border:1px solid black;">
[Windows Vista x64 Edition és Windows Vista x64 Edition Service Pack 1](http://www.microsoft.com/downloads/details.aspx?familyid=13a3fe0b-e300-4568-aa08-d586ab8d5434)  
(Fontos)
</td>
<td style="border:1px solid black;">
[Windows Vista x64 Edition, Windows Vista x64 Edition Service Pack 1 és Windows Vista x64 Edition Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=58c995ca-f308-4e07-8e60-2e542384d95d)  
(Fontos)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Windows Vista x64 Edition Service Pack 1
</td>
<td style="border:1px solid black;">
Ugyanaz, mint fent
</td>
<td style="border:1px solid black;">
Ugyanaz, mint fent
</td>
<td style="border:1px solid black;">
Nem érintett
</td>
<td style="border:1px solid black;">
Ugyanaz, mint fent
</td>
<td style="border:1px solid black;">
Ugyanaz, mint fent
</td>
<td style="border:1px solid black;">
[Microsoft .NET Framework 1.1 Service Pack 1](http://www.microsoft.com/downloads/details.aspx?familyid=78ac8b97-8327-4ae1-8bb0-6cf227f3968f) (KB953297)  
(Kritikus)  
[Microsoft .NET Framework 2.0 Service Pack 1](http://www.microsoft.com/downloads/details.aspx?familyid=30e5410d-0942-4964-9037-52330488efda) (KB974291)  
(Kritikus)  
[Microsoft .NET Framework 2.0 Service Pack 2 és Microsoft .NET Framework 3.5 Service Pack 1](http://www.microsoft.com/downloads/details.aspx?familyid=72fe9066-2397-439d-82fb-2b7f9d2bcce8) (KB974469)  
(Kritikus)
</td>
<td style="border:1px solid black;">
Ugyanaz, mint fent
</td>
<td style="border:1px solid black;">
Ugyanaz, mint fent
</td>
<td style="border:1px solid black;">
Ugyanaz, mint fent
</td>
<td style="border:1px solid black;">
Nem érintett
</td>
<td style="border:1px solid black;">
Ugyanaz, mint fent
</td>
<td style="border:1px solid black;">
Ugyanaz, mint fent
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
Windows Vista x64 Edition Service Pack 2
</td>
<td style="border:1px solid black;">
Ugyanaz, mint fent
</td>
<td style="border:1px solid black;">
Ugyanaz, mint fent
</td>
<td style="border:1px solid black;">
Nem érintett
</td>
<td style="border:1px solid black;">
Ugyanaz, mint fent
</td>
<td style="border:1px solid black;">
Ugyanaz, mint fent
</td>
<td style="border:1px solid black;">
[Microsoft .NET Framework 1.1 Service Pack 1](http://www.microsoft.com/downloads/details.aspx?familyid=78ac8b97-8327-4ae1-8bb0-6cf227f3968f) (KB953297)  
(Kritikus)  
[Microsoft .NET Framework 2.0 Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=614a92ee-0512-4ccc-b6b8-32ebcec8e6a4) (KB974470)  
(Kritikus)
</td>
<td style="border:1px solid black;">
Nem érintett
</td>
<td style="border:1px solid black;">
Ugyanaz, mint fent
</td>
<td style="border:1px solid black;">
Ugyanaz, mint fent
</td>
<td style="border:1px solid black;">
Nem érintett
</td>
<td style="border:1px solid black;">
[Windows Vista x64 Edition Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=13a3fe0b-e300-4568-aa08-d586ab8d5434)  
(Mérsékelt)
</td>
<td style="border:1px solid black;">
Ugyanaz, mint fent
</td>
</tr>
<tr>
<th colspan="13">
Windows Server 2008
</th>
</tr>
<tr>
<td style="border:1px solid black;">
**Közlemény azonosítója**
</td>
<td style="border:1px solid black;">
[**MS09-050**](http://go.microsoft.com/fwlink/?linkid=163970)
</td>
<td style="border:1px solid black;">
[**MS09-051**](http://go.microsoft.com/fwlink/?linkid=125438)
</td>
<td style="border:1px solid black;">
[**MS09-052**](http://go.microsoft.com/fwlink/?linkid=163913)
</td>
<td style="border:1px solid black;">
[**MS09-054**](http://go.microsoft.com/fwlink/?linkid=163979)
</td>
<td style="border:1px solid black;">
[**MS09-055**](http://technet.microsoft.com/security/bulletin/ms09-055)
</td>
<td style="border:1px solid black;">
[**MS09-061**](http://go.microsoft.com/fwlink/?linkid=160527)
</td>
<td style="border:1px solid black;">
[**MS09-062**](http://go.microsoft.com/fwlink/?linkid=161342)
</td>
<td style="border:1px solid black;">
[**MS09-053**](http://go.microsoft.com/fwlink/?linkid=164004)
</td>
<td style="border:1px solid black;">
[**MS09-056**](http://go.microsoft.com/fwlink/?linkid=163830)
</td>
<td style="border:1px solid black;">
[**MS09-057**](http://go.microsoft.com/fwlink/?linkid=163832)
</td>
<td style="border:1px solid black;">
[**MS09-058**](http://go.microsoft.com/fwlink/?linkid=162442)
</td>
<td style="border:1px solid black;">
[**MS09-059**](http://go.microsoft.com/fwlink/?linkid=163843)
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
Nincsenek
</td>
<td style="border:1px solid black;">
[**Kritikus**](http://go.microsoft.com/fwlink/?linkid=21140)
</td>
<td style="border:1px solid black;">
[**Alacsony**](http://go.microsoft.com/fwlink/?linkid=21140)
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
Windows Server 2008 32 bites rendszerekhez
</td>
<td style="border:1px solid black;">
[Windows Server 2008 32 bites rendszerekhez és Windows Server 2008 32 bites rendszerekhez, Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=ff6bfcf3-76c9-4c45-b57d-22f94458dd6e)\*  
(Kritikus)
</td>
<td style="border:1px solid black;">
[Windows Media Audio Voice Decoder](http://www.microsoft.com/downloads/details.aspx?familyid=2eaa9857-a147-4f31-9bf4-b9e2cf4c15c3)\*\*  
(KB954155)  
(Kritikus)
</td>
<td style="border:1px solid black;">
Nem érintett
</td>
<td style="border:1px solid black;">
[Windows Internet Explorer 7](http://www.microsoft.com/downloads/details.aspx?familyid=72dd580e-eb53-41da-a5c0-a392ad388bfc)\*\*  
(Kritikus)  
[Windows Internet Explorer 8](http://www.microsoft.com/downloads/details.aspx?familyid=1baf7e96-ba3e-47e7-8ea3-eb092e653a39)\*\*  
(Kritikus)
</td>
<td style="border:1px solid black;">
[Windows Server 2008 32 bites rendszerekhez és Windows Server 2008 32 bites rendszerekhez Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=51eb56fa-8204-45f3-86d7-6d03a2c8d78d)\*\*  
(Alacsony)
</td>
<td style="border:1px solid black;">
[Microsoft .NET Framework 1.1 Service Pack 1](http://www.microsoft.com/downloads/details.aspx?familyid=78ac8b97-8327-4ae1-8bb0-6cf227f3968f)\*\*  
(KB953297)  
(Fontos)  
[Microsoft .NET Framework 2.0 Service Pack 1](http://www.microsoft.com/downloads/details.aspx?familyid=30e5410d-0942-4964-9037-52330488efda)\*\*  
(KB974291)  
(Fontos)  
[Microsoft .NET Framework 2.0 Service Pack 2 és Microsoft .NET Framework 3.5 Service Pack 1](http://www.microsoft.com/downloads/details.aspx?familyid=72fe9066-2397-439d-82fb-2b7f9d2bcce8)\*\*  
(KB974469)  
(Fontos)
</td>
<td style="border:1px solid black;">
[Windows Server 2008 32 bites rendszerekhez](http://www.microsoft.com/downloads/details.aspx?familyid=fd1694af-8873-43aa-9243-91f7cde452b7)\*\*  
(Kritikus)
</td>
<td style="border:1px solid black;">
[Windows Server 2008 32 bites rendszerekhez és Windows Server 2008 32 bites rendszerekhez, Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=d9c5039f-d0cf-4d84-850f-f2f7701dcb79)\*  
(Fontos)
</td>
<td style="border:1px solid black;">
[Windows Server 2008 32 bites rendszerekhez és Windows Server 2008 32 bites rendszerekhez, Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=f9b487af-fe73-42a8-b240-d59c4321f95b)\*  
(Fontos)
</td>
<td style="border:1px solid black;">
Nem érintett
</td>
<td style="border:1px solid black;">
[Windows Server 2008 32 bites rendszerekhez](http://www.microsoft.com/downloads/details.aspx?familyid=71aec6f6-a36b-465e-8885-b094dfd30423)\*  
(Fontos)
</td>
<td style="border:1px solid black;">
[Windows Server 2008 32 bites rendszerekhez és Windows Server 2008 32 bites rendszerekhez, Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=f2f617c2-f149-4e9b-bfdd-08ed0f3f99db)\*  
(Fontos)
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
Windows Server 2008 32 bites rendszerekhez, Service Pack 2\*
</td>
<td style="border:1px solid black;">
Ugyanaz, mint fent
</td>
<td style="border:1px solid black;">
Ugyanaz, mint fent
</td>
<td style="border:1px solid black;">
Nem érintett
</td>
<td style="border:1px solid black;">
Ugyanaz, mint fent
</td>
<td style="border:1px solid black;">
Ugyanaz, mint fent
</td>
<td style="border:1px solid black;">
[Microsoft .NET Framework 1.1 Service Pack 1](http://www.microsoft.com/downloads/details.aspx?familyid=78ac8b97-8327-4ae1-8bb0-6cf227f3968f)\*\*  
(KB953297)  
(Fontos)  
[Microsoft .NET Framework 2.0 Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=614a92ee-0512-4ccc-b6b8-32ebcec8e6a4)\*\*  
(KB974470)  
(Fontos)
</td>
<td style="border:1px solid black;">
Nem érintett
</td>
<td style="border:1px solid black;">
Ugyanaz, mint fent
</td>
<td style="border:1px solid black;">
Ugyanaz, mint fent
</td>
<td style="border:1px solid black;">
Nem érintett
</td>
<td style="border:1px solid black;">
[Windows Server 2008 32 bites rendszerekhez, Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=71aec6f6-a36b-465e-8885-b094dfd30423)\*  
(Mérsékelt)
</td>
<td style="border:1px solid black;">
Ugyanaz, mint fent
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Windows Server 2008 x64 alapú rendszerekhez
</td>
<td style="border:1px solid black;">
[Windows Server 2008 x64 alapú rendszerekhez és Windows Server 2008 x64 alapú rendszerekhez, Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=aff6f9c7-4a72-48f2-b750-204d796c7daa)\*  
(Kritikus)
</td>
<td style="border:1px solid black;">
[Windows Media Audio Voice Decoder](http://www.microsoft.com/downloads/details.aspx?familyid=70aabba3-53d6-4b52-be83-6d3f3869ecbd)\*\*  
(KB954155)  
(Kritikus)
</td>
<td style="border:1px solid black;">
Nem érintett
</td>
<td style="border:1px solid black;">
[Windows Internet Explorer 7](http://www.microsoft.com/downloads/details.aspx?familyid=0111d741-bda4-4a50-a12b-d3337ff4441d)\*\*  
(Kritikus)  
[Windows Internet Explorer 8](http://www.microsoft.com/downloads/details.aspx?familyid=7a4b755b-7fa0-43aa-8862-c1d0c7d94c2c)\*\*  
(Kritikus)
</td>
<td style="border:1px solid black;">
[Windows Server 2008 x64 alapú rendszerekhez és Windows Server 2008 x64 alapú rendszerekhez Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=131b047a-ae93-4a99-83e5-71d5a79e96ea)\*\*  
(Alacsony)
</td>
<td style="border:1px solid black;">
[Microsoft .NET Framework 1.1 Service Pack 1](http://www.microsoft.com/downloads/details.aspx?familyid=78ac8b97-8327-4ae1-8bb0-6cf227f3968f)\*\*  
(KB953297)  
(Fontos)  
[Microsoft .NET Framework 2.0 Service Pack 1](http://www.microsoft.com/downloads/details.aspx?familyid=30e5410d-0942-4964-9037-52330488efda)\*\*  
(KB974291)  
(Fontos)  
[Microsoft .NET Framework 2.0 Service Pack 2 és Microsoft .NET Framework 3.5 Service Pack 1](http://www.microsoft.com/downloads/details.aspx?familyid=72fe9066-2397-439d-82fb-2b7f9d2bcce8)\*\*  
(KB974469)  
(Fontos)
</td>
<td style="border:1px solid black;">
[Windows Server 2008 x64-alapú rendszerekhez](http://www.microsoft.com/downloads/details.aspx?familyid=41bc4cdb-273a-4a6e-80d9-c8ce20e32da9)\*\*  
(Kritikus)
</td>
<td style="border:1px solid black;">
[Windows Server 2008 x64 alapú rendszerekhez és Windows Server 2008 x64 alapú rendszerekhez, Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=db969ddc-708e-42b7-9956-6c27bf346bbb)\*  
(Fontos)
</td>
<td style="border:1px solid black;">
[Windows Server 2008 x64 alapú rendszerekhez és Windows Server 2008 x64 alapú rendszerekhez, Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=0d8a2a3e-d7d4-47fb-8364-16fce28e4d38)\*  
(Fontos)
</td>
<td style="border:1px solid black;">
Nem érintett
</td>
<td style="border:1px solid black;">
[Windows Server 2008 x64 alapú rendszerekhez](http://www.microsoft.com/downloads/details.aspx?familyid=88f4189f-71fe-404a-869e-3f76692acf94)\*  
(Fontos)
</td>
<td style="border:1px solid black;">
[Windows Server 2008 x64 alapú rendszerekhez és Windows Server 2008 x64 alapú rendszerekhez, Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=deb84cb8-2ba3-47e3-9185-2bbc5b0a7e18)\*  
(Fontos)
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
Windows Server 2008 x64 alapú rendszerekhez, Service Pack 2\*
</td>
<td style="border:1px solid black;">
Ugyanaz, mint fent
</td>
<td style="border:1px solid black;">
Ugyanaz, mint fent
</td>
<td style="border:1px solid black;">
Nem érintett
</td>
<td style="border:1px solid black;">
Ugyanaz, mint fent
</td>
<td style="border:1px solid black;">
Ugyanaz, mint fent
</td>
<td style="border:1px solid black;">
[Microsoft .NET Framework 1.1 Service Pack 1](http://www.microsoft.com/downloads/details.aspx?familyid=78ac8b97-8327-4ae1-8bb0-6cf227f3968f)\*\*  
(KB953297)  
(Fontos)  
[Microsoft .NET Framework 2.0 Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=614a92ee-0512-4ccc-b6b8-32ebcec8e6a4)\*\*  
(KB974470)  
(Fontos)
</td>
<td style="border:1px solid black;">
Nem érintett
</td>
<td style="border:1px solid black;">
Ugyanaz, mint fent
</td>
<td style="border:1px solid black;">
Ugyanaz, mint fent
</td>
<td style="border:1px solid black;">
Nem érintett
</td>
<td style="border:1px solid black;">
[Windows Server 2008 x64 alapú rendszerekhez, Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=88f4189f-71fe-404a-869e-3f76692acf94)\*  
(Mérsékelt)
</td>
<td style="border:1px solid black;">
Ugyanaz, mint fent
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Windows Server 2008 Itanium alapú rendszerekhez
</td>
<td style="border:1px solid black;">
[Windows Server 2008 Itanium alapú rendszerekhez és Windows Server 2008 Itanium alapú rendszerekhez, Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=7b70108b-7f59-4898-ab4e-76be990de878)  
(Kritikus)
</td>
<td style="border:1px solid black;">
Nem érintett
</td>
<td style="border:1px solid black;">
Nem érintett
</td>
<td style="border:1px solid black;">
[Windows Internet Explorer 7](http://www.microsoft.com/downloads/details.aspx?familyid=e81f30b7-ef05-4488-b62a-d330e17129cf)  
(Kritikus)
</td>
<td style="border:1px solid black;">
[Windows Server 2008 Itanium alapú rendszerekhez és Windows Server 2008 Itanium alapú rendszerekhez, Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=3d16c5bf-ee5c-4220-9755-5cb92eac2aae)  
(Alacsony)
</td>
<td style="border:1px solid black;">
[Microsoft .NET Framework 1.1 Service Pack 1](http://www.microsoft.com/downloads/details.aspx?familyid=78ac8b97-8327-4ae1-8bb0-6cf227f3968f)  
(KB953297)  
(Fontos)  
[Microsoft .NET Framework 2.0 Service Pack 1](http://www.microsoft.com/downloads/details.aspx?familyid=30e5410d-0942-4964-9037-52330488efda)  
(KB974291)  
(Fontos)  
[Microsoft .NET Framework 2.0 Service Pack 2 és Microsoft .NET Framework 3.5 Service Pack 1](http://www.microsoft.com/downloads/details.aspx?familyid=72fe9066-2397-439d-82fb-2b7f9d2bcce8)  
(KB974469)  
(Fontos)
</td>
<td style="border:1px solid black;">
[Windows Server 2008 Itanium alapú rendszerekhez](http://www.microsoft.com/downloads/details.aspx?familyid=a4f42085-1cb9-4b8d-a931-85be71fdf06d)  
(Kritikus)
</td>
<td style="border:1px solid black;">
[Windows Server 2008 Itanium alapú rendszerekhez és Windows Server 2008 Itanium alapú rendszerekhez, Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=a221451a-cb4e-4a43-a225-4b1e86e87525)  
(Fontos)
</td>
<td style="border:1px solid black;">
[Windows Server 2008 Itanium alapú rendszerekhez és Windows Server 2008 Itanium alapú rendszerekhez, Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=8962f0b6-f346-4e88-9d83-4d15b699dd9d)  
(Fontos)
</td>
<td style="border:1px solid black;">
Nem érintett
</td>
<td style="border:1px solid black;">
[Windows Server 2008 Itanium alapú rendszerekhez](http://www.microsoft.com/downloads/details.aspx?familyid=3e0f0b1c-ca5d-43fc-9770-73396a5f191c)  
(Fontos)
</td>
<td style="border:1px solid black;">
[Windows Server 2008 Itanium alapú rendszerekhez és Windows Server 2008 Itanium alapú rendszerekhez, Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=4aac0e3e-9b49-4a4a-ab17-707ff03b4d9b)  
(Fontos)
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
Windows Server 2008 Itanium alapú rendszerekhez, Service Pack 2
</td>
<td style="border:1px solid black;">
Ugyanaz, mint fent
</td>
<td style="border:1px solid black;">
Nem érintett
</td>
<td style="border:1px solid black;">
Nem érintett
</td>
<td style="border:1px solid black;">
Ugyanaz, mint fent
</td>
<td style="border:1px solid black;">
Ugyanaz, mint fent
</td>
<td style="border:1px solid black;">
[Microsoft .NET Framework 1.1 Service Pack 1](http://www.microsoft.com/downloads/details.aspx?familyid=78ac8b97-8327-4ae1-8bb0-6cf227f3968f)  
(KB953297)  
(Fontos)  
[Microsoft .NET Framework 2.0 Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=614a92ee-0512-4ccc-b6b8-32ebcec8e6a4)  
(KB974470)  
(Fontos)
</td>
<td style="border:1px solid black;">
Nem érintett
</td>
<td style="border:1px solid black;">
Ugyanaz, mint fent
</td>
<td style="border:1px solid black;">
Ugyanaz, mint fent
</td>
<td style="border:1px solid black;">
Nem érintett
</td>
<td style="border:1px solid black;">
[Windows Server 2008 Itanium-alapú rendszerekhez, Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=3e0f0b1c-ca5d-43fc-9770-73396a5f191c)  
(Mérsékelt)
</td>
<td style="border:1px solid black;">
Ugyanaz, mint fent
</td>
</tr>
<tr>
<th colspan="13">
Windows 7
</th>
</tr>
<tr>
<td style="border:1px solid black;">
**Közlemény azonosítója**
</td>
<td style="border:1px solid black;">
[**MS09-050**](http://go.microsoft.com/fwlink/?linkid=163970)
</td>
<td style="border:1px solid black;">
[**MS09-051**](http://go.microsoft.com/fwlink/?linkid=125438)
</td>
<td style="border:1px solid black;">
[**MS09-052**](http://go.microsoft.com/fwlink/?linkid=163913)
</td>
<td style="border:1px solid black;">
[**MS09-054**](http://go.microsoft.com/fwlink/?linkid=163979)
</td>
<td style="border:1px solid black;">
[**MS09-055**](http://technet.microsoft.com/security/bulletin/ms09-055)
</td>
<td style="border:1px solid black;">
[**MS09-061**](http://go.microsoft.com/fwlink/?linkid=160527)
</td>
<td style="border:1px solid black;">
[**MS09-062**](http://go.microsoft.com/fwlink/?linkid=161342)
</td>
<td style="border:1px solid black;">
[**MS09-053**](http://go.microsoft.com/fwlink/?linkid=164004)
</td>
<td style="border:1px solid black;">
[**MS09-056**](http://go.microsoft.com/fwlink/?linkid=163830)
</td>
<td style="border:1px solid black;">
[**MS09-057**](http://go.microsoft.com/fwlink/?linkid=163832)
</td>
<td style="border:1px solid black;">
[**MS09-058**](http://go.microsoft.com/fwlink/?linkid=162442)
</td>
<td style="border:1px solid black;">
[**MS09-059**](http://go.microsoft.com/fwlink/?linkid=163843)
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
**Összesített súlyossági besorolás**
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
[**Fontos**](http://go.microsoft.com/fwlink/?linkid=21140)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Windows 7 32 bites rendszerekhez
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
[Windows Internet Explorer 8](http://www.microsoft.com/downloads/details.aspx?familyid=89d1fb78-68cd-48dd-afc2-15a79ebe9fde)  
(Kritikus)
</td>
<td style="border:1px solid black;">
[Windows 7 32 bites rendszerekhez](http://www.microsoft.com/downloads/details.aspx?familyid=b64bcc14-38a7-45b9-8f85-acc573777506)  
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
[Windows 7 32 bites rendszerekhez](http://www.microsoft.com/downloads/details.aspx?familyid=ad6f06d5-27db-445d-a8b2-c42adc90afc0)  
(Fontos)
</td>
<td style="border:1px solid black;">
Nem érintett
</td>
<td style="border:1px solid black;">
Nem érintett
</td>
<td style="border:1px solid black;">
[Windows 7 32 bites rendszerekhez](http://www.microsoft.com/downloads/details.aspx?familyid=35b85783-90df-4f67-a3cb-02351432133e)  
(Fontos)
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
Windows 7 x64 alapú rendszerekhez
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
[Windows Internet Explorer 8](http://www.microsoft.com/downloads/details.aspx?familyid=10d9f7ac-65f4-437c-91cc-171632c69b0e)  
(Kritikus)
</td>
<td style="border:1px solid black;">
[Windows 7 x64 alapú rendszerekhez](http://www.microsoft.com/downloads/details.aspx?familyid=809e29f3-ec68-4a2b-b04e-11759dd16001)  
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
[Windows 7 x64 alapú rendszerekhez](http://www.microsoft.com/downloads/details.aspx?familyid=70cd0270-77e9-492a-82d9-798364640c10)  
(Fontos)
</td>
<td style="border:1px solid black;">
Nem érintett
</td>
<td style="border:1px solid black;">
Nem érintett
</td>
<td style="border:1px solid black;">
[Windows 7 x64 alapú rendszerekhez](http://www.microsoft.com/downloads/details.aspx?familyid=97010f2c-6c10-4fda-84fd-6c8749968db5)  
(Fontos)
</td>
</tr>
<tr>
<th colspan="13">
Windows Server 2008 R2
</th>
</tr>
<tr>
<td style="border:1px solid black;">
**Közlemény azonosítója**
</td>
<td style="border:1px solid black;">
[**MS09-050**](http://go.microsoft.com/fwlink/?linkid=163970)
</td>
<td style="border:1px solid black;">
[**MS09-051**](http://go.microsoft.com/fwlink/?linkid=125438)
</td>
<td style="border:1px solid black;">
[**MS09-052**](http://go.microsoft.com/fwlink/?linkid=163913)
</td>
<td style="border:1px solid black;">
[**MS09-054**](http://go.microsoft.com/fwlink/?linkid=163979)
</td>
<td style="border:1px solid black;">
[**MS09-055**](http://technet.microsoft.com/security/bulletin/ms09-055)
</td>
<td style="border:1px solid black;">
[**MS09-061**](http://go.microsoft.com/fwlink/?linkid=160527)
</td>
<td style="border:1px solid black;">
[**MS09-062**](http://go.microsoft.com/fwlink/?linkid=161342)
</td>
<td style="border:1px solid black;">
[**MS09-053**](http://go.microsoft.com/fwlink/?linkid=164004)
</td>
<td style="border:1px solid black;">
[**MS09-056**](http://go.microsoft.com/fwlink/?linkid=163830)
</td>
<td style="border:1px solid black;">
[**MS09-057**](http://go.microsoft.com/fwlink/?linkid=163832)
</td>
<td style="border:1px solid black;">
[**MS09-058**](http://go.microsoft.com/fwlink/?linkid=162442)
</td>
<td style="border:1px solid black;">
[**MS09-059**](http://go.microsoft.com/fwlink/?linkid=163843)
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
**Összesített súlyossági besorolás**
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
[**Kritikus**](http://go.microsoft.com/fwlink/?linkid=21140)
</td>
<td style="border:1px solid black;">
[**Alacsony**](http://go.microsoft.com/fwlink/?linkid=21140)
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
Windows Server 2008 R2 x64 alapú rendszerekhez
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
[Windows Internet Explorer 8](http://www.microsoft.com/downloads/details.aspx?familyid=f50307d6-7869-4996-9ff7-23f87d08994b)\*\*  
(Kritikus)
</td>
<td style="border:1px solid black;">
[Windows Server 2008 R2 x64 alapú rendszerekhez](http://www.microsoft.com/downloads/details.aspx?familyid=bcd2b944-6852-48f2-820b-cce7d195e391)\*\*  
(Alacsony)
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
[Windows Server 2008 R2 x64 alapú rendszerekhez](http://www.microsoft.com/downloads/details.aspx?familyid=ce78c019-ec08-4ec6-abec-334f5ec5cb76)\*  
(Fontos)
</td>
<td style="border:1px solid black;">
Nem érintett
</td>
<td style="border:1px solid black;">
Nem érintett
</td>
<td style="border:1px solid black;">
[Windows Server 2008 R2 x64 alapú rendszerekhez](http://www.microsoft.com/downloads/details.aspx?familyid=597ac3a7-e02d-49a5-9b8e-d097e867acea)\*  
(Fontos)
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
Windows Server 2008 R2 Itanium alapú rendszerekhez
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
[Windows Internet Explorer 8](http://www.microsoft.com/downloads/details.aspx?familyid=9b6a28ae-b3f2-42b0-8209-e3950ec37abb)  
(Kritikus)
</td>
<td style="border:1px solid black;">
[Windows Server 2008 R2 Itanium alapú rendszerekhez](http://www.microsoft.com/downloads/details.aspx?familyid=85e76e55-3766-4ffe-9a18-8655de935b7c)  
(Alacsony)
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
[Windows Server 2008 R2 Itanium alapú rendszerekhez](http://www.microsoft.com/downloads/details.aspx?familyid=6442a77a-3c0d-4beb-b2d2-2885376c2135)  
(Fontos)
</td>
<td style="border:1px solid black;">
Nem érintett
</td>
<td style="border:1px solid black;">
Nem érintett
</td>
<td style="border:1px solid black;">
[Windows Server 2008 R2 Itanium alapú rendszerekhez](http://www.microsoft.com/downloads/details.aspx?familyid=abc94857-37d8-4bb8-ad9e-46e687fca40e)  
(Fontos)
</td>
</tr>
</table>
 
**Megjegyzések a Windows Server 2008 és Windows Server 2008 R2 rendszerhez**

**\*A kiszolgálómag telepítését érinti.** Ez a frissítés ugyanolyan biztonsági besorolás mellett, a megadottak szerint érvényes az Windows Server 2008 és a Windows Server 2008 R2 összes támogatott kiadására, függetlenül attól, hogy a kiszolgálómag-telepítési opcióval telepítették-e. Erről a telepítési opcióról bővebben a [Kiszolgálómag](http://msdn.microsoft.com/en-us/library/ms723891(vs.85).aspx) és a [Kiszolgálómag a Windows Server 2008 R2 rendszerhez](http://msdn.microsoft.com/en-us/library/ee391631(vs.85).aspx) MSDN-cikkekben olvashat. A kiszolgálómag-telepítési opció nem vonatkozik a Windows Server 2008 és a Windows Server 2008 R2 bizonyos kiadásaira; lásd: [A kiszolgálómag-telepítési opciók összehasonlítása](http://www.microsoft.com/windowsserver2008/en/us/compare-core-installation.aspx).

**\*\*A kiszolgálómag-telepítés nem érintett.** A frissítésben tárgyalt biztonsági rések nem érintik a jelzett módon a Windows Server 2008 és a Windows Server 2008 R2 támogatott kiadásait, amennyiben a telepítés a kiszolgálómag-telepítési opció használatával történt. Erről a telepítési opcióról bővebben a [Kiszolgálómag](http://msdn.microsoft.com/en-us/library/ms723891(vs.85).aspx) és a [Kiszolgálómag a Windows Server 2008 R2 rendszerhez](http://msdn.microsoft.com/en-us/library/ee391631(vs.85).aspx) MSDN-cikkekben olvashat. A kiszolgálómag-telepítési opció nem vonatkozik a Windows Server 2008 és a Windows Server 2008 R2 bizonyos kiadásaira; lásd: [A kiszolgálómag-telepítési opciók összehasonlítása](http://www.microsoft.com/windowsserver2008/en/us/compare-core-installation.aspx).

**Megjegyzés az MS09-061 közleményhez**

Az ugyanezen a közlemény azonosító alatt található, további frissített fájlokat illetően lásd még az egyéb szoftverkategóriák részt ebben a fejezetben, **Érintett szoftverek és letöltési helyek**. Ez a közlemény több szoftverkategóriát ölel fel.

**Megjegyzések az MS09-062 közleményhez**

Az ugyanezen a közlemény azonosító alatt található, további frissített fájlokat illetően lásd még az egyéb szoftverkategóriák részt ebben a fejezetben, **Érintett szoftverek és letöltési helyek**. Ez a közlemény több szoftverkategóriát ölel fel.

**Megjegyzés az MS09-059 közleményhez**

<sup>[1]</sup>Ez az operációs rendszer csak akkor érintett, ha telepítették a KB968389, Javított védelem a hitelesítési műveletekhez alkalmazást (lásd [Microsoft Security Advisory 973811](http://technet.microsoft.com/security/advisory/973811)). További tájékoztatásért tekintse meg a Gyakran ismételt kérdések a biztonsági frissítéssel kapcsolatban című részt az [MS09-059](http://go.microsoft.com/fwlink/?linkid=163843) közleményben.

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
[**MS09-060**](http://go.microsoft.com/fwlink/?linkid=160633)
</td>
<td style="border:1px solid black;">
[**MS09-062**](http://go.microsoft.com/fwlink/?linkid=161342)
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
</tr>
<tr>
<td style="border:1px solid black;">
Microsoft Office XP
</td>
<td style="border:1px solid black;">
[Microsoft Outlook 2002 Service Pack 3](http://www.microsoft.com/downloads/details.aspx?familyid=04878c2c-eb97-426f-be08-89036a6799db)  
(KB973702)  
(Kritikus)
</td>
<td style="border:1px solid black;">
[Microsoft Office XP Service Pack 3](http://www.microsoft.com/downloads/details.aspx?familyid=b4ac7fbe-dd19-4940-a576-89a6b7ed602d)<sup>[2]</sup>
(KB974811)  
(Fontos)
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
Microsoft Office 2003
</td>
<td style="border:1px solid black;">
[Microsoft Office Outlook 2003 Service Pack 3](http://www.microsoft.com/downloads/details.aspx?familyid=79e2b2e8-d5e8-4014-b489-720af2b5083d)  
(KB973705)  
(Kritikus)
</td>
<td style="border:1px solid black;">
[Microsoft Office 2003 Service Pack 3](http://www.microsoft.com/downloads/details.aspx?familyid=48752ab4-5928-476d-a8bc-e998d188b1f7)<sup>[3]</sup>
(KB972580)  
(Fontos)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
2007 Microsoft Office rendszer
</td>
<td style="border:1px solid black;">
[Microsoft Office Outlook 2007 Service Pack 1 és Microsoft Office Outlook 2007 Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=d39234a3-c62c-44ba-a626-3179a183ca09)  
(KB972363)  
(Kritikus)
</td>
<td style="border:1px solid black;">
[2007 Microsoft Office System Service Pack 1 és 2007 Microsoft Office System Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=98d7c4ab-f8ca-4806-a609-453fb29b02ec)\[4\]  
(KB972581)  
(Fontos)
</td>
</tr>
<tr>
<th colspan="3">
Egyéb Microsoft Office szoftver
</th>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
**Közlemény azonosítója**
</td>
<td style="border:1px solid black;">
[**MS09-060**](http://go.microsoft.com/fwlink/?linkid=160633)
</td>
<td style="border:1px solid black;">
[**MS09-062**](http://go.microsoft.com/fwlink/?linkid=161342)
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
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
Microsoft Visio
</td>
<td style="border:1px solid black;">
Nem érintett
</td>
<td style="border:1px solid black;">
[Microsoft Visio 2002 Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=920ee70b-c5c1-47b5-8f33-938ffe14eea4)  
(KB975365)  
(Fontos)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Microsoft Office Visio Viewer
</td>
<td style="border:1px solid black;">
Microsoft Visio 2002 Viewer<sup>[1]</sup>
(Kritikus)  
Microsoft Office Visio 2003 Viewer<sup>[1]</sup>
(Kritikus)  
[Microsoft Office Visio Viewer 2007 Service Pack 1 és Microsoft Office Visio Viewer 2007 Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=d20004c5-dd01-459e-8120-5f127e20c085)  
(KB973709)  
(Kritikus)
</td>
<td style="border:1px solid black;">
[Microsoft Office Visio Viewer 2007 Service Pack 1 és Microsoft Office Visio Viewer 2007 Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=98d7c4ab-f8ca-4806-a609-453fb29b02ec)\[4\]  
(KB972581)  
(Fontos)
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
Microsoft Office Project
</td>
<td style="border:1px solid black;">
Nem érintett
</td>
<td style="border:1px solid black;">
[Microsoft Office Project 2002 Service Pack 1](http://www.microsoft.com/downloads/details.aspx?familyid=b4ac7fbe-dd19-4940-a576-89a6b7ed602d)<sup>[2]</sup>
(KB974811)  
(Fontos)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Microsoft Office Word Viewer, Microsoft Office Excel Viewer és Microsoft PowerPoint Viewer
</td>
<td style="border:1px solid black;">
Nem érintett
</td>
<td style="border:1px solid black;">
[Microsoft Word Viewer 2003 Service Pack 3 és Microsoft Office Excel Viewer 2003 Service Pack 3](http://www.microsoft.com/downloads/details.aspx?familyid=48752ab4-5928-476d-a8bc-e998d188b1f7)<sup>[3]</sup>
(KB972580)  
(Fontos)  
[Microsoft Office Excel Viewer Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=98d7c4ab-f8ca-4806-a609-453fb29b02ec)\[4\]  
(KB972581)  
(Fontos)  
[PowerPoint Viewer 2007 Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=98d7c4ab-f8ca-4806-a609-453fb29b02ec)\[4\]  
(KB972581)  
(Fontos)
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
Microsoft Office kompatibilitási csomag a Word, Excel és PowerPoint 2007 fájlformátumokhoz
</td>
<td style="border:1px solid black;">
Nem érintett
</td>
<td style="border:1px solid black;">
[Microsoft Office Compatibility Pack for Word, Excel, and PowerPoint 2007 File Formats Service Pack 1 and Microsoft Office Compatibility Pack for Word, Excel and PowerPoint 2007 File Formats Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=98d7c4ab-f8ca-4806-a609-453fb29b02ec)\[4\]  
(KB972581)  
Fontos)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Microsoft Works
</td>
<td style="border:1px solid black;">
Nem érintett
</td>
<td style="border:1px solid black;">
[Microsoft Works 8.5](http://www.microsoft.com/downloads/details.aspx?familyid=6f96de9a-62d8-428f-9567-51d55c129be6)  
(KB973636)  
(Fontos)
</td>
</tr>
</table>
 
**Megjegyzések az MS09-060 közleményhez**

<sup>[1]</sup>A Microsoft a Microsoft Visio Viewer 2002 és Microsoft Visio Viewer 2003 felhasználóknak azt javasolja, hogy frissítsenek Microsoft Office Visio Viewer 2007 Service Pack 2 verzióra.

**Megjegyzések az MS09-062 közleményhez**

<sup>[2]</sup>Ezek a frissítések azonosak.

<sup>[3]</sup>Ezek a frissítések azonosak.

\[4\]Ezek a frissítések azonosak.

Az ugyanezen a közlemény azonosító alatt található, további frissített fájlokat illetően lásd még az egyéb szoftverkategóriák részt ebben a fejezetben, **Érintett szoftverek és letöltési helyek**. Ez a közlemény több szoftverkategóriát ölel fel.

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
Microsoft SQL Server
</th>
</tr>
<tr>
<td style="border:1px solid black;">
**Közlemény azonosítója**
</td>
<td style="border:1px solid black;">
[**MS09-062**](http://go.microsoft.com/fwlink/?linkid=161342)
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
SQL Server 2000 Reporting Services Service Pack 2
</td>
<td style="border:1px solid black;">
GDR-frissítés  
Nem érintett  
QFE-frissítés:  
[SQL Server 2000 Reporting Services Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=33554f96-5af7-4683-a537-9db293b67b8d)  
(KB970899)  
(Kritikus)
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
SQL Server 2005 Service Pack 2
</td>
<td style="border:1px solid black;">
GDR-frissítés:  
[SQL Server 2005 Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=d971a262-1dfb-498c-a4f3-59fdc1b85d23)<sup>[1]</sup>
(KB970895)  
(Kritikus)  
QFE-frissítés:  
[SQL Server 2005 Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=76d3d653-e9a0-48bc-afae-d3553f7b9235)<sup>[1]</sup>
(KB970896)  
(Kritikus)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
SQL Server 2005 x64 Edition Service Pack 2
</td>
<td style="border:1px solid black;">
GDR-frissítés:  
[SQL Server 2005 x64 Edition Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=d971a262-1dfb-498c-a4f3-59fdc1b85d23)<sup>[1]</sup>
(KB970895)  
(Kritikus)  
QFE-frissítés:  
[SQL Server 2005 x64 Edition Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=76d3d653-e9a0-48bc-afae-d3553f7b9235)<sup>[1]</sup>
(KB970896)  
(Kritikus)
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
SQL Server 2005 Itanium alapú rendszerekhez, Service Pack 2
</td>
<td style="border:1px solid black;">
GDR-frissítés:  
[SQL Server 2005 Itanium alapú rendszerekhez, Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=d971a262-1dfb-498c-a4f3-59fdc1b85d23)<sup>[1]</sup>
(KB970895)  
(Kritikus)  
QFE-frissítés:  
[SQL Server 2005 Itanium alapú rendszerekhez, Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=76d3d653-e9a0-48bc-afae-d3553f7b9235)<sup>[1]</sup>
(KB970896)  
(Kritikus)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
SQL Server 2005 Service Pack 3
</td>
<td style="border:1px solid black;">
GDR-frissítés  
[SQL Server 2005 Service Pack 3](http://www.microsoft.com/downloads/details.aspx?familyid=0d878f4b-71e8-4170-9a14-1bce684811ce)<sup>[2]</sup>
(KB970892)  
(Kritikus)  
QFE-frissítés:  
[SQL Server 2005 Service Pack 3](http://www.microsoft.com/downloads/details.aspx?familyid=e6f307c1-8b21-406e-9c6f-b1a3a1e9a98f)<sup>[2]</sup>
(KB970894)  
(Kritikus)
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
SQL Server 2005 x64 Edition Service Pack 3
</td>
<td style="border:1px solid black;">
GDR-frissítés:  
[SQL Server 2005 x64 Edition Service Pack 3](http://www.microsoft.com/downloads/details.aspx?familyid=0d878f4b-71e8-4170-9a14-1bce684811ce)<sup>[2]</sup>
(KB970892)  
(Kritikus)  
QFE-frissítés:  
[SQL Server 2005 x64 Edition Service Pack 3](http://www.microsoft.com/downloads/details.aspx?familyid=e6f307c1-8b21-406e-9c6f-b1a3a1e9a98f)<sup>[2]</sup>
(KB970894)  
(Kritikus)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
SQL Server 2005 Itanium alapú rendszerekhez, Service Pack 3
</td>
<td style="border:1px solid black;">
GDR-frissítés:  
[SQL Server 2005 Itanium alapú rendszerekhez, Service Pack 3](http://www.microsoft.com/downloads/details.aspx?familyid=0d878f4b-71e8-4170-9a14-1bce684811ce)<sup>[2]</sup>
(KB970892)  
(Kritikus)  
QFE-frissítés:  
[SQL Server 2005 Itanium alapú rendszerekhez, Service Pack 3](http://www.microsoft.com/downloads/details.aspx?familyid=e6f307c1-8b21-406e-9c6f-b1a3a1e9a98f)<sup>[2]</sup>
(KB970894)  
(Kritikus)
</td>
</tr>
</table>
 
**Megjegyzés az MS09-062 közleményhez**

<sup>[1]</sup>A Reporting Services SharePoint szolgáltatástól függő SQL Server 2005 Service Pack 2 felhasználóknak telepíteniük kell a [Microsoft SQL Server 2005 Reporting Services kiegészítőt a Service Pack 2 javítócsomaghoz](http://www.microsoft.com/downloads/details.aspx?familyid=%20f4d4d0ae-e5d4-4ed1-8d78-7137578161ce&displaylang=en) a Microsoft Letöltőközpontból.

<sup>[2]</sup>A Reporting Services SharePoint szolgáltatástól függő SQL Server 2005 Service Pack 3 felhasználóknak telepíteniük kell a [Microsoft SQL Server 2005 Reporting Services kiegészítőt a Service Pack 3 javítócsomaghoz](http://www.microsoft.com/downloads/details.aspx?familyid=%20648766ac-2a35-4238-a3f4-c26d7077f2a9&displaylang=en) a Microsoft Letöltőközpontból.

Az ugyanezen a közlemény azonosító alatt található, további frissített fájlokat illetően lásd még az egyéb szoftverkategóriák részt ebben a fejezetben, **Érintett szoftverek és letöltési helyek**. Ez a közlemény több szoftverkategóriát ölel fel.

#### Microsoft fejlesztői eszközök és szoftver

 
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
Microsoft Silverlight
</th>
</tr>
<tr>
<td style="border:1px solid black;">
**Közlemény azonosítója**
</td>
<td style="border:1px solid black;">
[**MS09-061**](http://go.microsoft.com/fwlink/?linkid=160527)
</td>
<td style="border:1px solid black;">
[**MS09-062**](http://go.microsoft.com/fwlink/?linkid=161342)
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
Nincsenek
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Microsoft Silverlight
</td>
<td style="border:1px solid black;">
[Microsoft Silverlight 2](http://www.microsoft.com/silverlight/get-started/install/default.aspx)<sup>[1]</sup> Mac rendszerre telepítve  
(KB970363)  
(Kritikus)
</td>
<td style="border:1px solid black;">
Nem érintett
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
Microsoft Silverlight
</td>
<td style="border:1px solid black;">
[Microsoft Silverlight 2](http://www.microsoft.com/silverlight/get-started/install/default.aspx)<sup>[1]</sup> bármilyen Microsoft Windows ügyfélkiadásra telepítve  
(KB970363)  
(Kritikus)
</td>
<td style="border:1px solid black;">
Nem érintett
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Microsoft Silverlight
</td>
<td style="border:1px solid black;">
[Microsoft Silverlight 2](http://www.microsoft.com/silverlight/get-started/install/default.aspx)<sup>[1]</sup> a Microsoft Windows kiszolgálók bármilyen kiadására telepítve\*\*  
(KB970363)  
(Mérsékelt)
</td>
<td style="border:1px solid black;">
Nem érintett
</td>
</tr>
<tr>
<th colspan="3">
Microsoft Visual Studio
</th>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
**Közlemény azonosítója**
</td>
<td style="border:1px solid black;">
[**MS09-061**](http://go.microsoft.com/fwlink/?linkid=160527)
</td>
<td style="border:1px solid black;">
[**MS09-062**](http://go.microsoft.com/fwlink/?linkid=161342)
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
Nincsenek
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
Microsoft Visual Studio .NET 2003 Service Pack 1
</td>
<td style="border:1px solid black;">
Nem érintett
</td>
<td style="border:1px solid black;">
[Microsoft Visual Studio .NET 2003 Service Pack 1](http://www.microsoft.com/downloads/details.aspx?familyid=9e3b52d3-b211-4d62-891c-ae8f2e4ffc6c)  
(KB971022)  
(Nincs súlyossági besorolás<sup>[2]</sup>)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Microsoft Visual Studio 2005 Service Pack 1
</td>
<td style="border:1px solid black;">
Nem érintett
</td>
<td style="border:1px solid black;">
[Microsoft Visual Studio 2005 Service Pack 1](http://www.microsoft.com/downloads/details.aspx?familyid=e186aeed-e9d7-4a02-84b3-bbed116ca060)  
(KB971023)  
(Nincs súlyossági besorolás<sup>[2]</sup>)
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
Microsoft Visual Studio 2008
</td>
<td style="border:1px solid black;">
Nem érintett
</td>
<td style="border:1px solid black;">
[Microsoft Visual Studio 2008](http://www.microsoft.com/downloads/details.aspx?familyid=4fa10c93-ce20-43df-a725-ef4c77353747)  
(KB972221)  
(Nincs súlyossági besorolás<sup>[2]</sup>)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Microsoft Visual Studio 2008 Service Pack 1
</td>
<td style="border:1px solid black;">
Nem érintett
</td>
<td style="border:1px solid black;">
[Microsoft Visual Studio 2008 Service Pack 1](http://www.microsoft.com/downloads/details.aspx?familyid=b904dee8-8a26-43f8-8ca9-86ad12cfdb52)  
(KB972222)  
(Nincs súlyossági besorolás<sup>[2]</sup>)
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
Microsoft Visual FoxPro 8.0 Service Pack 1 alkalmazás Windows 2000 Service Pack 4 rendszerre telepítve  
(KB971104)
</td>
<td style="border:1px solid black;">
Nem érintett
</td>
<td style="border:1px solid black;">
[Microsoft Visual FoxPro 8.0 Service Pack 1](http://www.microsoft.com/downloads/details.aspx?familyid=e5d0d515-4b36-4025-bc6f-1c5cdf09e1af)  
Microsoft Windows 2000 Service Pack 4 rendszeren  
(KB971104)  
(Nincs súlyossági besorolás<sup>[2]</sup>)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Microsoft Visual FoxPro 9.0 Service Pack 2 alkalmazás Windows 2000 Service Pack 4 rendszerre telepítve  
(KB971105)
</td>
<td style="border:1px solid black;">
Nem érintett
</td>
<td style="border:1px solid black;">
[Microsoft Visual FoxPro 9.0 Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=2a930f56-59ac-49a6-830f-bfae7c540ec7)  
Microsoft Windows 2000 Service Pack 4 rendszeren  
(KB971105)  
(Nincs súlyossági besorolás<sup>[2]</sup>)
</td>
</tr>
<tr>
<th colspan="3">
Microsoft Report Viewer
</th>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
**Közlemény azonosítója**
</td>
<td style="border:1px solid black;">
[**MS09-061**](http://go.microsoft.com/fwlink/?linkid=160527)
</td>
<td style="border:1px solid black;">
[**MS09-062**](http://go.microsoft.com/fwlink/?linkid=161342)
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
[**Kritikus**](http://go.microsoft.com/fwlink/?linkid=21140)
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
Microsoft Report Viewer 2005 Service Pack 1 Redistributable Package
</td>
<td style="border:1px solid black;">
Nem érintett
</td>
<td style="border:1px solid black;">
[Microsoft Report Viewer 2005 Service Pack 1 Redistributable Package](http://www.microsoft.com/downloads/details.aspx?familyid=0dfaf300-2b53-4678-a779-0d805ddfe538)  
(KB971117)  
(Kritikus)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Microsoft Report Viewer 2008 Redistributable Package
</td>
<td style="border:1px solid black;">
Nem érintett
</td>
<td style="border:1px solid black;">
[Microsoft Report Viewer 2008 Redistributable Package](http://www.microsoft.com/downloads/details.aspx?familyid=42ed040f-cf94-4754-b0b3-c8016fbcbe22)  
(KB971118)  
(Kritikus)
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
Microsoft Report Viewer 2008 Service Pack 1 terjeszthető csomag
</td>
<td style="border:1px solid black;">
Nem érintett
</td>
<td style="border:1px solid black;">
[Microsoft Report Viewer 2008 Redistributable Package Service Pack 1](http://www.microsoft.com/downloads/details.aspx?familyid=6aaa74bd-a46e-4478-b4e1-2063d18d2d42)  
(KB971119)  
(Kritikus)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Microsoft Platform SDK Redistributable: GDI+
</td>
<td style="border:1px solid black;">
Nem érintett
</td>
<td style="border:1px solid black;">
[Microsoft Platform SDK Redistributable: GDI+](http://www.microsoft.com/downloads/details.aspx?familyid=6a63ab9c-df12-4d41-933c-be590feaa05a)  
(KB975337)  
(Nincs súlyossági besorolás<sup>[2]</sup>)
</td>
</tr>
</table>
 
**Megjegyzések az MS09-061 közleményhez**

<sup>[1]</sup>Ez a letöltés a Microsoft Silverlight 2 programot frissíti Microsoft Silverlight 3-ra, ami elhárítja a közleményben leírt biztonsági rést.

**\*\*A kiszolgálómag-telepítés nem érintett.** A frissítésben tárgyalt biztonsági rések nem érintik a jelzett módon a Windows Server 2008 és a Windows Server 2008 R2 támogatott kiadásait, amennyiben a telepítés a kiszolgálómag-telepítési opció használatával történt. Erről a telepítési opcióról bővebben a [Kiszolgálómag](http://msdn.microsoft.com/en-us/library/ms723891(vs.85).aspx) és a [Kiszolgálómag a Windows Server 2008 R2 rendszerhez](http://msdn.microsoft.com/en-us/library/ee391631(vs.85).aspx) MSDN-cikkekben olvashat. A kiszolgálómag-telepítési opció nem vonatkozik a Windows Server 2008 és a Windows Server 2008 R2 bizonyos kiadásaira; lásd: [A kiszolgálómag-telepítési opciók összehasonlítása](http://www.microsoft.com/windowsserver2008/en/us/compare-core-installation.aspx).

Az ugyanezen a közlemény azonosító alatt található, további frissített fájlokat illetően lásd még az egyéb szoftverkategóriák részt ebben a fejezetben, **Érintett szoftverek és letöltési helyek**. Ez a közlemény több szoftverkategóriát ölel fel.

**Megjegyzések az MS09-062 közleményhez**

<sup>[2]</sup>Erre a frissítésre nem vonatkozik súlyossági besorolás, mert a Microsoft ezekre a szoftverekre vonatkozóan nem talált a közleményben tárgyalt biztonsági rések jelentette támadási pontot. Mindazonáltal a rendszer felajánlja a biztonsági frissítést a szoftvert használó fejlesztőknek az alkalmazásaik frissített verzióinak kiadásához.

Az ugyanezen a közlemény azonosító alatt található, további frissített fájlokat illetően lásd még az egyéb szoftverkategóriák részt ebben a fejezetben, **Érintett szoftverek és letöltési helyek**. Ez a közlemény több szoftverkategóriát ölel fel.

#### Microsoft Security Software

 
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
Microsoft Forefront Security
</th>
</tr>
<tr>
<td style="border:1px solid black;">
**Közlemény azonosítója**
</td>
<td style="border:1px solid black;">
[**MS09-062**](http://go.microsoft.com/fwlink/?linkid=161342)
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
Microsoft Forefront Client Security 1.0
</td>
<td style="border:1px solid black;">
[Microsoft Forefront Client Security 1.0](http://www.microsoft.com/downloads/details.aspx?familyid=c0ce624c-8df3-4223-8a7a-5cba4ac334a8)  
Microsoft Windows 2000 Service Pack 4 rendszeren  
(KB975962)  
(Fontos)
</td>
</tr>
</table>
 
**Megjegyzés az MS09-062 közleményhez**

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

A Microsoft Software Update Services (WSUS) szolgáltatással a rendszergazdák gyorsan és megbízható módon telepíthetik központilag a legújabb fontos és biztonsági frissítéseket Windows 2000 és újabb operációs rendszerekhez, Office XP és újabb operációs rendszerekhez, Exchange Server 2003 és SQL Server 2000 Windows 2000 és újabb operációs rendszerekre.

A biztonsági frissítésnek Windows Server Update Services szolgáltatással történő központi telepítéséről a [Windows Server Update Services](http://go.microsoft.com/fwlink/?linkid=50120) webhelyen tudhat meg többet.

**Systems Management Server**

A Microsoft Systems Management Server (SMS) rendszer egy sokoldalúan beállítható vállalati megoldás, amely a frissítések kezelésére szolgál. Az SMS segítségével a rendszergazda megállapíthatja, hogy melyik Windows alapú számítógép szorul biztonsági frissítésre, és ezeket a frissítéseket szabályozott módon, a felhasználók minimális zavarásával központilag telepítheti a vállalat teljes informatikai környezetében. Az SMS, vagyis a System Center Configuration Manager 2007 újabb kiadása immáron elérhető, lásd még: [System Center Configuration Manager 2007](http://technet.microsoft.com/en-us/library/bb735860.aspx). Arról, hogy a rendszergazdák hogyan használhatják a biztonsági frissítések telepítéséhez az SMS 2003 alkalmazást, az [SMS 2003 Security Patch Management](http://go.microsoft.com/fwlink/?linkid=22939) részben olvashat. A biztonsági frissítések felderítéséhez az SMS 2.0 felhasználók a Security Update Inventory Tool (SUIT) eszközt is használhatják. Az SMS-szolgáltatásról bővebben a [Microsoft Systems Management Server](http://go.microsoft.com/fwlink/?linkid=21158) oldalán olvashat.

**Megjegyzés** Az SMS a Microsoft Baseline Security Analyzer eszközön keresztül széles körű támogatást nyújt a biztonsági közlemények frissítéseinek észleléséhez, valamint a frissítések telepítéséhez. Előfordulhat, hogy egyes szoftverfrissítéseket ezek az eszközök nem észlelnek. Az SMS-alkalmazás leltározási szolgáltatásai segítségével a rendszergazdák adott rendszereken hajthatják végre a frissítést. Az eljárással kapcsolatban olvassa el a [szoftverfrissítések telepítése az SMS szoftverelosztó ügynök segítségével](http://go.microsoft.com/fwlink/?linkid=33341) című tájékoztatót. Egyes biztonsági frissítésekhez rendszergazdai jogosultságokra van szükség a számítógép újraindítása után. A rendszergazdák az [SMS 2003 Administration Feature Pack](http://go.microsoft.com/fwlink/?linkid=33387) és az [SMS 2.0 Administration Feature Pack](http://go.microsoft.com/fwlink/?linkid=21161) csomag részét képező Elevated Rights Deployment Tool nevű eszközzel telepíthetik ezeket a frissítéseket.

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

-   [Matthieu Suiche](http://www.msuiche.net/), [Netherlands Forensics Institute](http://www.nederlandsforensischinstituut.nl/), az MS09-050 közleményben leírt probléma jelentéséért
-   Ivan Fratric, [Zero Day Initiative](http://www.zerodayinitiative.com/), és Jun Xie, [McAfee Avert Labs](http://www.avertlabs.com/), az MS09-051 közleményben leírt probléma jelentéséért
-   Vinay Anantharaman, [Adobe Systems, Inc.](http://www.adobe.com/), az MS09-051 közleményben bemutatott probléma jelentéséért
-   Yamata Li, [Palo Alto Networks](http://www.paloaltonetworks.com/), az MS09-052 közleményben ismertetett probléma jelentéséért
-   SkyLined, [Google Inc.](http://www.google.com/), az MS09-054 közleményben bemutatott probléma jelentéséért
-   Mark Dowd, [IBM ISS X-Force](http://www.iss.net/), az MS09-054 közleményben ismertetett egyik probléma jelentéséért
-   [Tippingpoint](http://www.tippingpoint.com/) és [Zero Day Initiative](http://www.zerodayinitiative.com/), az MS09-054 közleményben ismertetett probléma jelentéséért
-   Sam Thomas, eshu.co.uk, a [TippingPoint](http://www.tippingpoint.com/) és a [Zero Day Initiative](http://www.zerodayinitiative.com/) munkatársa, az MS09-054 számú közleményben bemutatott probléma jelentéséért
-   Ian Wright és Jean-Luc Giraud, [Citrix](http://www.citrix.com/), az MS09-056 közleményben ismertetett probléma megoldásában nyújtott segítségéért
-   Dan Kaminsky, [IOActive](http://www.ioactive.com/), az MS09-056 közleményben ismertetett két probléma jelentéséért
-   Yamata Li, [Palo Alto Networks](http://www.paloaltonetworks.com/), az MS09-057 közleményben ismertetett probléma jelentéséért
-   Tavis Ormandy és Neel Mehta, [Google Inc.](http://www.google.com/),az MS09-058 közleményben ismertetett két probléma jelentéséért
-   Az [NSFocus Security Team](http://www.nsfocus.com/) az MS09-058 közleményben leírt probléma jelentéséért.
-   David Dewey, [IBM ISS X-Force](http://www.iss.net/), az MS09-060 közleményben ismertetett probléma jelentéséért
-   Ryan Smith, [VeriSign iDefense Labs](http://labs.idefense.com/), az MS09-060 közleményben bemutatott két probléma jelentéséért
-   [Pavel Minajev](http://int19h.org/), az MS09-061 közleményben bemutatott probléma jelentéséért
-   Jeroen Frijters, [Sumatra](http://www.sumatra.nl/), az MS09-061 közleményben ismertetett probléma jelentéséért
-   Yamata Li, [Palo Alto Networks](http://www.paloaltonetworks.com/), az MS09-062 közleményben ismertetett probléma jelentéséért
-   Thomas Garnier, [SkyRecon](http://www.skyrecon.com/), az MS09-062 közleményben ismertetett egyik probléma jelentéséért
-   Wushi, [VeriSign iDefense Labs](http://labs.idefense.com/), az MS09-062 közleményben bemutatott két probléma jelentéséért
-   Ivan Fratric, [Zero Day Initiative](http://www.zerodayinitiative.com/), az MS09-062 közleményben bemutatott probléma jelentéséért
-   Tavis Ormandy, [Google Inc.](http://www.google.com/), az MS09-062 közleményben bemutatott két probléma jelentéséért
-   Carlo Di Dato (shinnai) az MS09-062 közleményben ismertetett probléma jelentéséért
-   Marsu Pilami, [VeriSign iDefense Labs](http://labs.idefense.com/), az MS09-062 közleményben bemutatott két probléma jelentéséért
-   Carsten H. Eiram, [Secunia](http://secunia.com/), az MS09-062 közleményben ismertetett egyik probléma jelentéséért

#### Terméktámogatás

-   Teszteléssel állapították meg a felsorolt szoftverek egyes verzióinak érintettségét. A többi verzió támogatási életciklusa végére ért. Az egyes szoftververziók támogatási életciklusáról a [Microsoft termékek terméktámogatási életciklusát ismertető webhelyen](http://go.microsoft.com/fwlink/?linkid=21742) talál felvilágosítást.
-   Az Amerikai Egyesült Államokban és Kanada területén élő ügyfelek technikai támogatást kérhetnek a [biztonsági támogatás szolgáltatójától](http://go.microsoft.com/fwlink/?linkid=21131) vagy az 1-866-PCSAFETY telefonszámon. A biztonsági frissítésekkel kapcsolatos hívások ingyenesek. Az elérhető támogatási lehetőségekről további információt talál a [Microsoft segítségnyújtással és támogatással foglalkozó webhelyén](http://support.microsoft.com/).
-   Más országokban a helyi Microsoft-képviseletek nyújtanak támogatást. A biztonsági frissítésekkel kapcsolatos hívások ingyenesek. A [nemzetközi támogatási webhely](http://go.microsoft.com/fwlink/?linkid=21155) felvilágosítást nyújt arról, támogatási kérdéseivel hogyan fordulhat a Microsofthoz.

#### Felelősséget kizáró nyilatkozat

A Microsoft Tudásbázisban leírtak előzetes bejelentés nélkül változhatnak, és a cikkek tartalmáért a Microsoft nem vállal garanciát. A Microsoft egyben elhárít minden kifejezett és értelemszerű garanciát, beleértve az eladhatóságra és az adott célra való alkalmasságra vonatkozó garanciát is. A Microsoft Corporation vagy annak szállítói semmilyen körülmények között nem tehetők felelőssé közvetlen, közvetett, eseti, ok-okozati vagy különleges kárért (beleértve az elmaradt hasznot is), még akkor sem, ha a Microsoft Corporation vagy szállítói tudatában voltak a kár lehetséges voltának. Egyes államok törvényi szabályozása nem teszi lehetővé a véletlen vagy ok-okozati károkért vállalt felelősség korlátozását vagy kizárását, így ezekben az államokban az ez a felelősségkizárás nincs érvényben.

#### Verziók

-   1.0 verzió (2009. október 13.): Összefoglaló közlemény közzététele.
-   1.1 verzió (2009. október 14.): Kijavítottuk a Windows XP x64 Edition Service Pack 2 letöltési hivatkozását az MS09-055 közleményhez.
-   1.2 verzió (2009. október 18.): Módosítottuk az Összefoglalást az MS09-054 közleményhez, hogy segítséget nyújtsunk a Firefox felhasználók számára.
-   2.0 verzió (2009. október 28.): A Microsoft Office Visio Viewer 2007, Microsoft Office Visio Viewer 2007 Service Pack 1 és Microsoft Office Visio Viewer 2007 Service Pack 2 bekerült a Reporting Services SharePoint szolgáltatástól függő SQL Server 2005 felhasználókra vonatkozó MS09-062 közleményben foglalt biztonsági rés által érintett szoftverek táblázatába.
-   3.0 verzió (2009. november 2.): A frissített közleményben már szerepelnek az alkalmazáskompatibilitási problémákra megoldást jelentő gyorsjavítások a MS09-054 közleményhez. Azok a felhasználók, akik ezt a frissítést már telepítették, telepíthetik a Microsoft Tudásbázis 976749 cikkének gyorsjavítását.
-   3.1 verzió (2009. november 4.): Az MS09-060 és az MS09-062 számú közleményben a Microsoft Office Visio Viewer 2007 eredeti kiadásainak érintettként említése téves volt, és törölve lett.
-   4.0 verzió (2009. november 10.): A frissített közlemény tájékoztat a Microsoft Windows 2000 Service Pack 4 rendszeren futó hangtömörítés-kezelő érzékelési problémáját javító frissítés (MS09-051) újrakiadásáról. Ez csak észlelési módosítás; a bináris értékek nem változtak. A rendszerüket sikeresen frissített felhasználóknak nem kell újra telepíteniük a frissítést.
-   4.1 verzió (2010. január 12.): A Microsoft Expression Web, Microsoft Expression Web 2, Microsoft Office Groove 2007 és Microsoft Office Groove 2007 Service Pack 1 kikerült az MS09-062 közleményben ismertetett probléma által érintett szoftverek felsorolásából.
-   4.2 verzió (2010. június 22.): Az MS09-061 közlemény vonatkozásában a .NET Framework 1.1 Service Pack 1 már nem szerepel érintett csomagként Windows 7 és Windows Server 2008 R2 rendszeren.

*Built at 2014-04-18T01:50:00Z-07:00*
