---
TOCTitle: 'MS11-JUL'
Title: 'Microsoft biztonsági közlemény - összefoglalás, július 2011'
ms:assetid: 'ms11-jul'
ms:contentKeyID: 61227755
ms:mtpsurl: 'https://technet.microsoft.com/hu-HU/library/ms11-jul(v=Security.10)'
---

Security Bulletin Summary

Microsoft biztonsági közlemény - összefoglalás, július 2011
===========================================================

Közzétéve: 2011. július 12.

**Verzió:** 1.0

Az összefoglaló a 2011 júliusára kiadott biztonsági közleményeket összegzi.

A 2011. júliusi biztonsági közlemények kiadása folytán az összefoglaló a 2011. július 7-én kiadott előzetes értesítés helyébe lép. A biztonsági közlemények kiadásáról szóló előzetes értesítés szolgáltatásról itt olvashat bővebben: [Előzetes értesítés a Microsoft biztonsági közleményeinek kiadásáról](http://go.microsoft.com/fwlink/?linkid=217213).

Ha automatikus értesítést szeretne kapni a Microsoft biztonsági közleményeinek megjelenéséről, fizessen elő a [Microsoft Technical Security Notifications](http://go.microsoft.com/fwlink/?linkid=21163) szolgáltatásra.

A közleményekkel kapcsolatos kérdések megválaszolására a Microsoft 2011. július 13-án, csendes-óceáni idő szerint 11 órakor webes szemináriumot tart. [Jelentkezzen most a júliusi közleményeket bemutató webes szemináriumra](https://msevents.microsoft.com/cui/webcasteventdetails.aspx?eventid=1032487855&eventcategory=4). Ezt követően a webes szeminárium igény szerint kerül megrendezésre. További információkért látogasson el a [Microsoft biztonsági közleményeit és a webes szemináriumokat](http://go.microsoft.com/fwlink/?linkid=217214)bemutató oldalra.

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
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=217102">MS11-053</a></td>
<td style="border:1px solid black;"><br />
<strong>A Bluetooth köteg biztonsági rése (2566220) távolról történő programkódfuttatást tehet lehetővé </strong><br />
Ez a biztonsági frissítés a Windows Bluetooth Stack közvetlenül jelentett biztonsági rését szünteti meg. A biztonsági rés távolról történő programkódfuttatást tehet lehetővé, ha a támadó speciálisan kialakított Bluetooth csomagokat küld az érintett rendszernek. Ezt követően programokat telepíthet, illetve adatokat tekinthet meg, módosíthat és törölhet, de korlátozás nélküli jogosultságokkal rendelkező új fiókokat is létrehozhat. Ez a biztonsági rés csupán a Bluetooth-kompatibilis rendszereket érinti</td>
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=21140">Kritikus</a><br />
Távoli kódfuttatás</td>
<td style="border:1px solid black;">Újraindítást igényel</td>
<td style="border:1px solid black;">Microsoft Windows</td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=220172">MS11-054</a></td>
<td style="border:1px solid black;"><strong>A Windows kernelmódú illesztőprogramjainak biztonsági rései jogok kiterjesztéséhez vezethetnek (2555917)</strong> <br />
<br />
A biztonsági frissítés a Microsoft Windows 15 közvetlenül jelentett biztonsági rését szünteti meg. A biztonsági rések legsúlyosabbika jogok kiterjesztését teheti lehetővé, ha a támadó helyben bejelentkezett, és ott különlegesen kialakított alkalmazást futtatott. A támadónak a biztonsági rések kihasználásához érvényes bejelentkezési adatokkal kell rendelkeznie, és képesnek kell lennie helyileg bejelentkezni a rendszerbe.</td>
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=21140">Fontos</a><br />
Jogok kiterjesztése</td>
<td style="border:1px solid black;">Újraindítást igényel</td>
<td style="border:1px solid black;">Microsoft Windows</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=217465">MS11-056</a></td>
<td style="border:1px solid black;"><strong>A Windows futásidejű ügyfél/kiszolgáló alrendszerének biztonsági rései jogok kiterjesztését tehetik lehetővé (2507938)</strong><br />
<br />
A biztonsági frissítés a Microsoft Windows futásidejű ügyfélkiszolgáló alrendszerének (CRSS) öt közvetlenül jelentett biztonsági rését szünteti meg. A biztonsági rések jogok kiterjesztését tehetik lehetővé, ha a támadó bejelentkezik a felhasználó rendszerére, és ott speciálisan kialakított alkalmazást futtat. A támadónak ezen biztonsági rések kihasználásához érvényes bejelentkezési adatokkal kell rendelkeznie, és képesnek kell lennie helyileg bejelentkezni a rendszerbe.</td>
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=21140">Fontos</a><br />
Jogok kiterjesztése</td>
<td style="border:1px solid black;">Újraindítást igényel</td>
<td style="border:1px solid black;">Microsoft Windows</td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=220276">MS11-055</a></td>
<td style="border:1px solid black;"><strong>A Microsoft Visio biztonsági rése távoli kódfuttatást tehet lehetővé (2560847)</strong><br />
<br />
A biztonsági frissítés a Microsoft Visio nyilvánosan jelentett biztonsági rését szünteti meg. A támadó a biztonsági résen keresztül távoli kódfuttatást tud elérni, ha rá tudja venni a felhasználót, hogy nyisson meg egy normál Visio fájlt, amely azonban azonos hálózati meghajtón található, mint a speciálisan létrehozott függvénytárfájl. A biztonsági rést kihasználó támadó a bejelentkezett felhasználóval egyező hozzáférést nyer a rendszerhez. A kevesebb jogosultsággal bíró fiókkal rendelkező felhasználók esetében kisebb a veszélyeztetettség, mint a rendszergazdai jogosultságokkal rendelkezők esetén</td>
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
  
Az alábbi táblázatból minden telepítendő biztonsági frissítésről megtudhatja, hogy mekkora a valószínűsége annak, hogy a biztonsági közlemény kiadása után 30 napon belül kódvégrehajtási és szolgáltatásmegtagadási támadások jelenhetnek meg. A havi frissítések telepítési sorrendjének meghatározásához, az adott konfigurációnak megfelelően tekintse át az alábbi értékeléseket. A minősítések jelentéséről és meghatározásuk módjáról a [Microsoft biztonsági rések jegyzéke](http://technet.microsoft.com/en-us/security/cc998259.aspx) tartalmaz bővebb információt.
  
Az alábbi oszlopokban a „legújabb szoftver” kifejezés az adott szoftver legutóbb kiadott változatára vonatkozik, a „korábbi szoftver” kifejezés az adott szoftver valamennyi, korábban kiadott támogatott verziójára vonatkozik, amint az az érintett vagy a nem érintett szoftverek felsorolásában szerepel.
  
| Közlemény azonosítója                                     | A biztonsági rés címe                                                                                   | CVE-azonosító                                                                    | Kódfuttatás kihasználhatóságának felmérése a legújabb szoftvereknél                                                  | Kódfuttatás kihasználhatóságának felmérése a korábbi szoftvereknél                                                   | Szolgáltatásmegtagadás kihasználhatóságának felmérése | Fontos megjegyzések                                                                                                             |  
|-----------------------------------------------------------|---------------------------------------------------------------------------------------------------------|----------------------------------------------------------------------------------|----------------------------------------------------------------------------------------------------------------------|----------------------------------------------------------------------------------------------------------------------|-------------------------------------------------------|---------------------------------------------------------------------------------------------------------------------------------|  
| [MS11-053](http://go.microsoft.com/fwlink/?linkid=217102) | Bluetooth köteg biztonsági rés                                                                          | [CVE-2011-1265](http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2011-1265) | [2](http://technet.microsoft.com/en-us/security/cc998259.aspx) - Valószínűleg inkonzisztens rosszindulatú programkód | [2](http://technet.microsoft.com/en-us/security/cc998259.aspx) – Valószínűleg inkonzisztens rosszindulatú programkód | Állandó                                               | Ez a biztonsági rés csak a Bluetooth-kompatibilis ügyfélrendszereket érinti (Windows Vista és Windows 7 kiadásokon futó verzió) |  
| [MS11-054](http://go.microsoft.com/fwlink/?linkid=220172) | A Win32k használat utáni felszabadítás miatti biztonsági rése                                           | [CVE-2011-1874](http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2011-1874) | [1](http://technet.microsoft.com/en-us/security/cc998259.aspx) - Konzisztens rosszindulatú programkódról van szó     | [1](http://technet.microsoft.com/en-us/security/cc998259.aspx) - Konzisztens rosszindulatú programkódról van szó     | Állandó                                               | (Nincs)                                                                                                                         |  
| [MS11-054](http://go.microsoft.com/fwlink/?linkid=220172) | A Win32k használat utáni felszabadítás miatti biztonsági rése                                           | [CVE-2011-1875](http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2011-1875) | [1](http://technet.microsoft.com/en-us/security/cc998259.aspx) - Konzisztens rosszindulatú programkódról van szó     | [1](http://technet.microsoft.com/en-us/security/cc998259.aspx) - Konzisztens rosszindulatú programkódról van szó     | Állandó                                               | (Nincs)                                                                                                                         |  
| [MS11-054](http://go.microsoft.com/fwlink/?linkid=220172) | A Win32k használat utáni felszabadítás miatti biztonsági rése                                           | [CVE-2011-1876](http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2011-1876) | [2](http://technet.microsoft.com/en-us/security/cc998259.aspx) – Valószínűleg inkonzisztens rosszindulatú programkód | [2](http://technet.microsoft.com/en-us/security/cc998259.aspx) – Valószínűleg inkonzisztens rosszindulatú programkód | Állandó                                               | (Nincs)                                                                                                                         |  
| [MS11-054](http://go.microsoft.com/fwlink/?linkid=220172) | A Win32k használat utáni felszabadítás miatti biztonsági rése                                           | [CVE-2011-1877](http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2011-1877) | [2](http://technet.microsoft.com/en-us/security/cc998259.aspx) – Valószínűleg inkonzisztens rosszindulatú programkód | [2](http://technet.microsoft.com/en-us/security/cc998259.aspx) – Valószínűleg inkonzisztens rosszindulatú programkód | Állandó                                               | (Nincs)                                                                                                                         |  
| [MS11-054](http://go.microsoft.com/fwlink/?linkid=220172) | A Win32k használat utáni felszabadítás miatti biztonsági rése                                           | [CVE-2011-1878](http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2011-1878) | [1](http://technet.microsoft.com/en-us/security/cc998259.aspx) - Konzisztens rosszindulatú programkódról van szó     | [1](http://technet.microsoft.com/en-us/security/cc998259.aspx) - Konzisztens rosszindulatú programkódról van szó     | Állandó                                               | (Nincs)                                                                                                                         |  
| [MS11-054](http://go.microsoft.com/fwlink/?linkid=220172) | A Win32k használat utáni felszabadítás miatti biztonsági rése                                           | [CVE-2011-1879](http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2011-1879) | [1](http://technet.microsoft.com/en-us/security/cc998259.aspx) - Konzisztens rosszindulatú programkódról van szó     | [1](http://technet.microsoft.com/en-us/security/cc998259.aspx) - Konzisztens rosszindulatú programkódról van szó     | Állandó                                               | (Nincs)                                                                                                                         |  
| [MS11-054](http://go.microsoft.com/fwlink/?linkid=220172) | A Win32k Null mutatójának visszakeresési biztonsági rése                                                | [CVE-2011-1880](http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2011-1880) | [1](http://technet.microsoft.com/en-us/security/cc998259.aspx) - Konzisztens rosszindulatú programkódról van szó     | [1](http://technet.microsoft.com/en-us/security/cc998259.aspx) - Konzisztens rosszindulatú programkódról van szó     | Állandó                                               | (Nincs)                                                                                                                         |  
| [MS11-054](http://go.microsoft.com/fwlink/?linkid=220172) | A Win32k Null mutatójának visszakeresési biztonsági rése                                                | [CVE-2011-1881](http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2011-1881) | [1](http://technet.microsoft.com/en-us/security/cc998259.aspx) - Konzisztens rosszindulatú programkódról van szó     | [1](http://technet.microsoft.com/en-us/security/cc998259.aspx) - Konzisztens rosszindulatú programkódról van szó     | Állandó                                               | (Nincs)                                                                                                                         |  
| [MS11-054](http://go.microsoft.com/fwlink/?linkid=220172) | A Win32k használat utáni felszabadítás miatti biztonsági rése                                           | [CVE-2011-1882](http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2011-1882) | [1](http://technet.microsoft.com/en-us/security/cc998259.aspx) - Konzisztens rosszindulatú programkódról van szó     | [1](http://technet.microsoft.com/en-us/security/cc998259.aspx) - Konzisztens rosszindulatú programkódról van szó     | Állandó                                               | (Nincs)                                                                                                                         |  
| [MS11-054](http://go.microsoft.com/fwlink/?linkid=220172) | A Win32k használat utáni felszabadítás miatti biztonsági rése                                           | [CVE-2011-1883](http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2011-1883) | [1](http://technet.microsoft.com/en-us/security/cc998259.aspx) - Konzisztens rosszindulatú programkódról van szó     | [1](http://technet.microsoft.com/en-us/security/cc998259.aspx) - Konzisztens rosszindulatú programkódról van szó     | Állandó                                               | (Nincs)                                                                                                                         |  
| [MS11-054](http://go.microsoft.com/fwlink/?linkid=220172) | A Win32k használat utáni felszabadítás miatti biztonsági rése                                           | [CVE-2011-1884](http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2011-1884) | [1](http://technet.microsoft.com/en-us/security/cc998259.aspx) - Konzisztens rosszindulatú programkódról van szó     | [1](http://technet.microsoft.com/en-us/security/cc998259.aspx) - Konzisztens rosszindulatú programkódról van szó     | Állandó                                               | (Nincs)                                                                                                                         |  
| [MS11-054](http://go.microsoft.com/fwlink/?linkid=220172) | A Win32k Null mutatójának visszakeresési biztonsági rése                                                | [CVE-2011-1885](http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2011-1885) | [1](http://technet.microsoft.com/en-us/security/cc998259.aspx) - Konzisztens rosszindulatú programkódról van szó     | [1](http://technet.microsoft.com/en-us/security/cc998259.aspx) - Konzisztens rosszindulatú programkódról van szó     | Állandó                                               | (Nincs)                                                                                                                         |  
| [MS11-054](http://go.microsoft.com/fwlink/?linkid=220172) | A nem megfelelő paramétere Win32k adatokhoz való illetéktelen hozzáférést lehetővé tévő biztonsági rése | [CVE-2011-1886](http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2011-1886) | [3](http://technet.microsoft.com/en-us/security/cc998259.aspx) – Nem valószínű működő rosszindulatú programkód       | [3](http://technet.microsoft.com/en-us/security/cc998259.aspx) – Nem valószínű működő rosszindulatú programkód       | Állandó                                               | A biztonsági rés illetéktelen adatelérést okoz                                                                                  |  
| [MS11-054](http://go.microsoft.com/fwlink/?linkid=220172) | A Win32k Null mutatójának visszakeresési biztonsági rése                                                | [CVE-2011-1887](http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2011-1887) | [1](http://technet.microsoft.com/en-us/security/cc998259.aspx) - Konzisztens rosszindulatú programkódról van szó     | [1](http://technet.microsoft.com/en-us/security/cc998259.aspx) - Konzisztens rosszindulatú programkódról van szó     | Állandó                                               | (Nincs)                                                                                                                         |  
| [MS11-054](http://go.microsoft.com/fwlink/?linkid=220172) | A Win32k Null mutatójának visszakeresési biztonsági rése                                                | [CVE-2011-1888](http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2011-1888) | [1](http://technet.microsoft.com/en-us/security/cc998259.aspx) - Konzisztens rosszindulatú programkódról van szó     | [1](http://technet.microsoft.com/en-us/security/cc998259.aspx) - Konzisztens rosszindulatú programkódról van szó     | Állandó                                               | (Nincs)                                                                                                                         |  
| [MS11-055](http://go.microsoft.com/fwlink/?linkid=220276) | Microsoft Visio nem biztonságos függvénytárbetöltése miatti biztonsági rés                              | [CVE-2010-3148](http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2010-3148) | Nem érintett                                                                                                         | [1](http://technet.microsoft.com/en-us/security/cc998259.aspx) - Konzisztens rosszindulatú programkódról van szó     | Nem érintett                                          | A biztonsági rés nyilvánosságra került                                                                                          |  
| [MS11-056](http://go.microsoft.com/fwlink/?linkid=217465) | CSRSS helyi EOP AllocConsole biztonsági rés                                                             | [CVE-2011-1281](http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2011-1281) | [3](http://technet.microsoft.com/en-us/security/cc998259.aspx) – Nem valószínű működő rosszindulatú programkód       | [1](http://technet.microsoft.com/en-us/security/cc998259.aspx) - Konzisztens rosszindulatú programkódról van szó     | Nem érintett                                          | (Nincs)                                                                                                                         |  
| [MS11-056](http://go.microsoft.com/fwlink/?linkid=217465) | CSRSS helyi EOP SrvSetConsoleLocalEUDC biztonsági rés                                                   | [CVE-2011-1282](http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2011-1282) | [3](http://technet.microsoft.com/en-us/security/cc998259.aspx) – Nem valószínű működő rosszindulatú programkód       | [1](http://technet.microsoft.com/en-us/security/cc998259.aspx) - Konzisztens rosszindulatú programkódról van szó     | Állandó                                               | (Nincs)                                                                                                                         |  
| [MS11-056](http://go.microsoft.com/fwlink/?linkid=217465) | CSRSS helyi EOP SrvSetConsoleNumberOfCommand biztonsági rés                                             | [CVE-2011-1283](http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2011-1283) | [1](http://technet.microsoft.com/en-us/security/cc998259.aspx) - Konzisztens rosszindulatú programkódról van szó     | [1](http://technet.microsoft.com/en-us/security/cc998259.aspx) - Konzisztens rosszindulatú programkódról van szó     | Állandó                                               | (Nincs)                                                                                                                         |  
| [MS11-056](http://go.microsoft.com/fwlink/?linkid=217465) | CSRSS helyi EOP SrvWriteConsoleOutput biztonsági rés                                                    | [CVE-2011-1284](http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2011-1284) | [1](http://technet.microsoft.com/en-us/security/cc998259.aspx) - Konzisztens rosszindulatú programkódról van szó     | [1](http://technet.microsoft.com/en-us/security/cc998259.aspx) - Konzisztens rosszindulatú programkódról van szó     | Állandó                                               | (Nincs)                                                                                                                         |  
| [MS11-056](http://go.microsoft.com/fwlink/?linkid=217465) | CSRSS helyi EOP SrvWriteConsoleOutputString biztonsági rés                                              | [CVE-2011-1870](http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2011-1870) | [3](http://technet.microsoft.com/en-us/security/cc998259.aspx) – Nem valószínű működő rosszindulatú programkód       | [1](http://technet.microsoft.com/en-us/security/cc998259.aspx) - Konzisztens rosszindulatú programkódról van szó     | Állandó                                               | (Nincs)                                                                                                                         |
  
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
</tr>
<tr>
<th colspan="4">
Windows XP  
</th>
</tr>
<tr>
<td style="border:1px solid black;">
**Közlemény azonosítója**
</td>
<td style="border:1px solid black;">
[**MS11-053**](http://go.microsoft.com/fwlink/?linkid=217102)
</td>
<td style="border:1px solid black;">
[**MS11-054**](http://go.microsoft.com/fwlink/?linkid=220172)
</td>
<td style="border:1px solid black;">
[**MS11-056**](http://go.microsoft.com/fwlink/?linkid=217465)
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
Nem érintett
</td>
<td style="border:1px solid black;">
[Windows XP Service Pack 3](http://www.microsoft.com/downloads/details.aspx?familyid=d7a47370-f415-46ea-9a82-a943f743c8b6)  
(Fontos)
</td>
<td style="border:1px solid black;">
[Windows XP Service Pack 3](http://www.microsoft.com/downloads/details.aspx?familyid=425c705e-94f2-4fa6-9df2-dc71897215fa)  
(Fontos)
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
Windows XP Professional x64 Edition Service Pack 2
</td>
<td style="border:1px solid black;">
Nem érintett
</td>
<td style="border:1px solid black;">
[Windows XP Professional x64 Edition Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=db89d88f-d0d4-4ed6-8589-bf27557c0304)  
(Fontos)
</td>
<td style="border:1px solid black;">
[Windows XP Professional x64 Edition Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=c389fa20-677e-49b6-af44-781e5522d08b)  
(Fontos)
</td>
</tr>
<tr>
<th colspan="4">
Windows Server 2003
</th>
</tr>
<tr>
<td style="border:1px solid black;">
**Közlemény azonosítója**
</td>
<td style="border:1px solid black;">
[**MS11-053**](http://go.microsoft.com/fwlink/?linkid=217102)
</td>
<td style="border:1px solid black;">
[**MS11-054**](http://go.microsoft.com/fwlink/?linkid=220172)
</td>
<td style="border:1px solid black;">
[**MS11-056**](http://go.microsoft.com/fwlink/?linkid=217465)
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
Nem érintett
</td>
<td style="border:1px solid black;">
[Windows Server 2003 Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=7a26a437-a705-4d48-8389-50f159a39891)  
(Fontos)
</td>
<td style="border:1px solid black;">
[Windows Server 2003 Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=dff4c67a-8c8b-4d7d-84c7-57429becf0ff)  
(Fontos)
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
Windows Server 2003 x64 Edition Service Pack 2
</td>
<td style="border:1px solid black;">
Nem érintett
</td>
<td style="border:1px solid black;">
[Windows Server 2003 x64 Edition Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=95393f89-0b05-4243-95ed-17bcdad24bfb)  
(Fontos)
</td>
<td style="border:1px solid black;">
[Windows Server 2003 x64 Edition Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=1615a995-9a04-440a-ae52-5917738f0ecb)  
(Fontos)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Windows Server 2003 SP2 Itanium-alapú rendszerekhez
</td>
<td style="border:1px solid black;">
Nem érintett
</td>
<td style="border:1px solid black;">
[Windows Server 2003 SP2 javítócsomaggal Itanium-alapú rendszerekhez](http://www.microsoft.com/downloads/details.aspx?familyid=3b094bdb-4150-44f2-a638-afd5f41b00a3)  
(Fontos)
</td>
<td style="border:1px solid black;">
[Windows Server 2003 SP2 javítócsomaggal Itanium-alapú rendszerekhez](http://www.microsoft.com/downloads/details.aspx?familyid=a81c011d-eeea-4383-9efb-df70515ab357)  
(Fontos)
</td>
</tr>
<tr>
<th colspan="4">
Windows Vista
</th>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
**Közlemény azonosítója**
</td>
<td style="border:1px solid black;">
[**MS11-053**](http://go.microsoft.com/fwlink/?linkid=217102)
</td>
<td style="border:1px solid black;">
[**MS11-054**](http://go.microsoft.com/fwlink/?linkid=220172)
</td>
<td style="border:1px solid black;">
[**MS11-056**](http://go.microsoft.com/fwlink/?linkid=217465)
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
[**Fontos**](http://go.microsoft.com/fwlink/?linkid=21140)
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
Windows Vista Service Pack 1 és Windows Vista Service Pack 2
</td>
<td style="border:1px solid black;">
[Windows Vista Service Pack 1](http://www.microsoft.com/downloads/details.aspx?familyid=6bff74ac-45f3-4585-92da-316921b458fa)<sup>[1]</sup>
(KB2561109)  
(Kritikus)  
[Windows Vista Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=a1e5aa7d-5f38-4ce2-9575-4b4cb7520160)  
(KB2532531)  
(Kritikus)
</td>
<td style="border:1px solid black;">
[Windows Vista Service Pack 1 és Windows Vista Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=c1fe1e53-34d5-497e-8ba2-50caa8dc1158)  
(Fontos)
</td>
<td style="border:1px solid black;">
[Windows Vista Service Pack 1 és Windows Vista Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=a5e192af-dae5-47ef-a9d0-f761a8caa974)  
(Fontos)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Windows Vista x64 Edition Service Pack 1 és Windows Vista x64 Edition Service Pack 2
</td>
<td style="border:1px solid black;">
[Windows Vista x64 Edition Service Pack 1](http://www.microsoft.com/downloads/details.aspx?familyid=849d2694-c8b3-4670-8203-912661bccabf)<sup>[1]</sup>
(KB2561109)  
(Kritikus)  
[Windows Vista x64 Edition Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=4287eeb4-ab29-4727-83f2-260d838b44d4)  
(KB2532531)  
(Kritikus)
</td>
<td style="border:1px solid black;">
[Windows Vista x64 Edition Service Pack 1 és Windows Vista x64 Edition Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=7bc0a285-cc32-4c6b-abee-d92130d459b7)  
(Fontos)
</td>
<td style="border:1px solid black;">
[Windows Vista x64 Edition Service Pack 1 és Windows Vista x64 Edition Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=1007f5d3-9be1-4f03-a3f0-12ddb555653c)  
(Fontos)
</td>
</tr>
<tr>
<th colspan="4">
Windows Server 2008
</th>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
**Közlemény azonosítója**
</td>
<td style="border:1px solid black;">
[**MS11-053**](http://go.microsoft.com/fwlink/?linkid=217102)
</td>
<td style="border:1px solid black;">
[**MS11-054**](http://go.microsoft.com/fwlink/?linkid=220172)
</td>
<td style="border:1px solid black;">
[**MS11-056**](http://go.microsoft.com/fwlink/?linkid=217465)
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
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
Windows Server 2008 32 bites rendszerekhez és Windows Server 2008 32 bites rendszerekhez, Service Pack 2
</td>
<td style="border:1px solid black;">
Nem érintett
</td>
<td style="border:1px solid black;">
[Windows Server 2008 32 bites rendszerekhez és Windows Server 2008 32 bites rendszerekhez, Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=b88d0471-4427-4835-9446-db71116481f0)\*  
(Fontos)
</td>
<td style="border:1px solid black;">
[Windows Server 2008 32 bites rendszerekhez és Windows Server 2008 32 bites rendszerekhez, Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=36e3dbaf-36f5-4c74-8f11-ecbef46f58e1)\*  
(Fontos)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Windows Server 2008 x64-alapú rendszerekhez és Windows Server 2008 x64-alapú rendszerekhez, Service Pack 2
</td>
<td style="border:1px solid black;">
Nem érintett
</td>
<td style="border:1px solid black;">
[Windows Server 2008 x64 alapú rendszerekhez és Windows Server 2008 x64 alapú rendszerekhez, Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=d3df6184-3e3c-4949-a1ee-293ec68f8149)\*  
(Fontos)
</td>
<td style="border:1px solid black;">
[Windows Server 2008 x64 alapú rendszerekhez és Windows Server 2008 x64 alapú rendszerekhez, Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=b43d2ab5-e281-4c6b-bb37-1f1b5d86ac82)\*  
(Fontos)
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
Windows Server 2008 Itanium-alapú rendszerekhez és Windows Server 2008 Itanium-alapú rendszerekhez, Service Pack 2
</td>
<td style="border:1px solid black;">
Nem érintett
</td>
<td style="border:1px solid black;">
[Windows Server 2008 Itanium-alapú rendszerekhez és Windows Server 2008 Itanium-alapú rendszerekhez, Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=9e021d69-7f0c-457f-af86-07e760d8f421)  
(Fontos)
</td>
<td style="border:1px solid black;">
[Windows Server 2008 Itanium-alapú rendszerekhez és Windows Server 2008 Itanium-alapú rendszerekhez, Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=b70209f2-1c51-45af-b3c4-3473aebcdb35)  
(Fontos)
</td>
</tr>
<tr>
<th colspan="4">
Windows 7
</th>
</tr>
<tr>
<td style="border:1px solid black;">
**Közlemény azonosítója**
</td>
<td style="border:1px solid black;">
[**MS11-053**](http://go.microsoft.com/fwlink/?linkid=217102)
</td>
<td style="border:1px solid black;">
[**MS11-054**](http://go.microsoft.com/fwlink/?linkid=220172)
</td>
<td style="border:1px solid black;">
[**MS11-056**](http://go.microsoft.com/fwlink/?linkid=217465)
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
</tr>
<tr>
<td style="border:1px solid black;">
Windows 7 32 bites rendszerekhez és Windows 7 32 bites rendszerekhez Service Pack 1
</td>
<td style="border:1px solid black;">
[Windows 7 32 bites rendszerekhez és Windows 7 32 bites rendszerekhez Service Pack 1](http://www.microsoft.com/downloads/details.aspx?familyid=7f811b75-c3ff-411a-aaa9-126dce34cc01)  
(KB2532531)  
(Kritikus)
</td>
<td style="border:1px solid black;">
[Windows 7 32 bites rendszerekhez és Windows 7 32 bites rendszerekhez Service Pack 1](http://www.microsoft.com/downloads/details.aspx?familyid=41db1b2f-f862-43bb-89bc-4b97737e5cb9)  
(Fontos)
</td>
<td style="border:1px solid black;">
[Windows 7 32 bites rendszerekhez és Windows 7 32 bites rendszerekhez Service Pack 1](http://www.microsoft.com/downloads/details.aspx?familyid=ac3b435c-8caf-40cc-8f13-b52261b3b9e6)  
(Fontos)
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
Windows 7 x64 alapú rendszerekhez és Windows 7 x64 alapú rendszerekhez Service Pack 1
</td>
<td style="border:1px solid black;">
[Windows 7 x64 alapú rendszerekhez és Windows 7 x64 alapú rendszerekhez Service Pack 1](http://www.microsoft.com/downloads/details.aspx?familyid=90b2da71-18f9-46ee-9e3d-b08620ca06aa)  
(KB2532531)  
(Kritikus)
</td>
<td style="border:1px solid black;">
[Windows 7 x64 alapú rendszerekhez és Windows 7 x64 alapú rendszerekhez Service Pack 1](http://www.microsoft.com/downloads/details.aspx?familyid=211abdc6-40c7-4bfc-8c2d-be72981f311e)  
(Fontos)
</td>
<td style="border:1px solid black;">
[Windows 7 x64 alapú rendszerekhez és Windows 7 x64 alapú rendszerekhez Service Pack 1](http://www.microsoft.com/downloads/details.aspx?familyid=64e5f889-fa46-4884-9b22-3ba4e2fba1b9)  
(Fontos)
</td>
</tr>
<tr>
<th colspan="4">
Windows Server 2008 R2
</th>
</tr>
<tr>
<td style="border:1px solid black;">
**Közlemény azonosítója**
</td>
<td style="border:1px solid black;">
[**MS11-053**](http://go.microsoft.com/fwlink/?linkid=217102)
</td>
<td style="border:1px solid black;">
[**MS11-054**](http://go.microsoft.com/fwlink/?linkid=220172)
</td>
<td style="border:1px solid black;">
[**MS11-056**](http://go.microsoft.com/fwlink/?linkid=217465)
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
[**Fontos**](http://go.microsoft.com/fwlink/?linkid=21140)
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
Nem érintett
</td>
<td style="border:1px solid black;">
[Windows Server 2008 R2 x64 alapú rendszerekhez és Windows Server 2008 R2 x64 alapú rendszerekhez Service Pack 1](http://www.microsoft.com/downloads/details.aspx?familyid=4f54e498-3825-407d-a036-1900a65d34f1)\*  
(Fontos)
</td>
<td style="border:1px solid black;">
[Windows Server 2008 R2 x64 alapú rendszerekhez és Windows Server 2008 R2 x64 alapú rendszerekhez Service Pack 1](http://www.microsoft.com/downloads/details.aspx?familyid=b99a40cf-8a31-43d9-bd0b-a458a533068b)\*  
(Fontos)
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
Windows Server 2008 R2 Itanium alapú rendszerekhez és Windows Server 2008 R2 Itanium alapú rendszerekhez Service Pack 1
</td>
<td style="border:1px solid black;">
Nem érintett
</td>
<td style="border:1px solid black;">
[Windows Server 2008 R2 Itanium alapú rendszerekhez és Windows Server 2008 R2 Itanium alapú rendszerekhez Service Pack 1](http://www.microsoft.com/downloads/details.aspx?familyid=e7ae39e8-1154-4a13-8598-29d4a6358762)  
(Fontos)
</td>
<td style="border:1px solid black;">
[Windows Server 2008 R2 Itanium alapú rendszerekhez és Windows Server 2008 R2 Itanium alapú rendszerekhez Service Pack 1](http://www.microsoft.com/downloads/details.aspx?familyid=784efc20-3a41-42ab-b48d-51fd59d71523)  
(Fontos)
</td>
</tr>
</table>
 
**Megjegyzések a Windows Server 2008 és Windows Server 2008 R2 rendszerhez**

**\*Érinti a kiszolgálómag telepítését.** Ez a frissítés ugyanolyan biztonsági besorolás mellett, a megadottak szerint érvényes az Windows Server 2008 és a Windows Server 2008 R2 összes támogatott kiadására, függetlenül attól, hogy a kiszolgálómag-telepítési opcióval telepítették-e. Erről a telepítési opcióról bővebben a [Kiszolgálómag-telepítés kezelése](http://technet.microsoft.com/en-us/library/ee441255(ws.10).aspx)és [Kiszolgálómag-telepítés szervizelése](http://technet.microsoft.com/en-us/library/ff698994(ws.10).aspx) TechNet cikkekben olvashat. A kiszolgálómag-telepítési opció nem vonatkozik a Windows Server 2008 és a Windows Server 2008 R2 bizonyos kiadásaira; lásd: [A kiszolgálómag-telepítési opciók összehasonlítása](http://www.microsoft.com/windowsserver2008/en/us/compare-core-installation.aspx).

**Megjegyzés az MS11-053 közleményhez**

<sup>[1]</sup> A Windows Vista Service Pack 1 csak akkor érintett, ha a Windows Vista Feature Pack for Wireless lett telepítve.

#### Microsoft Office programcsomagok és szoftverek

 
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
Microsoft Office programcsomagok és összetevők
</th>
</tr>
<tr>
<td style="border:1px solid black;">
**Közlemény azonosítója**
</td>
<td style="border:1px solid black;">
[**MS11-055**](http://go.microsoft.com/fwlink/?linkid=220276)
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
Microsoft Visio 2003 Service Pack 3
</td>
<td style="border:1px solid black;">
[Microsoft Visio 2003 Service Pack 3](http://www.microsoft.com/downloads/details.aspx?familyid=1c7b2a5b-4aa6-4006-90bf-89f8b2b7becd)  
(KB2493523)  
(Fontos)
</td>
</tr>
</table>
 

Észlelési és telepítési eszközök, útmutatás
-------------------------------------------

<span></span>
**Biztonsági központ**

A szoftveres és biztonsági frissítések kezeléséhez azokat a szervezet asztali és hordozható számítógépeire, valamint kiszolgálóira is telepíteni kell. További tájékoztatásért látogasson el a [TechNet Update Management Center](http://go.microsoft.com/fwlink/?linkid=69903) weboldalára. A [TechNet Security Center](http://go.microsoft.com/fwlink/?linkid=21171) bővebb tájékoztatással szolgál a Microsoft-termékek biztonsági funkcióival kapcsolatban. A [Biztonság otthon](http://go.microsoft.com/fwlink/?linkid=85102) weboldalon a megfelelő hivatkozásra kattintva elérhetőek a legújabb biztonsági frissítések.

A biztonsági frissítések a [Microsoft Update](http://go.microsoft.com/fwlink/?linkid=40747) és a [Windows Update](http://go.microsoft.com/fwlink/?linkid=21130) weboldalról tölthetők le. A biztonsági frissítések a [Microsoft letöltőközpontjában](http://go.microsoft.com/fwlink/?linkid=21129) is elérhetőek. Legegyszerűbben a „security update” kifejezésre irányuló kulcsszavas kereséssel találhatja meg ezeket.

A Microsoft Office for Mac felhasználói számára a Microsoft AutoUpdate for Mac szolgáltatás biztosítja a Microsoft szoftverek naprakész állapotát. A Microsoft AutoUpdate for Mac működésének részleteiről lásd: [Szoftverfrissítések automatikus keresése](http://mac2.microsoft.com/help/office/14/en-us/word/item/ffe35357-8f25-4df8-a0a3-c258526c64ea).

A biztonsági frissítések a [Microsoft Update katalógusából](http://go.microsoft.com/fwlink/?linkid=96155) is letölthetőek. A Microsoft Update katalógus a Windows Update és Microsoft Update szolgáltatáson keresztül elérhető tartalom kereshető adatbázisa; ide tartoznak a biztonsági frissítések, illesztőprogramok és szervizcsomagok. A biztonsági közlemény azonosítójára (pl. „MS07-036”) történő kereséssel hozzáadhatja az összes vonatkozó frissítést a kosárhoz (beleértve a frissítés különböző nyelvi változatait), és letöltheti azokat a megadott mappába. A Microsoft Update katalógus részletes leírását lásd a vonatkozó [GYIK](http://go.microsoft.com/fwlink/?linkid=97900)részben.

**Útmutató az észleléshez és a telepítéshez**

A biztonsági frissítésekkel kapcsolatban a Microsoft észlelési és telepítési segítséget nyújt. Ez az útmutató olyan javaslatokat és tudnivalókat tartalmaz, amelyeket segítséget nyújthatnak az informatikusoknak a biztonsági frissítések észlelési és telepítési eszközeinek használatához. További tudnivalókat a [Microsoft Tudásbázis 961747. számú cikkében](http://support.microsoft.com/kb/961747) talál.

**Microsoft Baseline Security Analyzer**

A Microsoft Baseline Security Analyzer (MBSA) segítségével a rendszergazda mind a helyi, mind a távoli számítógépeken ellenőrizheti, hogy mely biztonsági frissítések hiányoznak, illetve hogy mely biztonsági beállítások vannak helytelenül megadva. Ha többet szeretne tudni az MBSA -eszközről, látogasson el a [Microsoft Baseline Security Analyzer webhelyre](http://go.microsoft.com/fwlink/?linkid=21134).

**Windows Server Update Services**

A Microsoft Server Update Services (WSUS) szolgáltatással a rendszergazdák gyorsan és megbízhatóan telepíthetik a legújabb fontos és biztonsági frissítéseket Microsoft Windows 2000 és újabb operációs rendszerekhez, Office XP és újabb operációs rendszerekhez, Exchange Server 2003 és SQL Server 2000 Microsoft Windows 2000 és újabb operációs rendszerekre.

A biztonsági frissítésnek Windows Server Update Services szolgáltatással történő központi telepítéséről a [Windows Server Update Services](http://technet.microsoft.com/en-us/wsus/default.aspx) webhelyen tudhat meg többet.

**System Center Configuration Manager 2007**

A Configuration Manager 2007 szoftverfrissítés-kezelés leegyszerűsíti a frissítéseknek a vállalat minden IT-rendszerére történő eljuttatása és kezelése összetett feladatát. A Configuration Manager 2007 segítségével az IT-rendszergazdák a Microsoft-termékek frissítéseit számos készülékre juttathatják el, köztük asztali számítógépekre, hordozható számítógépekre, kiszolgálókra és mobilkészülékekre.

A Configuration Manager 2007 automatizált biztonságirés-elemzése jelzi a frissítések szükségességét és jelentést küld a javasolt lépésekről. A Configuration Manager 2007 szoftverfrissítés-kezelése a Microsoft Windows Software Update Services (WSUS) szolgáltatására épül, amely az IT-rendszergazdák számára világszerte ismerős, jól bevált frissítési infrastruktúra. További információkat a Configuration Manager 2007 rendszergazdai használatáról a frissítések telepítéséhez lásd: [Szoftverfrissítés-kezelés](http://www.microsoft.com/systemcenter/en/us/configuration-manager/cm-software-update-management.aspx). További információkért a Configuration Manager alkalmazásról látogasson el a [System Center Configuration Manager](http://www.microsoft.com/systemcenter/en/us/configuration-manager.aspx) oldalra.

**Systems Management Server 2003**

A Microsoft Systems Management Server (SMS) rendszer egy sokoldalúan beállítható vállalati megoldás, amely a frissítések kezelésére szolgál. Az SMS segítségével a rendszergazda megállapíthatja, hogy melyik Windows alapú számítógép szorul biztonsági frissítésre, és ezeket a frissítéseket szabályozott módon, a felhasználók minimális zavarásával központilag telepítheti a vállalat teljes informatikai környezetében.

**Megjegyzés** A System Management Server 2003 rendszer általános támogatása 2010. január 12-én lejár. Ha többet szeretne tudni a Windows termékek életciklusáról, keresse fel a [Microsoft támogatási életciklusokkal foglalkozó webhelyét](http://support.microsoft.com/common/international.aspx?rdpath=dm;en-us;lifecycle). Az SMS, vagyis a System Center Configuration Manager 2007 újabb kiadása már elérhető, lásd a korábbi, **System Center Configuration Manager 2007** c. részben.

Ha többet szeretne tudni arról, hogy a rendszergazdák miként telepíthetik a biztonsági frissítéseket az SMS 2003 alkalmazással, látogasson el a [Forgatókönyvek és eljárások a Microsoft Systems Management Server 2003 alkalmazáshoz Szoftverterjesztés és javításkezelés](http://www.microsoft.com/downloads/en/details.aspx?familyid=32f2bb4c-42f8-4b8d-844f-2553fd78049f&displaylang=en) oldalra. Az SMS-szolgáltatásról bővebben a [Microsoft Systems Management Server TechCenter](http://technet.microsoft.com/en-us/systemcenter/bb545936.aspx) oldalán olvashat.

**Megjegyzés** Az SMS a Microsoft Baseline Security Analyzer eszközön keresztül széles körű támogatást nyújt a biztonsági közlemények frissítéseinek észleléséhez, valamint a frissítések telepítéséhez. Előfordulhat, hogy egyes szoftverfrissítéseket ezek az eszközök nem észlelnek. Az SMS-alkalmazás leltározási szolgáltatásai segítségével a rendszergazdák adott rendszereken hajthatják végre a frissítést. Az eljárással kapcsolatban olvassa el a [szoftverfrissítések telepítése az SMS szoftverelosztó ügynök segítségével](http://go.microsoft.com/fwlink/?linkid=33341) című tájékoztatót. Egyes biztonsági frissítésekhez rendszergazdai jogosultságokra van szükség a számítógép újraindítása után. A rendszergazdák az Elevated Rights Deployment Tool eszközt (az [SMS 2003 Administration Feature Pack](http://www.microsoft.com/downloads/en/details.aspx?familyid=7bd3a16e-1899-4e0b-bb99-1320e816167d&displaylang=en) része) alkalmazhatják a frissítések telepítéséhez.

**Az Update Compatibility Evaluator (a frissítéskompatibilitás kiértékelője) és az Application Compatibility Toolkit (alkalmazáskompatibilitási eszközkészlet)**

Az alkalmazások működése érdekében a frissítések gyakran írnak ugyanazokba a fájlokba, illetve regisztrációs bejegyzésekbe. Ez inkompatibilitást okozhat, és növelheti a biztonsági frissítések központi telepítésére használt időt. A Windows frissítések és az alkalmazásoknak való megfelelőség tesztelése és ellenőrzése egyszerűsíthető az [Update Compatibility Evaluator](http://technet2.microsoft.com/windowsvista/en/library/4279e239-37a4-44aa-aec5-4e70fe39f9de1033.mspx?mfr=true) eszközeivel, ami része az [Application Compatibility Toolkit](http://www.microsoft.com/downloads/details.aspx?familyid=24da89e9-b581-47b0-b45e-492dd6da2971&displaylang=hu) alkalmazáskompatibilitási eszközkészletnek.

Az Application Compatibility Toolkit (ACT) tartalmazza a Microsoft Windows Vista, a Windows Update, a Microsoft Security Update vagy a Windows Internet Explorer új verziójának központi telepítése előtt az alkalmazáskompatibilitási problémák kiértékeléséhez és enyhítéséhez szükséges eszközöket és dokumentációt.

### Egyéb információ

#### A Microsoft Windows rosszindulatú szoftvereket eltávolító eszköze

A Microsoft a Windows Update, Microsoft Update, Windows Server Update Services és Letöltőközpont szolgáltatásán keresztül elérhetővé tette a Microsoft Windows rosszindulatú szoftvereket eltávolító eszközének frissített változatát.

#### Nem biztonsági jellegű frissítések a MU, WU és WSUS-szolgáltatásokban

A Windows Update és a Microsoft Update helyen elérhető, nem biztonsági jellegű frissítésekről tájékozódjon itt:

-   [Microsoft Tudásbázis 894199. cikke:](http://support.microsoft.com/kb/894199) Tartalommódosítás a Software Update Services és Windows Server Update Services rendszerek leírásában. Az összes Windows-tartalmat érinti.
-   [Az elmúlt hónapok frissítései Windows Server Frissítési szolgáltatások esetén](http://technet.microsoft.com/en-us/wsus/bb456965.aspx). Microsoft termékek új, módosított és újra kiadott frissítései, a Microsoft Windows rendszert kivéve.

#### Microsoft Active Protections Program (MAPP)

Az ügyfelek védelmének növelése érdekében a biztonsági szoftverekkel foglalkozó nagyobb gyártók a Microsoft a havi biztonsági közlemények megjelenése előtt ellátja biztonsági résekkel kapcsolatos információkkal. Így a biztonságiszoftver-gyártók a kapott biztonsági résekkel kapcsolatos információt felhasználhatják ügyfeleik hatásosabb védelmére az olyan biztonsági szoftverek vagy eszközök (például víruskeresők, hálózati behatolásérzékelő rendszerek vagy kiszolgálóalapú behatolásvédelmi rendszerek) frissítése által. A biztonságiszoftver-gyártók által kiadott aktív védelem elérhetőségéről a [Microsoft Active Protections Program (MAPP) Partners](http://go.microsoft.com/fwlink/?linkid=215201) webhelyén található listán szereplő és a programban részt vevő gyártók aktív védelmi webhelyein tájékozódhat.

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

-   Tarjei Mandt, [Norman](http://www.norman.com), az ms11-054 számú közleményben bemutatott 14 probléma jelentéséért
-   Mr. Liang Yin, Prof. Sihan Qing és Weiping Wen, valamint Mr. Husheng Zhou, [Pekingi Egyetem, Informatikai Tanszék](http://www.ss.pku.edu.cn/en/), az ms11-054 közleményben leírt probléma jelentéséért.
-   Matthew 'j00ru' Jurczyk, [Hispasec](http://www.hispasec.com/)[Virustotal](http://www.virustotal.com/), az ms11-056 közleményben ismertetett öt probléma jelentéséért

#### Terméktámogatás

-   Teszteléssel állapították meg a felsorolt szoftverek egyes verzióinak érintettségét. A többi verzió támogatási életciklusa végére ért. Az egyes szoftververziók támogatási életciklusáról a [Microsoft termékek terméktámogatási életciklusát ismertető webhelyen](http://go.microsoft.com/fwlink/?linkid=21742) talál felvilágosítást.
-   Az Amerikai Egyesült Államokban és Kanada területén élő ügyfelek technikai támogatást kérhetnek a [biztonsági támogatás szolgáltatójától](http://go.microsoft.com/fwlink/?linkid=21131) vagy az 1-866-PCSAFETY telefonszámon. A biztonsági frissítésekkel kapcsolatos hívások ingyenesek. Az elérhető támogatási lehetőségekről további információt talál a [Microsoft segítségnyújtással és támogatással foglalkozó webhelyén](http://support.microsoft.com/).
-   Más országokban a helyi Microsoft-képviseletek nyújtanak támogatást. A biztonsági frissítésekkel kapcsolatos hívások ingyenesek. A [nemzetközi támogatási webhely](http://go.microsoft.com/fwlink/?linkid=21155) felvilágosítást nyújt arról, támogatási kérdéseivel hogyan fordulhat a Microsofthoz.

#### Felelősséget kizáró nyilatkozat

A Microsoft Tudásbázisban leírtak előzetes bejelentés nélkül változhatnak, és a cikkek tartalmáért a Microsoft nem vállal garanciát. A Microsoft egyben elhárít minden kifejezett és értelemszerű garanciát, beleértve az eladhatóságra és az adott célra való alkalmasságra vonatkozó garanciát is. A Microsoft Corporation vagy annak szállítói semmilyen körülmények között nem tehetők felelőssé közvetlen, közvetett, eseti, ok-okozati vagy különleges kárért (beleértve az elmaradt hasznot is), még akkor sem, ha a Microsoft Corporation vagy szállítói tudatában voltak a kár lehetséges voltának. Egyes államok törvényi szabályozása nem teszi lehetővé a véletlen vagy ok-okozati károkért vállalt felelősség korlátozását vagy kizárását, így ezekben az államokban az ez a felelősségkizárás nincs érvényben.

#### Verziók

-   1.0 verzió (2011. július 12.): Összefoglaló közlemény közzététele.

*Built at 2014-04-18T01:50:00Z-07:00*
