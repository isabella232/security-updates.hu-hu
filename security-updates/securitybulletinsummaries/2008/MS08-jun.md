---
TOCTitle: 'MS08-JUN'
Title: 'Microsoft biztonsági közlemény - összefoglalás, június 2008'
ms:assetid: 'ms08-jun'
ms:contentKeyID: 61227722
ms:mtpsurl: 'https://technet.microsoft.com/hu-HU/library/ms08-jun(v=Security.10)'
author: SharonSears
ms.author: SharonSears
---

Security Bulletin Summary

Microsoft biztonsági közlemény - összefoglalás, június 2008
===========================================================

Közzétéve: 2008. június 10. | Frissítve: 2009. április 1.

**Verzió:** 2.1

Az összefoglaló a 2008 júniusára kiadott biztonsági közleményeket összegzi.

A 2008. júniusi közlemények kiadása folytán az összefoglaló a június 5-én kiadott előzetes értesítés helyébe lép. További információk a biztonsági közlemények kiadásáról szóló előzetes értesítés szolgáltatásról lásd: [Előzetes értesítés a Microsoft biztonsági közleményeinek kiadásáról](http://technet.microsoft.com/security/bulletin/advance).

Ha automatikus értesítést szeretne kapni a Microsoft biztonsági közleményeinek megjelenéséről, fizessen elő a [Microsoft Technical Security Notifications](http://go.microsoft.com/fwlink/?linkid=21163) szolgáltatásra.

A közleményekkel kapcsolatos kérdések megválaszolására a Microsoft 2008. június 11-én, csendes-óceáni idő szerint (Egyesült Államok és Kanada) 11 órakor webes szemináriumot tart. [Jelentkezzen most a júniusi közleményeket bemutató webes szemináriumra](http://msevents.microsoft.com/cui/webcasteventdetails.aspx?eventid=1032357225&eventcategory=4&culture=en-us&countrycode=us). Ezt követően a webes szeminárium igény szerint kerül megrendezésre. További információkért látogasson el a [Microsoft biztonsági közleményeit és a webes szemináriumokat](http://technet.microsoft.com/security/bulletin/summary)bemutató oldalra.

A Microsoft abban is segítséget nyújt felhasználóinak, hogy a havi biztonsági közleményekkel azonos napon kiadott, nem biztonsági jellegű, de fontos frissítéseket megfelelően rangsorolhassák. Lásd az **Egyéb információ című részt**.

### A közleménnyel kapcsolatos információk

#### Összefoglalások

Az e havi biztonsági közlemények súlyossági sorrendben:

Kritikus (3)
------------

<span></span>

| Közlemény azonosítója                          | A Microsoft MS08-030 számú biztonsági közleménye                                                                                                                                                                                                                                                                                                                                                                                                                 |
|------------------------------------------------|------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| **Közlemény címe**                             | [**A Bluetooth verem biztonsági rése (951376) távolról történő programkódfuttatást tehet lehetővé**](http://go.microsoft.com/fwlink/?linkid=119619)                                                                                                                                                                                                                                                                                                              |
| **Összefoglalás**                              | A biztonsági frissítés a Bluetooth verem Windows rendszerben tapasztalt, távolról történő programkódfuttatást okozó, közvetlenül jelentett biztonsági résére nyújt megoldást. Ha egy támadó kihasználja a biztonsági rést, teljes mértékben átveheti a rendszer irányítását. Ezt követően a támadó programokat telepíthet, illetve adatokat tekinthet meg, módosíthat és törölhet, de korlátozás nélküli jogosultságokkal rendelkező új fiókokat is létrehozhat. |
| **Súlyosság maximális foka**                   | [Kritikus](http://go.microsoft.com/fwlink/?linkid=21140)                                                                                                                                                                                                                                                                                                                                                                                                         |
| **A biztonsági rés hatása**                    | Távoli kódfuttatás                                                                                                                                                                                                                                                                                                                                                                                                                                               |
| **A szoftver észlelésével kapcsolatos adatok** | A Microsoft Baseline Security Analyzer képes észlelni, szükséges-e a számítógépen az adott frissítést. Előfordulhat, hogy a frissítés a rendszer újraindítását igényli.                                                                                                                                                                                                                                                                                          |
| **Érintett szoftverek**                        | **Microsoft Windows.** További információt az Érintett szoftverek és letöltési helyek című rész tartalmaz.                                                                                                                                                                                                                                                                                                                                                       |

| Közlemény azonosítója                          | A Microsoft MS08-031 számú biztonsági közleménye                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                         |
|------------------------------------------------|----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| **Közlemény címe**                             | [**Összesítő biztonsági frissítés az Internet Explorer programhoz (950759)**](http://go.microsoft.com/fwlink/?linkid=116367)                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                             |
| **Összefoglalás**                              | A biztonsági frissítés egy közvetlenül jelentett és egy nyilvánosan jelentett biztonsági rést szüntet meg. A közvetlenül jelentett biztonsági rés távoli kódvégrehajtást tehet lehetővé, amennyiben a felhasználó egy különlegesen kialakított weboldalt tekint meg az Internet Explorer alkalmazás segítségével. A kevesebb jogosultsággal bíró fiókkal rendelkező felhasználók esetében kisebb a veszélyeztetettség, mint a rendszergazdai jogosultságokkal rendelkezők esetén A nyilvánosan jelentett biztonsági rés adatokhoz való illetéktelen hozzáférést tehet lehetővé, amennyiben a felhasználó egy különlegesen kialakított weboldalt tekint meg az Internet Explorer alkalmazás segítségével. |
| **Súlyosság maximális foka**                   | [Kritikus](http://go.microsoft.com/fwlink/?linkid=21140)                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                 |
| **A biztonsági rés hatása**                    | Távoli kódfuttatás                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                       |
| **A szoftver észlelésével kapcsolatos adatok** | A Microsoft Baseline Security Analyzer képes észlelni, szükséges-e a számítógépen az adott frissítést. Ez a frissítés újraindítást igényel.                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                              |
| **Érintett szoftverek**                        | **Microsoft Windows, Internet Explorer.** További információt az Érintett szoftverek és letöltési helyek című rész tartalmaz.                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                            |

| Közlemény azonosítója                          | A Microsoft MS08-033 számú biztonsági közleménye                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                  |
|------------------------------------------------|---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| **Közlemény címe**                             | [**A DirectX távolról történő programkódfuttatást lehetővé tévő biztonsági rései (951698)**](http://go.microsoft.com/fwlink/?linkid=118655)                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                       |
| **Összefoglalás**                              | A biztonsági frissítés a Microsoft DirectX két, közvetlenül a Microsoftnak jelzett biztonsági rését szünteti meg, amely távoli kódfuttatást tesz lehetővé, amennyiben a felhasználó megnyit egy speciálisan létrehozott médiafájlt. A biztonsági rések valamelyikét kiaknázó támadó teljes mértékben átveheti az érintett rendszer vezérlését. Ezt követően a támadó programokat telepíthet, illetve adatokat tekinthet meg, módosíthat és törölhet, de korlátozás nélküli jogosultságokkal rendelkező új fiókokat is létrehozhat. A kevesebb jogosultsággal bíró fiókkal rendelkező felhasználók esetében kisebb a veszélyeztetettség, mint a rendszergazdai jogosultságokkal rendelkezők esetén |
| **Súlyosság maximális foka**                   | [Kritikus](http://go.microsoft.com/fwlink/?linkid=21140)                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                          |
| **A biztonsági rés hatása**                    | Távoli kódfuttatás                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                |
| **A szoftver észlelésével kapcsolatos adatok** | A Microsoft Baseline Security Analyzer képes észlelni, szükséges-e a számítógépen az adott frissítést. Előfordulhat, hogy a frissítés a rendszer újraindítását igényli.                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                           |
| **Érintett szoftverek**                        | **Microsoft Windows.** További információt az Érintett szoftverek és letöltési helyek című rész tartalmaz.                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                        |

Fontos (3)
----------

<span></span>

| Közlemény azonosítója                          | A Microsoft MS08-034 számú biztonsági közleménye                                                                                                                                                                                                                                                                                                                                                         |
|------------------------------------------------|----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| **Közlemény címe**                             | [**A WINS jogok kiterjesztését okozó biztonsági rése (948745)**](http://go.microsoft.com/fwlink/?linkid=111957)                                                                                                                                                                                                                                                                                          |
| **Összefoglalás**                              | A biztonsági frissítés egy közvetlenül jelentett biztonsági résre kínál megoldást, mely a Windows Internet Name Service (WINS) keretében jogok kiterjesztését teszi lehetővé. Ha egy támadó kihasználja a biztonsági rést, teljes mértékben átveheti a rendszer irányítását. Ezt követően programokat telepíthet, illetve adatokat tekinthet meg, módosíthat és törölhet, de új fiókokat is létrehozhat. |
| **Súlyosság maximális foka**                   | [Fontos](http://go.microsoft.com/fwlink/?linkid=21140)                                                                                                                                                                                                                                                                                                                                                   |
| **A biztonsági rés hatása**                    | Jogok kiterjesztése                                                                                                                                                                                                                                                                                                                                                                                      |
| **A szoftver észlelésével kapcsolatos adatok** | A Microsoft Baseline Security Analyzer képes észlelni, szükséges-e a számítógépen az adott frissítést. Ez a frissítés újraindítást igényel.                                                                                                                                                                                                                                                              |
| **Érintett szoftverek**                        | **Microsoft Windows.** További információt az Érintett szoftverek és letöltési helyek című rész tartalmaz.                                                                                                                                                                                                                                                                                               |

| Közlemény azonosítója                          | A Microsoft MS08-035 számú biztonsági közleménye                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                   |
|------------------------------------------------|------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| **Közlemény címe**                             | [**Az Active Directory biztonsági rése szolgáltatásmegtagadást okozhat (953235)**](http://go.microsoft.com/fwlink/?linkid=111953)                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                  |
| **Összefoglalás**                              | Ez a biztonsági frissítés a Microsoft Windows 2000 Server, Windows Server 2003 és Windows Server 2008 rendszereken futó Active Directory, illetve a Windows XP Professional és Windows Server 2003 rendszerekre telepített alkalmazásmódú Active Directory (ADAM), továbbá a Windows Server 2008 rendszerben működő Active Directory Lightweight Directory-szolgáltatás (AD LDS) közvetlenül jelentett biztonsági rését szünteti meg, amely lehetővé teszi, hogy az ezt kihasználó támadó szolgáltatásmegtagadást okozzon. Windows XP Professional, Windows Server 2003 és Windows Server 2008 rendszerek esetében a támadó csak érvényes bejelentkezési adatok birtokában használhatja ki ezt a biztonsági rést. A biztonsági rést sikeresen kihasználó támadó a rendszer lefagyását vagy automatikus újraindulását idézheti elő. |
| **Súlyosság maximális foka**                   | [Fontos](http://go.microsoft.com/fwlink/?linkid=21140)                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                             |
| **A biztonsági rés hatása**                    | Szolgáltatásmegtagadás                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                             |
| **A szoftver észlelésével kapcsolatos adatok** | A Microsoft Baseline Security Analyzer képes észlelni, szükséges-e a számítógépen az adott frissítést. Ez a frissítés újraindítást igényel.                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                        |
| **Érintett szoftverek**                        | **Microsoft Windows.** További információt az Érintett szoftverek és letöltési helyek című rész tartalmaz.                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                         |

| Közlemény azonosítója                          | A Microsoft MS08-036 számú biztonsági közleménye                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                |
|------------------------------------------------|-------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| **Közlemény címe**                             | [**Az általános csoportos küldés (PGM) biztonsági rése szolgáltatásmegtagadást tesz lehetővé (950762)**](http://go.microsoft.com/fwlink/?linkid=117297)                                                                                                                                                                                                                                                                                                                                                                                                                                                                                         |
| **Összefoglalás**                              | Ez a biztonsági frissítés az általános csoportos küldés (PGM) két közvetlenül jelzett biztonsági rését szünteti meg, amely szolgáltatásmegtagadáshoz vezethet, ha valamely érintett rendszer hibás PGM-csomagokat kap. A biztonsági rést sikeresen kihasználó támadó a felhasználó rendszerének lefagyását idézheti elő, és a működés helyreállításához a rendszert újra kell indítani. Fontos megjegyezni, hogy a szolgáltatásmegtagadást okozó biztonsági rések a támadó számára nem teszik lehetővé programkód futtatását vagy jogosultságok illetéktelen megszerzését, de segítségükkel megakadályozható a rendszerben a kérelmek fogadása. |
| **Súlyosság maximális foka**                   | [Fontos](http://go.microsoft.com/fwlink/?linkid=21140)                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                          |
| **A biztonsági rés hatása**                    | Szolgáltatásmegtagadás                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                          |
| **A szoftver észlelésével kapcsolatos adatok** | A Microsoft Baseline Security Analyzer képes észlelni, szükséges-e a számítógépen az adott frissítést. Ez a frissítés újraindítást igényel.                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                     |
| **Érintett szoftverek**                        | **Microsoft Windows.** További információt az Érintett szoftverek és letöltési helyek című rész tartalmaz.                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                      |

Mérsékelt (1)
-------------

<span></span>

| Közlemény azonosítója                          | A Microsoft MS08-032 számú biztonsági közleménye                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                |
|------------------------------------------------|-----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| **Közlemény címe**                             | [**Összesítő biztonsági frissítés az ActiveX-tiltóbitekhez (950760)**](http://go.microsoft.com/fwlink/?linkid=116368)                                                                                                                                                                                                                                                                                                                                                                                                                                           |
| **Összefoglalás**                              | A frissítés a Microsoft Speech API egy nyilvánosan jelentett biztonsági rését szüntet meg. A biztonsági rés távoli kódvégrehajtást tehet lehetővé, amennyiben a felhasználó egy különlegesen kialakított weboldalt tekint meg az Internet Explorer alkalmazással úgy, hogy a Windows Beszédfelismerés szolgáltatása engedélyezve van. A kevesebb jogosultsággal bíró fiókkal rendelkező felhasználók esetében kisebb a veszélyeztetettség, mint a rendszergazdai jogosultságokkal rendelkezők esetén A frissítés a BackWeb szoftver tiltóbitjét is tartalmazza. |
| **Súlyosság maximális foka**                   | [Mérsékelt.](http://go.microsoft.com/fwlink/?linkid=21140)                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                      |
| **A biztonsági rés hatása**                    | Távoli kódfuttatás                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                              |
| **A szoftver észlelésével kapcsolatos adatok** | A Microsoft Baseline Security Analyzer képes észlelni, szükséges-e a számítógépen az adott frissítést. Előfordulhat, hogy a frissítés a rendszer újraindítását igényli.                                                                                                                                                                                                                                                                                                                                                                                         |
| **Érintett szoftverek**                        | **Microsoft Windows.** További információt az Érintett szoftverek és letöltési helyek című rész tartalmaz.                                                                                                                                                                                                                                                                                                                                                                                                                                                      |

Érintett szoftverek és letöltési helyek
---------------------------------------

<span></span>
**A táblázat használata**

A táblázat segítségével megtudhatja a szükséges információt a telepítendő biztonsági frissítésekről. Nézzen meg minden felsorolt szoftvert vagy összetevőt annak megállapításához, hogy van-e telepítendő biztonsági frissítés. Ha a szoftver vagy összetevő szerepel a listán, hiperhivatkozással kapcsolódik hozzá az elérhető szoftverfrissítés, és a frissítés besorolása is fel van tüntetve.

**Megjegyzés:** Előfordulhat, hogy egy biztonsági rés megszüntetéséhez több biztonsági frissítést kell telepíteni. Nézze át az egyes közleményazonosítókhoz tartozó teljes oszlopot, és ellenőrizze a telepítendő frissítéseket a rendszerre telepített programok vagy összetevők alapján.

#### A Windows operációs rendszer és kiszolgáló

 
<p> </p>
<table style="border:1px solid black;">
<caption>Microsoft Windows 2000</caption>
<tbody>
<tr class="odd">
<td style="border:1px solid black;"><strong>Közlemény azonosítója</strong></td>
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=119619"><strong>MS08-030</strong></a></td>
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=116367"><strong>MS08-031</strong></a></td>
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=118655"><strong>MS08-033</strong></a></td>
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=111957"><strong>MS08-034</strong></a></td>
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=111953"><strong>MS08-035</strong></a></td>
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=117297"><strong>MS08-036</strong></a></td>
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=116368"><strong>MS08-032</strong></a></td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><strong>Közlemény legmagasabb súlyossági besorolása</strong></td>
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=21140"><strong>Kritikus</strong></a></td>
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=21140"><strong>Kritikus</strong></a></td>
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=21140"><strong>Kritikus</strong></a></td>
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=21140"><strong>Fontos</strong></a></td>
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=21140"><strong>Fontos</strong></a></td>
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=21140"><strong>Fontos</strong></a></td>
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=21140"><strong>Mérsékelt</strong></a></td>
</tr>
<tr class="odd">
<td style="border:1px solid black;">Microsoft Windows 2000 Service Pack 4</td>
<td style="border:1px solid black;">Nem érintett</td>
<td style="border:1px solid black;"><a href="http://www.microsoft.com/downloads/details.aspx?familyid=88990b23-d37f-4d02-a5a3-2ee389ade53c">Microsoft Internet Explorer 5.01 Service Pack 4</a><br />
(Fontos)<br />
<br />
<a href="http://www.microsoft.com/downloads/details.aspx?familyid=4c47cf8a-8100-4d43-855a-f225a3492b19">Microsoft Internet Explorer 6 Service Pack 1 szervizcsomaggal</a><br />
(Kritikus)</td>
<td style="border:1px solid black;"><a href="http://www.microsoft.com/downloads/details.aspx?familyid=65640123-a9e4-455c-a51a-9df28bd2d412">DirectX 7.0</a><br />
(Kritikus)<br />
<br />
<a href="http://www.microsoft.com/downloads/details.aspx?familyid=c6a28d45-13cf-48c4-8f89-3417d552e90b">DirectX 8.1</a><br />
(Kritikus)<br />
<br />
<a href="http://www.microsoft.com/downloads/details.aspx?familyid=4dc47e04-5e95-4636-a814-3f912d961461">DirectX 9.0, DirectX 9.0a, DirectX 9.0b vagy DirectX 9.0c</a><br />
(Kritikus)</td>
<td style="border:1px solid black;">Nem érintett</td>
<td style="border:1px solid black;">Nem érintett</td>
<td style="border:1px solid black;">Nem érintett</td>
<td style="border:1px solid black;"><a href="http://www.microsoft.com/downloads/details.aspx?familyid=cedfd988-232c-4cba-ac65-beb54b8946e0">Microsoft Windows 2000 Service Pack 4</a><br />
(Mérsékelt)</td>
</tr>
<tr class="even">
<td style="border:1px solid black;">Microsoft Windows 2000 Server Service Pack 4</td>
<td style="border:1px solid black;">Nem érintett</td>
<td style="border:1px solid black;">Nem érintett</td>
<td style="border:1px solid black;">Nem érintett</td>
<td style="border:1px solid black;"><a href="http://www.microsoft.com/downloads/details.aspx?familyid=aa8aa79f-c2cc-440c-9e5c-089143e6f814">Microsoft Windows 2000 Server Service Pack 4</a><br />
(Fontos)</td>
<td style="border:1px solid black;"><a href="http://www.microsoft.com/downloads/details.aspx?familyid=53438880-9ea9-4975-9b85-2a1d3d232793">Active Directory</a><br />
(KB949014)<br />
(Fontos)</td>
<td style="border:1px solid black;">Nem érintett</td>
<td style="border:1px solid black;">Nem érintett</td>
</tr>
</tbody>
</table>

 
<p> </p>
<table style="border:1px solid black;">
<caption>Windows XP</caption>
<tbody>
<tr class="odd">
<td style="border:1px solid black;"><strong>Közlemény azonosítója</strong></td>
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=119619"><strong>MS08-030</strong></a></td>
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=116367"><strong>MS08-031</strong></a></td>
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=118655"><strong>MS08-033</strong></a></td>
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=111957"><strong>MS08-034</strong></a></td>
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=111953"><strong>MS08-035</strong></a></td>
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=117297"><strong>MS08-036</strong></a></td>
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=116368"><strong>MS08-032</strong></a></td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><strong>Közlemény legmagasabb súlyossági besorolása</strong></td>
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=21140"><strong>Kritikus</strong></a></td>
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=21140"><strong>Kritikus</strong></a></td>
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=21140"><strong>Kritikus</strong></a></td>
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=21140"><strong>Fontos</strong></a></td>
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=21140"><strong>Fontos</strong></a></td>
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=21140"><strong>Fontos</strong></a></td>
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=21140"><strong>Mérsékelt</strong></a></td>
</tr>
<tr class="odd">
<td style="border:1px solid black;">Windows XP Service Pack 2 és Windows XP Service Pack 3</td>
<td style="border:1px solid black;"><a href="http://www.microsoft.com/downloads/details.aspx?familyid=980bb421-950f-4825-8039-44cc961a47b8">Windows XP Service Pack 2 és Windows XP Service Pack 3</a><br />
(Kritikus)</td>
<td style="border:1px solid black;"><a href="http://www.microsoft.com/downloads/details.aspx?familyid=cc325017-3a48-4475-90e4-0c79a002fce3">Microsoft Internet Explorer 6</a><br />
(Kritikus)<br />
<br />
<a href="http://www.microsoft.com/downloads/details.aspx?familyid=fbc31bde-0bf5-490c-96a8-071310d9464a">Windows Internet Explorer 7</a><br />
(Kritikus)</td>
<td style="border:1px solid black;"><a href="http://www.microsoft.com/downloads/details.aspx?familyid=7aaa6427-1e22-4566-960c-836a3b9e5f36">DirectX 9.0, DirectX 9.0a, DirectX 9.0b vagy DirectX 9.0c</a><br />
(Kritikus)</td>
<td style="border:1px solid black;">Nem érintett</td>
<td style="border:1px solid black;">Nem érintett</td>
<td style="border:1px solid black;"><a href="http://www.microsoft.com/downloads/details.aspx?familyid=36b14a81-5979-4e38-9ba3-ed83dfc17adf">Windows XP Service Pack 2 és Windows XP Service Pack 3</a><br />
(Fontos)</td>
<td style="border:1px solid black;"><a href="http://www.microsoft.com/downloads/details.aspx?familyid=2d8957c2-e473-4dca-8d68-19fdaea36e26">Windows XP Service Pack 2 és Windows XP Service Pack 3</a><br />
(Mérsékelt)</td>
</tr>
<tr class="even">
<td style="border:1px solid black;">Windows XP Professional Service Pack 2 és Windows XP Professional Service Pack 3</td>
<td style="border:1px solid black;">(Lásd: Windows XP Service Pack 2 és Windows XP Service Pack 3 sora)</td>
<td style="border:1px solid black;">(Lásd: Windows XP Service Pack 2 és Windows XP Service Pack 3 sora)</td>
<td style="border:1px solid black;">(Lásd: Windows XP Service Pack 2 és Windows XP Service Pack 3 sora)</td>
<td style="border:1px solid black;">Nem érintett</td>
<td style="border:1px solid black;"><a href="http://www.microsoft.com/downloads/details.aspx?familyid=7d6aec31-cfb4-470c-983e-78c6a3ebabfe">ADAM</a><br />
(KB949269)<br />
(Mérsékelt)</td>
<td style="border:1px solid black;">(Lásd: Windows XP Service Pack 2 és Windows XP Service Pack 3 sora)</td>
<td style="border:1px solid black;">(Lásd: Windows XP Service Pack 2 és Windows XP Service Pack 3 sora)</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;">Windows XP Professional x64 Edition és Windows XP Professional x64 Edition Service Pack 2</td>
<td style="border:1px solid black;"><a href="http://www.microsoft.com/downloads/details.aspx?familyid=81ab56ca-933f-4974-a393-290a54c30a78">Windows XP Professional x64 Edition és Windows XP Professional x64 Edition Service Pack 2</a><br />
(Kritikus)</td>
<td style="border:1px solid black;"><a href="http://www.microsoft.com/downloads/details.aspx?familyid=c8783cfe-9da5-4842-ab3a-1e2be4fafc47">Microsoft Internet Explorer 6</a><br />
(Kritikus)<br />
<br />
<a href="http://www.microsoft.com/downloads/details.aspx?familyid=19c0ccdc-95c9-4151-96b6-4f49b594ebe0">Windows Internet Explorer 7</a><br />
(Kritikus)</td>
<td style="border:1px solid black;"><a href="http://www.microsoft.com/downloads/details.aspx?familyid=5e8e7e9d-828d-442c-acac-8d91e80dfb36">DirectX 9.0, DirectX 9.0a, DirectX 9.0b vagy DirectX 9.0c</a><br />
(Kritikus)</td>
<td style="border:1px solid black;">Nem érintett</td>
<td style="border:1px solid black;"><a href="http://www.microsoft.com/downloads/details.aspx?familyid=ef2e0b48-1bde-4ccc-8f40-2918c2568b2b">ADAM</a><br />
(KB949269)<br />
(Mérsékelt)</td>
<td style="border:1px solid black;"><a href="http://www.microsoft.com/downloads/details.aspx?familyid=9e9d24ee-8183-428c-8067-168a8d85eaa1">Windows XP Professional x64 Edition és Windows XP Professional x64 Edition Service Pack 2</a><br />
(Fontos)</td>
<td style="border:1px solid black;"><a href="http://www.microsoft.com/downloads/details.aspx?familyid=62874096-7d17-4116-9795-4756e2fb6dae">Windows XP Professional x64 Edition és Windows XP Professional x64 Edition Service Pack 2</a><br />
(Mérsékelt)</td>
</tr>
</tbody>
</table>
 

 
<p> </p>
<table style="border:1px solid black;">
<caption>Windows Server 2003</caption>
<tbody>
<tr class="odd">
<td style="border:1px solid black;"><strong>Közlemény azonosítója</strong></td>
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=119619"><strong>MS08-030</strong></a></td>
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=116367"><strong>MS08-031</strong></a></td>
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=118655"><strong>MS08-033</strong></a></td>
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=111957"><strong>MS08-034</strong></a></td>
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=111953"><strong>MS08-035</strong></a></td>
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=117297"><strong>MS08-036</strong></a></td>
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=116368"><strong>MS08-032</strong></a></td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><strong>Közlemény legmagasabb súlyossági besorolása</strong></td>
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=21140"><strong>Kritikus</strong></a></td>
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=21140"><strong>Kritikus</strong></a></td>
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=21140"><strong>Kritikus</strong></a></td>
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=21140"><strong>Fontos</strong></a></td>
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=21140"><strong>Fontos</strong></a></td>
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=21140"><strong>Fontos</strong></a></td>
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=21140"><strong>Mérsékelt</strong></a></td>
</tr>
<tr class="odd">
<td style="border:1px solid black;">Windows Server 2003 Service Pack 1 és Windows Server 2003 Service Pack 2 rendszerhez</td>
<td style="border:1px solid black;">Nem érintett</td>
<td style="border:1px solid black;"><a href="http://www.microsoft.com/downloads/details.aspx?familyid=286aada6-a358-41f1-b81a-8de39b9f908a">Microsoft Internet Explorer 6</a><br />
(Mérsékelt)<br />
<br />
<a href="http://www.microsoft.com/downloads/details.aspx?familyid=a1ae9ad2-8329-4c96-b950-7534b3287eaa">Windows Internet Explorer 7</a><br />
(Mérsékelt)</td>
<td style="border:1px solid black;"><a href="http://www.microsoft.com/downloads/details.aspx?familyid=2274ecb2-2802-47e2-84fd-6621fcb17758">DirectX 9.0, DirectX 9.0a, DirectX 9.0b vagy DirectX 9.0c</a><br />
(Kritikus)</td>
<td style="border:1px solid black;"><a href="http://www.microsoft.com/downloads/details.aspx?familyid=08fc90d5-23aa-4327-8aef-16bc5170769d">Windows Server 2003 Service Pack 1 és Windows Server 2003 Service Pack 2</a><br />
(Fontos)</td>
<td style="border:1px solid black;"><a href="http://www.microsoft.com/downloads/details.aspx?familyid=a4aed117-3c76-4d80-b50e-8e07e2ef2f7d">Active Directory</a><br />
(KB949014)<br />
(Mérsékelt)<br />
<br />
<a href="http://www.microsoft.com/downloads/details.aspx?familyid=0a983ffb-4f5a-4b78-9bf5-813dcc5df8d3">ADAM</a><br />
(KB949269)<br />
(Mérsékelt)</td>
<td style="border:1px solid black;"><a href="http://www.microsoft.com/downloads/details.aspx?familyid=1e8e2faf-009f-403b-a5fe-a47cf014db3a">Windows Server 2003 Service Pack 1 és Windows Server 2003 Service Pack 2</a><br />
(Fontos)</td>
<td style="border:1px solid black;"><a href="http://www.microsoft.com/downloads/details.aspx?familyid=dadead99-09cb-4f2b-850d-e98a627cb9f8">Windows Server 2003 Service Pack 1 és Windows Server 2003 Service Pack 2</a><br />
(Alacsony)</td>
</tr>
<tr class="even">
<td style="border:1px solid black;">Windows Server 2003 x64 Edition és Windows Server 2003 x64 Edition Service Pack 2 rendszerhez</td>
<td style="border:1px solid black;">Nem érintett</td>
<td style="border:1px solid black;"><a href="http://www.microsoft.com/downloads/details.aspx?familyid=6604569a-3db0-47e7-bd30-7dfba8145386">Microsoft Internet Explorer 6</a><br />
(Mérsékelt)<br />
<br />
<a href="http://www.microsoft.com/downloads/details.aspx?familyid=fb0c70b4-ce9f-43d6-875a-3cfd0d3a2681">Windows Internet Explorer 7</a><br />
(Mérsékelt)</td>
<td style="border:1px solid black;"><a href="http://www.microsoft.com/downloads/details.aspx?familyid=5ba63bb7-ed6d-4c59-88b3-456eda07e190">DirectX 9.0, DirectX 9.0a, DirectX 9.0b vagy DirectX 9.0c</a><br />
(Kritikus)</td>
<td style="border:1px solid black;"><a href="http://www.microsoft.com/downloads/details.aspx?familyid=71675ae8-d60a-4834-b358-2d8e761e62fc">Windows Server 2003 x64 Edition és Windows Server 2003 x64 Edition Service Pack 2</a><br />
(Fontos)</td>
<td style="border:1px solid black;"><a href="http://www.microsoft.com/downloads/details.aspx?familyid=8298a6e4-d3e2-48ea-ac29-aa4dc5a8ec77">Active Directory</a><br />
(KB949014)<br />
(Mérsékelt)<br />
<br />
<a href="http://www.microsoft.com/downloads/details.aspx?familyid=334252db-4a7a-4161-bb71-2a20c0b5bd93">ADAM</a><br />
(KB949269)<br />
(Mérsékelt)</td>
<td style="border:1px solid black;"><a href="http://www.microsoft.com/downloads/details.aspx?familyid=78bf92d8-63c4-4596-8425-8fcfea7f5582">Windows Server 2003 x64 Edition és Windows Server 2003 x64 Edition Service Pack 2</a><br />
(Fontos)</td>
<td style="border:1px solid black;"><a href="http://www.microsoft.com/downloads/details.aspx?familyid=84f9b533-b0cb-46d1-b4a8-5c9469abbd22">Windows Server 2003 x64 Edition és Windows Server 2003 x64 Edition Service Pack 2</a><br />
(Alacsony)</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;">Windows Server 2003 SP1 Itanium alapú rendszerekhez és Windows Server 2003 SP2 Itanium alapú rendszerekhez</td>
<td style="border:1px solid black;">Nem érintett</td>
<td style="border:1px solid black;"><a href="http://www.microsoft.com/downloads/details.aspx?familyid=0262beb8-1eb5-4c2d-a50a-0c6c6e0c1f61">Microsoft Internet Explorer 6</a><br />
(Mérsékelt)<br />
<br />
<a href="http://www.microsoft.com/downloads/details.aspx?familyid=28d2913c-1c6b-4671-9892-de08698cd5a6">Windows Internet Explorer 7</a><br />
(Mérsékelt)</td>
<td style="border:1px solid black;"><a href="http://www.microsoft.com/downloads/details.aspx?familyid=be71c002-2f64-49e9-9f4b-ba99c4f3caf6">DirectX 9.0, DirectX 9.0a, DirectX 9.0b vagy DirectX 9.0c</a><br />
(Kritikus)</td>
<td style="border:1px solid black;"><a href="http://www.microsoft.com/downloads/details.aspx?familyid=87affdc9-d9fe-413c-af30-f3d3b671ec72">Windows Server 2003 SP1 Itanium alapú rendszerekhez és Windows Server 2003 SP2 Itanium alapú rendszerekhez</a><br />
(Fontos)</td>
<td style="border:1px solid black;"><a href="http://www.microsoft.com/downloads/details.aspx?familyid=f6bf4b85-b91d-4378-a356-cd11f12cbbfd">Active Directory</a><br />
(KB949014)<br />
(Mérsékelt)</td>
<td style="border:1px solid black;"><a href="http://www.microsoft.com/downloads/details.aspx?familyid=5b7e94fa-22ed-4f7c-b452-647b2e620113">Windows Server 2003 SP1 Itanium alapú rendszerekhez és Windows Server 2003 SP2 Itanium alapú rendszerekhez</a><br />
(Fontos)</td>
<td style="border:1px solid black;"><a href="http://www.microsoft.com/downloads/details.aspx?familyid=ac35ce19-d761-4529-9f55-1e1b5b2447ad">Windows Server 2003 SP1 Itanium alapú rendszerekhez és Windows Server 2003 SP2 Itanium alapú rendszerekhez</a><br />
(Alacsony)</td>
</tr>
</tbody>
</table>
 

 
<p> </p>
<table style="border:1px solid black;">
<caption>Windows Vista</caption>
<tbody>
<tr class="odd">
<td style="border:1px solid black;"><strong>Közlemény azonosítója</strong></td>
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=119619"><strong>MS08-030</strong></a></td>
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=116367"><strong>MS08-031</strong></a></td>
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=118655"><strong>MS08-033</strong></a></td>
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=111957"><strong>MS08-034</strong></a></td>
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=111953"><strong>MS08-035</strong></a></td>
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=117297"><strong>MS08-036</strong></a></td>
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=116368"><strong>MS08-032</strong></a></td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><strong>Közlemény legmagasabb súlyossági besorolása</strong></td>
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=21140"><strong>Kritikus</strong></a></td>
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=21140"><strong>Kritikus</strong></a></td>
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=21140"><strong>Kritikus</strong></a></td>
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=21140"><strong>Fontos</strong></a></td>
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=21140"><strong>Fontos</strong></a></td>
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=21140"><strong>Fontos</strong></a></td>
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=21140"><strong>Mérsékelt</strong></a></td>
</tr>
<tr class="odd">
<td style="border:1px solid black;">Windows Vista és Windows Vista Service Pack 1</td>
<td style="border:1px solid black;"><a href="http://www.microsoft.com/downloads/details.aspx?familyid=6524debe-be50-44d1-8543-af0bfaf086ad">Windows Vista és Windows Vista Service Pack 1</a><br />
(Kritikus)</td>
<td style="border:1px solid black;"><a href="http://www.microsoft.com/downloads/details.aspx?familyid=6d68b39d-157f-4c3d-ac76-bc5a9386db59">Windows Internet Explorer 7</a><br />
(Kritikus)</td>
<td style="border:1px solid black;"><a href="http://www.microsoft.com/downloads/details.aspx?familyid=4d4b305b-57f8-448d-92fa-3dcdd1f42ed7">DirectX 10.0</a><br />
(Kritikus)</td>
<td style="border:1px solid black;">Nem érintett</td>
<td style="border:1px solid black;">Nem érintett</td>
<td style="border:1px solid black;"><a href="http://www.microsoft.com/downloads/details.aspx?familyid=ef2d2a4b-4831-41be-b5d0-8df5b01fd205">Windows Vista és Windows Vista Service Pack 1</a><br />
(Mérsékelt)</td>
<td style="border:1px solid black;"><a href="http://www.microsoft.com/downloads/details.aspx?familyid=4af6575e-b061-45a6-b3d8-ecb32d76b2d3">Windows Vista és Windows Vista Service Pack 1</a><br />
(Mérsékelt)</td>
</tr>
<tr class="even">
<td style="border:1px solid black;">Windows Vista x64 Edition és Windows Vista x64 Edition Service Pack 1</td>
<td style="border:1px solid black;"><a href="http://www.microsoft.com/downloads/details.aspx?familyid=6adee8b9-3455-4f3b-8bdd-2585c8ff83b8">Windows Vista x64 Edition és Windows Vista x64 Edition Service Pack 1</a><br />
(Kritikus)</td>
<td style="border:1px solid black;"><a href="http://www.microsoft.com/downloads/details.aspx?familyid=4cf92235-861e-4b74-bee3-8e977c8688d9">Windows Internet Explorer 7</a><br />
(Kritikus)</td>
<td style="border:1px solid black;"><a href="http://www.microsoft.com/downloads/details.aspx?familyid=b040cfad-2290-44f4-8f5a-5d1ed98a7265">DirectX 10.0</a><br />
(Kritikus)</td>
<td style="border:1px solid black;">Nem érintett</td>
<td style="border:1px solid black;">Nem érintett</td>
<td style="border:1px solid black;"><a href="http://www.microsoft.com/downloads/details.aspx?familyid=0839fcf4-85ca-445e-896b-f634b10b6700">Windows Vista x64 Edition és Windows Vista x64 Edition Service Pack 1</a><br />
(Mérsékelt)</td>
<td style="border:1px solid black;"><a href="http://www.microsoft.com/downloads/details.aspx?familyid=67576acb-9cb6-4c76-9a72-dc5e5556b658">Windows Vista x64 Edition és Windows Vista x64 Edition Service Pack 1</a><br />
(Mérsékelt)</td>
</tr>
</tbody>
</table>
 

 
<p> </p>
<table style="border:1px solid black;">
<caption>Windows Server 2008</caption>
<tbody>
<tr class="odd">
<td style="border:1px solid black;"><strong>Közlemény azonosítója</strong></td>
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=119619"><strong>MS08-030</strong></a></td>
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=116367"><strong>MS08-031</strong></a></td>
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=118655"><strong>MS08-033</strong></a></td>
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=111957"><strong>MS08-034</strong></a></td>
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=111953"><strong>MS08-035</strong></a></td>
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=117297"><strong>MS08-036</strong></a></td>
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=116368"><strong>MS08-032</strong></a></td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><strong>Közlemény legmagasabb súlyossági besorolása</strong></td>
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=21140"><strong>Kritikus</strong></a></td>
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=21140"><strong>Kritikus</strong></a></td>
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=21140"><strong>Kritikus</strong></a></td>
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=21140"><strong>Fontos</strong></a></td>
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=21140"><strong>Fontos</strong></a></td>
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=21140"><strong>Fontos</strong></a></td>
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=21140"><strong>Mérsékelt</strong></a></td>
</tr>
<tr class="odd">
<td style="border:1px solid black;">Windows Server 2008 32 bites rendszerekhez</td>
<td style="border:1px solid black;">Nem érintett</td>
<td style="border:1px solid black;"><a href="http://www.microsoft.com/downloads/details.aspx?familyid=a8922e7e-9264-4e09-b8ad-c5420fed8690">Windows Internet Explorer 7</a><br />
(Mérsékelt)<strong>**</strong></td>
<td style="border:1px solid black;"><a href="http://www.microsoft.com/downloads/details.aspx?familyid=c0c495f8-2a35-4638-a635-1e55dd15e062">DirectX 10.0</a><br />
(kritikus)<strong>**</strong></td>
<td style="border:1px solid black;">Nem érintett</td>
<td style="border:1px solid black;"><a href="http://www.microsoft.com/downloads/details.aspx?familyid=2981156e-2e2f-469e-91be-da127d50f3fc">Active Directory</a><br />
(KB949014)<br />
(mérsékelt)<strong>*</strong><br />
<br />
<a href="http://www.microsoft.com/downloads/details.aspx?familyid=2981156e-2e2f-469e-91be-da127d50f3fc">AD LDS</a><br />
(KB949014)<br />
(mérsékelt)<strong>*</strong></td>
<td style="border:1px solid black;"><a href="http://www.microsoft.com/downloads/details.aspx?familyid=0466a6e7-fdca-4647-af62-449e5f20d1e4">Windows Server 2008 32 bites rendszerekhez</a><br />
(Mérsékelt)<strong>**</strong></td>
<td style="border:1px solid black;"><a href="http://www.microsoft.com/downloads/details.aspx?familyid=8a507fba-8c93-4952-91e4-98e9e7affbd2">Windows Server 2008 32 bites rendszerekhez</a><br />
(Alacsony)<strong>***</strong></td>
</tr>
<tr class="even">
<td style="border:1px solid black;">Windows Server 2008 x64 alapú rendszerekhez</td>
<td style="border:1px solid black;">Nem érintett</td>
<td style="border:1px solid black;"><a href="http://www.microsoft.com/downloads/details.aspx?familyid=05b0e838-24d7-4387-b069-2604bbcc43b9">Windows Internet Explorer 7</a><br />
(Mérsékelt)<strong>**</strong></td>
<td style="border:1px solid black;"><a href="http://www.microsoft.com/downloads/details.aspx?familyid=0b70fc2e-4e80-4ae8-8682-41ea04c24e4e">DirectX 10.0</a><br />
(kritikus)<strong>**</strong></td>
<td style="border:1px solid black;">Nem érintett</td>
<td style="border:1px solid black;"><a href="http://www.microsoft.com/downloads/details.aspx?familyid=b5cfe6f4-c5ba-4be9-a6b8-9381c40c85aa">Active Directory</a><br />
(KB949014)<br />
(mérsékelt)<strong>*</strong><br />
<br />
<a href="http://www.microsoft.com/downloads/details.aspx?familyid=b5cfe6f4-c5ba-4be9-a6b8-9381c40c85aa">AD LDS</a><br />
(KB949014)<br />
(mérsékelt)<strong>*</strong></td>
<td style="border:1px solid black;"><a href="http://www.microsoft.com/downloads/details.aspx?familyid=304898e6-21a7-476f-b9ed-7ac0d88a91e2">Windows Server 2008 x64 alapú rendszerekhez</a><br />
(Mérsékelt)<strong>**</strong></td>
<td style="border:1px solid black;"><a href="http://www.microsoft.com/downloads/details.aspx?familyid=1a11499d-a008-407f-9084-a5189fa27015">Windows Server 2008 x64 alapú rendszerekhez</a><br />
(Alacsony)<strong>***</strong></td>
</tr>
<tr class="odd">
<td style="border:1px solid black;">Windows Server 2008 Itanium alapú rendszerekhez</td>
<td style="border:1px solid black;">Nem érintett</td>
<td style="border:1px solid black;"><a href="http://www.microsoft.com/downloads/details.aspx?familyid=640e1865-ebcc-4d69-a770-fd360020da1e">Windows Internet Explorer 7</a><br />
(Mérsékelt)</td>
<td style="border:1px solid black;"><a href="http://www.microsoft.com/downloads/details.aspx?familyid=80ec83e0-cfb8-4a5e-9254-6679a7225b83">DirectX 10.0</a><br />
(Kritikus)</td>
<td style="border:1px solid black;">Nem érintett</td>
<td style="border:1px solid black;">Nem érintett</td>
<td style="border:1px solid black;"><a href="http://www.microsoft.com/downloads/details.aspx?familyid=8907783b-e3fe-40b2-9fc8-4937e7d58b7e">Windows Server 2008 Itanium alapú rendszerekhez</a><br />
(Mérsékelt)</td>
<td style="border:1px solid black;"><a href="http://www.microsoft.com/downloads/details.aspx?familyid=59b1689c-e723-4d87-973e-4beac107a6f7">Windows Server 2008 Itanium alapú rendszerekhez</a><br />
(Alacsony)</td>
</tr>
</tbody>
</table>
 

**\*Érinti a Windows Server 2008 kiszolgálómag-telepítését.** A frissítés besorolása ugyanaz a Windows Server 2008 támogatott kiadásain függetlenül attól, hogy a Windows Server 2008 alkalmazást a kiszolgálómag-telepítési opcióval telepítették-e. További tudnivalókat ezzel a telepítési beállítással kapcsolatban a következő weboldalon talál:[Server Core](http://msdn.microsoft.com/en-us/library/ms723891(vs.85).aspx). A Server Core telepítési beállítás a Windows Server 2008 egyes kiadásainál nem alkalmazható. További tudnivalók: [Server Core telepítési beállítások összehasonlítása](http://www.microsoft.com/windowsserver2008/en/us/compare-core-installation.aspx).

**\*\*Nem érinti a Windows Server 2008 kiszolgálómag-telepítését.** A frissítésben tárgyalt biztonsági rések nem érintik a Windows Server 2008 támogatott kiadásait, amennyiben a Windows Server 2008 telepítése a kiszolgálómag-telepítési opció használatával történt. További tudnivalókat ezzel a telepítési beállítással kapcsolatban a következő weboldalon talál:[Server Core](http://msdn.microsoft.com/en-us/library/ms723891(vs.85).aspx). A Server Core telepítési beállítás a Windows Server 2008 egyes kiadásainál nem alkalmazható. További tudnivalók: [Server Core telepítési beállítások összehasonlítása](http://www.microsoft.com/windowsserver2008/en/us/compare-core-installation.aspx).

**\*\*\*A Windows Server 2008 Server Core telepítését a biztonsági rés ugyan nem érinti, de a frissítést felajánljuk hozzá.** Amennyiben a Windows Server 2008 telepítése a Server Core telepítési opció használatával történt, a frissítésben tárgyalt biztonsági rések nem érintik a Windows Server 2008 támogatott kiadásait, bár a biztonsági rések által érintett fájlok jelen lehetnek a rendszeren. Az érintett fájlokkal rendelkező felhasználóknak mégis felajánlják a frissítést, mivel a frissített fájlok újabbak (magasabb verziószámúak), mint a jelenleg a rendszeren található fájlok. További tudnivalókat ezzel a telepítési beállítással kapcsolatban a következő weboldalon talál:[Server Core](http://msdn.microsoft.com/en-us/library/ms723891(vs.85).aspx). A Server Core telepítési beállítás a Windows Server 2008 egyes kiadásainál nem alkalmazható. További tudnivalók: [Server Core telepítési beállítások összehasonlítása](http://www.microsoft.com/windowsserver2008/en/us/compare-core-installation.aspx).

Észlelési és telepítési eszközök, útmutatás
-------------------------------------------

<span></span>
**Biztonsági központ**

A szoftveres és biztonsági frissítések kezeléséhez azokat a szervezet asztali és hordozható számítógépeire, valamint kiszolgálóira is telepíteni kell. További tájékoztatásért látogasson el a [TechNet Update Management Center](http://go.microsoft.com/fwlink/?linkid=69903) weboldalára. A [TechNet Security Center](http://go.microsoft.com/fwlink/?linkid=21171) bővebb tájékoztatással szolgál a Microsoft-termékek biztonsági funkcióival kapcsolatban. A [Biztonság otthon](http://go.microsoft.com/fwlink/?linkid=85102) weboldalon a megfelelő hivatkozásra kattintva elérhetőek a legújabb biztonsági frissítések.

A biztonsági frissítések a [Microsoft Update](http://go.microsoft.com/fwlink/?linkid=40747), [Windows Update](http://go.microsoft.com/fwlink/?linkid=21130) és az [Office Update](http://go.microsoft.com/fwlink/?linkid=21135) weboldalakról tölthetőek le. A biztonsági frissítések a [Microsoft letöltőközpontjában](http://go.microsoft.com/fwlink/?linkid=21129) is elérhetőek. Legegyszerűbben a „security update” kifejezésre irányuló kulcsszavas kereséssel találhatja meg ezeket.

A biztonsági frissítések a [Microsoft Update katalógusából](http://go.microsoft.com/fwlink/?linkid=96155) is letölthetőek. A Microsoft Update katalógus a Windows Update és Microsoft Update szolgáltatáson keresztül elérhető tartalom kereshető adatbázisa; ide tartoznak a biztonsági frissítések, illesztőprogramok és szervizcsomagok. A biztonsági közlemény számára (pl. „MS07-036”) történő kereséssel hozzáadhatja az összes vonatkozó frissítést a kosárhoz (beleértve a frissítés különböző nyelvi változatait), és letöltheti azokat a megadott mappába. A Microsoft Update katalógus részletes leírását lásd a vonatkozó [GYIK](http://go.microsoft.com/fwlink/?linkid=97900)részben.

**Útmutató az észleléshez és a telepítéshez**

A Microsoft az e havi biztonsági frissítésekhez észlelési és telepítési útmutatót adott ki. Az útmutató a számítógépes szakembereknek is ötleteket adhat ahhoz, hogyan használják a különböző eszközöket, pl. Windows Update, Microsoft Update, Office Update, Microsoft Baseline Security Analyzer (MBSA), Office Detection Tool, Microsoft Systems Management Server (SMS) és Extended Security Update Inventory Tool (ESUIT) a biztonsági frissítések telepítéséhez. További információt a [Microsoft Tudásbázis 910723. számú cikkében](http://support.microsoft.com/kb/910723) talál.

**Microsoft Baseline Security Analyzer**

A Microsoft Baseline Security Analyzer (MBSA) segítségével a rendszergazda mind a helyi, mind a távoli számítógépeken ellenőrizheti, hogy mely biztonsági frissítések hiányoznak, illetve hogy mely biztonsági beállítások vannak helytelenül megadva. Ha többet szeretne tudni az MBSA -eszközről, látogasson el a [Microsoft Baseline Security Analyzer webhelyre](http://go.microsoft.com/fwlink/?linkid=21134).

**Windows Server Update Services**

A Microsoft Software Update Services (WSUS) szolgáltatással a rendszergazdák gyorsan és megbízható módon telepíthetik központilag a legújabb fontos és biztonsági frissítéseket Windows 2000 és újabb operációs rendszerekhez, Office XP és újabb operációs rendszerekhez, Exchange Server 2003 és SQL Server 2000 Windows 2000 és újabb operációs rendszerekre.

A biztonsági frissítésnek Windows Server Update Services szolgáltatással történő központi telepítéséről a [Windows Server Update Services](http://go.microsoft.com/fwlink/?linkid=50120) webhelyen tudhat meg többet.

**Systems Management Server**

A Microsoft Systems Management Server (SMS) rendszer egy sokoldalúan beállítható vállalati megoldás, amely a frissítések kezelésére szolgál. Az SMS segítségével a rendszergazda megállapíthatja, hogy melyik Windows alapú számítógép szorul biztonsági frissítésre, és ezeket a frissítéseket szabályozott módon, a felhasználók minimális zavarásával központilag telepítheti a vállalat teljes informatikai környezetében. Az SMS, vagyis a System Center Configuration Manager 2007 újabb kiadása immáron elérhető, lásd még: [System Center Configuration Manager 2007](http://technet.microsoft.com/en-us/library/bb735860.aspx). Arról, hogy a rendszergazdák hogyan használhatják a biztonsági frissítések telepítéséhez az SMS 2003 alkalmazást, az [SMS 2003 Security Patch Management](http://go.microsoft.com/fwlink/?linkid=22939) részben olvashat. Az SMS 2.0 verzióját használók a [Software Updates Services Feature Pack](http://go.microsoft.com/fwlink/?linkid=33340) szolgáltatásait is segítségül hívhatják a biztonsági frissítések központi telepítéséhez. Az SMS-szolgáltatásról bővebben a [Microsoft Systems Management Server](http://go.microsoft.com/fwlink/?linkid=21158) oldalán olvashat.

**Megjegyzés:** Az SMS a Microsoft Baseline Security Analyzer és a Microsoft Office Detection Tool program segítségével széles körű támogatást nyújt a frissítések biztonsági értesítők segítségével történő észleléséhez és telepítéséhez. Előfordulhat, hogy egyes szoftverfrissítéseket ezek az eszközök nem észlelnek. Az SMS alkalmazás leltározási szolgáltatásai segítségével a rendszergazdák adott rendszereken hajthatják végre a frissítést. Az eljárással kapcsolatban olvassa el a [szoftverfrissítések telepítése az SMS szoftverelosztó ügynök segítségével](http://go.microsoft.com/fwlink/?linkid=33341) című tájékoztatót. Egyes biztonsági frissítésekhez rendszergazdai jogosultságokra van szükség a számítógép újraindítása után. A rendszergazdák az [SMS 2003 Administration Feature Pack](http://go.microsoft.com/fwlink/?linkid=33387) és az [SMS 2.0 Administration Feature Pack](http://go.microsoft.com/fwlink/?linkid=21161) csomag részét képező Elevated Rights Deployment Tool nevű eszközzel telepíthetik ezeket a frissítéseket.

### Egyéb információ

#### A Microsoft Windows rosszindulatú szoftvereket eltávolító eszköze

A Microsoft a Windows Update, Microsoft Update, Windows Server Update Services és Letöltőközpont szolgáltatásán keresztül elérhetővé tette a Microsoft Windows rosszindulatú szoftvereket eltávolító eszközének frissített változatát.

#### Nem biztonsági jellegű, kiemelt fontosságú frissítések a MU, WU és WSUS-szolgáltatásokban

A Windows Update és a Microsoft Update helyen elérhető, nem biztonsági jellegű frissítésekről tájékozódjon itt:

-   [Microsoft Tudásbázis 894199. cikke](http://support.microsoft.com/kb/894199): A Software Update Services és a Windows Server Update Services 2008-as tartalmi módosításainak ismertetése. Minden, Windows rendszerre vonatkozó tartalom.
-   [Microsoft-termékek új, módosított és közreadott frissítései, a Microsoft Windows rendszert kivéve](http://technet.microsoft.com/en-us/wsus/bb466214.aspx).

#### Biztonsági stratégiák és közösségek

**Frissítésekkel kapcsolatos stratégiák**

[A frissítések kezelésére vonatkozó útmutatás](http://go.microsoft.com/fwlink/?linkid=21168) a Microsoft által a biztonsági frissítések telepítéséhez ajánlott legjobban bevált eljárást ismerteti.

**Egyéb biztonsági frissítések beszerzése**

Az alábbi helyekről más típusú biztonsági problémákhoz szerezhetők be frissítések.

-   A biztonsági frissítések a [Microsoft letöltőközpontban](http://go.microsoft.com/fwlink/?linkid=21129) érhetők el. Legegyszerűbben a „security update” kifejezésre irányuló kulcsszavas kereséssel találhatja meg ezeket.
-   Az ügyfélrendszerek frissítései a [Microsoft Update](http://go.microsoft.com/fwlink/?linkid=40747) oldalról elérhetőek.
-   A Windows Update szolgáltatáson keresztül terjesztett havi aktuális biztonsági frissítések a letöltőközpontból a biztonsági és kritikus frissítéseket tartalmazó ISO CD-képfájlként is letölthetőek. További információt a [Microsoft Tudásbázis 913086](http://support.microsoft.com/kb/913086) számú cikkében talál.

**IT Pro Security közösség**

Az [IT Pro Security Community](http://go.microsoft.com/fwlink/?linkid=21164) közösségben hasznos információt találhat a biztonság javításáról és az informatikai infrastruktúrák optimalizálásáról, továbbá eszmecserét folytathat a biztonsági kérdésekről más informatikai szakemberekkel.

#### Köszönetnyilvánítás

A Microsoft [köszönetét](http://go.microsoft.com/fwlink/?linkid=21127) fejezi ki a vásárlók védelmének biztosításában nyújtott segítségért az alábbi szervezet(ek)nek és szakember(ek)nek:

-   Sebastian Apelt, Peter Vreugdenhil és egy nevét meg nem adó kutató, [Tipping Point](http://www.tippingpoint.com/) és [Zero Day Initiative](http://www.zerodayinitiative.com/), az MS08-031 közleményben leírt probléma jelentéséért.
-   Mark Dowd, az [IBM Internet Security Systems X-Force](http://xforce.iss.net/) kutatója, az MS08-033 közleményben leírt probléma jelentéséért.
-   A [Tipping Point](http://www.tippingpoint.com/) és [Zero Day Initiative](http://www.zerodayinitiative.com/) cégekkel együttműködő anonim kutató, az MS08-033 közleményben leírt probléma jelentéséért.
-   Alex Matthews és John Guzik, [Securify](http://www.securify.com/), az MS08-035 közleményben leírt probléma jelentéséért.

#### Terméktámogatás

-   Teszteléssel állapították meg a felsorolt szoftverek egyes verzióinak érintettségét. A többi verzió támogatási életciklusa végére ért. Az egyes szoftververziók támogatási életciklusáról a [Microsoft termékek terméktámogatási életciklusát ismertető webhelyen](http://go.microsoft.com/fwlink/?linkid=21742) talál felvilágosítást.
-   Az Amerikai Egyesült Államokban és Kanadában technikai segítség igényelhető a [Microsoft terméktámogatási szolgáltatásától](http://go.microsoft.com/fwlink/?linkid=21131), amelynek telefonszáma 1-866-PCSAFETY. A biztonsági frissítésekkel kapcsolatos hívások ingyenesek.
-   Más országokban a helyi Microsoft-képviseletek nyújtanak támogatást. A biztonsági frissítésekkel kapcsolatos hívások ingyenesek. A [nemzetközi támogatási webhely](http://go.microsoft.com/fwlink/?linkid=21155) felvilágosítást nyújt arról, támogatási kérdéseivel hogyan fordulhat a Microsofthoz.

#### Felelősséget kizáró nyilatkozat

A Microsoft Tudásbázisban leírtak előzetes bejelentés nélkül változhatnak, és a cikkek tartalmáért a Microsoft nem vállal garanciát. A Microsoft egyben elhárít minden kifejezett és értelemszerű garanciát, beleértve az eladhatóságra és az adott célra való alkalmasságra vonatkozó garanciát is. A Microsoft Corporation vagy annak szállítói semmilyen körülmények között nem tehetők felelőssé közvetlen, közvetett, eseti, ok-okozati vagy különleges kárért (beleértve az elmaradt hasznot is), még akkor sem, ha a Microsoft Corporation vagy szállítói tudatában voltak a kár lehetséges voltának. Egyes államok törvényi szabályozása nem teszi lehetővé a véletlen vagy ok-okozati károkért vállalt felelősség korlátozását vagy kizárását, így ezekben az államokban az ez a felelősségkizárás nincs érvényben.

#### Verziók

-   1.0 verzió (2008. június 10.): Összefoglaló közlemény közzététele.
-   1.1 verzió (2008. június 11.): Az Érintett szoftverek táblázat Windows XP rendszerre vonatkozó részében javítottuk az MS08-030, MS08-031, MS08-032, MS08-033 és MS08-036 közlemények Windows XP Service Pack 2 és Windows XP Service Pack 3 rendszerekkel kapcsolatos bejegyzéseit.
-   2.0 verzió (2008. július 16.): A DirectX 9.0a felkerült az MS08-033 érintett szoftvereket tartalmazó listájára.
-   2.1 verzió (2009. április 1.): Az MS08-032 vonatkozásában tisztáztuk, hogy a Windows Server 2008 Server Core telepítéseket a közleményben tárgyalt biztonsági rés nem érinti, de ettől függetlenül a frissítést felajánljuk. A módosítás csak tájékoztató jellegű. Az ilyen telepítésekre a frissítést nem kell alkalmazni.

*Built at 2014-04-18T01:50:00Z-07:00*
