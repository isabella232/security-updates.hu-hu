---
TOCTitle: 'MS09-SEP'
Title: 'Microsoft biztonsági közlemény - összefoglalás, szeptember 2009'
ms:assetid: 'ms09-sep'
ms:contentKeyID: 61227737
ms:mtpsurl: 'https://technet.microsoft.com/hu-HU/library/ms09-sep(v=Security.10)'
author: SharonSears
ms.author: SharonSears
---

Security Bulletin Summary

Microsoft biztonsági közlemény - összefoglalás, szeptember 2009
===============================================================

Közzétéve: 2009. szeptember 8. | Frissítve: 2009. november 10.

**Verzió:** 3.0

Az összefoglaló a 2009. szeptemberében kiadott biztonsági közleményeket összegzi.

A 2009. szeptemberi közlemények kiadása folytán az összefoglaló a 2009. szeptember 3-án kiadott előzetes értesítés helyébe lép. További információk a biztonsági közlemények kiadásáról szóló előzetes értesítés szolgáltatásról lásd: [Előzetes értesítés a Microsoft biztonsági közleményeinek kiadásáról](http://technet.microsoft.com/security/bulletin/advance).

Ha automatikus értesítést szeretne kapni a Microsoft biztonsági közleményeinek megjelenéséről, fizessen elő a [Microsoft Technical Security Notifications](http://go.microsoft.com/fwlink/?linkid=21163) szolgáltatásra.

A közleményekkel kapcsolatos kérdések megválaszolására a Microsoft 2009. szeptember 9-én, csendes-óceáni idő szerint 11 órakor webszemináriumot tart. [Jelentkezzen most a szeptemberi közleményeket bemutató webes szemináriumra](http://msevents.microsoft.com/cui/webcasteventdetails.aspx?eventid=1032407486&eventcategory=4&culture=en-us&countrycode=us). Ezt követően a webes szeminárium igény szerint kerül megrendezésre. További információkért látogasson el a [Microsoft biztonsági közleményeit és a webes szemináriumokat](http://technet.microsoft.com/security/bulletin/summary)bemutató oldalra.

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
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=157304">MS09-045</a></td>
<td style="border:1px solid black;"><strong>A JScript parancsértelmezőben lévő biztonsági rés távolról történő programkódfuttatást tehet lehetővé (971961)</strong><br />
<br />
A biztonsági frissítés egy közvetlenül jelzett biztonsági rést szüntet meg a JScript parancsértelmezőben, mely távoli kódfuttatást tesz lehetővé amennyiben a felhasználó megnyit egy speciálisan létrehozott fájlt vagy megtekint egy speciálisan kialakított weboldalt, amely hibás parancsfájlt hív meg. Ha valamely felhasználó felügyeleti jogosultságokkal bejelentkezett a rendszerbe, akkor a biztonsági rést kihasználó támadó teljes mértékben átveheti az irányítást a számítógép felett, Ezt követően a támadó programokat telepíthet, illetve adatokat tekinthet meg, módosíthat és törölhet, de korlátozás nélküli jogosultságokkal rendelkező új fiókokat is létrehozhat. A kevesebb jogosultsággal bíró fiókkal rendelkező felhasználók esetében kisebb a veszélyeztetettség, mint a rendszergazdai jogosultságokkal rendelkezők esetén</td>
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=21140">Kritikus</a><br />
Távoli kódfuttatás</td>
<td style="border:1px solid black;">Esetleg újra kell indítani a rendszert</td>
<td style="border:1px solid black;">Microsoft Windows</td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=151360">MS09-049</a></td>
<td style="border:1px solid black;"><strong>A Wireless LAN AutoConfig Service biztonsági rése távoli kódfuttatást tehet lehetővé (970710)</strong><br />
<br />
Ez a biztonsági frissítés a Wireless LAN AutoConfig Service közvetlenül jelentett biztonsági rését szünteti meg. A biztonsági rés távoli kódfuttatást tehet lehetővé, ha egy ügyfél vagy kiszolgáló vezeték nélküli hálózati kapcsolat engedélyezésével speciálisan kialakított vezeték nélküli kereteket fogad. Az engedélyezett vezeték nélküli kártya nélküli rendszerek nincsenek kitéve a biztonsági rés kockázatának.</td>
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=21140">Kritikus</a><br />
Távoli kódfuttatás</td>
<td style="border:1px solid black;">Újraindítást igényel</td>
<td style="border:1px solid black;">Microsoft Windows</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=158082">MS09-047</a></td>
<td style="border:1px solid black;"><strong>A Windows Media Format biztonsági rései távoli programkódfuttatást tesznek lehetővé (973812)</strong><br />
<br />
Ez a biztonsági frissítés a Windows Media Format két közvetlenül jelzett biztonsági rését szünteti meg. Bármelyik biztonsági rés távoli kódvégrehajtást tehet lehetővé, ha a felhasználó megnyit egy speciálisan kialakított médiafájlt. Ha valamely felhasználó felügyeleti jogosultságokkal bejelentkezett a rendszerbe, akkor a biztonsági rést kihasználó támadó teljes mértékben átveheti az irányítást a számítógép felett, Ezt követően a támadó programokat telepíthet, illetve adatokat tekinthet meg, módosíthat és törölhet, de korlátozás nélküli jogosultságokkal rendelkező új fiókokat is létrehozhat. A kevesebb jogosultsággal bíró fiókkal rendelkező felhasználók esetében kisebb a veszélyeztetettség, mint a rendszergazdai jogosultságokkal rendelkezők esetén</td>
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=21140">Kritikus</a><br />
Távoli kódfuttatás</td>
<td style="border:1px solid black;">Esetleg újra kell indítani a rendszert</td>
<td style="border:1px solid black;">Microsoft Windows</td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=155978">MS09-048</a></td>
<td style="border:1px solid black;"><strong>A Windows TCP/IP protokolljának biztonsági rései távoli kódfuttatást tehetnek lehetővé (967723)</strong><br />
<br />
Ez a biztonsági frissítés több közvetlenül jelentett biztonsági rés hibáját szünteti meg az átvitelvezérlő protokoll/internetprotokoll (TCP/IP) feldolgozási folyamatában. A biztonsági rések távoli kódfuttatást tesznek lehetővé, ha a támadó speciálisan kialakított TCP-/IP-csomagokat küld a hálózaton keresztül a figyelőszolgáltatással ellátott számítógépre. A tűzfalakra vonatkozó gyakorlati tanácsok, valamint a szabványos alapértelmezett tűzfal-konfigurációk segítséget nyújtanak a hálózatot érő, a szervezet határain kívülről eredő támadások kivédésében. Gyakorlati tanácsként azt javasoljuk, hogy az internetkapcsolattal rendelkező számítógépeken a lehető legkevesebb port legyen megnyitva.</td>
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=21140">Kritikus</a><br />
Távoli kódfuttatás</td>
<td style="border:1px solid black;">Újraindítást igényel</td>
<td style="border:1px solid black;">Microsoft Windows</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=158009">MS09-046</a></td>
<td style="border:1px solid black;"><strong>A DHTML-szerkesztő ActiveX vezérlőjének biztonsági rése távoli programkódfuttatást tehet lehetővé (956844)</strong><br />
<br />
A biztonsági frissítés a DHTML-szerkesztő ActiveX vezérlőjének közvetlenül jelentett biztonsági rését szünteti meg. A támadó a biztonsági rés kihasználásához különlegesen kialakított weboldalt hozhat létre. Ha a felhasználó megtekinti ezt az oldalt, a biztonsági rés távoli kódfuttatást tehet lehetővé. A biztonsági rést kihasználó támadó a bejelentkezett felhasználóval egyező hozzáférést nyer a rendszerhez. A kevesebb jogosultsággal bíró fiókkal rendelkező felhasználók esetében kisebb a veszélyeztetettség, mint a rendszergazdai jogosultságokkal rendelkezők esetén</td>
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=21140">Kritikus</a><br />
Távoli kódfuttatás</td>
<td style="border:1px solid black;">Esetleg újra kell indítani a rendszert</td>
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
  
| Közlemény azonosítója                                     | Közlemény címe                                                                                                 | CVE-azonosító                                                                    | Kihasználhatósági információk értékelése                                                                                 | Fontos megjegyzések                                                                                                  |  
|-----------------------------------------------------------|----------------------------------------------------------------------------------------------------------------|----------------------------------------------------------------------------------|--------------------------------------------------------------------------------------------------------------------------|----------------------------------------------------------------------------------------------------------------------|  
| [MS09-045](http://go.microsoft.com/fwlink/?linkid=157304) | A JScript parancsértelmezőben lévő biztonsági rés távolról történő programkódfuttatást tehet lehetővé (971961) | [CVE-2009-1920](http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2009-1920) | [**1**](http://technet.microsoft.com/en-us/security/cc998259.aspx) - Valószínűleg konzisztens rosszindulatú programkód   | (Nincs)                                                                                                              |  
| [MS09-046](http://go.microsoft.com/fwlink/?linkid=158009) | A DHTML-szerkesztő ActiveX vezérlőjének biztonsági rése távoli programkódfuttatást tehet lehetővé (956844)     | [CVE-2009-2519](http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2009-2519) | [**2**](http://technet.microsoft.com/en-us/security/cc998259.aspx) - Valószínűleg inkonzisztens rosszindulatú programkód | (Nincs)                                                                                                              |  
| [MS09-047](http://go.microsoft.com/fwlink/?linkid=158082) | A Windows Media Format biztonsági rései távoli programkódfuttatást tesznek lehetővé (973812)                   | [CVE-2009-2498](http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2009-2498) | [**1**](http://technet.microsoft.com/en-us/security/cc998259.aspx) - Valószínűleg konzisztens rosszindulatú programkód   | (Nincs)                                                                                                              |  
| [MS09-047](http://go.microsoft.com/fwlink/?linkid=158082) | A Windows Media Format biztonsági rései távoli programkódfuttatást tesznek lehetővé (973812)                   | [CVE-2009-2499](http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2009-2499) | [**1**](http://technet.microsoft.com/en-us/security/cc998259.aspx) - Valószínűleg konzisztens rosszindulatú programkód   | (Nincs)                                                                                                              |  
| [MS09-048](http://go.microsoft.com/fwlink/?linkid=155978) | A Windows TCP/IP protokolljának biztonsági rései távoli programkódfuttatásra adhatnak lehetőséget (967723)     | [CVE-2008-4609](http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2008-4609) | [**3**](http://technet.microsoft.com/en-us/security/cc998259.aspx) - Nem valószínű működő rosszindulatú programkód       | A szolgáltatásmegtagadás memóriahasználattal függ össze.                                                             |  
| [MS09-048](http://go.microsoft.com/fwlink/?linkid=155978) | A Windows TCP/IP protokolljának biztonsági rései távoli programkódfuttatásra adhatnak lehetőséget (967723)     | [CVE-2009-1925](http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2009-1925) | [**2**](http://technet.microsoft.com/en-us/security/cc998259.aspx) - Valószínűleg inkonzisztens rosszindulatú programkód | Elképzelhető működő rosszindulatú programkód, de igen csekély a valószínűsége. A szolgáltatásmegtagadás valószínűbb. |  
| [MS09-048](http://go.microsoft.com/fwlink/?linkid=155978) | A Windows TCP/IP protokolljának biztonsági rései távoli programkódfuttatásra adhatnak lehetőséget (967723)     | [CVE-2009-1926](http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2009-1926) | [**3**](http://technet.microsoft.com/en-us/security/cc998259.aspx) - Nem valószínű működő rosszindulatú programkód       | A szolgáltatásmegtagadás memóriahasználattal függ össze.                                                             |  
| [MS09-049](http://go.microsoft.com/fwlink/?linkid=151360) | A Wireless LAN AutoConfig Service biztonsági rése távoli kódfuttatást tehet lehetővé (970710)                  | [CVE-2009-1132](http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2009-1132) | [**2**](http://technet.microsoft.com/en-us/security/cc998259.aspx) - Valószínűleg inkonzisztens rosszindulatú programkód | A halomvédelmi eljárások megnehezítik a biztonsági rés sikeres kihasználását.                                        |
  
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
</tr>
<tr>
<th colspan="6">
Microsoft Windows 2000  
</th>
</tr>
<tr>
<td style="border:1px solid black;">
**Közlemény azonosítója**
</td>
<td style="border:1px solid black;">
[**MS09-045**](http://go.microsoft.com/fwlink/?linkid=157304)
</td>
<td style="border:1px solid black;">
[**MS09-049**](http://go.microsoft.com/fwlink/?linkid=151360)
</td>
<td style="border:1px solid black;">
[**MS09-047**](http://go.microsoft.com/fwlink/?linkid=158082)
</td>
<td style="border:1px solid black;">
[**MS09-048**](http://go.microsoft.com/fwlink/?linkid=155978)
</td>
<td style="border:1px solid black;">
[**MS09-046**](http://go.microsoft.com/fwlink/?linkid=158009)
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
<td style="border:1px solid black;">
[**Kritikus**](http://go.microsoft.com/fwlink/?linkid=21140)
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
Microsoft Windows 2000 Service Pack 4
</td>
<td style="border:1px solid black;">
[JScript 5.1 és JScript 5.6](http://www.microsoft.com/downloads/details.aspx?familyid=2bb3af8d-f36c-4497-9f48-fc59bcff2583)  
(KB971961)  
(Kritikus)  
[JScript 5.7](http://www.microsoft.com/downloads/details.aspx?familyid=b2773db5-b17d-4b98-b4e2-219b23854abd)  
(KB975542)  
(Kritikus)
</td>
<td style="border:1px solid black;">
Nem érintett
</td>
<td style="border:1px solid black;">
[Windows Media Format Runtime 9.0](http://www.microsoft.com/downloads/details.aspx?familyid=02b9dc42-38c2-44b1-a77c-34854f4a86c4)  
(KB968816)  
(Kritikus)
</td>
<td style="border:1px solid black;">
Microsoft Windows 2000 Service Pack 4<sup>[3]</sup>
(Fontos)
</td>
<td style="border:1px solid black;">
[Microsoft Windows 2000 Service Pack 4](http://www.microsoft.com/downloads/details.aspx?familyid=6dd4b0f8-6b54-49a6-a6df-9420f9fd3333)  
(Kritikus)
</td>
</tr>
<tr>
<th colspan="6">
Windows XP
</th>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
**Közlemény azonosítója**
</td>
<td style="border:1px solid black;">
[**MS09-045**](http://go.microsoft.com/fwlink/?linkid=157304)
</td>
<td style="border:1px solid black;">
[**MS09-049**](http://go.microsoft.com/fwlink/?linkid=151360)
</td>
<td style="border:1px solid black;">
[**MS09-047**](http://go.microsoft.com/fwlink/?linkid=158082)
</td>
<td style="border:1px solid black;">
[**MS09-048**](http://go.microsoft.com/fwlink/?linkid=155978)
</td>
<td style="border:1px solid black;">
[**MS09-046**](http://go.microsoft.com/fwlink/?linkid=158009)
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
Nincsenek
</td>
<td style="border:1px solid black;">
[**Kritikus**](http://go.microsoft.com/fwlink/?linkid=21140)
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
[JScript 5.6 alkalmazás Windows XP Service Pack 2 rendszeren](http://www.microsoft.com/downloads/details.aspx?familyid=0af373b2-2240-4079-a748-a38d1bc06f39)  
(KB971961)  
(Kritikus)  
[JScript 5.7 alkalmazás Windows XP Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=c933377d-e0bc-4334-bc75-029045d7a62a)<sup>[1]</sup> rendszeren  
(KB971961)  
(Kritikus)  
[JScript 5.7 alkalmazás Windows XP Service Pack 3 rendszeren](http://www.microsoft.com/downloads/details.aspx?familyid=c933377d-e0bc-4334-bc75-029045d7a62a)  
(KB971961)  
(Kritikus)  
[JScript 5.8](http://www.microsoft.com/downloads/details.aspx?familyid=992602d8-d857-41cf-b7b1-527afdc1dc0f)<sup>[2]</sup>
(KB971961)  
(Kritikus)
</td>
<td style="border:1px solid black;">
Nem érintett
</td>
<td style="border:1px solid black;">
[Windows Media Format Runtime 9.0, Windows Media Format Runtime 9.5 és Windows Media Format Runtime 11](http://www.microsoft.com/downloads/details.aspx?familyid=6ffc081e-f892-4818-acb9-6d79e15d473c)  
(KB968816)  
(Kritikus)  
(csak Windows XP Service Pack 2 rendszerben)  
[Windows Media Format Runtime 9.0, Windows Media Format Runtime 9.5 és Windows Media Format Runtime 11](http://www.microsoft.com/downloads/details.aspx?familyid=31585f5a-9aaa-40da-b15a-11284b4b800c)  
(KB968816)  
(Kritikus)  
(csak Windows XP Service Pack 3 rendszerben)
</td>
<td style="border:1px solid black;">
Windows XP Service Pack 2 és Windows XP Service Pack 3<sup>[3]</sup>
(Alacsony)
</td>
<td style="border:1px solid black;">
[Windows XP Service Pack 2 és Windows XP Service Pack 3](http://www.microsoft.com/downloads/details.aspx?familyid=8523d5be-88a2-4124-9b02-660f612e2a12)  
(Kritikus)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Windows XP Professional x64 Edition Service Pack 2
</td>
<td style="border:1px solid black;">
[JScript 5.6](http://www.microsoft.com/downloads/details.aspx?familyid=0d671004-da4e-4dbd-a066-861b53b0c59c)  
(KB971961)  
(Kritikus)  
[JScript 5.7](http://www.microsoft.com/downloads/details.aspx?familyid=9aae426d-ee9a-4736-b0a2-e0f8890a6895)<sup>[1]</sup>
(KB971961)  
(Kritikus)  
[JScript 5.8](http://www.microsoft.com/downloads/details.aspx?familyid=00bae02a-64eb-4b91-965f-da2dc987a2ff)<sup>[2]</sup>
(KB971961)  
(Kritikus)
</td>
<td style="border:1px solid black;">
Nem érintett
</td>
<td style="border:1px solid black;">
[Windows Media Format Runtime 9.5](http://www.microsoft.com/downloads/details.aspx?familyid=3780d565-d027-4f54-8fc0-05f5c3c6ba1a)  
(KB968816)  
(Kritikus)  
[Windows Media Format Runtime 9.5 x64 Edition](http://www.microsoft.com/downloads/details.aspx?familyid=ce515188-db3c-4694-85da-177c8f76b68c)  
(KB968816)  
(Kritikus)  
[Windows Media Format Runtime 11](http://www.microsoft.com/downloads/details.aspx?familyid=9a465f92-3067-4a5a-9882-1fc2cf796c99)  
(KB968816)  
(Kritikus)
</td>
<td style="border:1px solid black;">
Windows XP Professional x64 Edition Service Pack 2<sup>[3]</sup>
(Alacsony)
</td>
<td style="border:1px solid black;">
[Windows XP Professional x64 Edition Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=dbc33f6b-61bf-409a-89b5-60002192e0e0)  
(Kritikus)
</td>
</tr>
<tr>
<th colspan="6">
Windows Server 2003
</th>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
**Közlemény azonosítója**
</td>
<td style="border:1px solid black;">
[**MS09-045**](http://go.microsoft.com/fwlink/?linkid=157304)
</td>
<td style="border:1px solid black;">
[**MS09-049**](http://go.microsoft.com/fwlink/?linkid=151360)
</td>
<td style="border:1px solid black;">
[**MS09-047**](http://go.microsoft.com/fwlink/?linkid=158082)
</td>
<td style="border:1px solid black;">
[**MS09-048**](http://go.microsoft.com/fwlink/?linkid=155978)
</td>
<td style="border:1px solid black;">
[**MS09-046**](http://go.microsoft.com/fwlink/?linkid=158009)
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
Nincsenek
</td>
<td style="border:1px solid black;">
[**Kritikus**](http://go.microsoft.com/fwlink/?linkid=21140)
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
[JScript 5.6](http://www.microsoft.com/downloads/details.aspx?familyid=6acc9d2d-b71f-4b5c-9aea-b217b6ae240b)  
(KB971961)  
(Kritikus)  
[JScript 5.7](http://www.microsoft.com/downloads/details.aspx?familyid=6af5d034-fd89-42e2-bc18-d44b7a6b0a85)<sup>[1]</sup>
(KB971961)  
(Kritikus)  
[JScript 5.8](http://www.microsoft.com/downloads/details.aspx?familyid=ecf9f7e2-3104-4de2-8b3d-99dcdcae6e62)<sup>[2]</sup>
(KB971961)  
(Kritikus)
</td>
<td style="border:1px solid black;">
Nem érintett
</td>
<td style="border:1px solid black;">
[Windows Media Format Runtime 9.5](http://www.microsoft.com/downloads/details.aspx?familyid=4ab34e3d-34cb-4e35-a2da-b348ace8a8f7)  
(KB968816)  
(Kritikus)  
[Windows Media Services 9.1](http://www.microsoft.com/downloads/details.aspx?familyid=61cd0581-c36e-4da6-ae95-41609adbe922)  
(KB972554)  
(Kritikus)
</td>
<td style="border:1px solid black;">
[Windows Server 2003 Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=48d82036-2fde-4bb0-a60e-92eed83ddc3f)  
(Fontos)
</td>
<td style="border:1px solid black;">
[Windows Server 2003 Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=7478f73f-dd20-4cfa-a650-4c84f37ada2f)  
(Mérsékelt)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Windows Server 2003 x64 Edition Service Pack 2
</td>
<td style="border:1px solid black;">
[JScript 5.6](http://www.microsoft.com/downloads/details.aspx?familyid=d0de3ab1-73e9-4a09-841f-81ade41a8c81)  
(KB971961)  
(Kritikus)  
[JScript 5.7](http://www.microsoft.com/downloads/details.aspx?familyid=8f48bc05-ffac-4a21-8d21-dd20355cda8a)<sup>[1]</sup>
(KB971961)  
(Kritikus)  
[JScript 5.8](http://www.microsoft.com/downloads/details.aspx?familyid=643f9e2f-2e5b-48dd-b1a0-22ccb633ed18)<sup>[2]</sup>
(KB971961)  
(Kritikus)
</td>
<td style="border:1px solid black;">
Nem érintett
</td>
<td style="border:1px solid black;">
[Windows Media Format Runtime 9.5](http://www.microsoft.com/downloads/details.aspx?familyid=8654ee33-6083-447f-ae5b-43ef8d8b613d)  
(KB968816)  
(Kritikus)  
[Windows Media Format Runtime 9.5 x64 Edition](http://www.microsoft.com/downloads/details.aspx?familyid=ce515188-db3c-4694-85da-177c8f76b68c)  
(KB968816)  
(Kritikus)  
[Windows Media Services 9.1](http://www.microsoft.com/downloads/details.aspx?familyid=67c46f26-e6df-4ba2-9c03-1590b31e454c)  
(KB972554)  
(Kritikus)
</td>
<td style="border:1px solid black;">
[Windows Server 2003 x64 Edition Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=e0298ddf-026e-4137-8197-ed9d9b889825)  
(Fontos)
</td>
<td style="border:1px solid black;">
[Windows Server 2003 x64 Edition Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=88bf502d-1a7c-447a-ac4c-401e1698669b)  
(Mérsékelt)
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
Windows Server 2003 SP2 for Itanium-based Systems
</td>
<td style="border:1px solid black;">
[JScript 5.6](http://www.microsoft.com/downloads/details.aspx?familyid=e78cf021-54f5-4526-b5f0-f781aebf9d72)  
(KB971961)  
(Kritikus)  
[JScript 5.7](http://www.microsoft.com/downloads/details.aspx?familyid=fb1ca290-cea4-49c0-a37e-613a654bff3c)<sup>[1]</sup>
(KB971961)  
(Kritikus)
</td>
<td style="border:1px solid black;">
Nem érintett
</td>
<td style="border:1px solid black;">
Nem érintett
</td>
<td style="border:1px solid black;">
[Windows Server 2003 SP2 javítócsomaggal Itanium alapú rendszerekhez](http://www.microsoft.com/downloads/details.aspx?familyid=c948c4d8-5788-4c1a-9fb6-a969b06a888d)  
(Fontos)
</td>
<td style="border:1px solid black;">
[Windows Server 2003 SP2 javítócsomaggal Itanium alapú rendszerekhez](http://www.microsoft.com/downloads/details.aspx?familyid=8d881ff8-f51f-4476-8cb6-2bebd5b2047f)  
(Mérsékelt)
</td>
</tr>
<tr>
<th colspan="6">
Windows Vista
</th>
</tr>
<tr>
<td style="border:1px solid black;">
**Közlemény azonosítója**
</td>
<td style="border:1px solid black;">
[**MS09-045**](http://go.microsoft.com/fwlink/?linkid=157304)
</td>
<td style="border:1px solid black;">
[**MS09-049**](http://go.microsoft.com/fwlink/?linkid=151360)
</td>
<td style="border:1px solid black;">
[**MS09-047**](http://go.microsoft.com/fwlink/?linkid=158082)
</td>
<td style="border:1px solid black;">
[**MS09-048**](http://go.microsoft.com/fwlink/?linkid=155978)
</td>
<td style="border:1px solid black;">
[**MS09-046**](http://go.microsoft.com/fwlink/?linkid=158009)
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
Nincsenek
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Windows Vista, Windows Vista Service Pack 1 és Windows Vista Service Pack 2
</td>
<td style="border:1px solid black;">
[JScript 5.7](http://www.microsoft.com/downloads/details.aspx?familyid=bcb12e57-f5d6-4b4e-88ab-13c28137f11a)  
(KB971961)  
(Kritikus)  
[JScript 5.8](http://www.microsoft.com/downloads/details.aspx?familyid=80e7390f-df39-4d99-b2e1-01c7f6a951bb)<sup>[2]</sup>
(KB971961)  
(Kritikus)
</td>
<td style="border:1px solid black;">
[Windows Vista, Windows Vista Service Pack 1, és Windows Vista Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=e9fe967f-d78d-43c2-bbcc-5098bd20267e)  
(Kritikus)
</td>
<td style="border:1px solid black;">
[Windows Media Format Runtime 11 és Microsoft Media Foundation](http://www.microsoft.com/downloads/details.aspx?familyid=d2bdefcc-f6b9-47c3-a55d-a4f33f967828)  
(KB968816)  
(Kritikus)
</td>
<td style="border:1px solid black;">
[Windows Vista, Windows Vista Service Pack 1, és Windows Vista Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=7d72f845-9feb-4685-a669-f9d6ab54f9ed)  
(Kritikus)
</td>
<td style="border:1px solid black;">
Nem érintett
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
Windows Vista x64 Edition, Windows Vista x64 Edition Service Pack 1 és Windows Vista x64 Edition Service Pack 2
</td>
<td style="border:1px solid black;">
[JScript 5.7](http://www.microsoft.com/downloads/details.aspx?familyid=8b1b76d5-a6b0-4c2f-8768-e55e82c2c118)  
(KB971961)  
(Kritikus)  
[JScript 5.8](http://www.microsoft.com/downloads/details.aspx?familyid=24457cdd-1973-40c9-9c2d-c1a75fdfa7fa)<sup>[2]</sup>
(KB971961)  
(Kritikus)
</td>
<td style="border:1px solid black;">
[Windows Vista x64 Edition, Windows Vista x64 Edition Service Pack 1 és Windows Vista x64 Edition Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=f93470bd-2e6d-4340-88c6-bb212baf750a)  
(Kritikus)
</td>
<td style="border:1px solid black;">
[Windows Media Format Runtime 11 és Microsoft Media Foundation](http://www.microsoft.com/downloads/details.aspx?familyid=97f00b25-fb8f-4300-80c0-c63179f32182)  
(KB968816)  
(Kritikus)
</td>
<td style="border:1px solid black;">
[Windows Vista x64 Edition, Windows Vista x64 Edition Service Pack 1 és Windows Vista x64 Edition Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=b2930ff1-5f0a-4a5d-bf2a-9fb76dd8da63)  
(Kritikus)
</td>
<td style="border:1px solid black;">
Nem érintett
</td>
</tr>
<tr>
<th colspan="6">
Windows Server 2008
</th>
</tr>
<tr>
<td style="border:1px solid black;">
**Közlemény azonosítója**
</td>
<td style="border:1px solid black;">
[**MS09-045**](http://go.microsoft.com/fwlink/?linkid=157304)
</td>
<td style="border:1px solid black;">
[**MS09-049**](http://go.microsoft.com/fwlink/?linkid=151360)
</td>
<td style="border:1px solid black;">
[**MS09-047**](http://go.microsoft.com/fwlink/?linkid=158082)
</td>
<td style="border:1px solid black;">
[**MS09-048**](http://go.microsoft.com/fwlink/?linkid=155978)
</td>
<td style="border:1px solid black;">
[**MS09-046**](http://go.microsoft.com/fwlink/?linkid=158009)
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
[**Kritikus**](http://go.microsoft.com/fwlink/?linkid=21140)
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
Windows Server 2008 32 bites rendszerekhez és Windows Server 2008 32 bites rendszerekhez, Service Pack 2
</td>
<td style="border:1px solid black;">
[JScript 5.7](http://www.microsoft.com/downloads/details.aspx?familyid=df88e6e5-78d3-4fa6-858d-b935d812cada)\*  
(KB971961)  
(Kritikus)  
[JScript 5.8](http://www.microsoft.com/downloads/details.aspx?familyid=e7b07be6-a4f8-4847-9c55-9b3d2965fa77)\* <sup>[2]</sup>
(KB971961)  
(Kritikus)
</td>
<td style="border:1px solid black;">
[Windows Server 2008 32 bites rendszerekhez és Windows Server 2008 32 bites rendszerekhez Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=ac3f6800-bc3e-4b35-a482-54e1a2da1ab5)\*\*  
(Fontos)
</td>
<td style="border:1px solid black;">
[Windows Media Format Runtime 11 és Microsoft Media Foundation](http://www.microsoft.com/downloads/details.aspx?familyid=9c111bff-aff6-4ff7-81f6-e736cfcbe3ed)\*\*  
(KB968816)  
(Kritikus)  
[Windows Media Services 2008](http://www.microsoft.com/downloads/details.aspx?familyid=2801f69b-37d0-4d0f-9632-31382b824d36)\*  
(KB972554)  
(Kritikus)
</td>
<td style="border:1px solid black;">
[Windows Server 2008 32 bites rendszerekhez és Windows Server 2008 32 bites rendszerekhez, Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=35c1d5a9-a953-4fc6-90c0-d2358c7b89e6)\*  
(Kritikus)
</td>
<td style="border:1px solid black;">
Nem érintett
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
Windows Server 2008 x64 alapú rendszerekhez és Windows Server 2008 x64 alapú rendszerekhez, Service Pack 2
</td>
<td style="border:1px solid black;">
[JScript 5.7](http://www.microsoft.com/downloads/details.aspx?familyid=f584f8ca-f6b1-4285-a44c-3df5e51e75de)\*  
(KB971961)  
(Kritikus)  
[JScript 5.8](http://www.microsoft.com/downloads/details.aspx?familyid=9eddbb89-4178-49c2-836a-2d292fe50936)\* <sup>[2]</sup>
(KB971961)  
(Kritikus)
</td>
<td style="border:1px solid black;">
[Windows Server 2008 x64 alapú rendszerekhez és Windows Server 2008 x64 alapú rendszerekhez Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=7d1b9b4f-bf35-44aa-a660-afb2ef2c9e30)\*\*  
(Fontos)
</td>
<td style="border:1px solid black;">
[Windows Media Format Runtime 11 és Microsoft Media Foundation](http://www.microsoft.com/downloads/details.aspx?familyid=59615c8b-a07f-4326-836d-f17b2fcc4695)\*\*  
(KB968816)  
(Kritikus)  
[Windows Media Services 2008](http://www.microsoft.com/downloads/details.aspx?familyid=7fad3793-174f-46db-9d0a-873a0ea8be65)\*  
(KB972554)  
(Kritikus)
</td>
<td style="border:1px solid black;">
[Windows Server 2008 x64 alapú rendszerekhez és Windows Server 2008 x64 alapú rendszerekhez, Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=6e46822e-f79d-492d-ad01-ee680ad324f5)\*  
(Kritikus)
</td>
<td style="border:1px solid black;">
Nem érintett
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Windows Server 2008 Itanium alapú rendszerekhez és Windows Server 2008 Itanium alapú rendszerekhez, Service Pack 2
</td>
<td style="border:1px solid black;">
[JScript 5.7](http://www.microsoft.com/downloads/details.aspx?familyid=b84fca1d-914d-45af-a48c-d9bc5d20c6b7)  
(KB971961)  
(Kritikus)
</td>
<td style="border:1px solid black;">
Nem érintett
</td>
<td style="border:1px solid black;">
Nem érintett
</td>
<td style="border:1px solid black;">
[Windows Server 2008 Itanium alapú rendszerekhez és Windows Server 2008 Itanium alapú rendszerekhez, Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=2ac76ee2-b1b6-4300-9cba-af33d9dd54eb)  
(Kritikus)
</td>
<td style="border:1px solid black;">
Nem érintett
</td>
</tr>
</table>
 
**Megjegyzések a Windows Server 2008 rendszerhez**

**\*Érinti a Windows Server 2008 kiszolgálómag-telepítését.** A frissítés besorolása ugyanaz a Windows Server 2008 támogatott kiadásain függetlenül attól, hogy a Windows Server 2008 alkalmazást a kiszolgálómag-telepítési opcióval telepítették-e. További tudnivalókat ezzel a telepítési beállítással kapcsolatban a következő weboldalon talál:[Server Core](http://msdn.microsoft.com/en-us/library/ms723891(vs.85).aspx). A Server Core telepítési beállítás a Windows Server 2008 egyes kiadásainál nem alkalmazható. További tudnivalók: [Server Core telepítési beállítások összehasonlítása](http://www.microsoft.com/windowsserver2008/en/us/compare-core-installation.aspx).

**\*\*Nem érinti a Windows Server 2008 kiszolgálómag-telepítését.** A frissítésben tárgyalt biztonsági rések nem érintik a Windows Server 2008 támogatott kiadásait, amennyiben a Windows Server 2008 telepítése a kiszolgálómag-telepítési opció használatával történt. További tudnivalókat ezzel a telepítési beállítással kapcsolatban a következő weboldalon talál:[Server Core](http://msdn.microsoft.com/en-us/library/ms723891(vs.85).aspx). A Server Core telepítési beállítás a Windows Server 2008 egyes kiadásainál nem alkalmazható. További tudnivalók: [Server Core telepítési beállítások összehasonlítása](http://www.microsoft.com/windowsserver2008/en/us/compare-core-installation.aspx).

**Megjegyzések az MS09-045 közleményhez**

<sup>[1]</sup>Az Internet Explorer 7 verzióval telepített rendszereken

<sup>[2]</sup>Az Internet Explorer 8 verzióval telepített rendszereken

**Megjegyzés az MS09-048 közleményhez**

<sup>[3]</sup> Nincs elérhető frissítés. További tájékoztatásért tekintse meg a **Gyakran ismételt kérdések a biztonsági frissítéssel kapcsolatban** című részt az [MS09-048](http://go.microsoft.com/fwlink/?linkid=155978) közleményben.

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

-   Ling és Wushi, [team509](http://www.team509.com/), a Tipping Point [Zero Day Initiative](http://www.zerodayinitiative.com/) programjával együttműködve az MS09-045 közleményben bemutatott egyik probléma jelentéséért
-   Tavis Ormandy, [Google Inc.](http://www.google.com/), az MS09-046 közleményben bemutatott probléma jelentéséért
-   Peter Winter-Smith [(NGS Software)](http://www.ngssoftware.com/) az MS09-047 számú közleményben bemutatott probléma jelentéséért
-   Hiroshi Noguchi az Alice Carroll rajongói klubtól az MS09-047 közleményben leírt probléma jelentéséért
-   Jack C. Louis, [Outpost24](http://www.outpost24.com/), az MS09-048 közleményben ismertetett probléma jelentéséért
-   Fabian Yamaguchi, [Recurity Labs GmbH](http://www.recurity-labs.com/), az MS09-048 közleményben ismertetett probléma jelentéséért

#### Terméktámogatás

-   Teszteléssel állapították meg a felsorolt szoftverek egyes verzióinak érintettségét. A többi verzió támogatási életciklusa végére ért. Az egyes szoftververziók támogatási életciklusáról a [Microsoft termékek terméktámogatási életciklusát ismertető webhelyen](http://go.microsoft.com/fwlink/?linkid=21742) talál felvilágosítást.
-   Az Amerikai Egyesült Államokban és Kanada területén élő ügyfelek technikai támogatást kérhetnek a [biztonsági támogatás szolgáltatójától](http://go.microsoft.com/fwlink/?linkid=21131) vagy az 1-866-PCSAFETY telefonszámon. A biztonsági frissítésekkel kapcsolatos hívások ingyenesek. Az elérhető támogatási lehetőségekről további információt talál a [Microsoft segítségnyújtással és támogatással foglalkozó webhelyén](http://support.microsoft.com/).
-   Más országokban a helyi Microsoft-képviseletek nyújtanak támogatást. A biztonsági frissítésekkel kapcsolatos hívások ingyenesek. A [nemzetközi támogatási webhely](http://go.microsoft.com/fwlink/?linkid=21155) felvilágosítást nyújt arról, támogatási kérdéseivel hogyan fordulhat a Microsofthoz.

#### Felelősséget kizáró nyilatkozat

A Microsoft Tudásbázisban leírtak előzetes bejelentés nélkül változhatnak, és a cikkek tartalmáért a Microsoft nem vállal garanciát. A Microsoft egyben elhárít minden kifejezett és értelemszerű garanciát, beleértve az eladhatóságra és az adott célra való alkalmasságra vonatkozó garanciát is. A Microsoft Corporation vagy annak szállítói semmilyen körülmények között nem tehetők felelőssé közvetlen, közvetett, eseti, ok-okozati vagy különleges kárért (beleértve az elmaradt hasznot is), még akkor sem, ha a Microsoft Corporation vagy szállítói tudatában voltak a kár lehetséges voltának. Egyes államok törvényi szabályozása nem teszi lehetővé a véletlen vagy ok-okozati károkért vállalt felelősség korlátozását vagy kizárását, így ezekben az államokban az ez a felelősségkizárás nincs érvényben.

#### Verziók

-   1.0 verzió (2009. szeptember 8.): Összefoglaló közlemény közzététele.
-   2.0 verzió (2009. szeptember 9.): A Windows XP Service Pack 2, Windows XP Service Pack 3 és Windows XP Professional x64 Edition Service Pack 2 bekerült a MS09-048 közlemény Érintett szoftverek táblázatába. Ezekhez a platformokhoz azonban nincs frissítés. Lásd a **Gyakran ismételt kérdések a biztonsági frissítéssel kapcsolatban** c. részt a MS09-048 közleményben. A felajánlott biztonsági frissítéseket a közlemény nem módosítja.
-   3.0 verzió (2009. november 10.): A Microsoft Windows 2000 Service Pack 4 rendszeren futó JScript 5.7 bekerült az Érintett szoftverek táblázatába az MS09-045 közleményhez.

*Built at 2014-04-18T01:50:00Z-07:00*
