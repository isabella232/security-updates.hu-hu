---
TOCTitle: 'MS07-AUG'
Title: 'Microsoft biztonsági közlemény - összefoglalás, augusztus 2007'
ms:assetid: 'ms07-aug'
ms:contentKeyID: 61227705
ms:mtpsurl: 'https://technet.microsoft.com/hu-HU/library/ms07-aug(v=Security.10)'
author: SharonSears
ms.author: SharonSears
---

Security Bulletin Summary

Microsoft biztonsági közlemény - összefoglalás, augusztus 2007
==============================================================

Közzétéve: 2007. augusztus 14. | Frissítve: 2008. június 24.

**Verzió:** 4.0

Az összefoglaló a 2007 augusztusában kiadott biztonsági közleményeket összegzi.

A 2007. augusztusi közlemények kiadása folytán az összefoglaló az augusztus 9-én kiadott előzetes értesítés helyébe lép. További információk a biztonsági közlemények kiadásáról szóló előzetes értesítés szolgáltatásról lásd: [Előzetes értesítés a Microsoft biztonsági közleményeinek kiadásáról](http://technet.microsoft.com/security/bulletin/advance).

Ha automatikus értesítést szeretne kapni a Microsoft biztonsági közleményeinek megjelenéséről, fizessen elő a [Microsoft Technical Security Notifications](http://go.microsoft.com/fwlink/?linkid=21163) szolgáltatásra.

A közleményekkel kapcsolatos kérdések megválaszolására a Microsoft 2007. augusztus 15-én, csendes-óceáni idő szerint 11 órakor webszemináriumot tart. [Jelentkezzen most az augusztusi közleményeket bemutató webes szemináriumra](http://msevents.microsoft.com/cui/webcasteventdetails.aspx?eventid=1032344688&eventcategory=4&culture=en-us&countrycode=us). Ezt követően a webes szeminárium igény szerint kerül megrendezésre. További információkért látogasson el a [Microsoft biztonsági közleményeit és a webes szemináriumokat](http://technet.microsoft.com/security/bulletin/summary)bemutató oldalra.

A Microsoft abban is segítséget nyújt felhasználóinak, hogy a havi biztonsági közleményekkel azonos napon kiadott, nem biztonsági jellegű, de fontos frissítéseket megfelelően rangsorolhassák. Lásd az **Egyéb információ című részt**.

### A közleménnyel kapcsolatos információk

#### Összefoglalások

Az e havi biztonsági közlemények súlyossági sorrendben:

Kritikus (6)
------------

<span></span>
| Közlemény azonosítója                          | A Microsoft MS07-042 számú biztonsági közleménye                                                                                                                                                                                                                                                                                                                                                                                                                                                                                     |
|------------------------------------------------|--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| **Közlemény címe**                             | [**A Microsoft XML Core Services biztonsági rése (936227) távolról történő programkódfuttatást tehet lehetővé**](http://go.microsoft.com/fwlink/?linkid=88350)                                                                                                                                                                                                                                                                                                                                                                       |
| **Összefoglalás**                              | Ez a kritikus besorolású frissítés egy közvetlenül jelzett biztonsági rést szüntet meg. A biztonsági rés távoli kódvégrehajtást tehet lehetővé, amennyiben a felhasználó egy különlegesen kialakított weboldalt tekintett meg az Internet Explorer alkalmazás segítségével. A biztonsági rés kihasználható a Microsoft XML Core Services ellen indított támadásokkal. A kevesebb jogosultsággal bíró fiókkal rendelkező felhasználók esetében kisebb a veszélyeztetettség, mint a rendszergazdai jogosultságokkal rendelkezők esetén |
| **Súlyosság maximális foka**                   | [Kritikus](http://go.microsoft.com/fwlink/?linkid=21140)                                                                                                                                                                                                                                                                                                                                                                                                                                                                             |
| **A biztonsági rés hatása**                    | Távoli kódfuttatás                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                   |
| **A szoftver észlelésével kapcsolatos adatok** | A Microsoft Baseline Security Analyzer képes észlelni, szükséges-e a számítógépen az adott frissítést. A frissítés a rendszer újraindítását igényli.                                                                                                                                                                                                                                                                                                                                                                                 |
| **Érintett szoftverek**                        | **Windows, XML Core Services.** További információt az Érintett szoftverek és letöltési helyek című rész tartalmaz.                                                                                                                                                                                                                                                                                                                                                                                                                  |

| Közlemény azonosítója                          | A Microsoft MS07-043 számú biztonsági közleménye                                                                                                                                                                                                                                                                                                                                                                                                                                                 |
|------------------------------------------------|--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| **Közlemény címe**                             | [**Az OLE Automation távoli kódfuttatást lehetővé tévő biztonsági rése (921503)**](http://go.microsoft.com/fwlink/?linkid=70249)                                                                                                                                                                                                                                                                                                                                                                 |
| **Összefoglalás**                              | Ez a kritikus besorolású frissítés egy közvetlenül jelzett biztonsági rést szüntet meg. A biztonsági rés távoli kódvégrehajtást tehet lehetővé, amennyiben a felhasználó egy különlegesen kialakított weboldalt tekint meg. A biztonsági rés kihasználható az objektumcsatolás és -beillesztés (OLE) ellen indított támadásokkal. A kevesebb jogosultsággal bíró fiókkal rendelkező felhasználók esetében kisebb a veszélyeztetettség, mint a rendszergazdai jogosultságokkal rendelkezők esetén |
| **Súlyosság maximális foka**                   | [Kritikus](http://go.microsoft.com/fwlink/?linkid=21140)                                                                                                                                                                                                                                                                                                                                                                                                                                         |
| **A biztonsági rés hatása**                    | Távoli kódfuttatás                                                                                                                                                                                                                                                                                                                                                                                                                                                                               |
| **A szoftver észlelésével kapcsolatos adatok** | A Microsoft Baseline Security Analyzer képes észlelni, szükséges-e a számítógépen az adott frissítést. A frissítés a rendszer újraindítását igényli.                                                                                                                                                                                                                                                                                                                                             |
| **Érintett szoftverek**                        | **Windows, Visual Basic, Office for Mac**. További információt az Érintett szoftverek és letöltési helyek című rész tartalmaz.                                                                                                                                                                                                                                                                                                                                                                   |

| Közlemény azonosítója                          | A Microsoft MS07-044 számú biztonsági közleménye                                                                                                                                                                                                                                                                                                                                                                                                                          |
|------------------------------------------------|---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| **Közlemény címe**                             | [**A Microsoft Excel biztonsági rése távolról történő programkódfuttatást tehet lehetővé (940965)**](http://go.microsoft.com/fwlink/?linkid=96778)                                                                                                                                                                                                                                                                                                                        |
| **Összefoglalás**                              | Ez a biztonsági frissítés egy közvetlenül jelentett biztonsági rés hibáit szünteti meg, továbbá a vizsgálat során feltárt további biztonsági problémákat old meg. A biztonsági rések távoli kódvégrehajtást tehetnek lehetővé, amennyiben a felhasználó egy különlegesen kialakított Excel fájlt nyit meg. A kevesebb jogosultsággal bíró fiókkal rendelkező felhasználók esetében kisebb a veszélyeztetettség, mint a rendszergazdai jogosultságokkal rendelkezők esetén |
| **Súlyosság maximális foka**                   | [Kritikus](http://go.microsoft.com/fwlink/?linkid=21140)                                                                                                                                                                                                                                                                                                                                                                                                                  |
| **A biztonsági rés hatása**                    | Távoli kódfuttatás                                                                                                                                                                                                                                                                                                                                                                                                                                                        |
| **A szoftver észlelésével kapcsolatos adatok** | A Microsoft Baseline Security Analyzer képes észlelni, szükséges-e a számítógépen az adott frissítést. A frissítés nem teszi szükségessé a számítógép újraindítását.                                                                                                                                                                                                                                                                                                      |
| **Érintett szoftverek**                        | **Office**. További információt az Érintett szoftverek és letöltési helyek című rész tartalmaz.                                                                                                                                                                                                                                                                                                                                                                           |

| Közlemény azonosítója                          | A Microsoft MS07-045 számú biztonsági közleménye                                                                                                                                                                                                                                                                                                                                                                                                  |
|------------------------------------------------|---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| **Közlemény címe**                             | [**Összesítő biztonsági frissítés az Internet Explorerhez (937143)**](http://go.microsoft.com/fwlink/?linkid=91712)                                                                                                                                                                                                                                                                                                                               |
| **Összefoglalás**                              | Ez a kritikus besorolású frissítés három közvetlenül jelzett biztonsági rést szüntet meg. A biztonsági rések távoli kódvégrehajtást tehetnek lehetővé, amennyiben a felhasználó egy különlegesen kialakított weboldalt tekintett meg az Internet Explorer alkalmazás segítségével. A kevesebb jogosultsággal bíró fiókkal rendelkező felhasználók esetében kisebb a veszélyeztetettség, mint a rendszergazdai jogosultságokkal rendelkezők esetén |
| **Súlyosság maximális foka**                   | [Kritikus](http://go.microsoft.com/fwlink/?linkid=21140)                                                                                                                                                                                                                                                                                                                                                                                          |
| **A biztonsági rés hatása**                    | Távoli kódfuttatás                                                                                                                                                                                                                                                                                                                                                                                                                                |
| **A szoftver észlelésével kapcsolatos adatok** | A Microsoft Baseline Security Analyzer képes észlelni, szükséges-e a számítógépen az adott frissítést. A frissítés a rendszer újraindítását igényli.                                                                                                                                                                                                                                                                                              |
| **Érintett szoftverek**                        | **Windows, Internet Explorer**. További információt az Érintett szoftverek és letöltési helyek című rész tartalmaz.                                                                                                                                                                                                                                                                                                                               |

| Közlemény azonosítója                          | A Microsoft MS07-046 számú biztonsági közleménye                                                                                                                                                                                                                                                                                                                                                                                                                                                                                               |
|------------------------------------------------|------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| **Közlemény címe**                             | [**A GDI képmegjelenítő rendszer biztonsági rése távolról történő kódfuttatást tehet lehetővé (938829)**](http://go.microsoft.com/fwlink/?linkid=94466)                                                                                                                                                                                                                                                                                                                                                                                        |
| **Összefoglalás**                              | Ez a kritikus besorolású frissítés egy közvetlenül jelzett biztonsági rést szüntet meg. A képmegjelenítő rendszer távoli kódfuttatást lehetővé tévő biztonsági rését a speciális céllal létrehozott képek kezelési módja okozza. A támadó kihasználhatja a biztonsági rést, és speciális képet hozhat létre, amely lehetővé teheti a távoli programkódfuttatást, amikor egy felhasználó megnyit egy speciálisan kialakított e-mail mellékletet. Ha egy támadó kihasználja a biztonsági rést, teljes mértékben átveheti a rendszer irányítását. |
| **Súlyosság maximális foka**                   | [Kritikus](http://go.microsoft.com/fwlink/?linkid=21140)                                                                                                                                                                                                                                                                                                                                                                                                                                                                                       |
| **A biztonsági rés hatása**                    | Távoli kódfuttatás                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                             |
| **A szoftver észlelésével kapcsolatos adatok** | A Microsoft Baseline Security Analyzer képes észlelni, szükséges-e a számítógépen az adott frissítést. A frissítés a rendszer újraindítását igényli.                                                                                                                                                                                                                                                                                                                                                                                           |
| **Érintett szoftverek**                        | **Windows.** További információt az Érintett szoftverek és letöltési helyek című rész tartalmaz.                                                                                                                                                                                                                                                                                                                                                                                                                                               |

| Közlemény azonosítója                          | A Microsoft MS07-050 számú biztonsági közleménye                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                    |
|------------------------------------------------|---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| **Közlemény címe**                             | [**A Vector Markup Language biztonsági rése távolról történő programkódfuttatást tehet lehetővé (938127)**](http://go.microsoft.com/fwlink/?linkid=94737)                                                                                                                                                                                                                                                                                                                                                                                                           |
| **Összefoglalás**                              | A biztonsági frissítés a Windows Vector Markup Language (VML) implementációjában található, közvetlenül a Microsoftnak jelzett, távoli kódfuttatást lehetővé tévő biztonsági rés okozta problémára nyújt megoldást. A biztonsági rés távoli kódvégrehajtást tehet lehetővé, amennyiben a felhasználó egy különlegesen kialakított weboldalt tekint meg az Internet Explorer alkalmazás segítségével. A kevesebb jogosultsággal bíró fiókkal rendelkező felhasználók esetében kisebb a veszélyeztetettség, mint a rendszergazdai jogosultságokkal rendelkezők esetén |
| **Súlyosság maximális foka**                   | [Kritikus](http://go.microsoft.com/fwlink/?linkid=21140)                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                            |
| **A biztonsági rés hatása**                    | Távoli kódfuttatás                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                  |
| **A szoftver észlelésével kapcsolatos adatok** | A Microsoft Baseline Security Analyzer képes észlelni, szükséges-e a számítógépen az adott frissítést. A frissítés a rendszer újraindítását igényli.                                                                                                                                                                                                                                                                                                                                                                                                                |
| **Érintett szoftverek**                        | **Windows, Internet Explorer**. További információt az Érintett szoftverek és letöltési helyek című rész tartalmaz.                                                                                                                                                                                                                                                                                                                                                                                                                                                 |

Fontos (3)
----------

<span></span>
| Közlemény azonosítója                          | A Microsoft MS07-047 számú biztonsági közleménye                                                                                                                                                                                                                                                                                                                                           |
|------------------------------------------------|--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| **Közlemény címe**                             | [**A Windows Media Player biztonsági rése távoli programkódfuttatást tesz lehetővé (936782)**](http://go.microsoft.com/fwlink/?linkid=88628)                                                                                                                                                                                                                                               |
| **Összefoglalás**                              | A tárgyalt frissítés két közvetlenül jelzett biztonsági rést szüntet meg. A biztonsági rések kódfuttatást tesznek lehetővé, ha a felhasználó speciálisan létrehozott fájlt tekint meg a Windows Media Player alkalmazásban. A kevesebb jogosultsággal bíró fiókkal rendelkező felhasználók esetében kisebb a veszélyeztetettség, mint a rendszergazdai jogosultságokkal rendelkezők esetén |
| **Súlyosság maximális foka**                   | [Fontos](http://go.microsoft.com/fwlink/?linkid=21140)                                                                                                                                                                                                                                                                                                                                     |
| **A biztonsági rés hatása**                    | Távoli kódfuttatás                                                                                                                                                                                                                                                                                                                                                                         |
| **A szoftver észlelésével kapcsolatos adatok** | A Microsoft Baseline Security Analyzer képes észlelni, szükséges-e a számítógépen az adott frissítést. A frissítés nem teszi szükségessé a számítógép újraindítását.                                                                                                                                                                                                                       |
| **Érintett szoftverek**                        | **Windows.** További információt az Érintett szoftverek és letöltési helyek című rész tartalmaz.                                                                                                                                                                                                                                                                                           |

| Közlemény azonosítója                          | A Microsoft MS07-048 számú biztonsági közleménye                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                      |
|------------------------------------------------|---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| **Közlemény címe**                             | [**A Windows minialkalmazások biztonsági rése távoli programkódfuttatásra adhat lehetőséget (938123)**](http://go.microsoft.com/fwlink/?linkid=94465)                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                 |
| **Összefoglalás**                              | Ez a fontos besorolású frissítés két közvetlenül jelentett biztonsági rés hibáit szünteti meg, továbbá a vizsgálat során feltárt további biztonsági problémákat old meg. A biztonsági rések lehetővé teszik, hogy a névtelen támadó távolról a bejelentkezett felhasználó jogosultságaival kódot futtathasson. Ha a felhasználó rosszindulatú RSS-hírcsatornára fizetett elő a Hírcsatorna-hírek minialkalmazásban, vagy rosszindulatú névjegytárfájlt vett fel a Névjegytár minialkalmazásba, illetve rosszindulatú hivatkozásra kattintott az Időjárás minialkalmazásban, a támadó esetleg kódot futtathat a rendszeren. Mindegyik támadási pont esetében igaz, hogy a kevesebb jogosultsággal bíró fiókkal rendelkező felhasználók esetében kisebb a veszélyeztetettség, mint a rendszergazdai jogosultságokkal rendelkezők esetén |
| **Súlyosság maximális foka**                   | [Fontos](http://go.microsoft.com/fwlink/?linkid=21140)                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                |
| **A biztonsági rés hatása**                    | Távoli kódfuttatás                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                    |
| **A szoftver észlelésével kapcsolatos adatok** | A Microsoft Baseline Security Analyzer képes észlelni, szükséges-e a számítógépen az adott frissítést. A frissítés a rendszer újraindítását igényli.                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                  |
| **Érintett szoftverek**                        | **Windows** **Vista.** További információt az Érintett szoftverek és letöltési helyek című rész tartalmaz.                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                            |

| Közlemény azonosítója                          | A Microsoft MS07-049 számú biztonsági közleménye                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                  |
|------------------------------------------------|---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| **Közlemény címe**                             | [**A Virtual PC és a Virtual Server biztonsági rése (937986) jogosultság illetéktelen megszerzését teszi lehetővé**](http://go.microsoft.com/fwlink/?linkid=92734)                                                                                                                                                                                                                                                                                                                                                                                                                                                                                |
| **Összefoglalás**                              | Ez a fontos besorolású biztonsági frissítés egy közvetlenül jelzett biztonsági rést szüntet meg. A biztonsági rés jogok kiterjesztését teheti lehetővé. A Microsoft Virtual PC és a Microsoft Virtual Server biztonsági rése lehetővé teszi, hogy a vendég operációs rendszer felhasználója kódot futtasson a gazdarendszeren vagy egy másik vendég operációs rendszeren. Kizárólag a vendég operációs rendszer rendszergazdai jogosultsággal rendelkező felhasználói képesek a biztonsági rés kihasználására. A vendég operációs rendszer rendszergazdai jogosultsággal nem rendelkező felhasználói nem képesek a biztonsági rés kihasználására. |
| **Súlyosság maximális foka**                   | [Fontos](http://go.microsoft.com/fwlink/?linkid=21140)                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                            |
| **A biztonsági rés hatása**                    | Jogok kiterjesztése                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                               |
| **A szoftver észlelésével kapcsolatos adatok** | A Microsoft Baseline Security Analyzer képes észlelni, szükséges-e a számítógépen az adott frissítést. A frissítés nem teszi szükségessé a számítógép újraindítását.                                                                                                                                                                                                                                                                                                                                                                                                                                                                              |
| **Érintett szoftverek**                        | **Virtual PC, Virtual Server.** További információt az Érintett szoftverek és letöltési helyek című rész tartalmaz.                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                               |

Érintett szoftverek és letöltési helyek
---------------------------------------

<span></span>
**A táblázat használata**

A táblázat segítségével megtudhatja a szükséges információt a telepítendő biztonsági frissítésekről. Nézzen meg minden felsorolt szoftvert vagy összetevőt annak megállapításához, hogy van-e telepítendő biztonsági frissítés. Ha egy szoftver vagy összetevő szerepel a felsorolásban, akkor a biztonsági rés hatását is tartalmazza a táblázat az elérhető szoftverfrissítésre mutató hivatkozással együtt.

**Megjegyzés:** Előfordulhat, hogy egy biztonsági rés megszüntetéséhez több biztonsági frissítést kell telepíteni. Nézze át az egyes közleményazonosítókhoz tartozó teljes oszlopot, és ellenőrizze a telepítendő frissítéseket a rendszerre telepített programok vagy összetevők alapján.

#### Érintett szoftverek és letöltési helyek az MS07-042 – MS07-046 közlemények vonatkozásában

**Érintett szoftverek és letöltési helyek**

 
<p> </p>
<table style="border:1px solid black;">
<tr class="thead">
<th style="border:1px solid black;" >
</th>
<th style="border:1px solid black;" >
Részletek        
</th>
<th style="border:1px solid black;" >
Részletek        
</th>
<th style="border:1px solid black;" >
Részletek        
</th>
<th style="border:1px solid black;" >
Részletek        
</th>
<th style="border:1px solid black;" >
Részletek        
</th>
</tr>
<tr>
<td style="border:1px solid black;">
**Közlemény azonosítója**
</td>
<td style="border:1px solid black;">
[**MS07-042**](http://go.microsoft.com/fwlink/?linkid=88350)
</td>
<td style="border:1px solid black;">
[**MS07-043**](http://go.microsoft.com/fwlink/?linkid=70249)
</td>
<td style="border:1px solid black;">
[**MS07-044**](http://go.microsoft.com/fwlink/?linkid=96778)
</td>
<td style="border:1px solid black;">
[**MS07-045**](http://go.microsoft.com/fwlink/?linkid=91712)
</td>
<td style="border:1px solid black;">
[**MS07-046**](http://go.microsoft.com/fwlink/?linkid=94466)
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
**Súlyosság maximális foka**
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
</tr>
<tr>
<th colspan="6">
Érintett Windows-szoftverek
</th>
</tr>
<tr>
<td style="border:1px solid black;">
Microsoft Windows 2000 Service Pack 4
</td>
<td style="border:1px solid black;">
**<sup>[1]</sup>**
</td>
<td style="border:1px solid black;">
[Kritikus](http://www.microsoft.com/downloads/details.aspx?familyid=5c35b6e8-732a-4451-b5d4-23ed63e6e792)
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
**<sup>[1]</sup>**
</td>
<td style="border:1px solid black;">
[Kritikus](http://www.microsoft.com/downloads/details.aspx?familyid=8fc8340b-c2b3-4559-835c-caa00cf086b9)
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
Windows XP Service Pack 2
</td>
<td style="border:1px solid black;">
**<sup>[1]</sup>**
</td>
<td style="border:1px solid black;">
[Kritikus](http://www.microsoft.com/downloads/details.aspx?familyid=6e8de050-8589-4831-ae19-075c93509485)
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
**<sup>[1]</sup>**
</td>
<td style="border:1px solid black;">
[Kritikus](http://www.microsoft.com/downloads/details.aspx?familyid=dc29475d-c0bb-4d35-8dd6-4ca1cac32315)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Windows XP Service Pack 3
</td>
<td style="border:1px solid black;">
**<sup>[1]</sup>**
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
Windows XP Professional x64 Edition
</td>
<td style="border:1px solid black;">
**<sup>[1]</sup>**
</td>
<td style="border:1px solid black;">
[Kritikus](http://www.microsoft.com/downloads/details.aspx?familyid=b85bb583-dc61-4d37-b458-208f5bb07ece)
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
**<sup>[1]</sup>**
</td>
<td style="border:1px solid black;">
[Kritikus](http://www.microsoft.com/downloads/details.aspx?familyid=3c81730a-981a-4649-b2d9-45144230d512)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Windows XP Professional x64 Edition Service Pack 2
</td>
<td style="border:1px solid black;">
**<sup>[1]</sup>**
</td>
<td style="border:1px solid black;">
[Kritikus](http://www.microsoft.com/downloads/details.aspx?familyid=b85bb583-dc61-4d37-b458-208f5bb07ece)
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
**<sup>[1]</sup>**
</td>
<td style="border:1px solid black;">
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
Windows Server 2003 Service Pack 1
</td>
<td style="border:1px solid black;">
**<sup>[1]</sup>**
</td>
<td style="border:1px solid black;">
[Mérsékelt.](http://www.microsoft.com/downloads/details.aspx?familyid=15d4d4fa-9bab-4da5-978e-f89c78c8086a)
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
**<sup>[1]</sup>**
</td>
<td style="border:1px solid black;">
[Kritikus](http://www.microsoft.com/downloads/details.aspx?familyid=5374583d-de68-4d65-bca8-598d6b98b8b3)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Windows Server 2003 Service Pack 2
</td>
<td style="border:1px solid black;">
**<sup>[1]</sup>**
</td>
<td style="border:1px solid black;">
[Mérsékelt.](http://www.microsoft.com/downloads/details.aspx?familyid=15d4d4fa-9bab-4da5-978e-f89c78c8086a)
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
**<sup>[1]</sup>**
</td>
<td style="border:1px solid black;">
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
Windows Server 2003 x64 Edition
</td>
<td style="border:1px solid black;">
**<sup>[1]</sup>**
</td>
<td style="border:1px solid black;">
[Mérsékelt.](http://www.microsoft.com/downloads/details.aspx?familyid=6608d722-3ef8-4085-b771-7b17bb0ba06e)
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
**<sup>[1]</sup>**
</td>
<td style="border:1px solid black;">
[Kritikus](http://www.microsoft.com/downloads/details.aspx?familyid=c3359f27-e03e-4a4f-b896-3bda39f69f7e)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Windows Server 2003 x64 Edition Service Pack 2
</td>
<td style="border:1px solid black;">
**<sup>[1]</sup>**
</td>
<td style="border:1px solid black;">
[Mérsékelt.](http://www.microsoft.com/downloads/details.aspx?familyid=6608d722-3ef8-4085-b771-7b17bb0ba06e)
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
**<sup>[1]</sup>**
</td>
<td style="border:1px solid black;">
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
Windows Server 2003 SP1 for Itanium-based Systems
</td>
<td style="border:1px solid black;">
**<sup>[1]</sup>**
</td>
<td style="border:1px solid black;">
[Mérsékelt.](http://www.microsoft.com/downloads/details.aspx?familyid=fc04451a-0696-4a21-b2b6-f02d4e2c33bf)
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
**<sup>[1]</sup>**
</td>
<td style="border:1px solid black;">
[Kritikus](http://www.microsoft.com/downloads/details.aspx?familyid=92822479-2060-4357-a340-ed096f180b2b)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Windows Server 2003 SP2 for Itanium-based Systems
</td>
<td style="border:1px solid black;">
**<sup>[1]</sup>**
</td>
<td style="border:1px solid black;">
[Mérsékelt.](http://www.microsoft.com/downloads/details.aspx?familyid=fc04451a-0696-4a21-b2b6-f02d4e2c33bf)
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
**<sup>[1]</sup>**
</td>
<td style="border:1px solid black;">
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
Windows Vista
</td>
<td style="border:1px solid black;">
**<sup>[1]</sup>**
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
**<sup>[1]</sup>**
</td>
<td style="border:1px solid black;">
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Windows Vista Service Pack 1
</td>
<td style="border:1px solid black;">
**<sup>[1]</sup>**
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
Windows Vista x64 Edition
</td>
<td style="border:1px solid black;">
**<sup>[1]</sup>**
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
**<sup>[1]</sup>**
</td>
<td style="border:1px solid black;">
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Windows Vista x64 Edition Service Pack 1
</td>
<td style="border:1px solid black;">
**<sup>[1]</sup>**
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
Windows Server 2008 32 bites rendszerekhez
</td>
<td style="border:1px solid black;">
**<sup>[1]</sup>**
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Windows Server 2008 x64 alapú rendszerekhez
</td>
<td style="border:1px solid black;">
**<sup>[1]</sup>**
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
Windows Server 2008 for Itanium-based Systems
</td>
<td style="border:1px solid black;">
**<sup>[1]</sup>**
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
</td>
</tr>
<tr>
<th colspan="6">
A Windows operációs rendszer érintett összetevői
</th>
</tr>
<tr>
<td style="border:1px solid black;">
Internet Explorer 5.01 Service Pack 4 alkalmazás Microsoft Windows 2000 Service Pack 4 rendszeren
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
[Kritikus](http://www.microsoft.com/downloads/details.aspx?familyid=fcf9440f-bb36-4ed1-9b6b-74a4f055650b)
</td>
<td style="border:1px solid black;">
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
Internet Explorer 6 Service Pack 1, Microsoft Windows 2000 Service Pack 4 rendszerre telepítve
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
[Kritikus](http://www.microsoft.com/downloads/details.aspx?familyid=8db75461-4dca-43db-aa30-c7e67ce954ad)
</td>
<td style="border:1px solid black;">
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Internet Explorer 6 Windows XP Service Pack 2 rendszeren
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
[Kritikus](http://www.microsoft.com/downloads/details.aspx?familyid=5d31d916-867f-4dbf-b8a4-c75ea83f4f51)
</td>
<td style="border:1px solid black;">
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
Internet Explorer 6 alkalmazás Windows XP Professional x64 Edition és Windows XP Professional x64 Edition Service Pack 2 rendszeren
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
[Kritikus](http://www.microsoft.com/downloads/details.aspx?familyid=b15b2442-d6da-41dd-a424-11c9893be595)
</td>
<td style="border:1px solid black;">
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Internet Explorer 6 alkalmazás Windows Server 2003 Service Pack 1 és Windows Server 2003 Service Pack 2 rendszerhez:
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
[Mérsékelt.](http://www.microsoft.com/downloads/details.aspx?familyid=f2f9fb69-0399-4df0-9f5b-8f42a130c581)
</td>
<td style="border:1px solid black;">
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
Internet Explorer 6 Windows Server 2003 x64 Edition és Windows Server 2003 x64 Edition Service Pack 2 rendszeren
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
[Mérsékelt.](http://www.microsoft.com/downloads/details.aspx?familyid=d0bd886d-2c80-4dd7-82b7-1bd1f8d398cc)
</td>
<td style="border:1px solid black;">
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Internet Explorer 6 Windows Server 2003 SP1 javítócsomaggal ellátott Itanium-alapú rendszerekhez és Windows Server 2003 SP2 csomaggal ellátott Itanium-alapú rendszerekhez
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
[Mérsékelt.](http://www.microsoft.com/downloads/details.aspx?familyid=bf41033a-d6f0-451e-9b69-4cbe2bb3f804)
</td>
<td style="border:1px solid black;">
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
Internet Explorer 7 Windows XP Service Pack 2 rendszeren
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
[Fontos](http://www.microsoft.com/downloads/details.aspx?familyid=7a2b4395-eaba-45ec-8d0c-932ebcc3d344)
</td>
<td style="border:1px solid black;">
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Internet Explorer 7 alkalmazás Windows XP Professional x64 Edition és Windows XP Professional x64 Edition Service Pack 2 rendszeren
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
[Fontos](http://www.microsoft.com/downloads/details.aspx?familyid=cd7ed4d5-7790-41db-8b68-cfd59105ca36)
</td>
<td style="border:1px solid black;">
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
Internet Explorer 7 alkalmazás Windows Server 2003 Service Pack 1 és Windows Server 2003 Service Pack 2 rendszeren
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
[Alacsony](http://www.microsoft.com/downloads/details.aspx?familyid=4f8daed8-9925-494d-b2f5-1e29f4040f6a)
</td>
<td style="border:1px solid black;">
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Internet Explorer 7 Windows Server 2003 x64 Edition és Windows Server 2003 x64 Edition Service Pack 2 rendszeren
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
[Alacsony](http://www.microsoft.com/downloads/details.aspx?familyid=34669ca2-46b0-4fbf-8fbd-ad7a13920103)
</td>
<td style="border:1px solid black;">
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
Internet Explorer 7 Windows Server 2003 SP1 javítócsomaggal ellátott Itanium-alapú rendszerekhez és Windows Server 2003 SP2 csomaggal ellátott Itanium-alapú rendszerekhez
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
[Alacsony](http://www.microsoft.com/downloads/details.aspx?familyid=5bd7bcbd-528a-4a16-a39a-a5ff5f69a2e2)
</td>
<td style="border:1px solid black;">
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Internet Explorer 7 alkalmazás a Windows Vista rendszeren
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
[Fontos](http://www.microsoft.com/downloads/details.aspx?familyid=9ae27b2f-aca4-4758-8ce4-a98f1ff6ba70)
</td>
<td style="border:1px solid black;">
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
Internet Explorer 7 alkalmazás Windows Vista x64 rendszeren
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
[Fontos](http://www.microsoft.com/downloads/details.aspx?familyid=53497e53-d10c-43af-ad56-9f07739a5284)
</td>
<td style="border:1px solid black;">
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Microsoft XML Core Services 3.0 (KB936021) alkalmazás Microsoft Windows 2000 Service Pack 4 rendszeren
</td>
<td style="border:1px solid black;">
[Kritikus](http://www.microsoft.com/downloads/details.aspx?familyid=245214ea-76f9-4755-8a14-a74232e20c1c)
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
Microsoft XML Core Services 3.0 alkalmazás (KB936021) Windows XP Service Pack 2 rendszeren
</td>
<td style="border:1px solid black;">
[Kritikus](http://www.microsoft.com/downloads/details.aspx?familyid=dea6a48f-fb00-43f3-a374-3220f9759c2d)
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Microsoft XML Core Services 3.0 alkalmazás (KB936021) Windows XP Professional x64 Edition és Windows XP Professional x64 Edition Service Pack 2 rendszeren
</td>
<td style="border:1px solid black;">
[Kritikus](http://www.microsoft.com/downloads/details.aspx?familyid=b8862ca9-1203-4056-a257-29271838ac0d)
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
Microsoft XML Core Services 3.0 alkalmazás (KB936021) Windows Server 2003 Service Pack 1 és Windows Server 2003 Service Pack 2 rendszeren
</td>
<td style="border:1px solid black;">
[Mérsékelt.](http://www.microsoft.com/downloads/details.aspx?familyid=12618ad0-aefd-4c9a-a769-4b14a7603d6e)
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Microsoft XML Core Services 3.0 alkalmazás (KB936021) Windows Server 2003 x64 Edition és Windows Server 2003 x64 Edition Service Pack 2 rendszeren
</td>
<td style="border:1px solid black;">
[Mérsékelt.](http://www.microsoft.com/downloads/details.aspx?familyid=61bf00a9-aeea-431a-86d3-526a4a373bb7)
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
Microsoft XML Core Services 3.0 alkalmazás (KB936021) Windows Server 2003 SP1 Itanium alapú rendszerekhez és Windows Server 2003 SP2 Itanium alapú rendszerekhez telepítve
</td>
<td style="border:1px solid black;">
[Mérsékelt.](http://www.microsoft.com/downloads/details.aspx?familyid=b0285dd7-bf66-4226-9948-26e8aae99046)
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Microsoft XML Core Services 3.0 alkalmazás (KB936021) Windows Vista rendszeren
</td>
<td style="border:1px solid black;">
[Kritikus](http://www.microsoft.com/downloads/details.aspx?familyid=c734d7de-5d87-4904-81c3-714db2cb8b0d)
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
Microsoft XML Core Services 3.0 alkalmazás (KB936021) Windows Vista x64 rendszeren
</td>
<td style="border:1px solid black;">
[Kritikus](http://www.microsoft.com/downloads/details.aspx?familyid=0a465d77-a737-4d26-82a1-570f9c788a8a)
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Microsoft XML Core Services 4.0 alkalmazás (KB936181) Windows 2000 Service Pack 4 rendszeren
</td>
<td style="border:1px solid black;">
[Kritikus](http://www.microsoft.com/downloads/details.aspx?familyid=021e12f5-cb46-43df-a2b8-185639ba2807)
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
Microsoft XML Core Services 4.0 (KB936181) alkalmazás Windows XP Service Pack 2 és Windows XP Service Pack 3 rendszeren
</td>
<td style="border:1px solid black;">
[Kritikus](http://www.microsoft.com/downloads/details.aspx?familyid=021e12f5-cb46-43df-a2b8-185639ba2807)
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Microsoft XML Core Services 4.0 alkalmazás (KB936181) Windows XP Professional x64 Edition és Windows XP Professional x64 Edition Service Pack 2 rendszeren
</td>
<td style="border:1px solid black;">
[Kritikus](http://www.microsoft.com/downloads/details.aspx?familyid=021e12f5-cb46-43df-a2b8-185639ba2807)
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
Microsoft XML Core Services 4.0 alkalmazás (KB936181) Windows Server 2003 Service Pack 1 és Windows Server 2003 Service Pack 2 rendszeren
</td>
<td style="border:1px solid black;">
[Mérsékelt.](http://www.microsoft.com/downloads/details.aspx?familyid=021e12f5-cb46-43df-a2b8-185639ba2807)
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Microsoft XML Core Services 4.0 alkalmazás (KB936181) Windows Server 2003 x64 Edition és Windows Server 2003 x64 Edition Service Pack 2 rendszeren
</td>
<td style="border:1px solid black;">
[Mérsékelt.](http://www.microsoft.com/downloads/details.aspx?familyid=021e12f5-cb46-43df-a2b8-185639ba2807)
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
Microsoft XML Core Services 4.0 alkalmazás (KB936181) Windows Server 2003 SP1 Itanium alapú rendszerekhez és Windows Server 2003 SP2 Itanium alapú rendszerekhez telepítés esetén
</td>
<td style="border:1px solid black;">
[Mérsékelt.](http://www.microsoft.com/downloads/details.aspx?familyid=021e12f5-cb46-43df-a2b8-185639ba2807)
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Microsoft XML Core Services 4.0 (KB936181) alkalmazás Windows Vista és Windows Vista Service Pack 1 rendszeren
</td>
<td style="border:1px solid black;">
[Kritikus](http://www.microsoft.com/downloads/details.aspx?familyid=021e12f5-cb46-43df-a2b8-185639ba2807)
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
Microsoft XML Core Services 4.0 alkalmazás (KB936181) Windows Vista x64 Edition és Windows Vista x64 Edition Service Pack 1 rendszeren
</td>
<td style="border:1px solid black;">
[Kritikus](http://www.microsoft.com/downloads/details.aspx?familyid=021e12f5-cb46-43df-a2b8-185639ba2807)
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Microsoft XML Core Services 4.0 (KB936181) alkalmazás Windows Server 2008 32 bites rendszerekhez környezetben
</td>
<td style="border:1px solid black;">
[Mérsékelt.](http://www.microsoft.com/downloads/details.aspx?familyid=021e12f5-cb46-43df-a2b8-185639ba2807)
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
Microsoft XML Core Services 4.0 (KB936181) alkalmazás Windows Server 2008 x64 alapú rendszerekhez környezetben
</td>
<td style="border:1px solid black;">
[Mérsékelt.](http://www.microsoft.com/downloads/details.aspx?familyid=021e12f5-cb46-43df-a2b8-185639ba2807)
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Microsoft XML Core Services 4.0 (KB936181) alkalmazás Windows Server 2008 Itanium-alapú rendszerekhez környezetben
</td>
<td style="border:1px solid black;">
[Mérsékelt.](http://www.microsoft.com/downloads/details.aspx?familyid=021e12f5-cb46-43df-a2b8-185639ba2807)
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
Microsoft XML Core Services 6.0  
(KB933579) Microsoft Windows 2000 Service Pack 4 rendszeren
</td>
<td style="border:1px solid black;">
[Kritikus](http://www.microsoft.com/downloads/details.aspx?familyid=70c92e77-9e5a-41b1-a9d2-64443913c976)
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Microsoft XML Core Services 6.0 alkalmazás (KB933579) Windows XP Service Pack 2 rendszeren
</td>
<td style="border:1px solid black;">
[Kritikus](http://www.microsoft.com/downloads/details.aspx?familyid=70c92e77-9e5a-41b1-a9d2-64443913c976)
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
Microsoft XML Core Services 6.0 alkalmazás (KB933579) Windows XP Professional x64 Edition és Windows XP Professional x64 Edition Service Pack 2 rendszeren
</td>
<td style="border:1px solid black;">
[Kritikus](http://www.microsoft.com/downloads/details.aspx?familyid=70c92e77-9e5a-41b1-a9d2-64443913c976)
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Microsoft XML Core Services 6.0 alkalmazás (KB933579) Windows Server 2003 Service Pack 1 és Windows Server 2003 Service Pack 2 rendszeren
</td>
<td style="border:1px solid black;">
[Mérsékelt.](http://www.microsoft.com/downloads/details.aspx?familyid=70c92e77-9e5a-41b1-a9d2-64443913c976)
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
Microsoft XML Core Services 6.0 alkalmazás (KB933579) Windows Server 2003 x64 Edition és Windows Server 2003 x64 Edition Service Pack 2 rendszeren
</td>
<td style="border:1px solid black;">
[Mérsékelt.](http://www.microsoft.com/downloads/details.aspx?familyid=70c92e77-9e5a-41b1-a9d2-64443913c976)
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Microsoft XML Core Services 6.0 alkalmazás (KB933579) Windows Server 2003 SP1 Itanium alapú rendszerekhez és Windows Server 2003 SP2 Itanium alapú rendszerekhez telepítés esetén
</td>
<td style="border:1px solid black;">
[Mérsékelt.](http://www.microsoft.com/downloads/details.aspx?familyid=70c92e77-9e5a-41b1-a9d2-64443913c976)
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
Microsoft XML Core Services 6.0 alkalmazás (KB933579) Windows Vista rendszeren
</td>
<td style="border:1px solid black;">
[Kritikus](http://www.microsoft.com/downloads/details.aspx?familyid=14270529-3ae5-43bf-a471-722ab010d81e)
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Microsoft XML Core Services 6.0 alkalmazás (KB933579) Windows Vista x64 rendszeren
</td>
<td style="border:1px solid black;">
[Kritikus](http://www.microsoft.com/downloads/details.aspx?familyid=928da3d2-b0b9-447a-b37a-4350497fe563)
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
</td>
</tr>
<tr>
<th colspan="6">
Érintett Office-szoftverek
</th>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
Microsoft Excel 2000 Service Pack 3
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
[Kritikus](http://www.microsoft.com/downloads/details.aspx?familyid=082b98f7-9556-4f1f-823a-c41ddf5a7c9a)
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Microsoft Excel 2002 Service Pack 3
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
[Fontos](http://www.microsoft.com/downloads/details.aspx?familyid=91308769-2577-4f9f-8209-06f2c8c8a86f)
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
Microsoft Excel 2003 Service Pack 2
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
[Fontos](http://www.microsoft.com/downloads/details.aspx?familyid=b0130e9e-8845-4d79-aaa1-a21cc9388abe)
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Microsoft Office 2003 Service Pack 2 rendszer Microsoft XML Core Services 5.0 alkalmazással (KB936048)
</td>
<td style="border:1px solid black;">
[Kritikus](http://www.microsoft.com/downloads/details.aspx?familyid=a339cb7b-e08a-47f8-ac0b-df449191424a)
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
Microsoft Excel Viewer 2003
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
[Fontos](http://www.microsoft.com/downloads/details.aspx?familyid=c4a87572-3128-44f7-8069-95535a78500a)
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Microsoft Word Viewer 2003 alkalmazás Microsoft XML Core Services 5.0 alkalmazással (KB936048)
</td>
<td style="border:1px solid black;">
[Kritikus](http://www.microsoft.com/downloads/details.aspx?familyid=a339cb7b-e08a-47f8-ac0b-df449191424a)
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
Microsoft Office 2004 for Mac
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
[Kritikus](http://www.microsoft.com/mac/downloads.aspx)
</td>
<td style="border:1px solid black;">
[Fontos](http://www.microsoft.com/mac/downloads.aspx)
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Office 2007 rendszer Microsoft XML Core Services 5.0 alkalmazással (KB936960)
</td>
<td style="border:1px solid black;">
[Kritikus](http://www.microsoft.com/downloads/details.aspx?familyid=7a97478a-832c-4a6b-b074-0e18b1e4ed33)
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
Microsoft Office Groove Server 2007 rendszer Microsoft XML Core Services 5.0 alkalmazással (KB936056)
</td>
<td style="border:1px solid black;">
[Kritikus](http://www.microsoft.com/downloads/details.aspx?familyid=e875613b-2f32-4f28-a635-664a25c95c18)
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Microsoft Office SharePoint Server rendszer Microsoft XML Core Services 5.0 alkalmazással (KB936056)
</td>
<td style="border:1px solid black;">
[Kritikus](http://www.microsoft.com/downloads/details.aspx?familyid=e875613b-2f32-4f28-a635-664a25c95c18)
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
</td>
</tr>
<tr>
<th colspan="6">
Más érintett szoftverek
</th>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
Microsoft Visual Basic 6.0 Service Pack 6 (KB924053)
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
[Kritikus](http://www.microsoft.com/downloads/details.aspx?familyid=e1646fb0-29d5-4a6e-a8d2-304c4d7735b7)
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
</td>
</tr>
</table>
 
**Megjegyzések:**

**<sup>[1]</sup>** Ehhez az operációs rendszerhez rendelkezésre áll egy biztonsági frissítés. További információt a táblázat érintett szoftverre vagy összetevőre vonatkozó részében illetve az ide vonatkozó biztonsági közleményben talál.** **

#### Érintett szoftverek és letöltési helyek az MS07-047 – MS07-050 közlemények vonatkozásában

**Érintett szoftverek és letöltési helyek**

 
<p> </p>
<table style="border:1px solid black;">
<tr class="thead">
<th style="border:1px solid black;" >
</th>
<th style="border:1px solid black;" >
Részletek        
</th>
<th style="border:1px solid black;" >
Részletek        
</th>
<th style="border:1px solid black;" >
Részletek        
</th>
<th style="border:1px solid black;" >
Részletek        
</th>
</tr>
<tr>
<td style="border:1px solid black;">
**Közlemény azonosítója**
</td>
<td style="border:1px solid black;">
[**MS07-047**](http://go.microsoft.com/fwlink/?linkid=88628)
</td>
<td style="border:1px solid black;">
[**MS07-048**](http://go.microsoft.com/fwlink/?linkid=94465)
</td>
<td style="border:1px solid black;">
[**MS07-049**](http://go.microsoft.com/fwlink/?linkid=92734)
</td>
<td style="border:1px solid black;">
[**MS07-050**](http://go.microsoft.com/fwlink/?linkid=94737)
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
**Súlyosság maximális foka**
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
[**Kritikus**](http://go.microsoft.com/fwlink/?linkid=21140)
</td>
</tr>
<tr>
<th colspan="5">
Érintett Windows-szoftverek
</th>
</tr>
<tr>
<td style="border:1px solid black;">
Microsoft Windows 2000 Service Pack 4
</td>
<td style="border:1px solid black;">
**<sup>[1]</sup>**
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
**<sup>[1]</sup>**
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
Windows XP Service Pack 2
</td>
<td style="border:1px solid black;">
**<sup>[1]</sup>**
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
**<sup>[1]</sup>**
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Windows XP Professional x64 Edition
</td>
<td style="border:1px solid black;">
**<sup>[1]</sup>**
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
**<sup>[1]</sup>**
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
Windows XP Professional x64 Edition Service Pack 2
</td>
<td style="border:1px solid black;">
**<sup>[1]</sup>**
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
**<sup>[1]</sup>**
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Windows Server 2003 Service Pack 1
</td>
<td style="border:1px solid black;">
**<sup>[1]</sup>**
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
**<sup>[1]</sup>**
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
Windows Server 2003 Service Pack 2
</td>
<td style="border:1px solid black;">
**<sup>[1]</sup>**
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
**<sup>[1]</sup>**
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Windows Server 2003 x64 Edition
</td>
<td style="border:1px solid black;">
**<sup>[1]</sup>**
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
**<sup>[1]</sup>**
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
Windows Server 2003 x64 Edition Service Pack 2
</td>
<td style="border:1px solid black;">
**<sup>[1]</sup>**
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
**<sup>[1]</sup>**
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Windows Server 2003 SP1 for Itanium-based Systems
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
**<sup>[1]</sup>**
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
Windows Server 2003 SP2 for Itanium-based Systems
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
**<sup>[1]</sup>**
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Windows Vista
</td>
<td style="border:1px solid black;">
**<sup>[1]</sup>**
</td>
<td style="border:1px solid black;">
[Fontos](http://www.microsoft.com/downloads/details.aspx?familyid=49a5bd84-da71-4529-b4d3-ac57dab59e01)
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
**<sup>[1]</sup>**
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
Windows Vista x64 Edition
</td>
<td style="border:1px solid black;">
**<sup>[1]</sup>**
</td>
<td style="border:1px solid black;">
[Fontos](http://www.microsoft.com/downloads/details.aspx?familyid=24443f59-b908-480b-9b72-7094d4b5e128)
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
**<sup>[1]</sup>**
</td>
</tr>
<tr>
<th colspan="5">
A Windows operációs rendszer érintett összetevői
</th>
</tr>
<tr>
<td style="border:1px solid black;">
Internet Explorer 5.01 Service Pack 4 alkalmazás Microsoft Windows 2000 Service Pack 4 rendszeren
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
[Kritikus](http://www.microsoft.com/downloads/details.aspx?familyid=31e63d6f-b6b7-41d7-8ae6-dd7fcf89d477)
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
Internet Explorer 6 Service Pack 1, Microsoft Windows 2000 Service Pack 4 rendszerre telepítve
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
[Kritikus](http://www.microsoft.com/downloads/details.aspx?familyid=7099d33a-0ef6-423f-824e-757482517612)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Internet Explorer 6 Windows XP Service Pack 2 rendszeren
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
[Kritikus](http://www.microsoft.com/downloads/details.aspx?familyid=4447d74f-09ea-4be0-9dae-c243ce657fb7)
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
Internet Explorer 6 alkalmazás Windows XP Professional x64 Edition és Windows XP Professional x64 Edition Service Pack 2 rendszeren
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
[Kritikus](http://www.microsoft.com/downloads/details.aspx?familyid=98ccd207-f4d0-4625-aeab-0ebf1643a5fd)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Internet Explorer 6 alkalmazás Windows Server 2003 Service Pack 1 és Windows Server 2003 Service Pack 2 rendszerhez:
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
[Kritikus](http://www.microsoft.com/downloads/details.aspx?familyid=463535aa-e04e-4a30-b3ab-8cd6d8cdd13c)
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
Internet Explorer 6 Windows Server 2003 x64 Edition és Windows Server 2003 x64 Edition Service Pack 2 rendszeren
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
[Kritikus](http://www.microsoft.com/downloads/details.aspx?familyid=9d4375d4-fb9b-4771-bd6f-e5d23eedbc6b)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Internet Explorer 6 Windows Server 2003 SP1 javítócsomaggal ellátott Itanium-alapú rendszerekhez és Windows Server 2003 SP2 csomaggal ellátott Itanium-alapú rendszerekhez
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
[Kritikus](http://www.microsoft.com/downloads/details.aspx?familyid=c7be313b-3405-42e1-9e4b-0cb6bf3d2cb1)
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
Internet Explorer 7 Windows XP Service Pack 2 rendszeren
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
[Kritikus](http://www.microsoft.com/downloads/details.aspx?familyid=9f5da816-194c-478e-8a96-9421a0c52c9f)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Internet Explorer 7 alkalmazás Windows XP Professional x64 Edition és Windows XP Professional x64 Edition Service Pack 2 rendszeren
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
[Kritikus](http://www.microsoft.com/downloads/details.aspx?familyid=1c3168a9-d959-4137-868a-ec70da737c21)
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
Internet Explorer 7 alkalmazás Windows Server 2003 Service Pack 1 és Windows Server 2003 Service Pack 2 rendszeren
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
[Kritikus](http://www.microsoft.com/downloads/details.aspx?familyid=59884e97-4912-4a9a-8a31-8182ea2d24db)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Internet Explorer 7 Windows Server 2003 x64 Edition és Windows Server 2003 x64 Edition Service Pack 2 rendszeren
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
[Kritikus](http://www.microsoft.com/downloads/details.aspx?familyid=42060e27-de14-4d0c-92a0-138cb57fe2b5)
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
Internet Explorer 7 Windows Server 2003 SP1 javítócsomaggal ellátott Itanium-alapú rendszerekhez és Windows Server 2003 SP2 csomaggal ellátott Itanium-alapú rendszerekhez
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
[Kritikus](http://www.microsoft.com/downloads/details.aspx?familyid=a536206e-9d1b-49a8-81a1-53d46f2de973)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Internet Explorer 7 alkalmazás a Windows Vista rendszeren
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
[Kritikus](http://www.microsoft.com/downloads/details.aspx?familyid=2dd908a4-6152-4976-aaaa-01f5f37c9143)
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
Internet Explorer 7 alkalmazás Windows Vista x64 rendszeren
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
[Kritikus](http://www.microsoft.com/downloads/details.aspx?familyid=592435bc-1d43-4544-bd8a-4a2d829dc1a1)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Windows Media Player 7.1 alkalmazás Microsoft Windows 2000 Service Pack 4 rendszeren
</td>
<td style="border:1px solid black;">
[Fontos](http://www.microsoft.com/downloads/details.aspx?familyid=9f46b1fc-ee7b-437f-9492-67d003711021)
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
Windows Media Player 9 alkalmazás Microsoft Windows 2000 Service Pack 4 rendszeren
</td>
<td style="border:1px solid black;">
[Fontos](http://www.microsoft.com/downloads/details.aspx?familyid=bd4a6474-5fde-415e-840e-7d973cb71c95)
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Windows Media Player 9 Windows XP Service Pack 2 operációs rendszerhez
</td>
<td style="border:1px solid black;">
[Fontos](http://www.microsoft.com/downloads/details.aspx?familyid=bd4a6474-5fde-415e-840e-7d973cb71c95)
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
Windows Media Player 10 alkalmazás Windows XP Service Pack 2 rendszeren
</td>
<td style="border:1px solid black;">
[Fontos](http://www.microsoft.com/downloads/details.aspx?familyid=48f5a9d3-b859-4cb6-a68e-abde76a14782)
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Windows Media Player 10 alkalmazás Windows XP Professional x64 Edition és Windows XP Professional x64 Edition Service Pack 2 rendszeren
</td>
<td style="border:1px solid black;">
[Fontos](http://www.microsoft.com/downloads/details.aspx?familyid=949580be-cbb3-4271-8ca0-0ead7f2d8801)
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
Windows Media Player 10 alkalmazás Windows Server 2003 Service Pack 1 és Windows Server 2003 Service Pack 2 rendszeren
</td>
<td style="border:1px solid black;">
[Fontos](http://www.microsoft.com/downloads/details.aspx?familyid=8d9f1fdf-6d4c-44d4-9b5f-bdbe8ac28d7f)
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Windows Media Player 10 alkalmazás Windows Server 2003 x64 Edition és Windows Server 2003 x64 Edition Service Pack 2 rendszeren
</td>
<td style="border:1px solid black;">
[Fontos](http://www.microsoft.com/downloads/details.aspx?familyid=2c04c7f2-728e-43bd-8574-26e411fcd129)
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
Windows Media Player 11 alkalmazás Windows XP Service Pack 2 rendszeren
</td>
<td style="border:1px solid black;">
[Fontos](http://www.microsoft.com/downloads/details.aspx?familyid=a690d042-1137-4aaf-bd0e-565ea04d1f2b)
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Windows Media Player 11 alkalmazás Windows XP Professional x64 Edition és Windows XP Professional x64 Edition Service Pack 2 rendszeren
</td>
<td style="border:1px solid black;">
[Fontos](http://www.microsoft.com/downloads/details.aspx?familyid=bdc89f34-c1ff-46ab-b52d-c02d51c5c373)
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
Windows Media Player 11 alkalmazás Windows Vista rendszeren
</td>
<td style="border:1px solid black;">
[Fontos](http://www.microsoft.com/downloads/details.aspx?familyid=80e5167c-4f75-4ce3-8b15-2f50958deec8)
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Windows Vista x64 rendszeren működő Windows Media Player 11 esetén
</td>
<td style="border:1px solid black;">
[Fontos](http://www.microsoft.com/downloads/details.aspx?familyid=bf30b714-d6e7-47ea-b79e-84c18370a661)
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
</td>
</tr>
<tr>
<th colspan="5">
Más érintett szoftverek
</th>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
Microsoft Virtual PC 2004
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
[Fontos](http://www.microsoft.com/downloads/details.aspx?familyid=cbdeaa50-7115-4673-97c4-10009f9c5c42)
</td>
<td style="border:1px solid black;">
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Microsoft Virtual PC 2004 Service Pack 1
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
[Fontos](http://www.microsoft.com/downloads/details.aspx?familyid=17ffe5a2-3551-4858-93b6-5e25af87d808)
</td>
<td style="border:1px solid black;">
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
Microsoft Virtual Server 2005 Standard Edition
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
[Fontos](http://www.microsoft.com/downloads/details.aspx?familyid=bc02ea6d-2884-4637-9894-3413a71329ee)
</td>
<td style="border:1px solid black;">
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Microsoft Virtual Server 2005 Enterprise Edition
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
[Fontos](http://www.microsoft.com/downloads/details.aspx?familyid=da474b6f-9f0c-43f6-b432-050f7e76967d)
</td>
<td style="border:1px solid black;">
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
Microsoft Virtual Server 2005 R2 Standard Edition
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
[Fontos](http://www.microsoft.com/downloads/details.aspx?familyid=43fa1327-8e5e-4c92-901f-1ff2a0a087b4)
</td>
<td style="border:1px solid black;">
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Microsoft Virtual Server 2005 R2 Enterprise Edition
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
[Fontos](http://www.microsoft.com/downloads/details.aspx?familyid=c2fc16c4-1fb0-4c09-b04a-684b40df8517)
</td>
<td style="border:1px solid black;">
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
Microsoft Virtual PC for Mac Version 6.1
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
[Fontos](http://www.microsoft.com/mac/downloads.aspx)
</td>
<td style="border:1px solid black;">
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Microsoft Virtual PC for Mac Version 7
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
[Fontos](http://www.microsoft.com/mac/downloads.aspx)
</td>
<td style="border:1px solid black;">
</td>
</tr>
</table>
 
**Megjegyzések:**

**<sup>[1]</sup>** Ehhez az operációs rendszerhez rendelkezésre áll egy biztonsági frissítés. További információt a táblázat érintett szoftverre vagy összetevőre vonatkozó részében illetve az ide vonatkozó biztonsági közleményben talál.** **

Észlelési és telepítési eszközök, útmutatás
-------------------------------------------

<span></span>
**Biztonsági központ**

A szoftveres és biztonsági frissítések kezeléséhez azokat a szervezet asztali és hordozható számítógépeire, valamint kiszolgálóira is telepíteni kell. További tájékoztatásért látogasson el a [TechNet Update Management Center](http://go.microsoft.com/fwlink/?linkid=69903) weboldalára. A [TechNet Security Center](http://go.microsoft.com/fwlink/?linkid=21171) bővebb tájékoztatással szolgál a Microsoft-termékek biztonsági funkcióival kapcsolatban. A [Biztonság otthon](http://go.microsoft.com/fwlink/?linkid=85102) weboldalon a megfelelő hivatkozásra kattintva elérhetőek a legújabb biztonsági frissítések.

A biztonsági frissítések a [Microsoft Update](http://go.microsoft.com/fwlink/?linkid=40747), [Windows Update](http://go.microsoft.com/fwlink/?linkid=21130) és az [Office Update](http://go.microsoft.com/fwlink/?linkid=21135) weboldalakról tölthetőek le. A biztonsági frissítések a [Microsoft letöltőközpontjában](http://go.microsoft.com/fwlink/?linkid=21129) is elérhetőek. legegyszerűbben a „biztonsági javítás” kifejezésre irányuló kulcsszavas kereséssel találhatja meg őket. A biztonsági frissítések a Windows Update katalógusából is letölthetőek. A Windows Update katalógusról a [Microsoft Tudásbázis 323166](http://support.microsoft.com/kb/323166/hu) számú cikkében talál információkat.

**Útmutató az észleléshez és a telepítéshez**

A Microsoft az e havi biztonsági frissítésekhez észlelési és telepítési útmutatót adott ki. Az útmutató a számítógépes szakembereknek is ötleteket adhat ahhoz, hogyan használják a különböző eszközöket, pl. Windows Update, Microsoft Update, Office Update, Microsoft Baseline Security Analyzer (MBSA), Office Detection Tool, Microsoft Systems Management Server (SMS), Extended Security Update Inventory Tool vagy Enterprise Update Scan Tool (EST) a biztonsági frissítések telepítéséhez. További információt a [Microsoft Tudásbázis 910723. számú cikkében](http://support.microsoft.com/kb/910723/hu) talál.

**Microsoft Baseline Security Analyzer és** **Enterprise** **Update Scan Tool**

A Microsoft Baseline Security Analyzer (MBSA) segítségével a rendszergazda mind a helyi, mind a távoli számítógépeken ellenőrizheti, hogy mely biztonsági frissítések hiányoznak, illetve hogy mely biztonsági beállítások vannak helytelenül megadva. Ha többet szeretne tudni az MBSA -eszközről, látogasson el a [Microsoft Baseline Security Analyzer webhelyre](http://go.microsoft.com/fwlink/?linkid=21134).

Ha a MBSA 1.2.1 nem támogatja a különleges biztonsági frissítés észlelését, a Microsoft kiad egy külön Enterprise Update Scan Tool (EST) verziót az adott frissítéshez. Az EST-eszközről további információkat az [Enterprise UPdate Scan Tool](http://support.microsoft.com/default.aspx?id=894193&ln=hu) webhelyén talál.

**Megjegyzés** 2007. október 9. óta az MBSA 1.2.1 által felhasznált MSSecure.XML fájl már nem frissül. Ezután az MBSA 1.2.1 által felhasznált MSSecure.XML fájlhoz nem adódnak hozzá új biztonsági frissítések, és nem bocsátanak ki új verziót az Enterprise Scan Tool eszközből. Ha többet szeretne megtudni, látogasson el a [Microsoft Baseline Security Analyzer webhelyre](http://go.microsoft.com/fwlink/?linkid=21134).

**Windows Server Update Services**

A Microsoft Software Update Services (WSUS) szolgáltatással a rendszergazdák gyorsan és megbízható módon telepíthetik központilag a legújabb fontos és biztonsági frissítéseket Windows 2000 és újabb operációs rendszerekhez, Office XP és újabb operációs rendszerekhez, Exchange Server 2003 és SQL Server 2000 Windows 2000 és újabb operációs rendszerekre.

A biztonsági frissítésnek Windows Server Update Services szolgáltatással történő központi telepítéséről a [Windows Server Update Services](http://go.microsoft.com/fwlink/?linkid=50120) webhelyen tudhat meg többet.

**Systems Management Server**

A Microsoft Systems Management Server (SMS) rendszer egy sokoldalúan beállítható vállalati megoldás, amely a frissítések kezelésére szolgál. Az SMS segítségével a rendszergazda megállapíthatja, hogy melyik Windows alapú számítógép szorul biztonsági frissítésre, és ezeket a frissítéseket szabályozott módon, a felhasználók minimális zavarásával központilag telepítheti a vállalat teljes informatikai környezetében. Ha többet szeretne tudni arról, hogy a rendszergazdák miként telepíthetik a biztonsági frissítéseket az SMS 2003 alkalmazással, látogasson el az [SMS 2003 Security Patch Management webhelyre](http://go.microsoft.com/fwlink/?linkid=22939). Az SMS 2.0 verzióját használók a [Software Updates Services Feature Pack](http://go.microsoft.com/fwlink/?linkid=33340) szolgáltatásait is segítségül hívhatják a biztonsági frissítések központi telepítéséhez. Az SMS-szolgáltatásról bővebben a [Microsoft Systems Management Server](http://go.microsoft.com/fwlink/?linkid=21158) oldalán olvashat.

**Megjegyzés:** Az SMS a Microsoft Baseline Security Analyzer és a Microsoft Office Detection Tool program segítségével széles körű támogatást nyújt a frissítések biztonsági értesítők segítségével történő észleléséhez és telepítéséhez. Előfordulhat, hogy egyes szoftverfrissítéseket ezek az eszközök nem észlelnek. Az SMS alkalmazás leltározási szolgáltatásai segítségével a rendszergazdák adott rendszereken hajthatják végre a frissítést. Az eljárással kapcsolatban olvassa el a [szoftverfrissítések telepítése az SMS szoftverelosztó ügynök segítségével](http://go.microsoft.com/fwlink/?linkid=33341) című tájékoztatót. Egyes biztonsági frissítésekhez rendszergazdai jogosultságokra van szükség a számítógép újraindítása után. A rendszergazdák az [SMS 2003 Administration Feature Pack](http://go.microsoft.com/fwlink/?linkid=33387) és az [SMS 2.0 Administration Feature Pack](http://go.microsoft.com/fwlink/?linkid=21161) csomag részét képező Elevated Rights Deployment Tool nevű eszközzel telepíthetik ezeket a frissítéseket.

### Egyéb információ

#### A Microsoft Windows rosszindulatú szoftvereket eltávolító eszköze

A Microsoft a Windows Update, Microsoft Update, Windows Server Update Services és Letöltőközpont szolgáltatásán keresztül elérhetővé tette a Microsoft Windows rosszindulatú szoftvereket eltávolító eszközének frissített változatát.

#### Nem biztonsági jellegű, kiemelt fontosságú frissítések a MU, WU és WSUS-szolgáltatásokban

Ebben a hónapban:

-   A Microsoft négy **nem biztonsági jellegű**, kiemelt fontosságú frissítést adott ki a Microsoft Update (MU) és a Windows Server Update Services (WSUS) szolgáltatásokon keresztül.
-   A Microsoft két, **nem biztonsági jellegű**, kiemelt fontosságú Windows-frissítést adott ki a Windows Update (WU) szolgáltatáson keresztül.

Felhívjuk figyelmét, hogy a tájékoztatás **kizárólag** a biztonsági frissítéseket összegző kiadvánnyal azonos napon kiadott, **nem biztonsági jellegű**, a Microsoft Update, Windows Update, Windows Server Update Services szolgáltatásokon keresztül elérhető, kiemelt fontosságú frissítésekre vonatkozik. A más napokon kiadott, **nem biztonsági jellegű** frissítésekről tájékoztatást **nem** nyújtunk.

#### Biztonsági stratégiák és közösségek

**Frissítésekkel kapcsolatos stratégiák**

[A javítások telepítésére vonatkozó útmutatás](http://go.microsoft.com/fwlink/?linkid=21168) a Microsoft által a biztonsági frissítések telepítéséhez ajánlott legjobban bevált eljárást ismerteti.

**Egyéb biztonsági frissítések beszerzése**

Az alábbi helyekről más típusú biztonsági problémákhoz szerezhetők be frissítések.

-   A biztonsági frissítések a [Microsoft letöltőközpontban](http://go.microsoft.com/fwlink/?linkid=21129) érhetők el. legegyszerűbben a „biztonsági javítás” kifejezésre irányuló kulcsszavas kereséssel találhatja meg őket.
-   Az ügyfélrendszerek frissítései a [Microsoft Update](http://go.microsoft.com/fwlink/?linkid=40747) oldalról elérhetőek.
-   A Windows Update szolgáltatáson keresztül terjesztett havi aktuális biztonsági frissítések a letöltőközpontból a biztonsági és kritikus frissítéseket tartalmazó ISO CD-képfájlként is letölthetőek. További információt a [Microsoft Tudásbázis 913086](http://support.microsoft.com/kb/913086/hu) számú cikkében talál.

**IT Pro Security közösség**

Az [IT Pro Security Community](http://go.microsoft.com/fwlink/?linkid=21164) közösségben hasznos információt találhat a biztonság javításáról és az informatikai infrastruktúrák optimalizálásáról, továbbá eszmecserét folytathat a biztonsági kérdésekről más informatikai szakemberekkel.

#### Köszönetnyilvánítás

A Microsoft [köszönetét](http://go.microsoft.com/fwlink/?linkid=21127) fejezi ki a vásárlók védelmének biztosításában nyújtott segítségért az alábbi szervezet(ek)nek és szakember(ek)nek:

-   A [VeriSign iDefense VCP](http://idefense.com/) anonim kutatója, az [MS07-042](http://go.microsoft.com/fwlink/?linkid=88350) közleményben ismertetett probléma jelentéséért.
-   A [Zero Day Initiative](http://www.zerodayinitiative.com/) céggel együttműködő anonim kutató, az [MS07-042](http://go.microsoft.com/fwlink/?linkid=88350) közleményben leírt probléma jelentéséért.
-   A [VeriSign iDefense VCP](http://idefense.com/) anonim kutatója, az [MS07-043](http://go.microsoft.com/fwlink/?linkid=70249) közleményben ismertetett probléma jelentéséért.
-   A [Zero Day Initiative](http://www.zerodayinitiative.com/) céggel együttműködő anonim kutató, az [MS07-043](http://go.microsoft.com/fwlink/?linkid=70249) közleményben leírt probléma jelentéséért.
-   Dyon Balding, [Secunia](http://secunia.com/), az [MS07-044](http://go.microsoft.com/fwlink/?linkid=96778) közleményben leírt probléma jelentéséért.
-   Az [NSFOCUS Security Team](http://www.nsfocus.com/) az [MS07-045](http://go.microsoft.com/fwlink/?linkid=91712) közleményben leírt probléma jelentéséért.
-   Brett Moore [(Security-Assessment.com)](http://www.security-assessment.com/) - az [MS07-045](http://go.microsoft.com/fwlink/?linkid=91712) közleményben ismertetett probléma jelentéséért.
-   Az [eEye Digital Security](http://www.eeye.com/), az [MS05-046](http://go.microsoft.com/fwlink/?linkid=94466) közleményben ismertetett probléma jelentéséért.
-   Piotr Bania, a [TippingPoint](http://www.tippingpoint.com/) és a [Zero Day Initiative](http://www.zerodayintiative.com/) munkatársa, az [MS07-047](http://go.microsoft.com/fwlink/?linkid=88628) közleményben leírt probléma jelentéséért.
-   Aviv Raff, [Finjan](http://www.finjan.com/), az [MS07-048](http://go.microsoft.com/fwlink/?linkid=94465) közleményben ismertetett probléma jelentéséért.
-   Aviv Raff, az [iDefense Labs](http://labs.idefense.com/) munkatársa, az [MS07-048](http://go.microsoft.com/fwlink/?linkid=94465) közleményben bemutatott probléma jelentéséért.
-   Rafal Wojtczuk, [McAfee Avert Labs](http://www.avertlabs.com/), az [MS07-049](http://go.microsoft.com/fwlink/?linkid=92734) közleményben ismertetett probléma jelentéséért.
-   Az [eEye Digital Security](http://www.eeye.com/), az [MS05-050](http://go.microsoft.com/fwlink/?linkid=94737) közleményben ismertetett probléma jelentéséért.

#### Terméktámogatás

-   Teszteléssel állapították meg a felsorolt szoftverek egyes verzióinak érintettségét. A többi verzió támogatási életciklusa végére ért. Az egyes szoftververziók támogatási életciklusáról a [Microsoft termékek terméktámogatási életciklusát ismertető webhelyen](http://go.microsoft.com/fwlink/?linkid=21742) talál felvilágosítást.
-   Az Amerikai Egyesült Államokban és Kanadában technikai segítség igényelhető a [Microsoft terméktámogatási szolgáltatásától](http://go.microsoft.com/fwlink/?linkid=21131), amelynek telefonszáma 1-866-PCSAFETY. A biztonsági frissítésekkel kapcsolatos hívások ingyenesek.
-   Más országokban a helyi Microsoft-képviseletek nyújtanak támogatást. A biztonsági frissítésekkel kapcsolatos hívások ingyenesek. A [nemzetközi támogatási webhely](http://go.microsoft.com/fwlink/?linkid=21155) felvilágosítást nyújt arról, támogatási kérdéseivel hogyan fordulhat a Microsofthoz.

#### Felelősséget kizáró nyilatkozat

A Microsoft Tudásbázisban leírtak előzetes bejelentés nélkül változhatnak, és a cikkek tartalmáért a Microsoft nem vállal garanciát. A Microsoft egyben elhárít minden kifejezett és értelemszerű garanciát, beleértve az eladhatóságra és az adott célra való alkalmasságra vonatkozó garanciát is. A Microsoft Corporation vagy annak szállítói semmilyen körülmények között nem tehetők felelőssé közvetlen, közvetett, eseti, ok-okozati vagy különleges kárért (beleértve az elmaradt hasznot is), még akkor sem, ha a Microsoft Corporation vagy szállítói tudatában voltak a kár lehetséges voltának. Egyes államok törvényi szabályozása nem teszi lehetővé a véletlen vagy ok-okozati károkért vállalt felelősség korlátozását vagy kizárását, így ezekben az államokban az ez a felelősségkizárás nincs érvényben.

#### Verziók

-   1.0 verzió (2007. augusztus 14.): Összefoglaló közlemény közzététele.
-   1.1 verzió (2007. augusztus 29.): Az Érintett szoftverek táblázat frissült, az MS07-044 közleményben ismertetett probléma által érintett Office-szoftverek a következőképpen módosultak: Office 2000, Office XP és Office 2003 helyett Excel 2000, Excel 2002 és Excel 2003.
-   2.0 verzió (2007. november 13.): Az Érintett szoftverek táblázat az MS07-049 számú biztonsági közlemény frissített hivatkozásaival frissült. A Microsoft Virtual PC 2004, Microsoft Virtual PC 2004 Service Pack 1, Microsoft Virtual Server 2005 Standard Edition, Microsoft Virtual Server 2005 Enterprise Edition, Microsoft Virtual Server 2005 R2 Standard Edition, Microsoft Virtual Server 2005 R2 Enterprise Edition rendszerekhez telepíthető biztonsági frissítés új verziója immár rendelkezésre áll.
-   3.0 verzió (2008. január 9.): Az érintett szoftvereket részletező táblázat a Microsoft Word Viewer 2003 alkalmazással bővült az MS07-042 közlemény vonatkozásában. A Microsoft Office 2003 Service Pack 2 frissítése a Microsoft Word Viewer 2003 alkalmazásra is vonatkozik.
-   4.0 verzió (2008. június 24.): Az érintett szoftverek táblázata a Windows XP Service Pack 3, Windows Vista Service Pack 1, Windows Vista x64 Edition Service Pack 1, Windows Server 2008 32 bites rendszerekhez, Windows Server 2008 x64 alapú rendszerekhez, és Windows Server 2008 Itanium-alapú rendszerekhez kiegészítésével bővült a Microsoft XML Core Services 4.0 alkalmazás KB936181 frissítésére vonatkozó MS07-042 közleményben. Ez csak észlelési módosítás. A bináris fájlok nem változtak.

*Built at 2014-04-18T01:50:00Z-07:00*
