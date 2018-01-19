---
TOCTitle: 'MS08-JUL'
Title: 'Microsoft biztonsági közlemény - összefoglalás, július 2008'
ms:assetid: 'ms08-jul'
ms:contentKeyID: 61227721
ms:mtpsurl: 'https://technet.microsoft.com/hu-HU/library/ms08-jul(v=Security.10)'
---

Security Bulletin Summary

Microsoft biztonsági közlemény - összefoglalás, július 2008
===========================================================

Közzétéve: 2008. július 8. | Frissítve: 2009. február 11.

**Verzió:** 1.1

Az összefoglaló a 2008. júliusára kiadott biztonsági közleményeket összegzi.

A 2008. júliusi közlemények kiadása folytán az összefoglaló a 2008. július 3-án kiadott előzetes értesítés helyébe lép. A biztonsági közlemények kiadásáról szóló előzetes értesítés szolgáltatásról itt olvashat bővebben: [Előzetes értesítés a Microsoft biztonsági közleményeinek kiadásáról](http://technet.microsoft.com/security/bulletin/advance).

Ha automatikus értesítést szeretne kapni a Microsoft biztonsági közleményeinek megjelenéséről, fizessen elő a [Microsoft Technical Security Notifications](http://go.microsoft.com/fwlink/?linkid=21163) szolgáltatásra.

A közleményekkel kapcsolatos kérdések megválaszolására a Microsoft 2008. július 9-én, csendes-óceáni idő szerint 11 órakor webes szemináriumot tart. [Jelentkezzen most a júliusi közleményeket bemutató webes szemináriumra](http://msevents.microsoft.com/cui/eventdetail.aspx?eventid=1032374629&culture=en-us). Ezt követően a webes szeminárium igény szerint kerül megrendezésre. További információkért látogasson el a [Microsoft biztonsági közleményeit és a webes szemináriumokat](http://technet.microsoft.com/security/bulletin/summary)bemutató oldalra.

A Microsoft abban is segítséget nyújt felhasználóinak, hogy a havi biztonsági közleményekkel azonos napon kiadott, nem biztonsági jellegű, de fontos frissítéseket megfelelően rangsorolhassák. Lásd az **Egyéb információ című részt**.

### A közleménnyel kapcsolatos információk

#### Összefoglalások

Az e havi biztonsági közlemények súlyossági sorrendben:

Fontos (4)
----------

<span></span>

| Közlemény azonosítója                          | A Microsoft MS08-040 számú biztonsági közleménye                                                                                                                                                                                                                                                                                                                                                                                                    |
|------------------------------------------------|-----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| **Közlemény címe**                             | [**A Microsoft SQL Server biztonsági rései jogok kiterjesztését okozhatják (941203)**](http://go.microsoft.com/fwlink/?linkid=113725)                                                                                                                                                                                                                                                                                                               |
| **Összefoglalás**                              | Ez a biztonsági frissítés négy közvetlenül jelzett biztonsági rést szüntet meg. A legsúlyosabb kockázattal járó biztonsági rés lehetővé teszi, hogy az azt kihasználó támadó kódot futtasson, és átvegye a teljes érintett rendszer irányítását. Ezt követően a hitelesített támadó programokat telepíthet, illetve adatokat tekinthet meg, módosíthat és törölhet, de teljes rendszergazda jogosultságokkal rendelkező új fiókokat is létrehozhat. |
| **Súlyosság maximális foka**                   | [Fontos](http://go.microsoft.com/fwlink/?linkid=21140)                                                                                                                                                                                                                                                                                                                                                                                              |
| **A biztonsági rés hatása**                    | Jogok kiterjesztése                                                                                                                                                                                                                                                                                                                                                                                                                                 |
| **A szoftver észlelésével kapcsolatos adatok** | A Microsoft Baseline Security Analyzer képes észlelni, szükséges-e a számítógépen az adott frissítést. Előfordulhat, hogy a frissítés a rendszer újraindítását igényli.                                                                                                                                                                                                                                                                             |
| **Érintett szoftverek**                        | **Microsoft Windows, Microsoft SQL Server.** További információt az Érintett szoftverek és letöltési helyek című rész tartalmaz.                                                                                                                                                                                                                                                                                                                    |

| Közlemény azonosítója                          | A Microsoft MS08-038 számú biztonsági közleménye                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                               |
|------------------------------------------------|--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| **Közlemény címe**                             | [**A Windows Intézőnek a távolról történő programkódfuttatást lehetővé tévő biztonsági rése (950582)**](http://go.microsoft.com/fwlink/?linkid=117296)                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                         |
| **Összefoglalás**                              | A jelen biztonsági frissítés olyan biztonsági rést szüntet meg a Windows Intézőben, amely lehetővé teheti programkód távolból történő futtatását egy speciálisan kialakított és mentett keresési fájl megnyitásakor és mentésekor. Ha valamely felhasználó felügyeleti jogosultságokkal bejelentkezett a rendszerbe, akkor a biztonsági rést kihasználó támadó teljes mértékben átveheti az irányítást a számítógép felett, Ezt követően a támadó programokat telepíthet, illetve adatokat tekinthet meg, módosíthat és törölhet, de korlátozás nélküli jogosultságokkal rendelkező új fiókokat is létrehozhat. A kevesebb jogosultsággal bíró fiókkal rendelkező felhasználók esetében kisebb a veszélyeztetettség, mint a rendszergazdai jogosultságokkal rendelkezők esetén |
| **Súlyosság maximális foka**                   | [Fontos](http://go.microsoft.com/fwlink/?linkid=21140)                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                         |
| **A biztonsági rés hatása**                    | Távoli kódfuttatás                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                             |
| **A szoftver észlelésével kapcsolatos adatok** | A Microsoft Baseline Security Analyzer képes észlelni, szükséges-e a számítógépen az adott frissítést. Ez a frissítés újraindítást igényel.                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                    |
| **Érintett szoftverek**                        | **Microsoft Windows.** További információt az Érintett szoftverek és letöltési helyek című rész tartalmaz.                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                     |

| Közlemény azonosítója                          | A Microsoft MS08-037 számú biztonsági közleménye                                                                                                                                                                                                                                                                                                                               |
|------------------------------------------------|--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| **Közlemény címe**                             | [**A DNS szolgáltatás tartalomhamisítást lehetővé tévő biztonsági rései (953230)**](http://go.microsoft.com/fwlink/?linkid=119620)                                                                                                                                                                                                                                             |
| **Összefoglalás**                              | Ez a biztonsági frissítés a Windows Domain Name System (DNS) rendszerben tartalomhamisítást lehetővé tévő két közvetlenül jelzett biztonsági rést szüntet meg. Ezek a biztonsági rések megtalálhatók a DNS ügyfél és kiszolgálói változatában is, és lehetővé teszik, hogy az interneten lévő rendszereknek szánt hálózati forgalmat a támadó saját rendszerére irányítsák át. |
| **Súlyosság maximális foka**                   | [Fontos](http://go.microsoft.com/fwlink/?linkid=21140)                                                                                                                                                                                                                                                                                                                         |
| **A biztonsági rés hatása**                    | Tartalomhamisítás                                                                                                                                                                                                                                                                                                                                                              |
| **A szoftver észlelésével kapcsolatos adatok** | A Microsoft Baseline Security Analyzer képes észlelni, szükséges-e a számítógépen az adott frissítést. Ez a frissítés újraindítást igényel.                                                                                                                                                                                                                                    |
| **Érintett szoftverek**                        | **Microsoft Windows.** További információt az Érintett szoftverek és letöltési helyek című rész tartalmaz.                                                                                                                                                                                                                                                                     |

| Közlemény azonosítója                          | A Microsoft MS08-039 számú biztonsági közleménye                                                                                                                                                                                                                                                                                                                                                                                                                                      |
|------------------------------------------------|---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| **Közlemény címe**                             | [**Jogok kiterjesztését lehetővé tévő biztonsági rés az Outlook Web Access for Exchange Server szolgáltatásban (953747)**](http://go.microsoft.com/fwlink/?linkid=120820)                                                                                                                                                                                                                                                                                                             |
| **Összefoglalás**                              | Ez a biztonsági frissítés két közvetlenül jelentett biztonsági rést szüntet meg az Outlook Web Access (OWA) for Microsoft Exchange Server szolgáltatásban. Az ezeket a biztonsági réseket sikeresen kihasználó támadó hozzáférést szerezhet az egyéni OWA ügyfél munkameneti adataihoz, ami a jogosultság illetéktelen megszerzését teszi lehetővé. A támadó ezt követően végrehajthat minden olyan a műveletet, amit a felhasználó az egyéni ügyfél OWA munkamenetében végrehajthat. |
| **Súlyosság maximális foka**                   | [Fontos](http://go.microsoft.com/fwlink/?linkid=21140)                                                                                                                                                                                                                                                                                                                                                                                                                                |
| **A biztonsági rés hatása**                    | Jogok kiterjesztése                                                                                                                                                                                                                                                                                                                                                                                                                                                                   |
| **A szoftver észlelésével kapcsolatos adatok** | A Microsoft Baseline Security Analyzer képes észlelni, szükséges-e a számítógépen az adott frissítést. Előfordulhat, hogy a frissítés a rendszer újraindítását igényli.                                                                                                                                                                                                                                                                                                               |
| **Érintett szoftverek**                        | **Microsoft Windows.** További információt az Érintett szoftverek és letöltési helyek című rész tartalmaz.                                                                                                                                                                                                                                                                                                                                                                            |

Érintett szoftverek és letöltési helyek
---------------------------------------

<span></span>
**A táblázat használata**

A táblázat segítségével megtudhatja a szükséges információt a telepítendő biztonsági frissítésekről. Nézzen meg minden felsorolt szoftvert vagy összetevőt annak megállapításához, hogy van-e telepítendő biztonsági frissítés. Ha a szoftver vagy összetevő szerepel a listán, hiperhivatkozással kapcsolódik hozzá az elérhető szoftverfrissítés, és a frissítés besorolása is fel van tüntetve.

**Megjegyzés:** Előfordulhat, hogy egy biztonsági rés megszüntetéséhez több biztonsági frissítést kell telepíteni. Nézze át az egyes közleményazonosítókhoz tartozó teljes oszlopot, és ellenőrizze a telepítendő frissítéseket a rendszerre telepített programok vagy összetevők alapján.

#### Windows operációs rendszer:

 
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
Microsoft Windows 2000
</th>
</tr>
<tr>
<td style="border:1px solid black;">
**Közlemény azonosítója**
</td>
<td style="border:1px solid black;">
[**MS08-040**](http://go.microsoft.com/fwlink/?linkid=113725)
</td>
<td style="border:1px solid black;">
[**MS08-038**](http://go.microsoft.com/fwlink/?linkid=117296)
</td>
<td style="border:1px solid black;">
[**MS08-037**](http://go.microsoft.com/fwlink/?linkid=119620)
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
**Közlemény legmagasabb súlyossági besorolása**
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
Nem érintett
</td>
<td style="border:1px solid black;">
Nem érintett
</td>
<td style="border:1px solid black;">
DNS-ügyfélfrissítés:  
[Microsoft Windows 2000 Service Pack 4](http://www.microsoft.com/downloads/details.aspx?familyid=269c219c-9d6b-4b12-b621-c70cd07cdd22)  
(Fontos)  
DNS-kiszolgálófrissítés:  
[Microsoft Windows 2000 Server Service Pack 4](http://www.microsoft.com/downloads/details.aspx?familyid=332aa92f-a1ad-42a0-87d0-485d2d41335b)  
(Fontos)
</td>
</tr>
<tr>
<th colspan="4">
Windows XP
</th>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
**Közlemény azonosítója**
</td>
<td style="border:1px solid black;">
[**MS08-040**](http://go.microsoft.com/fwlink/?linkid=113725)
</td>
<td style="border:1px solid black;">
[**MS08-038**](http://go.microsoft.com/fwlink/?linkid=117296)
</td>
<td style="border:1px solid black;">
[**MS08-037**](http://go.microsoft.com/fwlink/?linkid=119620)
</td>
</tr>
<tr>
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
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
Windows XP Service Pack 2 és Windows XP Service Pack 3
</td>
<td style="border:1px solid black;">
Nem érintett
</td>
<td style="border:1px solid black;">
Nem érintett
</td>
<td style="border:1px solid black;">
DNS-ügyfélfrissítés:  
[Windows XP Service Pack 2 és Windows XP Service Pack 3](http://www.microsoft.com/downloads/details.aspx?familyid=ed989a33-7a9e-4423-93a8-b38907467cdf)  
(Fontos)  
Nincs alkalmazható DNS-kiszolgálófrissítés
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
Nem érintett
</td>
<td style="border:1px solid black;">
DNS-ügyfélfrissítés:  
[Windows XP Professional x64 Edition és Windows XP Professional x64 Edition Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=a2b016fa-b108-4e8e-b41b-4ca89002907b)  
(Fontos)  
Nincs alkalmazható DNS-kiszolgálófrissítés
</td>
</tr>
<tr>
<th colspan="4">
Windows Server 2003
</th>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
**Közlemény azonosítója**
</td>
<td style="border:1px solid black;">
[**MS08-040**](http://go.microsoft.com/fwlink/?linkid=113725)
</td>
<td style="border:1px solid black;">
[**MS08-038**](http://go.microsoft.com/fwlink/?linkid=117296)
</td>
<td style="border:1px solid black;">
[**MS08-037**](http://go.microsoft.com/fwlink/?linkid=119620)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
**Közlemény legmagasabb súlyossági besorolása**
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
[Microsoft SQL Server 2000 Desktop Engine (WMSDE)](http://www.microsoft.com/downloads/details.aspx?familyid=1c0ae18b-1f17-44b3-a337-b36e7de437a7)  
(KB948110)  
(Fontos)  
[Windows Internal Database (WYukon) Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=48f6aaa5-49fc-4a16-bc34-8514e214b8cf)  
(KB948109)  
(Fontos)
</td>
<td style="border:1px solid black;">
Nem érintett
</td>
<td style="border:1px solid black;">
DNS-ügyfélfrissítés:  
[Windows Server 2003 Service Pack 1 és Windows Server 2003 Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=4ef5033c-9843-4e0b-bfad-fcaf05d7dab9)  
(Fontos)  
DNS-kiszolgálófrissítés:  
[Windows Server 2003 Service Pack 1 és Windows Server 2003 Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=d1fcb794-e6a5-4c28-b3b3-9cd88f468a42)  
(Fontos)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Windows Server 2003 x64 Edition és Windows Server 2003 x64 Edition Service Pack 2 rendszerhez
</td>
<td style="border:1px solid black;">
[Microsoft SQL Server 2000 Desktop Engine (WMSDE)](http://www.microsoft.com/downloads/details.aspx?familyid=1c0ae18b-1f17-44b3-a337-b36e7de437a7)  
(KB948110)  
(Fontos)  
[Windows Internal Database (WYukon) x64 Edition Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=48f6aaa5-49fc-4a16-bc34-8514e214b8cf)  
(KB948109)  
(Fontos)
</td>
<td style="border:1px solid black;">
Nem érintett
</td>
<td style="border:1px solid black;">
DNS-ügyfélfrissítés:  
[Windows Server 2003 x64 Edition és Windows Server 2003 x64 Edition Service Pack 2 rendszerhez](http://www.microsoft.com/downloads/details.aspx?familyid=66624a1f-38bf-4af7-936d-3131474ffe1f)  
(Fontos)  
DNS-kiszolgálófrissítés:  
[Windows Server 2003 x64 Edition és Windows Server 2003 x64 Edition Service Pack 2 rendszerhez](http://www.microsoft.com/downloads/details.aspx?familyid=040a1ba8-21b0-439e-bf21-1acd1c43b162)  
(Fontos)
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
Nem érintett
</td>
<td style="border:1px solid black;">
DNS-ügyfélfrissítés:  
[Windows Server 2003 SP1 Itanium alapú rendszerekhez és Windows Server 2003 SP2 Itanium alapú rendszerekhez](http://www.microsoft.com/downloads/details.aspx?familyid=facc80da-61d6-49c5-872d-a1980b66ae3e)  
(Fontos)  
DNS-kiszolgálófrissítés:  
[Windows Server 2003 SP1 Itanium alapú rendszerekhez és Windows Server 2003 SP2 Itanium alapú rendszerekhez](http://www.microsoft.com/downloads/details.aspx?familyid=c63e3ee6-6055-4313-b0f1-fec7408886bb)  
(Fontos)
</td>
</tr>
<tr>
<th colspan="4">
Windows Vista
</th>
</tr>
<tr>
<td style="border:1px solid black;">
**Közlemény azonosítója**
</td>
<td style="border:1px solid black;">
[**MS08-040**](http://go.microsoft.com/fwlink/?linkid=113725)
</td>
<td style="border:1px solid black;">
[**MS08-038**](http://go.microsoft.com/fwlink/?linkid=117296)
</td>
<td style="border:1px solid black;">
[**MS08-037**](http://go.microsoft.com/fwlink/?linkid=119620)
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
**Közlemény legmagasabb súlyossági besorolása**
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
[Windows Vista és Windows Vista Service Pack 1](http://www.microsoft.com/downloads/details.aspx?familyid=06739ca6-7368-4acb-bb67-7e8146071a29)  
(Fontos)
</td>
<td style="border:1px solid black;">
Nincs alkalmazható DNS-ügyfélfrissítés  
Nincs alkalmazható DNS-kiszolgálófrissítés
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
[Windows Vista x64 Edition és Windows Vista x64 Edition Service Pack 1](http://www.microsoft.com/downloads/details.aspx?familyid=74ea0893-7c2f-4fad-ad27-588ad953b046)  
(Fontos)
</td>
<td style="border:1px solid black;">
Nincs alkalmazható DNS-ügyfélfrissítés  
Nincs alkalmazható DNS-kiszolgálófrissítés
</td>
</tr>
<tr>
<th colspan="4">
Windows Server 2008
</th>
</tr>
<tr>
<td style="border:1px solid black;">
**Közlemény azonosítója**
</td>
<td style="border:1px solid black;">
[**MS08-040**](http://go.microsoft.com/fwlink/?linkid=113725)
</td>
<td style="border:1px solid black;">
[**MS08-038**](http://go.microsoft.com/fwlink/?linkid=117296)
</td>
<td style="border:1px solid black;">
[**MS08-037**](http://go.microsoft.com/fwlink/?linkid=119620)
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
**Közlemény legmagasabb súlyossági besorolása**
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
[Windows Internal Database (WYukon) Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=48f6aaa5-49fc-4a16-bc34-8514e214b8cf)\*  
(KB948109)  
(Fontos)
</td>
<td style="border:1px solid black;">
[Windows Server 2008 32 bites rendszerekhez](http://www.microsoft.com/downloads/details.aspx?familyid=189a4170-b495-4904-9cbd-209e7494d303)\*  
(Fontos)
</td>
<td style="border:1px solid black;">
Nincs alkalmazható DNS-ügyfélfrissítés  
DNS-kiszolgálófrissítés:  
[Windows Server 2008 32 bites rendszerekhez](http://www.microsoft.com/downloads/details.aspx?familyid=1fcea8f4-b233-42e1-b913-c4fcae276c7b)\*  
(Fontos)
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
Windows Server 2008 x64 alapú rendszerekhez
</td>
<td style="border:1px solid black;">
[Windows Internal Database (WYukon) x64 Edition Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=48f6aaa5-49fc-4a16-bc34-8514e214b8cf)\*  
(KB948109)  
(Fontos)
</td>
<td style="border:1px solid black;">
[Windows Server 2008 x64 alapú rendszerekhez](http://www.microsoft.com/downloads/details.aspx?familyid=85d8701d-f8c7-4079-8a21-a3a9d5ba71ce)\*  
(Fontos)
</td>
<td style="border:1px solid black;">
Nincs alkalmazható DNS-ügyfélfrissítés  
DNS-kiszolgálófrissítés:  
[Windows Server 2008 x64 alapú rendszerekhez](http://www.microsoft.com/downloads/details.aspx?familyid=afac5bbc-71fa-457b-8b0a-f5902d37bfd0)\*  
(Fontos)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Windows Server 2008 Itanium alapú rendszerekhez
</td>
<td style="border:1px solid black;">
Nem érintett
</td>
<td style="border:1px solid black;">
[Windows Server 2008 Itanium alapú rendszerekhez](http://www.microsoft.com/downloads/details.aspx?familyid=b30ee4f0-850f-4ff3-86a4-663603a0a802)  
(Fontos)
</td>
<td style="border:1px solid black;">
Nincs alkalmazható DNS-ügyfélfrissítés  
Nincs alkalmazható DNS-kiszolgálófrissítés
</td>
</tr>
</table>
 
**\*Érinti a Windows Server 2008 kiszolgálómag-telepítését.** A frissítés besorolása ugyanaz a Windows Server 2008 támogatott kiadásain függetlenül attól, hogy a Windows Server 2008 alkalmazást a kiszolgálómag-telepítési opcióval telepítették-e. További tudnivalókat ezzel a telepítési beállítással kapcsolatban a következő weboldalon talál:[Server Core](http://msdn.microsoft.com/en-us/library/ms723891(vs.85).aspx). A Server Core telepítési beállítás a Windows Server 2008 egyes kiadásainál nem alkalmazható. További tudnivalók: [Server Core telepítési beállítások összehasonlítása](http://www.microsoft.com/windowsserver2008/en/us/compare-core-installation.aspx).

#### Microsoft Server Software

 
<p> </p>
<table style="border:1px solid black;">
<caption>Microsoft SQL Server</caption>
<tbody>
<tr class="odd">
<td style="border:1px solid black;"><strong>Közlemény azonosítója</strong></td>
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=113725"><strong>MS08-040</strong></a></td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><strong>Közlemény legmagasabb súlyossági besorolása</strong></td>
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=21140"><strong>Fontos</strong></a></td>
</tr>
<tr class="odd">
<td style="border:1px solid black;">SQL Server 7.0 Service Pack 4</td>
<td style="border:1px solid black;">GDR-frissítés:<br />
<a href="http://www.microsoft.com/downloads/details.aspx?familyid=c95b2cb3-51a4-44e4-b9f4-9416e9ce16a0">SQL Server 7.0 Service Pack 4</a><br />
(KB948113)<br />
(Fontos)<br />
<br />
QFE-frissítés:<br />
<a href="http://www.microsoft.com/downloads/details.aspx?familyid=c95b2cb3-51a4-44e4-b9f4-9416e9ce16a0">SQL Server 7.0 Service Pack 4</a><br />
(KB948113)<br />
(Fontos)</td>
</tr>
<tr class="even">
<td style="border:1px solid black;">SQL Server 2000 Service Pack 4</td>
<td style="border:1px solid black;">GDR-frissítés:<br />
<a href="http://www.microsoft.com/downloads/details.aspx?familyid=4fd1f86a-94a2-43d8-9b0a-774c81426d9e">SQL Server 2000 Service Pack 4</a><br />
(KB948110)<br />
(Fontos)<br />
<br />
QFE-frissítés:<br />
<a href="http://www.microsoft.com/downloads/details.aspx?familyid=8316bc5e-8c2d-4710-8acc-b815ccc81cd4">SQL Server 2000 Service Pack 4</a><br />
(KB948111)<br />
(Fontos)</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;">SQL Server 2000 Itanium alapú kiadás, Service Pack 4</td>
<td style="border:1px solid black;">GDR-frissítés:<br />
<a href="http://www.microsoft.com/downloads/details.aspx?familyid=4fd1f86a-94a2-43d8-9b0a-774c81426d9e">SQL Server 2000 Itanium alapú kiadás, Service Pack 4</a><br />
(KB948110)<br />
(Fontos)<br />
<br />
QFE-frissítés:<br />
<a href="http://www.microsoft.com/downloads/details.aspx?familyid=8316bc5e-8c2d-4710-8acc-b815ccc81cd4">SQL Server 2000 Itanium alapú kiadás, Service Pack 4</a><br />
(KB948111)<br />
(Fontos)</td>
</tr>
<tr class="even">
<td style="border:1px solid black;">SQL Server 2005 Service Pack 2</td>
<td style="border:1px solid black;">GDR-frissítés:<br />
<a href="http://www.microsoft.com/downloads/details.aspx?familyid=4c9851cc-2c4c-4190-872c-84993a7623b7">SQL Server 2005 Service Pack 2</a><br />
(KB948109)<br />
(Fontos)<br />
<br />
QFE-frissítés:<br />
<a href="http://www.microsoft.com/downloads/details.aspx?familyid=a60bb7e7-ef4e-4cbd-b63a-0ad7bd1402b3">SQL Server 2005 Service Pack 2</a><br />
(KB948108)<br />
(Fontos)</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;">SQL Server 2005 x64 Edition Service Pack 2</td>
<td style="border:1px solid black;">GDR-frissítés:<br />
<a href="http://www.microsoft.com/downloads/details.aspx?familyid=4c9851cc-2c4c-4190-872c-84993a7623b7">SQL Server 2005 x64 Edition Service Pack 2</a><br />
(KB948109)<br />
(Fontos)<br />
<br />
QFE-frissítés:<br />
<a href="http://www.microsoft.com/downloads/details.aspx?familyid=a60bb7e7-ef4e-4cbd-b63a-0ad7bd1402b3">SQL Server 2005 x64 Edition Service Pack 2</a><br />
(KB948108)<br />
(Fontos)</td>
</tr>
<tr class="even">
<td style="border:1px solid black;">SQL Server 2005 SP2 Itanium alapú rendszerekhez</td>
<td style="border:1px solid black;">GDR-frissítés:<br />
<a href="http://www.microsoft.com/downloads/details.aspx?familyid=4c9851cc-2c4c-4190-872c-84993a7623b7">SQL Server 2005 SP2 Itanium alapú rendszerekhez</a><br />
(KB948109)<br />
(Fontos)<br />
<br />
QFE-frissítés:<br />
<a href="http://www.microsoft.com/downloads/details.aspx?familyid=a60bb7e7-ef4e-4cbd-b63a-0ad7bd1402b3">SQL Server 2005 SP2 Itanium alapú rendszerekhez</a><br />
(KB948108)<br />
(Fontos)</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;">Microsoft Data Engine (MSDE) 1.0 Service Pack 4</td>
<td style="border:1px solid black;">GDR-frissítés:<br />
<a href="http://www.microsoft.com/downloads/details.aspx?familyid=c95b2cb3-51a4-44e4-b9f4-9416e9ce16a0">Microsoft Data Engine (MSDE) 1.0 Service Pack 4</a><br />
(KB948113)<br />
(Fontos)<br />
<br />
QFE-frissítés:<br />
<a href="http://www.microsoft.com/downloads/details.aspx?familyid=c95b2cb3-51a4-44e4-b9f4-9416e9ce16a0">Microsoft Data Engine (MSDE) 1.0 Service Pack 4</a><br />
(KB948113)<br />
(Fontos)</td>
</tr>
<tr class="even">
<td style="border:1px solid black;">Microsoft SQL Server 2000 Desktop Engine (MSDE 2000) Service Pack 4</td>
<td style="border:1px solid black;">GDR-frissítés:<br />
<a href="http://www.microsoft.com/downloads/details.aspx?familyid=4fd1f86a-94a2-43d8-9b0a-774c81426d9e">Microsoft SQL Server 2000 Desktop Engine (MSDE 2000) Service Pack 4</a><br />
(KB948110)<br />
(Fontos)<br />
<br />
QFE-frissítés:<br />
<a href="http://www.microsoft.com/downloads/details.aspx?familyid=8316bc5e-8c2d-4710-8acc-b815ccc81cd4">Microsoft SQL Server 2000 Desktop Engine (MSDE 2000) Service Pack 4</a><br />
(KB948111)<br />
(Fontos)</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;">Microsoft SQL Server 2005 Express Edition Service Pack 2</td>
<td style="border:1px solid black;">GDR-frissítés:<br />
<a href="http://www.microsoft.com/downloads/details.aspx?familyid=4c9851cc-2c4c-4190-872c-84993a7623b7">Microsoft SQL Server 2005 Express Edition Service Pack 2</a><br />
(KB948109)<br />
(Fontos)<br />
<br />
QFE-frissítés:<br />
<a href="http://www.microsoft.com/downloads/details.aspx?familyid=a60bb7e7-ef4e-4cbd-b63a-0ad7bd1402b3">Microsoft SQL Server 2005 Express Edition Service Pack 2</a><br />
(KB948108)<br />
(Fontos)</td>
</tr>
<tr class="even">
<td style="border:1px solid black;">Microsoft SQL Server 2005 Express Edition alkalmazás Advanced Services Service Pack 2 szervizcsomaggal</td>
<td style="border:1px solid black;">GDR-frissítés:<br />
<a href="http://www.microsoft.com/downloads/details.aspx?familyid=4c9851cc-2c4c-4190-872c-84993a7623b7">Microsoft SQL Server 2005 Express Edition alkalmazás Advanced Services Service Pack 2 szervizcsomaggal</a><br />
(KB948109)<br />
(Fontos)<br />
<br />
QFE-frissítés:<br />
<a href="http://www.microsoft.com/downloads/details.aspx?familyid=a60bb7e7-ef4e-4cbd-b63a-0ad7bd1402b3">Microsoft SQL Server 2005 Express Edition alkalmazás Advanced Services Service Pack 2 szervizcsomaggal</a><br />
(KB948108)<br />
(Fontos)</td>
</tr>
</tbody>
</table>
 

 
<p> </p>
<table style="border:1px solid black;">
<caption>Microsoft Exchange Server</caption>
<tbody>
<tr class="odd">
<td style="border:1px solid black;"><strong>Közlemény azonosítója</strong></td>
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=120820"><strong>MS08-039</strong></a></td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><strong>Közlemény legmagasabb súlyossági besorolása</strong></td>
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=21140"><strong>Fontos</strong></a></td>
</tr>
<tr class="odd">
<td style="border:1px solid black;">Microsoft Exchange Server 2003 Service Pack 2</td>
<td style="border:1px solid black;"><a href="http://www.microsoft.com/downloads/details.aspx?familyid=e099c1d1-5af6-4d6c-b735-9599412b3131">Microsoft Exchange Server 2003 Service Pack 2</a><br />
(Fontos)</td>
</tr>
<tr class="even">
<td style="border:1px solid black;">Microsoft Exchange Server 2007</td>
<td style="border:1px solid black;"><a href="http://www.microsoft.com/downloads/details.aspx?familyid=086a2a13-a1de-4b1d-bd12-b148bfd2dafa">Microsoft Exchange Server 2007</a><br />
(Fontos)</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;">Microsoft Exchange Server 2007 Service Pack 1</td>
<td style="border:1px solid black;"><a href="http://www.microsoft.com/downloads/details.aspx?familyid=63e7f26c-92a8-4264-882d-f96b348c96ab">Microsoft Exchange Server 2007 Service Pack 1</a><br />
(Fontos)</td>
</tr>
</tbody>
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

A Microsoft Systems Management Server (SMS) rendszer egy sokoldalúan beállítható vállalati megoldás, amely a frissítések kezelésére szolgál. Az SMS segítségével a rendszergazda megállapíthatja, hogy melyik Windows alapú számítógép szorul biztonsági frissítésre, és ezeket a frissítéseket szabályozott módon, a felhasználók minimális zavarásával központilag telepítheti a vállalat teljes informatikai környezetében. Az SMS, vagyis a System Center Configuration Manager 2007 újabb kiadása immáron elérhető, lásd még: [System Center Configuration Manager 2007](http://technet.microsoft.com/en-us/library/bb735860.aspx). Arról, hogy a rendszergazdák hogyan használhatják a biztonsági frissítések telepítéséhez az SMS 2003 alkalmazást, az [SMS 2003 Security Patch Management](http://go.microsoft.com/fwlink/?linkid=22939) részben olvashat. Az SMS 2.0 verzióját használók a [Software Updates Services Feature Pack](http://go.microsoft.com/fwlink/?linkid=33340) szolgáltatásait is segítségül hívhatják a biztonsági frissítések központi telepítéséhez. Az SMS-szolgáltatásról bővebben a [Microsoft Systems Management Server](http://go.microsoft.com/fwlink/?linkid=21158) oldalán olvashat.

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

-   Dan Kaminsky, [IOActive](http://www.ioactive.com/), az MS08-037 közleményben ismertetett probléma jelentéséért.
-   Michael Jordan, [Context Information Security](http://www.contextis.co.uk/), az MS08-039 közleményben ismertetett probléma jelentéséért.
-   Névtelen megtaláló, az MS08-040 közleményben leírt probléma jelentéséért
-   Névtelen megtaláló, az MS08-040 közleményben leírt probléma jelentéséért
-   Brett Moore, [Insomnia Security](http://www.insomniasec.com/), [iDefense VCP](http://labs.idefense.com/), az MS08-040 közleményben ismertetett probléma jelentéséért.
-   Névtelen megtaláló, az MS08-040 közleményben leírt probléma jelentéséért

#### Terméktámogatás

-   Teszteléssel állapították meg a felsorolt szoftverek egyes verzióinak érintettségét. A többi verzió támogatási életciklusa végére ért. Az egyes szoftververziók támogatási életciklusáról a [Microsoft termékek terméktámogatási életciklusát ismertető webhelyen](http://go.microsoft.com/fwlink/?linkid=21742) talál felvilágosítást.
-   Az Amerikai Egyesült Államokban és Kanadában technikai segítség igényelhető a [Microsoft terméktámogatási szolgáltatásától](http://go.microsoft.com/fwlink/?linkid=21131), amelynek telefonszáma 1-866-PCSAFETY. A biztonsági frissítésekkel kapcsolatos hívások ingyenesek.
-   Más országokban a helyi Microsoft-képviseletek nyújtanak támogatást. A biztonsági frissítésekkel kapcsolatos hívások ingyenesek. A [nemzetközi támogatási webhely](http://go.microsoft.com/fwlink/?linkid=21155) felvilágosítást nyújt arról, támogatási kérdéseivel hogyan fordulhat a Microsofthoz.

#### Felelősséget kizáró nyilatkozat

A Microsoft Tudásbázisban leírtak előzetes bejelentés nélkül változhatnak, és a cikkek tartalmáért a Microsoft nem vállal garanciát. A Microsoft egyben elhárít minden kifejezett és értelemszerű garanciát, beleértve az eladhatóságra és az adott célra való alkalmasságra vonatkozó garanciát is. A Microsoft Corporation vagy annak szállítói semmilyen körülmények között nem tehetők felelőssé közvetlen, közvetett, eseti, ok-okozati vagy különleges kárért (beleértve az elmaradt hasznot is), még akkor sem, ha a Microsoft Corporation vagy szállítói tudatában voltak a kár lehetséges voltának. Egyes államok törvényi szabályozása nem teszi lehetővé a véletlen vagy ok-okozati károkért vállalt felelősség korlátozását vagy kizárását, így ezekben az államokban az ez a felelősségkizárás nincs érvényben.

#### Verziók

-   1.0 verzió (2008. július 8.): Összefoglaló közlemény közzététele.
-   1.1 verzió (2009. február 11.): A Microsoft Windows 2000 Service Pack 4 rendszeren futó Microsoft SQL Server 2000 Desktop Engine (WMSDE) alkalmazásra utaló hibás utalás kikerült a Windows operációs rendszerre vonatkozó Érintett szoftverek és letöltési helyek táblázatból az MS08-040 közleményben.

*Built at 2014-04-18T01:50:00Z-07:00*
