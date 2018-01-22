---
TOCTitle: 'MS06-JAN'
Title: 'Microsoft biztonsági közlemény - összefoglalás, január 2006'
ms:assetid: 'ms06-jan'
ms:contentKeyID: 61227696
ms:mtpsurl: 'https://technet.microsoft.com/hu-HU/library/ms06-jan(v=Security.10)'
---

Security Bulletin Summary

Microsoft biztonsági közlemény - összefoglalás, január 2006
===========================================================

Közzétéve: 2006. január 5. | Frissítve: 2006. január 10.

**Verzió:** 1.0

Az információk végfelhasználók számára készült összefoglalója [ezen a webhelyen](http://www.microsoft.com/security/default.mspx) található.

**A számítógép védelme:** A Microsoft az alábbi helyeken tette közzé a számítógép védelmével kapcsolatos ajánlásait:

-   Végfelhasználók keressék fel [A számítógép védelme webhelyet](http://go.microsoft.com/fwlink/?linkid=21169).
-   Informatikai szakemberek látogassanak el a [Security Guidance Center](http://go.microsoft.com/fwlink/?linkid=21171) webhelyre.

**Frissítésekkel kapcsolatos stratégiák:** A [biztonsági javítások kezelésével, a biztonsági frissítésekkel és a letöltésekkel foglalkozó webhely](http://go.microsoft.com/fwlink/?linkid=21168) további információt nyújt a Microsoft biztonsági frissítések alkalmazásával kapcsolatos gyakorlati tanácsairól.

**IT Pro Security Zone közösség:** Az [IT Pro Security Zone webhelyen](http://go.microsoft.com/fwlink/?linkid=21164) hasznos információt találhat a biztonság fokozásáról és az informatikai infrastruktúrák optimalizálásáról, továbbá eszmecserét folytathat a biztonsági kérdésekről más informatikai szakemberekkel.

**Microsoft Security Notification Service:** Ha értesítést szeretne kapni a Microsoft Security Bulletin cikkeinek megjelenéséről, fizessen elő a Microsoft Security Notification Service szolgáltatásra a [Microsoft Security Notification Service](http://go.microsoft.com/fwlink/?linkid=21163) webhelyen.

#### Összefoglalás

Ez a dokumentum ismerteti a nemrégiben felfedezett biztonsági résekhez kiadott frissítéseket. A biztonsági rések (súlyosság szerint) az alábbiak.

Kritikus (3)
------------

<span></span>
| Közlemény azonosítója         | Microsoft biztonsági közlemény MS06-001                                                                                                   |
|-------------------------------|-------------------------------------------------------------------------------------------------------------------------------------------|
| **Közlemény címe**            | [**A képmegjelenítő rendszer biztonsági rése távoli kódfuttatást tehet lehetővé (912919)**](http://go.microsoft.com/fwlink/?linkid=58471) |
| **Összefoglalás**             | Biztonsági rés található a képmegjelenítő rendszerben, amely a lehetővé teheti programkód távoli futtatását.                              |
| **Súlyosság maximális foka:** | [Kritikus](http://go.microsoft.com/fwlink/?linkid=21140)                                                                                  |
| **A biztonsági rés hatása:**  | Távoli kódfuttatás                                                                                                                        |
| **Érintett szoftverek**       | **Windows.** További információt az Érintett szoftverek és letöltési helyek című rész tartalmaz.                                          |

| Közlemény azonosítója         | Microsoft biztonsági közlemény MS06-002                                                                                                     |
|-------------------------------|---------------------------------------------------------------------------------------------------------------------------------------------|
| **Közlemény címe**            | [**A beágyazott webes betűtípus biztonsági rése távoli kódfuttatást tesz lehetővé (908519)**](http://go.microsoft.com/fwlink/?linkid=55919) |
| **Összefoglalás**             | A biztonsági rést a beágyazott webes betűtípusok megtekintése okozza, amely távoli kódfuttatást eredményezhet.                              |
| **Súlyosság maximális foka:** | [Kritikus](http://go.microsoft.com/fwlink/?linkid=21140)                                                                                    |
| **A biztonsági rés hatása:**  | Távoli kódfuttatás                                                                                                                          |
| **Érintett szoftverek**       | **Windows.** További információt az Érintett szoftverek és letöltési helyek című rész tartalmaz.                                            |

| Közlemény azonosítója         | Microsoft biztonsági közlemény MS06-003                                                                                                                                                 |
|-------------------------------|-----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| **Közlemény címe**            | [**A Microsoft Outlook és a Microsoft Exchange TNEF-dekódolásának biztonsági rése programkód távoli futtatását teszi lehetővé (902412)**](http://go.microsoft.com/fwlink/?linkid=44168) |
| **Összefoglalás**             | A TNEF-üzenetek biztonsági rés programkód távoli futtatását teheti lehetővé.                                                                                                            |
| **Súlyosság maximális foka:** | [Kritikus](http://go.microsoft.com/fwlink/?linkid=21140)                                                                                                                                |
| **A biztonsági rés hatása:**  | Távoli kódfuttatás                                                                                                                                                                      |
| **Érintett szoftverek**       | **Exchange és Office.** További információt az Érintett szoftverek és letöltési helyek című rész tartalmaz.                                                                             |

Érintett szoftverek és letöltési helyek
---------------------------------------

<span></span>
**A táblázat használata**

A táblázat segítségével megtudhatja a szükséges információt a telepítendő biztonsági frissítésekről. Nézzen meg minden felsorolt szoftvert vagy összetevőt annak megállapításához, hogy van-e telepítendő biztonsági frissítés. Ha egy szoftver vagy összetevő szerepel a felsorolásban, akkor a biztonsági rés hatását is tartalmazza a táblázat az elérhető szoftverfrissítésre mutató hivatkozással együtt.

A táblázatban a zárójelben lévő szám \[x\] azt jelzi, hogy a problémához magyarázó megjegyzés tartozik. Ezek a megjegyzések a táblázat alatt találhatók.

**Megjegyzés:** Előfordulhat, hogy egy biztonsági rés megszüntetéséhez több biztonsági frissítést kell telepíteni. Nézze át az egyes közleményazonosítókhoz tartozó teljes oszlopot, és ellenőrizze a telepítendő frissítéseket a rendszerre telepített programok vagy összetevők alapján.

**Érintett szoftverek és letöltési helyek**

 
<p> </p>
<table style="border:1px solid black;">
<colgroup>
<col width="25%" />
<col width="25%" />
<col width="25%" />
<col width="25%" />
</colgroup>
<thead>
<tr class="header">
<th style="border:1px solid black;" ></th>
<th style="border:1px solid black;" >Részletek        </th>
<th style="border:1px solid black;" >Részletek        </th>
<th style="border:1px solid black;" >Részletek        </th>
</tr>
</thead>
<tbody>
<tr class="odd">
<td style="border:1px solid black;"><strong>Közlemény azonosítója</strong></td>
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=58471"><strong>MS06-001</strong></a></td>
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=55919"><strong>MS06-002</strong></a></td>
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=44168"><strong>MS06-003</strong></a></td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><strong>Súlyosság maximális foka:</strong></td>
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=21140"><strong>Kritikus</strong></a></td>
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=21140"><strong>Kritikus</strong></a></td>
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=21140"><strong>Kritikus</strong></a></td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><strong>Érintett Windows-szoftverek:</strong></td>
<td style="border:1px solid black;"></td>
<td style="border:1px solid black;"></td>
<td style="border:1px solid black;"></td>
</tr>
<tr class="even">
<td style="border:1px solid black;">Windows Server 2003</td>
<td style="border:1px solid black;"><a href="http://www.microsoft.com/downloads/details.aspx?familyid=1584aae0-51ce-47d6-9a03-db5b9077f1f2">Kritikus</a></td>
<td style="border:1px solid black;"><a href="http://www.microsoft.com/downloads/details.aspx?familyid=5fc12654-486f-45bf-8d34-bdf0998869c5">Fontos</a></td>
<td style="border:1px solid black;"></td>
</tr>
<tr class="odd">
<td style="border:1px solid black;">Windows Server 2003 Service Pack 1</td>
<td style="border:1px solid black;"><a href="http://www.microsoft.com/downloads/details.aspx?familyid=1584aae0-51ce-47d6-9a03-db5b9077f1f2">Kritikus</a></td>
<td style="border:1px solid black;"><a href="http://www.microsoft.com/downloads/details.aspx?familyid=5fc12654-486f-45bf-8d34-bdf0998869c5">Fontos</a></td>
<td style="border:1px solid black;"></td>
</tr>
<tr class="even">
<td style="border:1px solid black;">Windows Server 2003 x64 Edition</td>
<td style="border:1px solid black;"><a href="http://www.microsoft.com/downloads/details.aspx?familyid=a8f4dcba-5d28-4d9d-a6a4-3b71108cfe2d">Kritikus</a></td>
<td style="border:1px solid black;"><a href="http://www.microsoft.com/downloads/details.aspx?familyid=80b05c56-5bce-4262-8142-af0d8a7bc388">Fontos</a></td>
<td style="border:1px solid black;"></td>
</tr>
<tr class="odd">
<td style="border:1px solid black;">Windows Server 2003 Itanium alapú rendszerekhez</td>
<td style="border:1px solid black;"><a href="http://www.microsoft.com/downloads/details.aspx?familyid=6e372d41-2c16-415e-8306-a5ca8845cc09">Kritikus</a></td>
<td style="border:1px solid black;"><a href="http://www.microsoft.com/downloads/details.aspx?familyid=e39d2e29-8934-4aa1-844d-11efa57d9cc5">Fontos</a></td>
<td style="border:1px solid black;"></td>
</tr>
<tr class="even">
<td style="border:1px solid black;">Windows Server 2003 SP1 csomaggal felszerelt Itanium-alapú rendszerekhez</td>
<td style="border:1px solid black;"><a href="http://www.microsoft.com/downloads/details.aspx?familyid=6e372d41-2c16-415e-8306-a5ca8845cc09">Kritikus</a></td>
<td style="border:1px solid black;"><a href="http://www.microsoft.com/downloads/details.aspx?familyid=e39d2e29-8934-4aa1-844d-11efa57d9cc5">Fontos</a></td>
<td style="border:1px solid black;"></td>
</tr>
<tr class="odd">
<td style="border:1px solid black;">Windows XP Service Pack 1</td>
<td style="border:1px solid black;"><a href="http://www.microsoft.com/downloads/details.aspx?familyid=0c1b4c96-57ae-499e-b89b-215b7bb4d8e9">Kritikus</a></td>
<td style="border:1px solid black;"><a href="http://www.microsoft.com/downloads/details.aspx?familyid=6daea2af-3723-4cdf-b5bd-b21ac75b5243">Kritikus</a></td>
<td style="border:1px solid black;"></td>
</tr>
<tr class="even">
<td style="border:1px solid black;">Windows XP Service Pack 2</td>
<td style="border:1px solid black;"><a href="http://www.microsoft.com/downloads/details.aspx?familyid=0c1b4c96-57ae-499e-b89b-215b7bb4d8e9">Kritikus</a></td>
<td style="border:1px solid black;"><a href="http://www.microsoft.com/downloads/details.aspx?familyid=6daea2af-3723-4cdf-b5bd-b21ac75b5243">Kritikus</a></td>
<td style="border:1px solid black;"></td>
</tr>
<tr class="odd">
<td style="border:1px solid black;">Windows XP Professional x64 Edition</td>
<td style="border:1px solid black;"><a href="http://www.microsoft.com/downloads/details.aspx?familyid=3a1166e6-5e9e-4e73-bcd4-28eca6ece877">Kritikus</a></td>
<td style="border:1px solid black;"><a href="http://www.microsoft.com/downloads/details.aspx?familyid=1990b2cf-ae88-4849-aeab-3f833969e197">Kritikus</a></td>
<td style="border:1px solid black;"></td>
</tr>
<tr class="even">
<td style="border:1px solid black;">Windows 2000 Service Pack 4</td>
<td style="border:1px solid black;"><a href="http://www.microsoft.com/downloads/details.aspx?familyid=aa9e27bd-cb9a-4ef1-92a3-00ffe7b2ac74">Kritikus</a></td>
<td style="border:1px solid black;"><a href="http://www.microsoft.com/downloads/details.aspx?familyid=dc6c2fe8-3c81-4661-994b-4146775bf590">Kritikus</a></td>
<td style="border:1px solid black;"></td>
</tr>
<tr class="odd">
<td style="border:1px solid black;">Windows Millennium Edition (Me)</td>
<td style="border:1px solid black;"></td>
<td style="border:1px solid black;"><strong>[1]</strong></td>
<td style="border:1px solid black;"></td>
</tr>
<tr class="even">
<td style="border:1px solid black;">Windows 98 Second Edition (SE)</td>
<td style="border:1px solid black;"></td>
<td style="border:1px solid black;"><strong>[1]</strong></td>
<td style="border:1px solid black;"></td>
</tr>
<tr class="odd">
<td style="border:1px solid black;">Windows 98</td>
<td style="border:1px solid black;"></td>
<td style="border:1px solid black;"><strong>[1]</strong></td>
<td style="border:1px solid black;"></td>
</tr>
<tr class="even">
<td style="border:1px solid black;"></td>
<td style="border:1px solid black;"></td>
<td style="border:1px solid black;"></td>
<td style="border:1px solid black;"></td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><strong>Érintett Office-szoftverek:</strong></td>
<td style="border:1px solid black;"></td>
<td style="border:1px solid black;"></td>
<td style="border:1px solid black;"></td>
</tr>
<tr class="even">
<td style="border:1px solid black;">Office Outlook 2000</td>
<td style="border:1px solid black;"></td>
<td style="border:1px solid black;"></td>
<td style="border:1px solid black;"><a href="http://www.microsoft.com/downloads/details.aspx?familyid=64d0336d-f962-4ab1-a724-9f6ba2108cb9">Kritikus</a></td>
</tr>
<tr class="odd">
<td style="border:1px solid black;">Office Outlook 2002</td>
<td style="border:1px solid black;"></td>
<td style="border:1px solid black;"></td>
<td style="border:1px solid black;"><a href="http://www.microsoft.com/downloads/details.aspx?familyid=9a85cebb-0d9a-465d-a4bc-af501562772d">Kritikus</a></td>
</tr>
<tr class="even">
<td style="border:1px solid black;">Office Outlook 2003</td>
<td style="border:1px solid black;"></td>
<td style="border:1px solid black;"></td>
<td style="border:1px solid black;"><a href="http://www.microsoft.com/downloads/details.aspx?familyid=1d156043-b041-4305-8442-3c4e3b832788">Kritikus</a></td>
</tr>
<tr class="odd">
<td style="border:1px solid black;">Office 2000 Multilanguage csomagok:</td>
<td style="border:1px solid black;"></td>
<td style="border:1px solid black;"></td>
<td style="border:1px solid black;"><a href="http://www.microsoft.com/downloads/details.aspx?familyid=2c0fa7c7-91aa-49b4-9731-9e83e3e0823d">Kritikus</a></td>
</tr>
<tr class="even">
<td style="border:1px solid black;">Office XP Multilingual User Interface csomagok</td>
<td style="border:1px solid black;"></td>
<td style="border:1px solid black;"></td>
<td style="border:1px solid black;"><a href="http://www.microsoft.com/downloads/details.aspx?familyid=cca9399a-6da3-4163-8398-c58dc328182b">Kritikus</a></td>
</tr>
<tr class="odd">
<td style="border:1px solid black;">Office 2003 Multilingual User Interface csomagok</td>
<td style="border:1px solid black;"></td>
<td style="border:1px solid black;"></td>
<td style="border:1px solid black;"><a href="http://www.microsoft.com/downloads/details.aspx?familyid=d69554ad-196f-4789-91e5-b2a753eed854">Kritikus</a></td>
</tr>
<tr class="even">
<td style="border:1px solid black;"></td>
<td style="border:1px solid black;"></td>
<td style="border:1px solid black;"></td>
<td style="border:1px solid black;"></td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><strong>Érintett Exchange szoftverek:</strong></td>
<td style="border:1px solid black;"></td>
<td style="border:1px solid black;"></td>
<td style="border:1px solid black;"></td>
</tr>
<tr class="even">
<td style="border:1px solid black;">Exchange 5.0</td>
<td style="border:1px solid black;"></td>
<td style="border:1px solid black;"></td>
<td style="border:1px solid black;"><a href="http://www.microsoft.com/downloads/details.aspx?familyid=0a8df1c3-abf9-4a21-9b49-81fa362b251f">Kritikus</a></td>
</tr>
<tr class="odd">
<td style="border:1px solid black;">Exchange 5.5</td>
<td style="border:1px solid black;"></td>
<td style="border:1px solid black;"></td>
<td style="border:1px solid black;"><a href="http://www.microsoft.com/downloads/details.aspx?familyid=ec6bd30e-12de-4ca1-9432-d2e73af62427">Kritikus</a></td>
</tr>
<tr class="even">
<td style="border:1px solid black;">Exchange 2000</td>
<td style="border:1px solid black;"></td>
<td style="border:1px solid black;"></td>
<td style="border:1px solid black;"><a href="http://www.microsoft.com/downloads/details.aspx?familyid=372ff07f-c3ca-4301-8559-9b90344edc02">Kritikus</a></td>
</tr>
</tbody>
</table>
  
**Megjegyzés**
  
<sup>[1]</sup> Ezekhez a rendszerekhez a biztonsági közlemény részeként közreadva kritikus biztonsági frissítések állnak rendelkezésre, amelyek a Windows Update webhelyről tölthetők le. 
  
Telepítés  
---------
  
<span></span>
**Software Update Services:**
  
A Microsoft Software Update Services (SUS) szolgáltatással a rendszergazdák gyorsan és megbízható módon telepíthetik központilag a legújabb fontos és biztonsági frissítéseket a Windows 2000 és a Windows Server 2003 rendszerű kiszolgálókra, valamint a Windows 2000 Professional vagy a Windows XP Professional rendszert futtató asztali rendszerekre.
  
A biztonsági frissítés Software Update Services szolgáltatással történő központi telepítéséről a [Software Update Services webhelyen](http://go.microsoft.com/fwlink/?linkid=21133) tudhat meg többet.
  
**Windows Server Update Services:**
  
A Microsoft Software Update Services (WSUS) szolgáltatással a rendszergazdák gyorsan és megbízható módon telepíthetik központilag a legújabb fontos és biztonsági frissítéseket Windows 2000 és újabb operációs rendszerekhez, Office XP és újabb operációs rendszerekhez, Exchange Server 2003 és SQL Server 2000 Windows 2000 és újabb operációs rendszerekre.
  
A biztonsági frissítésnek Windows Server Update Services szolgáltatással történő központi telepítéséről a [Windows Server Update Services](http://go.microsoft.com/fwlink/?linkid=50120) webhelyen tudhat meg többet.
  
**Systems Management Server:**
  
A Microsoft Systems Management Server (SMS) rendszer egy sokoldalúan beállítható vállalati megoldás, amely a frissítések kezelésére szolgál. Az SMS segítségével a rendszergazda megállapíthatja, hogy melyik Windows alapú számítógép szorul biztonsági frissítésre, és ezeket a frissítéseket szabályozott módon, a felhasználók minimális zavarásával központilag telepítheti a vállalat teljes informatikai környezetében. Ha többet szeretne tudni arról, hogy a rendszergazdák miként telepíthetik központilag a biztonsági frissítéseket az SMS 2003 alkalmazással, látogasson el az [SMS 2003 Security Patch Management webhelyre](http://go.microsoft.com/fwlink/?linkid=22939). Az SMS 2.0-s verzióját használók a [Software Updates Service Feature Pack](http://go.microsoft.com/fwlink/?linkid=33340) szolgáltatásait is segítségül hívhatják a biztonsági frissítések központi telepítéséhez. Az SMS rendszerről az [SMS webhelyén](http://go.microsoft.com/fwlink/?linkid=21158) talál további információt.
  
**Megjegyzés:** Az SMS a Microsoft Baseline Security Analyzer és a Microsoft Office Detection Tool program segítségével széles körű támogatást nyújt a biztonsági értesítők frissítéseinek észleléséhez és telepítéséhez. Előfordulhat, hogy egyes szoftverfrissítéseket ezek az eszközök nem észlelnek. Az SMS alkalmazás leltározási szolgáltatásai segítségével a rendszergazdák adott rendszereken hajthatják végre a frissítést. Az eljárásról további információt talál [ezen a webhelyen](http://go.microsoft.com/fwlink/?linkid=33341). Egyes biztonsági frissítésekhez rendszergazdai jogosultságokra van szükség a számítógép újraindítása után. A rendszergazdák az [SMS 2003 Administration Feature Pack](http://go.microsoft.com/fwlink/?linkid=33387) és az [SMS 2.0 Administration Feature Pack](http://go.microsoft.com/fwlink/?linkid=21161) csomag részét képező Elevated Rights Deployment Tool nevű eszközzel telepíthetik ezeket a frissítéseket.
  
**A QChain.exe és Update.exe fájlok használata:**
  
A Microsoft által kibocsátott QChain.exe nevű parancssori eszközzel a rendszergazda biztonságosan egybefűzheti a biztonsági frissítéseket. *Az egybefűzés* azt jelenti, hogy egymás után több frissítés is telepíthető a számítógép újraindítása nélkül. A jelen dokumentum frissítéseihez használt Update.exe beépített egybefűzési funkcióval rendelkezik. Windows 2000 Service Pack 2 vagy újabb, Windows XP vagy Windows Server 2003 operációs rendszer esetén a Qchain.exe programra nincs szükség a frissítések egybefűzéséhez. A Qchain.exe ennek ellenére támogatja e Windows rendszerek frissítéseinek egybefűzését, így a rendszergazda különböző operációs rendszerekhez egységes telepítési parancsfájlt készíthet. Ha többet szeretne tudni a QChain eszközről, látogasson el erre a [webhelyre](http://go.microsoft.com/fwlink/?linkid=21156).
  
**Microsoft Baseline Security Analyzer:**
  
A Microsoft Baseline Security Analyzer (MBSA) segítségével a rendszergazda mind a helyi, mind a távoli számítógépeken ellenőrizheti, hogy mely biztonsági frissítések hiányoznak, illetve hogy mely biztonsági beállítások vannak helytelenül megadva. Ha többet szeretne tudni az MBSA eszközről, látogasson el a [Microsoft Baseline Security Analyzer webhelyre](http://go.microsoft.com/fwlink/?linkid=21134).
  
**Útmutató az észleléshez és a telepítéshez:**
  
A Microsoft az e havi biztonsági frissítésekhez észlelési és telepítési útmutatót adott ki. Az útmutató a számítógépes szakembereknek is ötleteket adhat ahhoz, hogyan használják a különböző eszközöket, pl. Windows Update, Microsoft Update, Office Update, Microsoft Baseline Security Analyzer (MBSA), Office Detection Tool, Microsoft Systems Management Server (SMS), Extended Security Update Inventory Tool vagy Enterprise Update Scan Tool (EST) a biztonsági frissítések telepítéséhez. További információt a [Microsoft Tudásbázis 910723. számú cikkében](http://support.microsoft.com/kb/910723) talál.
  
#### Egyéb információ
  
**Köszönetnyilvánítás**
  
A Microsoft [köszönetét](http://go.microsoft.com/fwlink/?linkid=21127) fejezi ki a vásárlók védelmének biztosításában nyújtott segítségért az alábbi szervezet(ek)nek és szakember(ek)nek:
  
-   Dan Hubbard [(WebSense)](http://websense.com/) az [MS06-001](http://go.microsoft.com/fwlink/?linkid=58471) közleményben ismertetett probléma megoldásában nyújtott segítségéért.  
-   eEye Digital Security for reporting the issue described in [MS06-002](http://technet.microsoft.com/security/bulletin/ms06-002).  
-   John Heasman-nak és Mark Litchfield-nek a [NGS Software](http://www.ngssoftware.com/index.htm) a [MS06-003](http://technet.microsoft.com/security/bulletin/ms06-003) közleményben leírt probléma felfedezéséért
  
**Egyéb biztonsági frissítések beszerzése:**
  
Az alábbi helyekről más típusú biztonsági problémákhoz szerezhetők be frissítések.
  
-   A biztonsági frissítések a [Microsoft letöltőközpontban](http://go.microsoft.com/fwlink/?linkid=21129) érhetők el: legegyszerűbben a „biztonsági javítás” kifejezésre irányuló kulcsszavas kereséssel találhatja meg őket.  
-   A kereskedelmi forgalomban kapható operációs rendszerekhez a [Microsoft Update webhelyről](http://go.microsoft.com/fwlink/?linkid=40747) tölthetők le frissítések.
  
**Terméktámogatás:**
  
-   Az Amerikai Egyesült Államokban és Kanadában technikai segítség igényelhető a [Microsoft terméktámogatási szolgáltatásától](http://go.microsoft.com/fwlink/?linkid=21131), amelynek telefonszáma 1-866-PCSAFETY. A biztonsági frissítésekkel kapcsolatos hívások ingyenesek.  
-   Más országokban a helyi Microsoft képviseletek nyújtanak támogatást. A biztonsági frissítésekkel kapcsolatos hívások ingyenesek. A [nemzetközi támogatási webhely](http://go.microsoft.com/fwlink/?linkid=21155) felvilágosítást nyújt arról, támogatási kérdéseivel hogyan fordulhat a Microsofthoz.
  
**Egyéb adatvédelmi és biztonsági források:**
  
-   A [Microsoft TechNet Security](http://go.microsoft.com/fwlink/?linkid=21132) biztonsággal foglalkozó webhelye további információkat tartalmaz a Microsoft termékeinek biztonsági kérdéseiről.  
-   [Microsoft Software Update Services szoftverfrissítési szolgáltatás](http://go.microsoft.com/fwlink/?linkid=21133)  
-   [Microsoft Windows Server Update Services](http://go.microsoft.com/fwlink/?linkid=50120)  
-   [Microsoft Baseline Security Analyzer](http://go.microsoft.com/fwlink/?linkid=21134) (MBSA)  
-   [Windows Update](http://go.microsoft.com/fwlink/?linkid=21130)  
-   [Microsoft Update](http://update.microsoft.com/microsoftupdate)  
-   Windows Update katalógus: A Windows Update katalógusról a Microsoft Tudásbázis [323166](http://support.microsoft.com/default.aspx?scid=kb;en-us;323166) számú cikkében talál információkat.  
-   [Office Update](http://go.microsoft.com/fwlink/?linkid=21135)
  
**Felelősséget kizáró nyilatkozat:**
  
A Microsoft Tudásbázisban leírtak előzetes bejelentés nélkül változhatnak, és a cikkek tartalmáért a Microsoft nem vállal garanciát. A Microsoft egyben elhárít minden kifejezett és értelemszerű garanciát, beleértve az eladhatóságra és az adott célra való alkalmasságra vonatkozó garanciát is. A Microsoft Corporation vagy annak szállítói semmilyen körülmények között nem tehetők felelőssé közvetlen, közvetett, eseti, ok-okozati vagy különleges kárért (beleértve az elmaradt hasznot is), még akkor sem, ha a Microsoft Corporation vagy szállítói tudatában voltak a kár lehetséges voltának. Egyes államok törvényi szabályozása nem teszi lehetővé a véletlen vagy ok-okozati károkért vállalt felelősség korlátozását vagy kizárását, így ezekben az államokban az ez a felelősségkizárás nincs érvényben.
  
**Verziók:**
  
-   1.0 verzió (2006. január 5.): Kiadás dátuma  
-   2.0-s verzió (2006. január 10.): A frissítés további Microsoft biztonsági közleményeket tartalmaz
  
*Built at 2014-04-18T01:50:00Z-07:00*
