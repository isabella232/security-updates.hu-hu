---
TOCTitle: 'MS08-OCT'
Title: 'Microsoft biztonsági közlemény - összefoglalás, október 2008'
ms:assetid: 'ms08-oct'
ms:contentKeyID: 61227724
ms:mtpsurl: 'https://technet.microsoft.com/hu-HU/library/ms08-oct(v=Security.10)'
author: SharonSears
ms.author: SharonSears
---

Security Bulletin Summary

Microsoft biztonsági közlemény - összefoglalás, október 2008
============================================================

Közzétéve: 2008. október 14. | Frissítve: 2008. október 16.

**Verzió:** 2.1

Az összefoglaló a 2008 októberében kiadott biztonsági közleményeket összegzi.

A 2008. októberi közlemények kiadása folytán az összefoglaló a 2007. október 9-én kiadott előzetes értesítés helyébe lép. További információkat a biztonsági közlemények kiadásáról szóló előzetes értesítési szolgáltatásról lásd: [Előzetes értesítés a Microsoft biztonsági közleményeinek kiadásáról](http://technet.microsoft.com/security/bulletin/advance).

Ha automatikus értesítést szeretne kapni a Microsoft biztonsági közleményeinek megjelenéséről, fizessen elő a [Microsoft Technical Security Notifications](http://go.microsoft.com/fwlink/?linkid=21163) szolgáltatásra.

A közleményekkel kapcsolatos kérdések megválaszolására a Microsoft 2008. október 15-én, csendes-óceáni idő szerint 11 órakor webes szemináriumot tart. [Jelentkezzen most az októberi közleményeket bemutató webes szemináriumra](http://msevents.microsoft.com/cui/webcasteventdetails.aspx?eventid=1032374639). Ezt követően a webes szeminárium igény szerint kerül megrendezésre. További információkért látogasson el a [Microsoft biztonsági közleményeit és a webes szemináriumokat](http://technet.microsoft.com/security/bulletin/summary)bemutató oldalra.

A Microsoft abban is segítséget nyújt felhasználóinak, hogy a havi biztonsági közleményekkel azonos napon kiadott, nem biztonsági jellegű, de fontos frissítéseket megfelelően rangsorolhassák. Lásd az **Egyéb információ című részt**.

### A közleménnyel kapcsolatos információk

#### Összefoglalások

Az e havi biztonsági közlemények súlyossági sorrendben:

Kritikus (4)
------------

<span></span>

| Közlemény azonosítója                          | A Microsoft MS08-060 számú biztonsági közleménye                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                            |
|------------------------------------------------|-----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| **Közlemény címe**                             | [**Az Active Directory biztonsági rése távoli kódfuttatást tehet lehetővé (957280)**](http://go.microsoft.com/fwlink/?linkid=128125)                                                                                                                                                                                                                                                                                                                                                                                                                                                                                        |
| **Összefoglalás**                              | Ez a biztonsági frissítés a Microsoft Windows 2000 Server rendszeren az Active Directory közvetlenül jelentett biztonsági rését szünteti meg. A biztonsági rés távoli kódfuttatást tehet lehetővé, ha a támadó hozzáférést szerez az érintett hálózatra. Ez a biztonsági rés csak a tartományvezérlőként konfigurált Microsoft Windows 2000 kiszolgálókat érinti. Ha a Microsoft Windows 2000 kiszolgáló nem lett előléptetve tartományvezérlővé, nem veszi figyelembe az LDAP (Lightweight Directory Access Protocol) és az LDAPS (SSL protokollon érkezett LDAP) lekéréseket, így nincs kitéve ennek a biztonsági résnek. |
| **Súlyosság maximális foka**                   | [Kritikus](http://go.microsoft.com/fwlink/?linkid=21140)                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                    |
| **A biztonsági rés hatása**                    | Távoli kódfuttatás                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                          |
| **A szoftver észlelésével kapcsolatos adatok** | A Microsoft Baseline Security Analyzer képes észlelni, szükséges-e a számítógépen az adott frissítést. Ez a frissítés újraindítást igényel.                                                                                                                                                                                                                                                                                                                                                                                                                                                                                 |
| **Érintett szoftverek**                        | **Microsoft Windows.** További információt az Érintett szoftverek és letöltési helyek című rész tartalmaz.                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                  |

| Közlemény azonosítója                          | A Microsoft MS08-058 számú biztonsági közleménye                                                                                                                                                                                                                                                                                                                                                                                                                            |
|------------------------------------------------|-----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| **Közlemény címe**                             | [**Összesítő biztonsági frissítés az Internet Explorer programhoz (956390)**](http://go.microsoft.com/fwlink/?linkid=128060)                                                                                                                                                                                                                                                                                                                                                |
| **Összefoglalás**                              | Ez a biztonsági frissítés öt közvetlenül jelentett, valamint egy nyilvánosan jelentett biztonsági rést szüntet meg. A biztonsági rés lehetővé teheti adatok felfedést vagy távoli kódvégrehajtást, amikor a felhasználó egy különlegesen kialakított weboldalt tekint meg az Internet Explorer segítségével. A kevesebb jogosultsággal bíró fiókkal rendelkező felhasználók esetében kisebb a veszélyeztetettség, mint a rendszergazdai jogosultságokkal rendelkezők esetén |
| **Súlyosság maximális foka**                   | [Kritikus](http://go.microsoft.com/fwlink/?linkid=21140)                                                                                                                                                                                                                                                                                                                                                                                                                    |
| **A biztonsági rés hatása**                    | Távoli kódfuttatás                                                                                                                                                                                                                                                                                                                                                                                                                                                          |
| **A szoftver észlelésével kapcsolatos adatok** | A Microsoft Baseline Security Analyzer képes észlelni, szükséges-e a számítógépen az adott frissítést. Ez a frissítés újraindítást igényel.                                                                                                                                                                                                                                                                                                                                 |
| **Érintett szoftverek**                        | **Microsoft Windows, Internet Explorer.** További információt az Érintett szoftverek és letöltési helyek című rész tartalmaz.                                                                                                                                                                                                                                                                                                                                               |

| Közlemény azonosítója                          | A Microsoft MS08-059 számú biztonsági közleménye                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                      |
|------------------------------------------------|-----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| **Közlemény címe**                             | [**A Host Integration Server RPC szolgáltatás távoli kódfuttatást lehetővé tévő biztonsági rése (956695)**](http://go.microsoft.com/fwlink/?linkid=125712)                                                                                                                                                                                                                                                                                                                                                                                                                                                            |
| **Összefoglalás**                              | A biztonsági frissítés a Microsoft Microsoft Host Integration Server közvetlenül jelentett biztonsági rését szünteti meg. A biztonsági rés távolról történő programkódfuttatást tehet lehetővé, ha a támadó speciálisan kialakított RPC (Remote Procedure Call) kérelmet küld az érintett rendszernek. Azok az ügyfelek, akik a gyakorlati tanácsokat szem előtt tartva úgy konfigurálják az SNA RPC szolgáltatási fiókbejegyzését, hogy kevesebb felhasználói jogosultság legyen a rendszer részére, kevésbé érintettek, mint akik rendszergazdai jogosultsággal látják el az SNA RPC szolgáltatási fiókbejegyzését. |
| **Súlyosság maximális foka**                   | [Kritikus](http://go.microsoft.com/fwlink/?linkid=21140)                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                              |
| **A biztonsági rés hatása**                    | Távoli kódfuttatás                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                    |
| **A szoftver észlelésével kapcsolatos adatok** | A Microsoft Baseline Security Analyzer képes észlelni, szükséges-e a számítógépen az adott frissítést. Előfordulhat, hogy a frissítés a rendszer újraindítását igényli.                                                                                                                                                                                                                                                                                                                                                                                                                                               |
| **Érintett szoftverek**                        | **Microsoft Host Integration Server.** További információt az Érintett szoftverek és letöltési helyek című rész tartalmaz.                                                                                                                                                                                                                                                                                                                                                                                                                                                                                            |

| Közlemény azonosítója                          | A Microsoft MS08-057 számú biztonsági közleménye                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                      |
|------------------------------------------------|-------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| **Közlemény címe**                             | [**A Microsoft Excel biztonsági rései távolról történő kódfuttatást tehetnek lehetővé (956416)**](http://go.microsoft.com/fwlink/?linkid=124653)                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                      |
| **Összefoglalás**                              | A kritikus biztonsági frissítés a Microsoft Office Excel közvetlenül a Microsoftnak jelzett három biztonsági rését szünteti meg, melyek távoli kódfuttatást tesznek lehetővé, ha a felhasználó megnyit egy speciálisan létrehozott Excel fájlt. A biztonsági réseket kihasználó támadó teljes mértékben átveheti az érintett rendszer irányítását. Ezt követően a támadó programokat telepíthet, illetve adatokat tekinthet meg, módosíthat és törölhet, de korlátozás nélküli jogosultságokkal rendelkező új fiókokat is létrehozhat. A kevesebb jogosultsággal bíró fiókkal rendelkező felhasználók esetében kisebb a veszélyeztetettség, mint a rendszergazdai jogosultságokkal rendelkezők esetén |
| **Súlyosság maximális foka**                   | [Kritikus](http://go.microsoft.com/fwlink/?linkid=21140)                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                              |
| **A biztonsági rés hatása**                    | Távoli kódfuttatás                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                    |
| **A szoftver észlelésével kapcsolatos adatok** | A Microsoft Baseline Security Analyzer képes észlelni, szükséges-e a számítógépen az adott frissítést. A frissítés nem teszi szükségessé a számítógép újraindítását.                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                  |
| **Érintett szoftverek**                        | **Microsoft Office.** További információt az Érintett szoftverek és letöltési helyek című rész tartalmaz.                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                             |

Fontos (6)
----------

<span></span>

| Közlemény azonosítója                          | A Microsoft MS08-066 számú biztonsági közleménye                                                                                                                                                                                                                                                                                                                                                                    |
|------------------------------------------------|---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| **Közlemény címe**                             | [**A Microsoft kiegészítő funkció-illesztőprogramjában lévő biztonsági rés a jogok kiterjesztését teheti lehetővé (956803)**](http://go.microsoft.com/fwlink/?linkid=125709)                                                                                                                                                                                                                                        |
| **Összefoglalás**                              | Ez a biztonsági frissítés megszünteti a Microsoft kiegészítő funkció-illesztőprogramjában a közvetlenül jelzett biztonsági rést. Ha egy támadó kihasználja a biztonsági rést, teljes mértékben átveheti a rendszer irányítását. Ezt követően a támadó programokat telepíthet, illetve adatokat tekinthet meg, módosíthat és törölhet, de korlátozás nélküli jogosultságokkal rendelkező új fiókokat is létrehozhat. |
| **Súlyosság maximális foka**                   | [Fontos](http://go.microsoft.com/fwlink/?linkid=21140)                                                                                                                                                                                                                                                                                                                                                              |
| **A biztonsági rés hatása**                    | Jogok kiterjesztése                                                                                                                                                                                                                                                                                                                                                                                                 |
| **A szoftver észlelésével kapcsolatos adatok** | A Microsoft Baseline Security Analyzer képes észlelni, szükséges-e a számítógépen az adott frissítést. Ez a frissítés újraindítást igényel.                                                                                                                                                                                                                                                                         |
| **Érintett szoftverek**                        | **Microsoft Windows.** További információt az Érintett szoftverek és letöltési helyek című rész tartalmaz.                                                                                                                                                                                                                                                                                                          |

| Közlemény azonosítója                          | A Microsoft MS08-061 számú biztonsági közleménye                                                                                                                                                                                                                                                                            |
|------------------------------------------------|-----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| **Közlemény címe**                             | [**A Windows Kernel biztonsági rései a jogok kiterjesztését tehetik lehetővé (954211)**](http://go.microsoft.com/fwlink/?linkid=121738)                                                                                                                                                                                     |
| **Összefoglalás**                              | Ez a biztonsági frissítés egy nyilvánosságra került és két közvetlenül jelentett biztonsági rést szüntet meg a Windows kernelben. A biztonsági réseket kihasználó helyi támadó teljes mértékben átveheti az érintett rendszer irányítását. Névtelen felhasználók nem tudják távolról kiaknázni ezeket a biztonsági réseket. |
| **Súlyosság maximális foka**                   | [Fontos](http://go.microsoft.com/fwlink/?linkid=21140)                                                                                                                                                                                                                                                                      |
| **A biztonsági rés hatása**                    | Jogok kiterjesztése                                                                                                                                                                                                                                                                                                         |
| **A szoftver észlelésével kapcsolatos adatok** | A Microsoft Baseline Security Analyzer képes észlelni, szükséges-e a számítógépen az adott frissítést. Ez a frissítés újraindítást igényel.                                                                                                                                                                                 |
| **Érintett szoftverek**                        | **Microsoft Windows.** További információt az Érintett szoftverek és letöltési helyek című rész tartalmaz.                                                                                                                                                                                                                  |

| Közlemény azonosítója                          | A Microsoft MS08-062 számú biztonsági közleménye                                                                                                                                                                                                                                                                                                                                  |
|------------------------------------------------|-----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| **Közlemény címe**                             | [**A Windows Internet Printing Service biztonsági rése távoli kódfuttatást tehet lehetővé (953155)**](http://go.microsoft.com/fwlink/?linkid=120829)                                                                                                                                                                                                                              |
| **Összefoglalás**                              | A frissítés a Windows Internet Printing Service egy közvetlenül jelentett biztonsági rését szünteti meg, amely távoli kódfuttatásra adott lehetőséget. Ha egy támadó kihasználja a biztonsági rést, teljes mértékben átveheti a rendszer irányítását. Ezt követően programokat telepíthet, illetve adatokat tekinthet meg, módosíthat és törölhet, de új fiókokat is létrehozhat. |
| **Súlyosság maximális foka**                   | [Fontos](http://go.microsoft.com/fwlink/?linkid=21140)                                                                                                                                                                                                                                                                                                                            |
| **A biztonsági rés hatása**                    | Távoli kódfuttatás                                                                                                                                                                                                                                                                                                                                                                |
| **A szoftver észlelésével kapcsolatos adatok** | A Microsoft Baseline Security Analyzer képes észlelni, szükséges-e a számítógépen az adott frissítést. Ez a frissítés újraindítást igényel.                                                                                                                                                                                                                                       |
| **Érintett szoftverek**                        | **Microsoft Windows.** További információt az Érintett szoftverek és letöltési helyek című rész tartalmaz.                                                                                                                                                                                                                                                                        |

| Közlemény azonosítója                          | A Microsoft MS08-063 számú biztonsági közleménye                                                                                                                                                                                                                                                                                                                                                                                                                                     |
|------------------------------------------------|--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| **Közlemény címe**                             | [**Az SMB biztonsági rése távolról történő kódfuttatást tehet lehetővé (957095)**](http://go.microsoft.com/fwlink/?linkid=127994)                                                                                                                                                                                                                                                                                                                                                    |
| **Összefoglalás**                              | A fontos besorolású biztonsági frissítés a Microsoft Server Message Block (SMB) közvetlenül jelentett biztonsági rését szünteti meg. A biztonsági rés távolról történő programkódfuttatást tehet lehetővé olyan kiszolgálón, amelyik fájlokat vagy mappákat oszt meg. A biztonsági réseket sikeresen kihasználó támadó programokat telepíthet, illetve adatokat tekinthet meg, módosíthat és törölhet, de korlátozás nélküli jogosultságokkal rendelkező új fiókokat is létrehozhat. |
| **Súlyosság maximális foka**                   | [Fontos](http://go.microsoft.com/fwlink/?linkid=21140)                                                                                                                                                                                                                                                                                                                                                                                                                               |
| **A biztonsági rés hatása**                    | Távoli kódfuttatás                                                                                                                                                                                                                                                                                                                                                                                                                                                                   |
| **A szoftver észlelésével kapcsolatos adatok** | A Microsoft Baseline Security Analyzer képes észlelni, szükséges-e a számítógépen az adott frissítést. Ez a frissítés újraindítást igényel.                                                                                                                                                                                                                                                                                                                                          |
| **Érintett szoftverek**                        | **Microsoft Windows.** További információt az Érintett szoftverek és letöltési helyek című rész tartalmaz.                                                                                                                                                                                                                                                                                                                                                                           |

| Közlemény azonosítója                          | A Microsoft MS08-064 számú biztonsági közleménye                                                                                                                                                                                                                                                                                                                                                                                                                                                                                     |
|------------------------------------------------|--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| **Közlemény címe**                             | [**A virtuális címleíró manipulálása miatti biztonsági rés a jogok kiterjesztését teheti lehetővé (956841)**](http://go.microsoft.com/fwlink/?linkid=128103)                                                                                                                                                                                                                                                                                                                                                                         |
| **Összefoglalás**                              | Ez a biztonsági frissítés a virtuális címek leírójában lévő, közvetlenül jelentett biztonsági rést szünteti meg. A biztonsági rés a jogok kiterjesztését teszi lehetővé, ha a felhasználó elindít egy speciálisan kialakított alkalmazást. A biztonsági rést sikeresen kihasználó támadó kiterjesztett jogokat szerezhet az érintett rendszeren. Ezt követően a támadó programokat telepíthet, illetve adatokat tekinthet meg, módosíthat és törölhet, de korlátozás nélküli jogosultságokkal rendelkező új fiókokat is létrehozhat. |
| **Súlyosság maximális foka**                   | [Fontos](http://go.microsoft.com/fwlink/?linkid=21140)                                                                                                                                                                                                                                                                                                                                                                                                                                                                               |
| **A biztonsági rés hatása**                    | Jogok kiterjesztése                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                  |
| **A szoftver észlelésével kapcsolatos adatok** | A Microsoft Baseline Security Analyzer képes észlelni, szükséges-e a számítógépen az adott frissítést. Ez a frissítés újraindítást igényel.                                                                                                                                                                                                                                                                                                                                                                                          |
| **Érintett szoftverek**                        | **Microsoft Windows.** További információt az Érintett szoftverek és letöltési helyek című rész tartalmaz.                                                                                                                                                                                                                                                                                                                                                                                                                           |

| Közlemény azonosítója                          | A Microsoft MS08-065 számú biztonsági közleménye                                                                                                                                                                                                                             |
|------------------------------------------------|------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| **Közlemény címe**                             | [**Az üzenetsor-kezelés biztonsági rése távoli kódfuttatást tehet lehetővé (951071)**](http://go.microsoft.com/fwlink/?linkid=128102)                                                                                                                                        |
| **Összefoglalás**                              | Ez a biztonsági frissítés a Microsoft Windows Message Queuing Service (MSMQ) közvetlenül jelentett biztonsági rését szünteti meg. A biztonsági rés az engedélyezett MSMQ szolgáltatás esetén lehetővé tette távoli kód végrehajtását a Microsoft Windows 2000 rendszereknél. |
| **Súlyosság maximális foka**                   | [Fontos](http://go.microsoft.com/fwlink/?linkid=21140)                                                                                                                                                                                                                       |
| **A biztonsági rés hatása**                    | Távoli kódfuttatás                                                                                                                                                                                                                                                           |
| **A szoftver észlelésével kapcsolatos adatok** | A Microsoft Baseline Security Analyzer képes észlelni, szükséges-e a számítógépen az adott frissítést. Ez a frissítés újraindítást igényel.                                                                                                                                  |
| **Érintett szoftverek**                        | **Microsoft Windows.** További információt az Érintett szoftverek és letöltési helyek című rész tartalmaz.                                                                                                                                                                   |

Mérsékelt (1)
-------------

<span></span>

| Közlemény azonosítója                          | A Microsoft MS08-056 számú biztonsági közleménye                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                               |
|------------------------------------------------|----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| **Közlemény címe**                             | [**A Microsoft Office biztonsági rése adatokhoz való illetéktelen hozzáférést tehet lehetővé (957699)**](http://go.microsoft.com/fwlink/?linkid=128145)                                                                                                                                                                                                                                                                                                                                                                                                        |
| **Összefoglalás**                              | A biztonsági frissítés a Microsoft Office közvetlenül jelentett biztonsági rését szünteti meg. A biztonsági rés adatokhoz való illetéktelen hozzáférést tehet lehetővé, ha a felhasználó egy különlegesen kialakított CDO URL-címre kattint. A biztonsági rést sikeresen kihasználó támadó olyan ügyféloldali parancsfájlt helyezhet el a felhasználó böngészőjében, amely lehetővé teheti a tartalom meghamisítását, az adatokhoz való illetéktelen hozzáférést, illetve a felhasználó által az érintett webhelyen végrehajtható bármilyen műveletet elvégez. |
| **Súlyosság maximális foka**                   | [Mérsékelt.](http://go.microsoft.com/fwlink/?linkid=21140)                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                     |
| **A biztonsági rés hatása**                    | Adatokhoz való illetéktelen hozzáférés                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                         |
| **A szoftver észlelésével kapcsolatos adatok** | A Microsoft Baseline Security Analyzer képes észlelni, szükséges-e a számítógépen az adott frissítést. A frissítés nem teszi szükségessé a számítógép újraindítását.                                                                                                                                                                                                                                                                                                                                                                                           |
| **Érintett szoftverek**                        | **Microsoft Office.** További információt az Érintett szoftverek és letöltési helyek című rész tartalmaz.                                                                                                                                                                                                                                                                                                                                                                                                                                                      |

Kihasználhatósági információk
-----------------------------

<span></span>
**A táblázat használata**

A táblázatból megtudható, milyen valószínűséggel kerül nyilvánosságra működő rosszindulatú programkód az egyes telepítendő biztonsági frissítések esetén. A telepítés fontossági sorrendjének megállapításához az adott konfigurációnak megfelelően tekintse át az alábbi értékeléseket. A minősítések jelentéséről és meghatározásuk módjáról a [Microsoft biztonsági rések jegyzéke](http://technet.microsoft.com/en-us/security/cc998259.aspx) tartalmaz bővebb információt.

| Közlemény azonosítója                                     | Közlemény címe                                                                                                                                                                     | CVE-azonosító | Kihasználhatósági információk értékelése                                                                             | Fontos megjegyzések                                                                                                                                                                                                                                                                                   |
|-----------------------------------------------------------|------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|---------------|----------------------------------------------------------------------------------------------------------------------|-------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| [MS08-056](http://go.microsoft.com/fwlink/?linkid=128145) | [A Microsoft Office biztonsági rése adatokhoz való illetéktelen hozzáférést tehet lehetővé (957699)](http://go.microsoft.com/fwlink/?linkid=128145)                                | CVE-2008-4020 | [2 - Valószínűleg inkonzisztens rosszindulatú programkód](http://technet.microsoft.com/en-us/security/cc998259.aspx) | Működő rosszindulatú programkód létrehozható. A hatás súlyossága azonban korlátozott , mivel a biztonsági rés csak bizonyos webes alkalmazások esetében teszi lehetővé a hamisítást a párbeszédpanelekben. Ennek eredményeként a támadók csak kis mértékben fordítanak erre figyelmet.                |
| [MS08-057](http://go.microsoft.com/fwlink/?linkid=124653) | [A Microsoft Excel biztonsági rései távolról történő programkódfuttatást tehetnek lehetővé (956416)](http://go.microsoft.com/fwlink/?linkid=124653)                                | CVE-2008-4019 | [2 - Valószínűleg konzisztens rosszindulatú programkód](http://technet.microsoft.com/en-us/security/cc998259.aspx)   |                                                                                                                                                                                                                                                                                                       |
| [MS08-057](http://go.microsoft.com/fwlink/?linkid=124653) | [A Microsoft Excel biztonsági rései távolról történő programkódfuttatást tehetnek lehetővé (956416)](http://go.microsoft.com/fwlink/?linkid=124653)                                | CVE-2008-3471 | [2 - Valószínűleg inkonzisztens rosszindulatú programkód](http://technet.microsoft.com/en-us/security/cc998259.aspx) |                                                                                                                                                                                                                                                                                                       |
| [MS08-057](http://go.microsoft.com/fwlink/?linkid=124653) | [A Microsoft Excel biztonsági rései távolról történő programkódfuttatást tehetnek lehetővé (956416)](http://go.microsoft.com/fwlink/?linkid=124653)                                | CVE-2008-3477 | [2 - Valószínűleg inkonzisztens rosszindulatú programkód](http://technet.microsoft.com/en-us/security/cc998259.aspx) |                                                                                                                                                                                                                                                                                                       |
| [MS08-058](http://go.microsoft.com/fwlink/?linkid=128060) | [Összesítő biztonsági frissítés az Internet Explorer programhoz (956390)](http://go.microsoft.com/fwlink/?linkid=128060)                                                           | CVE-2008-2947 | (A közlemény kiadásakor nyilvános)                                                                                   |                                                                                                                                                                                                                                                                                                       |
| [MS08-058](http://go.microsoft.com/fwlink/?linkid=128060) | [Összesítő biztonsági frissítés az Internet Explorer programhoz (956390)](http://go.microsoft.com/fwlink/?linkid=128060)                                                           | CVE-2008-3472 | [2 - Valószínűleg konzisztens rosszindulatú programkód](http://technet.microsoft.com/en-us/security/cc998259.aspx)   |                                                                                                                                                                                                                                                                                                       |
| [MS08-058](http://go.microsoft.com/fwlink/?linkid=128060) | [Összesítő biztonsági frissítés az Internet Explorer programhoz (956390)](http://go.microsoft.com/fwlink/?linkid=128060)                                                           | CVE-2008-3473 | [2 - Valószínűleg konzisztens rosszindulatú programkód](http://technet.microsoft.com/en-us/security/cc998259.aspx)   |                                                                                                                                                                                                                                                                                                       |
| [MS08-058](http://go.microsoft.com/fwlink/?linkid=128060) | [Összesítő biztonsági frissítés az Internet Explorer programhoz (956390)](http://go.microsoft.com/fwlink/?linkid=128060)                                                           | CVE-2008-3475 | [2 - Valószínűleg inkonzisztens rosszindulatú programkód](http://technet.microsoft.com/en-us/security/cc998259.aspx) |                                                                                                                                                                                                                                                                                                       |
| [MS08-058](http://go.microsoft.com/fwlink/?linkid=128060) | [Összesítő biztonsági frissítés az Internet Explorer programhoz (956390)](http://go.microsoft.com/fwlink/?linkid=128060)                                                           | CVE-2008-3474 | [2 - Nem valószínű működő rosszindulatú programkód](http://technet.microsoft.com/en-us/security/cc998259.aspx)       |                                                                                                                                                                                                                                                                                                       |
| [MS08-058](http://go.microsoft.com/fwlink/?linkid=128060) | [Összesítő biztonsági frissítés az Internet Explorer programhoz (956390)](http://go.microsoft.com/fwlink/?linkid=128060)                                                           | CVE-2008-3476 | [2 - Nem valószínű működő rosszindulatú programkód](http://technet.microsoft.com/en-us/security/cc998259.aspx)       |                                                                                                                                                                                                                                                                                                       |
| [MS08-059](http://go.microsoft.com/fwlink/?linkid=125712) | [A Host Integration Server RPC szolgáltatás távoli programkódfuttatást lehetővé tévő biztonsági rése (956695)](http://go.microsoft.com/fwlink/?linkid=125712)                      | CVE-2008-3466 | [2 - Valószínűleg konzisztens rosszindulatú programkód](http://technet.microsoft.com/en-us/security/cc998259.aspx)   | Bár valószínűleg csak bizonyos típusú vállalati felhasználók telepítik a Host Integration Server kiszolgálót, a támadók létrehozhatnak működő rosszindulatú programkódot.                                                                                                                             |
| [MS08-060](http://go.microsoft.com/fwlink/?linkid=128125) | [Az Active Directory biztonsági rése távoli programkódfuttatást tehet lehetővé (957280)](http://go.microsoft.com/fwlink/?linkid=128125)                                            | CVE-2008-4023 | [2 - Valószínűleg inkonzisztens rosszindulatú programkód](http://technet.microsoft.com/en-us/security/cc998259.aspx) | Valószínű, hogy a támadók a biztonsági rés kihasználásával szolgáltatásmegtagadást okoznak. A működő rosszindulatú programkód távoli kódvégrehajtáshoz történő létrehozása azonban a szükséges írási cím elérhetetlensége miatt nem egyszerű.                                                         |
| [MS08-061](http://go.microsoft.com/fwlink/?linkid=121738) | [A Windows Kernel biztonsági rései illetéktelen jogosultságmegszerzést eredményezhetnek (954211)](http://go.microsoft.com/fwlink/?linkid=121738)                                   | CVE-2008-2250 | [2 - Valószínűleg konzisztens rosszindulatú programkód](http://technet.microsoft.com/en-us/security/cc998259.aspx)   |                                                                                                                                                                                                                                                                                                       |
| [MS08-061](http://go.microsoft.com/fwlink/?linkid=121738) | [A Windows Kernel biztonsági rései illetéktelen jogosultságmegszerzést eredményezhetnek (954211)](http://go.microsoft.com/fwlink/?linkid=121738)                                   | CVE-2008-2252 | [2 - Valószínűleg konzisztens rosszindulatú programkód](http://technet.microsoft.com/en-us/security/cc998259.aspx)   | A legvalószínűbb eset, hogy többprocesszoros rendszerekhez hoznak létre működő programkódot.                                                                                                                                                                                                          |
| [MS08-061](http://go.microsoft.com/fwlink/?linkid=121738) | [A Windows Kernel biztonsági rései illetéktelen jogosultságmegszerzést eredményezhetnek (954211)](http://go.microsoft.com/fwlink/?linkid=121738)                                   | CVE-2008-2251 | [2 - Nem valószínű működő rosszindulatú programkód](http://technet.microsoft.com/en-us/security/cc998259.aspx)       | A biztonsági rés kihasználása lehetséges ugyan, de nagyon nehéz létrehozni megbízhatóan működő rosszindulatú programkódot.                                                                                                                                                                            |
| [MS08-062](http://go.microsoft.com/fwlink/?linkid=120829) | [A Windows Internet Printing Service biztonsági rése, amely távoli programkódfuttatást tesz lehetővé (953155)](http://go.microsoft.com/fwlink/?linkid=120829)                      | CVE-2008-1446 | [2 - Valószínűleg konzisztens rosszindulatú programkód](http://technet.microsoft.com/en-us/security/cc998259.aspx)   | Korlátozott, célzott támadások esetében felfedeztünk már konzisztens rosszindulatú programkódot. Noha az Internet Printing Protocol (IPP) szolgáltatás alapértelmezésben engedélyezett, a szolgáltatás IIS segítségével történő eléréséhez alapértelmezésben minden platformon hitelesítés szükséges. |
| [MS08-063](http://go.microsoft.com/fwlink/?linkid=127994) | [A SMB képmegjelenítő rendszer biztonsági rése távolról történő kódfuttatást tehet lehetővé (957095)](http://go.microsoft.com/fwlink/?linkid=127994)                               | CVE-2008-4038 | [2 - Valószínűleg inkonzisztens rosszindulatú programkód](http://technet.microsoft.com/en-us/security/cc998259.aspx) |                                                                                                                                                                                                                                                                                                       |
| [MS08-064](http://go.microsoft.com/fwlink/?linkid=128103) | [A virtuális címek leírójának manipulálása miatti biztonsági rés (956841) a jogosultság illetéktelen megszerzését teszi lehetővé](http://go.microsoft.com/fwlink/?linkid=128103)   | CVE-2008-4036 | [2 - Valószínűleg inkonzisztens rosszindulatú programkód](http://technet.microsoft.com/en-us/security/cc998259.aspx) |                                                                                                                                                                                                                                                                                                       |
| [MS08-065](http://go.microsoft.com/fwlink/?linkid=128102) | [Az Üzenetsor-kezelés szolgáltatás távoli kódfuttatást lehetővé tévő biztonsági rése (951071)](http://go.microsoft.com/fwlink/?linkid=128102)                                      | CVE-2008-3479 | [2 - Nem valószínű működő rosszindulatú programkód](http://technet.microsoft.com/en-us/security/cc998259.aspx)       | Noha az adatokhoz való illetéktelen hozzáférés előfordulhat, a memóriából nem mindig lehetséges hasznos tartalomhoz jutni. A memóriameghibásodás miatti hiba kihasználható, de a távoli kódvégrehajtás nehezen kivitelezhető.                                                                         |
| [MS08-066](http://go.microsoft.com/fwlink/?linkid=125709) | [A Microsoft kiegészítő funkció-illesztőprogramjában a jogosultság illetéktelen megszerzését lehetővé tévő biztonsági rés (956803)](http://go.microsoft.com/fwlink/?linkid=125709) | CVE-2008-3464 | [2 - Valószínűleg konzisztens rosszindulatú programkód](http://technet.microsoft.com/en-us/security/cc998259.aspx)   |                                                                                                                                                                                                                                                                                                       |

Érintett szoftverek és letöltési helyek
---------------------------------------

<span></span>
**A táblázat használata**

A táblázat segítségével megtudhatja a szükséges információt a telepítendő biztonsági frissítésekről. Nézzen meg minden felsorolt szoftvert vagy összetevőt annak megállapításához, hogy van-e telepítendő biztonsági frissítés. Ha a szoftver vagy összetevő szerepel a listán, hiperhivatkozással kapcsolódik hozzá az elérhető szoftverfrissítés, és a frissítés besorolása is fel van tüntetve.

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
</tr>
<tr>
<th colspan="9">
Microsoft Windows 2000
</th>
</tr>
<tr>
<td style="border:1px solid black;">
**Közlemény azonosítója**
</td>
<td style="border:1px solid black;">
[**MS08-060**](http://go.microsoft.com/fwlink/?linkid=128125)
</td>
<td style="border:1px solid black;">
[**MS08-058**](http://go.microsoft.com/fwlink/?linkid=128060)
</td>
<td style="border:1px solid black;">
[**MS08-066**](http://go.microsoft.com/fwlink/?linkid=125709)
</td>
<td style="border:1px solid black;">
[**MS08-061**](http://go.microsoft.com/fwlink/?linkid=121738)
</td>
<td style="border:1px solid black;">
[**MS08-062**](http://go.microsoft.com/fwlink/?linkid=120829)
</td>
<td style="border:1px solid black;">
[**MS08-063**](http://go.microsoft.com/fwlink/?linkid=127994)
</td>
<td style="border:1px solid black;">
[**MS08-064**](http://go.microsoft.com/fwlink/?linkid=128103)
</td>
<td style="border:1px solid black;">
[**MS08-065**](http://go.microsoft.com/fwlink/?linkid=128102)
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
**Közlemény legmagasabb súlyossági besorolása**
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
Microsoft Windows 2000 Service Pack 4
</td>
<td style="border:1px solid black;">
[Active Directory Microsoft Windows 2000 Server Service Pack 4 rendszeren](http://www.microsoft.com/downloads/details.aspx?familyid=8ed7bb9a-4b26-49d7-8c14-60226d2bc20d)  
(Kritikus)
</td>
<td style="border:1px solid black;">
[Microsoft Internet Explorer 5.01 Service Pack 4](http://www.microsoft.com/downloads/details.aspx?familyid=257c0478-56dd-42eb-a90e-607d01613db7)  
(Kritikus)  
[Microsoft Internet Explorer 6 Service Pack 1 szervizcsomaggal](http://www.microsoft.com/downloads/details.aspx?familyid=02390258-08e9-4b75-960d-be081b749558)  
(Kritikus)
</td>
<td style="border:1px solid black;">
Nem érintett
</td>
<td style="border:1px solid black;">
[Microsoft Windows 2000 Service Pack 4](http://www.microsoft.com/downloads/details.aspx?familyid=3a6165a6-d7e7-4526-9291-290caf0639b4)  
(Fontos)
</td>
<td style="border:1px solid black;">
[Microsoft Windows 2000 Service Pack 4](http://www.microsoft.com/downloads/details.aspx?familyid=8163bd1be6-cc5-4f39-8134-3d42326d822afe1d)  
(Fontos)
</td>
<td style="border:1px solid black;">
[Microsoft Windows 2000 Service Pack 4](http://www.microsoft.com/downloads/details.aspx?familyid=9ed29c3a-0682-4586-bbc2-a73deaa18e4c)  
(Fontos)
</td>
<td style="border:1px solid black;">
Nem érintett
</td>
<td style="border:1px solid black;">
[Microsoft Windows 2000 Service Pack 4](http://www.microsoft.com/downloads/details.aspx?familyid=899e2728-2433-4ccb-a195-05b5d65e5469)  
(Fontos)
</td>
</tr>
<tr>
<th colspan="9">
Windows XP
</th>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
**Közlemény azonosítója**
</td>
<td style="border:1px solid black;">
[**MS08-060**](http://go.microsoft.com/fwlink/?linkid=128125)
</td>
<td style="border:1px solid black;">
[**MS08-058**](http://go.microsoft.com/fwlink/?linkid=128060)
</td>
<td style="border:1px solid black;">
[**MS08-066**](http://go.microsoft.com/fwlink/?linkid=125709)
</td>
<td style="border:1px solid black;">
[**MS08-061**](http://go.microsoft.com/fwlink/?linkid=121738)
</td>
<td style="border:1px solid black;">
[**MS08-062**](http://go.microsoft.com/fwlink/?linkid=120829)
</td>
<td style="border:1px solid black;">
[**MS08-063**](http://go.microsoft.com/fwlink/?linkid=127994)
</td>
<td style="border:1px solid black;">
[**MS08-064**](http://go.microsoft.com/fwlink/?linkid=128103)
</td>
<td style="border:1px solid black;">
[**MS08-065**](http://go.microsoft.com/fwlink/?linkid=128102)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
**Közlemény legmagasabb súlyossági besorolása**
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
<tr class="alternateRow">
<td style="border:1px solid black;">
Windows XP Service Pack 2 és Windows XP Service Pack 3
</td>
<td style="border:1px solid black;">
Nem érintett
</td>
<td style="border:1px solid black;">
[Microsoft Internet Explorer 6](http://www.microsoft.com/downloads/details.aspx?familyid=a7f0f47b-b1ee-4516-9fbf-bf8e579963d0)  
(Kritikus)  
[Windows Internet Explorer 7](http://www.microsoft.com/downloads/details.aspx?familyid=4e73de2b-05e6-4901-9bac-46d8f469e635)  
(Fontos)
</td>
<td style="border:1px solid black;">
[Windows XP Service Pack 2 és Windows XP Service Pack 3](http://www.microsoft.com/downloads/details.aspx?familyid=b16d9dac-c430-4dd8-a1e5-9a614801f1d9)  
(Fontos)
</td>
<td style="border:1px solid black;">
[Windows XP Service Pack 2 és Windows XP Service Pack 3](http://www.microsoft.com/downloads/details.aspx?familyid=7718bf14-c26c-43f3-be67-4c79ab5b2607)  
(Fontos)
</td>
<td style="border:1px solid black;">
[Windows XP Service Pack 2 és Windows XP Service Pack 3](http://www.microsoft.com/downloads/details.aspx?familyid=e7ef571f-c9e8-4e14-95a3-3eeaec55b784)  
(Fontos)
</td>
<td style="border:1px solid black;">
[Windows XP Service Pack 2 és Windows XP Service Pack 3](http://www.microsoft.com/downloads/details.aspx?familyid=2f7e5981-6eef-4f08-86c0-c6a7607ea5d0)  
(Fontos)
</td>
<td style="border:1px solid black;">
[Windows XP Service Pack 2 és Windows XP Service Pack 3](http://www.microsoft.com/downloads/details.aspx?familyid=25997b73-a640-49c1-b19e-768a18bbe22c)  
(Fontos)
</td>
<td style="border:1px solid black;">
Nem érintett
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Windows XP Professional x64 Edition és Windows XP Professional x64 Edition Service Pack 2
</td>
<td style="border:1px solid black;">
Nem érintett
</td>
<td style="border:1px solid black;">
[Microsoft Internet Explorer 6](http://www.microsoft.com/downloads/details.aspx?familyid=234c05fb-988b-4e02-aab6-bb23e447df3d)  
(Kritikus)  
[Windows Internet Explorer 7](http://www.microsoft.com/downloads/details.aspx?familyid=ccf7a3e3-ec30-4b95-9a86-00032301513c)  
(Fontos)
</td>
<td style="border:1px solid black;">
[Windows XP Professional x64 Edition és Windows XP Professional x64 Edition Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=5b607efc-c6fb-4079-8478-e4f3262386d3)  
(Fontos)
</td>
<td style="border:1px solid black;">
[Windows XP Professional x64 Edition és Windows XP Professional x64 Edition Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=b06d3a02-b6e4-4d40-913a-3759a31f20f3)  
(Fontos)
</td>
<td style="border:1px solid black;">
[Windows XP Professional x64 Edition és Windows XP Professional x64 Edition Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=3e4b913-0-4974-b198-828a10db)  
(Fontos)
</td>
<td style="border:1px solid black;">
[Windows XP Professional x64 Edition és Windows XP Professional x64 Edition Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=4e1675eb-6b06-48e9-9765-23a2c7737bdc)  
(Fontos)
</td>
<td style="border:1px solid black;">
[Windows XP Professional x64 Edition és Windows XP Professional x64 Edition Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=50fae854-0bde-46f8-9444-b9e0d9bfecad)  
(Fontos)
</td>
<td style="border:1px solid black;">
Nem érintett
</td>
</tr>
<tr>
<th colspan="9">
Windows Server 2003
</th>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
**Közlemény azonosítója**
</td>
<td style="border:1px solid black;">
[**MS08-060**](http://go.microsoft.com/fwlink/?linkid=128125)
</td>
<td style="border:1px solid black;">
[**MS08-058**](http://go.microsoft.com/fwlink/?linkid=128060)
</td>
<td style="border:1px solid black;">
[**MS08-066**](http://go.microsoft.com/fwlink/?linkid=125709)
</td>
<td style="border:1px solid black;">
[**MS08-061**](http://go.microsoft.com/fwlink/?linkid=121738)
</td>
<td style="border:1px solid black;">
[**MS08-062**](http://go.microsoft.com/fwlink/?linkid=120829)
</td>
<td style="border:1px solid black;">
[**MS08-063**](http://go.microsoft.com/fwlink/?linkid=127994)
</td>
<td style="border:1px solid black;">
[**MS08-064**](http://go.microsoft.com/fwlink/?linkid=128103)
</td>
<td style="border:1px solid black;">
[**MS08-065**](http://go.microsoft.com/fwlink/?linkid=128102)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
**Közlemény legmagasabb súlyossági besorolása**
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
<tr class="alternateRow">
<td style="border:1px solid black;">
Windows Server 2003 Service Pack 1 és Windows Server 2003 Service Pack 2 rendszerhez
</td>
<td style="border:1px solid black;">
Nem érintett
</td>
<td style="border:1px solid black;">
[Microsoft Internet Explorer 6](http://www.microsoft.com/downloads/details.aspx?familyid=ae8d22d5-20aa-471d-a423-f54c9d75febe)  
(Mérsékelt)  
[Windows Internet Explorer 7](http://www.microsoft.com/downloads/details.aspx?familyid=feaf2adf-7892-4dbf-a147-db4d5dbe52f3)  
(Alacsony)
</td>
<td style="border:1px solid black;">
[Windows Server 2003 Service Pack 1 és Windows Server 2003 Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=ee88ff2d-1b12-4f4c-a081-9f27a6fba074)  
(Fontos)
</td>
<td style="border:1px solid black;">
[Windows Server 2003 Service Pack 1 és Windows Server 2003 Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=6e696762-d652-4a8f-ab8f-622f9746c320)  
(Fontos)
</td>
<td style="border:1px solid black;">
[Windows Server 2003 Service Pack 1 és Windows Server 2003 Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=437a9b68-6a0c-48c8-9348-0d6fda48aa21)  
(Fontos)
</td>
<td style="border:1px solid black;">
[Windows Server 2003 Service Pack 1 és Windows Server 2003 Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=dbbebb3f-f1c7-402c-bd16-6f88da0d042c)  
(Fontos)
</td>
<td style="border:1px solid black;">
[Windows Server 2003 Service Pack 1 és Windows Server 2003 Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=e8ef3d5f-dd8e-4945-92cd-9d3e30b16667)  
(Fontos)
</td>
<td style="border:1px solid black;">
Nem érintett
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Windows Server 2003 x64 Edition és Windows Server 2003 x64 Edition Service Pack 2 rendszerhez
</td>
<td style="border:1px solid black;">
Nem érintett
</td>
<td style="border:1px solid black;">
[Microsoft Internet Explorer 6](http://www.microsoft.com/downloads/details.aspx?familyid=07fc88c4-2571-4a4d-b573-ae576798ab4c)  
(Mérsékelt)  
[Windows Internet Explorer 7](http://www.microsoft.com/downloads/details.aspx?familyid=319dba34-07ca-47f9-a1e9-20df2df7966b)  
(Alacsony)
</td>
<td style="border:1px solid black;">
[Windows Server 2003 x64 Edition és Windows Server 2003 x64 Edition Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=ab4d94d3-458c-4946-ab7f-03a279629d25)  
(Fontos)
</td>
<td style="border:1px solid black;">
[Windows Server 2003 x64 Edition és Windows Server 2003 x64 Edition Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=57ca28ea-e5e1-4191-a3d6-84aa90a3d668)  
(Fontos)
</td>
<td style="border:1px solid black;">
[Windows Server 2003 x64 Edition és Windows Server 2003 x64 Edition Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=d3df6508-a568-449d-ac97-fbf3f97b98ef)  
(Fontos)
</td>
<td style="border:1px solid black;">
[Windows Server 2003 x64 Edition és Windows Server 2003 x64 Edition Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=989ac6f1-515c-467d-a200-2aabe66d9319)  
(Fontos)
</td>
<td style="border:1px solid black;">
[Windows Server 2003 x64 Edition és Windows Server 2003 x64 Edition Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=c2e754f9-086a-494c-bc19-5feed7df8b65)  
(Fontos)
</td>
<td style="border:1px solid black;">
Nem érintett
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
Windows Server 2003 SP1 Itanium alapú rendszerekhez és Windows Server 2003 SP2 Itanium alapú rendszerekhez
</td>
<td style="border:1px solid black;">
Nem érintett
</td>
<td style="border:1px solid black;">
[Microsoft Internet Explorer 6](http://www.microsoft.com/downloads/details.aspx?familyid=b68937af-f04a-4d1e-9d7f-ec92af5194de)  
(Mérsékelt)  
[Windows Internet Explorer 7](http://www.microsoft.com/downloads/details.aspx?familyid=47381d91-4a14-4a09-96b3-3345155df52d)  
(Alacsony)
</td>
<td style="border:1px solid black;">
[Windows Server 2003 SP1 Itanium alapú rendszerekhez és Windows Server 2003 SP2 Itanium alapú rendszerekhez](http://www.microsoft.com/downloads/details.aspx?familyid=63234f85-6e5d-4ef6-b7cf-d1d2c78a5517)  
(Fontos)
</td>
<td style="border:1px solid black;">
[Windows Server 2003 SP1 Itanium alapú rendszerekhez és Windows Server 2003 SP2 Itanium alapú rendszerekhez](http://www.microsoft.com/downloads/details.aspx?familyid=1e6c3f81-85bb-48e6-a5af-635a7e540c93)  
(Fontos)
</td>
<td style="border:1px solid black;">
[Windows Server 2003 SP1 Itanium alapú rendszerekhez és Windows Server 2003 SP2 Itanium alapú rendszerekhez](http://www.microsoft.com/downloads/details.aspx?familyid=748f54f1-40b9-407c-9819-909061b53743)  
(Fontos)
</td>
<td style="border:1px solid black;">
[Windows Server 2003 SP1 Itanium alapú rendszerekhez és Windows Server 2003 SP2 Itanium alapú rendszerekhez](http://www.microsoft.com/downloads/details.aspx?familyid=91589cfb-15ba-4dd2-9e3b-107899fbcba6)  
(Fontos)
</td>
<td style="border:1px solid black;">
[Windows Server 2003 SP1 Itanium alapú rendszerekhez és Windows Server 2003 SP2 Itanium alapú rendszerekhez](http://www.microsoft.com/downloads/details.aspx?familyid=5a3832ec-3f8f-42c1-a603-b1330d527547)  
(Fontos)
</td>
<td style="border:1px solid black;">
Nem érintett
</td>
</tr>
<tr>
<th colspan="9">
Windows Vista
</th>
</tr>
<tr>
<td style="border:1px solid black;">
**Közlemény azonosítója**
</td>
<td style="border:1px solid black;">
[**MS08-060**](http://go.microsoft.com/fwlink/?linkid=128125)
</td>
<td style="border:1px solid black;">
[**MS08-058**](http://go.microsoft.com/fwlink/?linkid=128060)
</td>
<td style="border:1px solid black;">
[**MS08-066**](http://go.microsoft.com/fwlink/?linkid=125709)
</td>
<td style="border:1px solid black;">
[**MS08-061**](http://go.microsoft.com/fwlink/?linkid=121738)
</td>
<td style="border:1px solid black;">
[**MS08-062**](http://go.microsoft.com/fwlink/?linkid=120829)
</td>
<td style="border:1px solid black;">
[**MS08-063**](http://go.microsoft.com/fwlink/?linkid=127994)
</td>
<td style="border:1px solid black;">
[**MS08-064**](http://go.microsoft.com/fwlink/?linkid=128103)
</td>
<td style="border:1px solid black;">
[**MS08-065**](http://go.microsoft.com/fwlink/?linkid=128102)
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
**Közlemény legmagasabb súlyossági besorolása**
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
Windows Vista és Windows Vista Service Pack 1
</td>
<td style="border:1px solid black;">
Nem érintett
</td>
<td style="border:1px solid black;">
[Windows Internet Explorer 7](http://www.microsoft.com/downloads/details.aspx?familyid=4756e04b-6e1c-4d78-a3c0-17f6b4b97975)  
(Fontos)
</td>
<td style="border:1px solid black;">
Nem érintett
</td>
<td style="border:1px solid black;">
[Windows Vista és Windows Vista Service Pack 1](http://www.microsoft.com/downloads/details.aspx?familyid=3483b400-cedc-441f-ba8e-594e3df89190)  
(Fontos)
</td>
<td style="border:1px solid black;">
[Windows Vista és Windows Vista Service Pack 1](http://www.microsoft.com/downloads/details.aspx?familyid=9b5995df-a3b8-4e81-b118-9bb057e19884)  
(Nincs súlyossági besorolás)
</td>
<td style="border:1px solid black;">
[Windows Vista és Windows Vista Service Pack 1](http://www.microsoft.com/downloads/details.aspx?familyid=72dd6015-25d1-45f4-a769-88ac43074b44)  
(Fontos)
</td>
<td style="border:1px solid black;">
[Windows Vista és Windows Vista Service Pack 1](http://www.microsoft.com/downloads/details.aspx?familyid=b4212db5-093e-497d-b999-2e3780f9f7c2)  
(Fontos)
</td>
<td style="border:1px solid black;">
Nem érintett
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
Windows Vista x64 Edition és Windows Vista x64 Edition Service Pack 1
</td>
<td style="border:1px solid black;">
Nem érintett
</td>
<td style="border:1px solid black;">
[Windows Internet Explorer 7](http://www.microsoft.com/downloads/details.aspx?familyid=bd19c72b-4f83-47ab-93be-d2c286e732c4)  
(Fontos)
</td>
<td style="border:1px solid black;">
Nem érintett
</td>
<td style="border:1px solid black;">
[Windows Vista x64 Edition és Windows Vista x64 Edition Service Pack 1](http://www.microsoft.com/downloads/details.aspx?familyid=905ab030-14a5-4a3d-aa11-e8f957f6a1ea)  
(Fontos)
</td>
<td style="border:1px solid black;">
[Windows Vista x64 Edition és Windows Vista x64 Edition Service Pack 1](http://www.microsoft.com/downloads/details.aspx?familyid=4a0fcf4b-eb8e-456a-b934-400ae18248ee)  
(Nincs súlyossági besorolás)
</td>
<td style="border:1px solid black;">
[Windows Vista x64 Edition és Windows Vista x64 Edition Service Pack 1](http://www.microsoft.com/downloads/details.aspx?familyid=f793af16-5464-4db1-a42b-1c5f17c538ed)  
(Fontos)
</td>
<td style="border:1px solid black;">
[Windows Vista x64 Edition és Windows Vista x64 Edition Service Pack 1](http://www.microsoft.com/downloads/details.aspx?familyid=c20808cb-c30a-4b53-91e5-810eb6b4b2e3)  
(Fontos)
</td>
<td style="border:1px solid black;">
Nem érintett
</td>
</tr>
<tr>
<th colspan="9">
Windows Server 2008
</th>
</tr>
<tr>
<td style="border:1px solid black;">
**Közlemény azonosítója**
</td>
<td style="border:1px solid black;">
[**MS08-060**](http://go.microsoft.com/fwlink/?linkid=128125)
</td>
<td style="border:1px solid black;">
[**MS08-058**](http://go.microsoft.com/fwlink/?linkid=128060)
</td>
<td style="border:1px solid black;">
[**MS08-066**](http://go.microsoft.com/fwlink/?linkid=125709)
</td>
<td style="border:1px solid black;">
[**MS08-061**](http://go.microsoft.com/fwlink/?linkid=121738)
</td>
<td style="border:1px solid black;">
[**MS08-062**](http://go.microsoft.com/fwlink/?linkid=120829)
</td>
<td style="border:1px solid black;">
[**MS08-063**](http://go.microsoft.com/fwlink/?linkid=127994)
</td>
<td style="border:1px solid black;">
[**MS08-064**](http://go.microsoft.com/fwlink/?linkid=128103)
</td>
<td style="border:1px solid black;">
[**MS08-065**](http://go.microsoft.com/fwlink/?linkid=128102)
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
**Közlemény legmagasabb súlyossági besorolása**
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
Windows Server 2008 32 bites rendszerekhez
</td>
<td style="border:1px solid black;">
Nem érintett
</td>
<td style="border:1px solid black;">
[Windows Internet Explorer 7](http://www.microsoft.com/downloads/details.aspx?familyid=ec73f416-2204-42d6-8932-c96578ac819f)\*\*  
(Alacsony)
</td>
<td style="border:1px solid black;">
Nem érintett
</td>
<td style="border:1px solid black;">
[Windows Server 2008 32 bites rendszerekhez](http://www.microsoft.com/downloads/details.aspx?familyid=8b97114a-71aa-47a2-b9e7-f4e158c18c80)\*  
(Fontos)
</td>
<td style="border:1px solid black;">
[Windows Server 2008 32 bites rendszerekhez](http://www.microsoft.com/downloads/details.aspx?familyid=3d6290d8-1745-4bc0-9ca9-eeb1ad0be4a5)\*  
(Fontos)
</td>
<td style="border:1px solid black;">
[Windows Server 2008 32 bites rendszerekhez](http://www.microsoft.com/downloads/details.aspx?familyid=cf6744e6-b54c-40f6-a78d-7ba9453133c0)\*  
(Fontos)
</td>
<td style="border:1px solid black;">
[Windows Server 2008 32 bites rendszerekhez](http://www.microsoft.com/downloads/details.aspx?familyid=ec9eeb82-0497-4c55-94bb-9a47cb3521b4)\*  
(Fontos)
</td>
<td style="border:1px solid black;">
Nem érintett
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
Windows Server 2008 x64 alapú rendszerekhez
</td>
<td style="border:1px solid black;">
Nem érintett
</td>
<td style="border:1px solid black;">
[Windows Internet Explorer 7](http://www.microsoft.com/downloads/details.aspx?familyid=baacd1c2-9764-4fea-bd4d-c49791974fef)\*\*  
(Alacsony)
</td>
<td style="border:1px solid black;">
Nem érintett
</td>
<td style="border:1px solid black;">
[Windows Server 2008 x64 alapú rendszerekhez](http://www.microsoft.com/downloads/details.aspx?familyid=6e641db2-90c8-458f-9795-3e46b70a5203)\*  
(Fontos)
</td>
<td style="border:1px solid black;">
[Windows Server 2008 x64 alapú rendszerekhez](http://www.microsoft.com/downloads/details.aspx?familyid=a33c833c-d5c5-4e37-8f89-7b9079f92e59)\*  
(Fontos)
</td>
<td style="border:1px solid black;">
[Windows Server 2008 x64 alapú rendszerekhez](http://www.microsoft.com/downloads/details.aspx?familyid=223236e8-7b19-4b47-8a90-bfc35eb9318a)\*  
(Fontos)
</td>
<td style="border:1px solid black;">
[Windows Server 2008 x64 alapú rendszerekhez](http://www.microsoft.com/downloads/details.aspx?familyid=0bc178b8-f8ae-4f41-8f88-fb6a75be1bca)\*  
(Fontos)
</td>
<td style="border:1px solid black;">
Nem érintett
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Windows Server 2008 for Itanium-based Systems
</td>
<td style="border:1px solid black;">
Nem érintett
</td>
<td style="border:1px solid black;">
[Windows Internet Explorer 7](http://www.microsoft.com/downloads/details.aspx?familyid=250a45dd-7eae-4440-bd10-02a703940976)  
(Alacsony)
</td>
<td style="border:1px solid black;">
Nem érintett
</td>
<td style="border:1px solid black;">
[Windows Server 2008 Itanium alapú rendszerekhez](http://www.microsoft.com/downloads/details.aspx?familyid=b6546e1c-bf7b-4354-8574-6c16fa707de0)  
(Fontos)
</td>
<td style="border:1px solid black;">
[Windows Server 2008 Itanium alapú rendszerekhez](http://www.microsoft.com/downloads/details.aspx?familyid=31783e88-76e2-4bc6-b4ae-308443c6d223)  
(Nincs súlyossági besorolás)
</td>
<td style="border:1px solid black;">
[Windows Server 2008 Itanium alapú rendszerekhez](http://www.microsoft.com/downloads/details.aspx?familyid=077b697c-04a0-45bd-b08c-331d5c30cb47)  
(Fontos)
</td>
<td style="border:1px solid black;">
[Windows Server 2008 Itanium alapú rendszerekhez](http://www.microsoft.com/downloads/details.aspx?familyid=0af72663-4945-4916-8c55-090ba4d82793)  
(Fontos)
</td>
<td style="border:1px solid black;">
Nem érintett
</td>
</tr>
</table>
 
**\*Érinti a Windows Server 2008 kiszolgálómag-telepítését.** A frissítés besorolása ugyanaz a Windows Server 2008 támogatott kiadásain függetlenül attól, hogy a Windows Server 2008 alkalmazást a kiszolgálómag-telepítési opcióval telepítették-e. További tudnivalókat ezzel a telepítési beállítással kapcsolatban a következő weboldalon talál:[Server Core](http://msdn.microsoft.com/en-us/library/ms723891(vs.85).aspx). A Server Core telepítési beállítás a Windows Server 2008 egyes kiadásainál nem alkalmazható. További tudnivalók: [Server Core telepítési beállítások összehasonlítása](http://www.microsoft.com/windowsserver2008/en/us/compare-core-installation.aspx).

**\*\*Nem érinti a Windows Server 2008 kiszolgálómag-telepítését.** A frissítésben tárgyalt biztonsági rések nem érintik a Windows Server 2008 támogatott kiadásait, amennyiben a Windows Server 2008 telepítése a kiszolgálómag-telepítési opció használatával történt. További tudnivalókat ezzel a telepítési beállítással kapcsolatban a következő weboldalon talál:[Server Core](http://msdn.microsoft.com/en-us/library/ms723891(vs.85).aspx). A Server Core telepítési beállítás a Windows Server 2008 egyes kiadásainál nem alkalmazható. További tudnivalók: [Server Core telepítési beállítások összehasonlítása](http://www.microsoft.com/windowsserver2008/en/us/compare-core-installation.aspx).

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
[**MS08-057**](http://go.microsoft.com/fwlink/?linkid=124653)
</td>
<td style="border:1px solid black;">
[**MS08-056**](http://go.microsoft.com/fwlink/?linkid=128145)
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
**Közlemény legmagasabb súlyossági besorolása**
</td>
<td style="border:1px solid black;">
[**Kritikus**](http://go.microsoft.com/fwlink/?linkid=21140)
</td>
<td style="border:1px solid black;">
[**Mérsékelt**](http://go.microsoft.com/fwlink/?linkid=21140)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Microsoft Office 2000 Service Pack 3
</td>
<td style="border:1px solid black;">
[Excel 2000 Service Pack 3](http://www.microsoft.com/downloads/details.aspx?familyid=1b2740e0-ecdd-48ca-84e0-eb187c31eb16)  
(KB955461)  
(Kritikus)
</td>
<td style="border:1px solid black;">
Nem érintett
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
Microsoft Office XP SP3
</td>
<td style="border:1px solid black;">
[Excel 2002 Service Pack 3](http://www.microsoft.com/downloads/details.aspx?familyid=27cedef1-c47c-472c-a343-cd9b4ebc2bba)  
(KB955464)  
(Fontos)
</td>
<td style="border:1px solid black;">
[Microsoft Office XP Service Pack 3](http://www.microsoft.com/downloads/details.aspx?familyid=b1aee2d5-bfa0-40e3-91b6-98bf65524e8c)  
(KB956464)  
(Mérsékelt)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Microsoft Office 2003 Service Pack 2 és Microsoft Office 2003 Service Pack 3
</td>
<td style="border:1px solid black;">
[Excel 2003 Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=4df27e8a-d803-483b-a700-0177d71bf368)  
(KB955466)  
(Fontos)  
[Excel 2003 Service Pack 3](http://www.microsoft.com/downloads/details.aspx?familyid=4df27e8a-d803-483b-a700-0177d71bf368)  
(KB955466)  
(Fontos)
</td>
<td style="border:1px solid black;">
Nem érintett
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
2007 Microsoft Office System és 2007 Microsoft Office System Service Pack 1
</td>
<td style="border:1px solid black;">
[Excel 2007](http://www.microsoft.com/downloads/details.aspx?familyid=2765bbc0-ea2e-4b6e-822c-222ee8e5021f)  
(KB955470)  
(Fontos)  
[Excel 2007 Service Pack 1](http://www.microsoft.com/downloads/details.aspx?familyid=2765bbc0-ea2e-4b6e-822c-222ee8e5021f)  
(KB955470)  
(Fontos)
</td>
<td style="border:1px solid black;">
Nem érintett
</td>
</tr>
<tr>
<th colspan="3">
Microsoft Office for Mac
</th>
</tr>
<tr>
<td style="border:1px solid black;">
**Közlemény azonosítója**
</td>
<td style="border:1px solid black;">
[**MS08-057**](http://go.microsoft.com/fwlink/?linkid=124653)
</td>
<td style="border:1px solid black;">
[**MS08-056**](http://go.microsoft.com/fwlink/?linkid=128145)
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
**Közlemény legmagasabb súlyossági besorolása**
</td>
<td style="border:1px solid black;">
[**Kritikus**](http://go.microsoft.com/fwlink/?linkid=21140)
</td>
<td style="border:1px solid black;">
[**Mérsékelt**](http://go.microsoft.com/fwlink/?linkid=21140)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Microsoft Office 2004 for Mac
</td>
<td style="border:1px solid black;">
[Microsoft Office 2004 for Mac](http://www.microsoft.com/downloads/details.aspx?familyid=ba4fa21a-7e01-4ef8-9b9f-9d51d00ef094)  
(KB958312)  
(Fontos)
</td>
<td style="border:1px solid black;">
Nem érintett
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
Microsoft Office 2008 for Mac
</td>
<td style="border:1px solid black;">
[Microsoft Office 2008 for Mac](http://www.microsoft.com/downloads/details.aspx?familyid=e70c5ae0-2858-46de-81f8-dcd1786656b7)  
(KB958267)  
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
[Open XML File Format Converter for Mac](http://www.microsoft.com/downloads/details.aspx?familyid=2a8d9a3b-b8a4-43b6-82a6-a2e7d16ae11d)  
(KB958304)  
(Fontos)
</td>
<td style="border:1px solid black;">
Nem érintett
</td>
</tr>
<tr>
<th colspan="3">
További Office-szoftverek
</th>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
**Közlemény azonosítója**
</td>
<td style="border:1px solid black;">
[**MS08-057**](http://go.microsoft.com/fwlink/?linkid=124653)
</td>
<td style="border:1px solid black;">
[**MS08-056**](http://go.microsoft.com/fwlink/?linkid=128145)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
**Közlemény legmagasabb súlyossági besorolása**
</td>
<td style="border:1px solid black;">
[**Kritikus**](http://go.microsoft.com/fwlink/?linkid=21140)
</td>
<td style="border:1px solid black;">
[**Mérsékelt**](http://go.microsoft.com/fwlink/?linkid=21140)
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
Microsoft Office Excel Viewer
</td>
<td style="border:1px solid black;">
[Microsoft Office Excel Viewer 2003](http://www.microsoft.com/downloads/details.aspx?familyid=9769ce08-5207-4c63-b7b9-536266ad6b2b)  
(KB955468)  
(Fontos)  
[Microsoft Office Excel Viewer 2003 Service Pack 3](http://www.microsoft.com/downloads/details.aspx?familyid=9769ce08-5207-4c63-b7b9-536266ad6b2b)  
(KB955468)  
(Fontos)  
[Microsoft Office Excel Viewer](http://www.microsoft.com/downloads/details.aspx?familyid=83c88444-75b8-44d1-b280-3671394ade45)  
(KB955935)  
(Fontos)
</td>
<td style="border:1px solid black;">
Nem érintett
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Microsoft Office kompatibilitási csomag a Word, Excel és PowerPoint 2007 fájlformátumokhoz
</td>
<td style="border:1px solid black;">
[Microsoft Office kompatibilitási csomag a Word, Excel és PowerPoint 2007 fájlformátumokhoz](http://www.microsoft.com/downloads/details.aspx?familyid=9a7be004-5903-4101-90c5-c0d5f8722af9)  
(KB955936)  
(Fontos)  
[Microsoft Office kompatibilitási csomag a Word, Excel és PowerPoint 2007 fájlformátumok Service Pack 1 csomagjához](http://www.microsoft.com/downloads/details.aspx?familyid=9a7be004-5903-4101-90c5-c0d5f8722af9)  
(KB955936)  
(Fontos)
</td>
<td style="border:1px solid black;">
Nem érintett
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
Microsoft Office SharePoint Server 2007
</td>
<td style="border:1px solid black;">
[Microsoft Office SharePoint Server 2007](http://www.microsoft.com/downloads/details.aspx?familyid=5c29e646-504c-4455-9d35-9a1bed6d7535)\*  
(KB955937)  
(Fontos)  
[Microsoft Office SharePoint Server 2007 SP1](http://www.microsoft.com/downloads/details.aspx?familyid=5c29e646-504c-4455-9d35-9a1bed6d7535)\*  
(KB955937)  
(Fontos)  
[Microsoft Office SharePoint Server 2007 x64](http://www.microsoft.com/downloads/details.aspx?familyid=3c21c405-2c9e-45d0-be4d-8ccd093af31f)\*  
(KB955937)  
(Fontos)  
[Microsoft Office SharePoint Server 2007 x64 SP1](http://www.microsoft.com/downloads/details.aspx?familyid=3c21c405-2c9e-45d0-be4d-8ccd093af31f)\*  
(KB955937)  
(Fontos)
</td>
<td style="border:1px solid black;">
Nem érintett
</td>
</tr>
</table>
 
\*A frissítés azokra a kiszolgálókra vonatkozik, amelyeken az Excel Services szolgáltatás telepítve van, vagyis a Microsoft Office SharePoint Server 2007 Enterprise és a Microsoft Office SharePoint Server 2007 For Internet Sites alapértelmezett konfigurációira. A Microsoft Office SharePoint Server 2007 Standard nem foglalja magában az Excel Services funkciót.

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
Microsoft Host Integration Server
</th>
</tr>
<tr>
<td style="border:1px solid black;">
**Közlemény azonosítója**
</td>
<td style="border:1px solid black;">
[**MS08-059**](http://go.microsoft.com/fwlink/?linkid=125712)
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
**Közlemény legmagasabb súlyossági besorolása**
</td>
<td style="border:1px solid black;">
[**Kritikus**](http://go.microsoft.com/fwlink/?linkid=21140)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Microsoft Host Integration Server 2000
</td>
<td style="border:1px solid black;">
[Microsoft Host Integration Server 2000 Service Pack 2 (Server)](http://www.microsoft.com/downloads/details.aspx?familyid=11cca58b-59a4-4e93-9eb1-19b07c290a10)  
(Kritikus)  
[Microsoft Host Integration Server 2000 Administrator Client](http://www.microsoft.com/downloads/details.aspx?familyid=41b49291-1231-4e23-aef7-818207453d56)  
(Kritikus)
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
Microsoft Host Integration Server 2004
</td>
<td style="border:1px solid black;">
[Microsoft Host Integration Server 2004 (Server)](http://www.microsoft.com/downloads/details.aspx?familyid=9ca255ed-9334-4848-af94-49ef3078cdc0)  
(Kritikus)  
[Microsoft Host Integration Server 2004 SP1 (Server)](http://www.microsoft.com/downloads/details.aspx?familyid=eca756a1-ca56-4481-b23c-53c159a4e08c)  
(Kritikus)  
[Microsoft Host Integration Server 2004 (Client)](http://www.microsoft.com/downloads/details.aspx?familyid=92cb54e7-f4ff-40a4-99cb-6257c4d8d4cd)  
(Kritikus)  
[Microsoft Host Integration Server 2004 SP1 (Client)](http://www.microsoft.com/downloads/details.aspx?familyid=d776515c-09aa-4a04-876d-606bfc26a006)  
(Kritikus)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Microsoft Host Integration Server 2006
</td>
<td style="border:1px solid black;">
[Microsoft Host Integration Server 2006 32 bites rendszerekhez](http://www.microsoft.com/downloads/details.aspx?familyid=1ae79da3-ec17-4d4b-8011-d777a237ac93)  
(Kritikus)  
[Microsoft Host Integration Server 2006 (x64 alapú rendszerekhez)](http://www.microsoft.com/downloads/details.aspx?familyid=05da4540-4976-458a-a612-7385d78695a2)  
(Kritikus)
</td>
</tr>
</table>
 

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

A Microsoft Systems Management Server (SMS) rendszer egy sokoldalúan beállítható vállalati megoldás, amely a frissítések kezelésére szolgál. Az SMS segítségével a rendszergazda megállapíthatja, hogy melyik Windows alapú számítógép szorul biztonsági frissítésre, és ezeket a frissítéseket szabályozott módon, a felhasználók minimális zavarásával központilag telepítheti a vállalat teljes informatikai környezetében. Az SMS, vagyis a System Center Configuration Manager 2007 újabb kiadása immáron elérhető, lásd még: [System Center Configuration Manager 2007](http://technet.microsoft.com/en-us/library/bb735860,aspx). Arról, hogy a rendszergazdák hogyan használhatják a biztonsági frissítések telepítéséhez az SMS 2003 alkalmazást, az [SMS 2003 Security Patch Management](http://go.microsoft.com/fwlink/?linkid=22939) részben olvashat. Az SMS 2.0 verzióját használók a [Software Updates Services Feature Pack](http://go.microsoft.com/fwlink/?linkid=33340) szolgáltatásait is segítségül hívhatják a biztonsági frissítések központi telepítéséhez. Az SMS-szolgáltatásról bővebben a [Microsoft Systems Management Server](http://go.microsoft.com/fwlink/?linkid=21158) oldalán olvashat.

**Megjegyzés:** Az SMS a Microsoft Baseline Security Analyzer és a Microsoft Office Detection Tool program segítségével széles körű támogatást nyújt a frissítések biztonsági értesítők segítségével történő észleléséhez és telepítéséhez. Előfordulhat, hogy egyes szoftverfrissítéseket ezek az eszközök nem észlelnek. Az SMS alkalmazás leltározási szolgáltatásai segítségével a rendszergazdák adott rendszereken hajthatják végre a frissítést. Az eljárással kapcsolatban olvassa el a [szoftverfrissítések telepítése az SMS szoftverelosztó ügynök segítségével](http://go.microsoft.com/fwlink/?linkid=33341) című tájékoztatót. Egyes biztonsági frissítésekhez rendszergazdai jogosultságokra van szükség a számítógép újraindítása után. A rendszergazdák az [SMS 2003 Administration Feature Pack](http://go.microsoft.com/fwlink/?linkid=33387) és az [SMS 2.0 Administration Feature Pack](http://go.microsoft.com/fwlink/?linkid=21161) csomag részét képező Elevated Rights Deployment Tool nevű eszközzel telepíthetik ezeket a frissítéseket.

**Az Update Compatibility Evaluator (a frissítéskompatibilitás kiértékelője) és az Application Compatibility Toolkit (alkalmazáskompatibilitási eszközkészlet)**

Az alkalmazások működése érdekében a frissítések gyakran írnak ugyanazokba a fájlokba, illetve regisztrációs bejegyzésekbe. Ez inkompatibilitást okozhat, és növelheti a biztonsági frissítések központi telepítésére használt időt. A Windows frissítések és az alkalmazásoknak való megfelelőségének tesztelése és ellenőrzése egyszerűsíthető az [Update Compatibility Evaluator](http://technet2.microsoft.com/windowsvista/en/library/4279e239-37a4-44aa-aec5-4e70fe39f9de1033.mspx?mfr=true) eszközeivel, ami része az [Application Compatibility Toolkit 5.0](http://www.microsoft.com/downloads/details.aspx?familyid=24da89e9-b581-47b0-b45e-492dd6da2971&displaylang=hu) csomagnak.

Az Application Compatibility Toolkit (ACT) tartalmazza a Microsoft Windows Vista, a Windows Update, a Microsoft Security Update vagy a Windows Internet Explorer új verziójának központi telepítése előtt az alkalmazáskompatibilitási problémák kiértékeléséhez és enyhítéséhez szükséges eszközöket és dokumentációt.

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

-   [NetAgent Co., Ltd.](http://www.netagent.co.jp/) az MS08-056 közleményben ismertetett probléma jelentéséért
-   Joshua J. Drake, [iDefense](http://labs.idefense.com/), az MS08-057 közleményben ismertetett probléma jelentéséért
-   Wushi, valamint az együttműködő [TippingPoint](http://www.tippingpoint.com/) és [Zero Day Initiative](http://www.zerodayinitiative.com/), az MS08-057 közleményben ismertetett probléma jelentéséért
-   Lionel d'Hauenens, [Labo Skopia](http://www.laboskopia.com/), és a vele együttműködő [iDefense VCP](http://labs.idefense.com/), az MS08-057 közleményben ismertetett probléma jelentéséért
-   David Bloom, az MS08-058 számú közleményben bemutatott probléma jelentéséért
-   Gregory Rubin, az MS08-058 számú közleményben bemutatott probléma jelentéséért
-   [Ivan Fratric](http://ifsec.blogspot.com/), valamint a vele együttműködő [TippingPoint](http://www.tippingpoint.com/) és a [Zero Day Initiative](http://www.zerodayinitiative.com/), az MS08-058 közleményben leírt probléma jelentéséért
-   Thierry Zoller, [n.runs](http://www.nruns.com/), az MS08-058 közleményben leírt probléma jelentéséért
-   Lee Dagon, [Composica](http://www.composica.com/), az MS08-058 közleményben leírt probléma jelentéséért
-   Stephen Fewer, [Harmony Security](http://www.harmonysecurity.com/), és az együttműködő [iDefense VCP](http://labs.idefense.com/), az MS08-059 közleményben leírt probléma jelentéséért
-   Paul Miseiko, [nCircle](http://www.ncircle.com/), az MS08-060 közleményben ismertetett probléma jelentéséért.
-   Paul Caton, [iShadow](http://www.ishadow.com/), az MS08-061 közleményben ismertetett probléma jelentéséért
-   Thomas Garnier, [SkyRecon](http://www.skyrecon.com/), az MS08-061 közleményben leírt probléma jelentéséért
-   [CERT/CC](http://www.cert.org/), az MS08-062 közleményben bemutatott probléma jelentéséért
-   Joshua Morin, [Codenomicon](http://www.codenomicon.com/), az MS08-063 közleményben ismertetett probléma jelentéséért.
-   Cody Pierce és Aaron Portnoy, [TippingPoint DVLabs](http://dvlabs.tippingpoint.com), az MS08-065 közleményben bemutatott probléma jelentéséért
-   Fabien Le Mentec, [SkyRecon](http://www.skyrecon.com/), az MS08-066 közleményben leírt probléma jelentéséért

#### Terméktámogatás

-   Teszteléssel állapították meg a felsorolt szoftverek egyes verzióinak érintettségét. A többi verzió támogatási életciklusa végére ért. Az egyes szoftververziók támogatási életciklusáról a [Microsoft termékek terméktámogatási életciklusát ismertető webhelyen](http://go.microsoft.com/fwlink/?linkid=21742) talál felvilágosítást.
-   Az Amerikai Egyesült Államokban és Kanadában technikai segítség igényelhető a [Microsoft terméktámogatási szolgáltatásától](http://go.microsoft.com/fwlink/?linkid=21131), amelynek telefonszáma 1-866-PCSAFETY. A biztonsági frissítésekkel kapcsolatos hívások ingyenesek.
-   Más országokban a helyi Microsoft-képviseletek nyújtanak támogatást. A biztonsági frissítésekkel kapcsolatos hívások ingyenesek. A [nemzetközi támogatási webhely](http://go.microsoft.com/fwlink/?linkid=21155) felvilágosítást nyújt arról, támogatási kérdéseivel hogyan fordulhat a Microsofthoz.

#### Felelősséget kizáró nyilatkozat

A Microsoft Tudásbázisban leírtak előzetes bejelentés nélkül változhatnak, és a cikkek tartalmáért a Microsoft nem vállal garanciát. A Microsoft egyben elhárít minden kifejezett és értelemszerű garanciát, beleértve az eladhatóságra és az adott célra való alkalmasságra vonatkozó garanciát is. A Microsoft Corporation vagy annak szállítói semmilyen körülmények között nem tehetők felelőssé közvetlen, közvetett, eseti, ok-okozati vagy különleges kárért (beleértve az elmaradt hasznot is), még akkor sem, ha a Microsoft Corporation vagy szállítói tudatában voltak a kár lehetséges voltának. Egyes államok törvényi szabályozása nem teszi lehetővé a véletlen vagy ok-okozati károkért vállalt felelősség korlátozását vagy kizárását, így ezekben az államokban az ez a felelősségkizárás nincs érvényben.

#### Verziók

-   1.0 verzió (2008. október 14.): Összefoglaló közlemény közzététele.
-   2.0 verzió (2008. október 15.): A Windows Server 2008 Itanium alapú rendszerekhez súlyossági besorolása törölve (MS08-062).
-   2.1 verzió (2008. október 16.): Frissült az Összefoglalás a Microsoft MS08-062 számú frissített biztonsági közleményéhez.

*Built at 2014-04-18T01:50:00Z-07:00*
