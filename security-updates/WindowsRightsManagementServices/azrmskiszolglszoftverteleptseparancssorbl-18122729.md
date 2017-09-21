---
TOCTitle: Az RMS kiszolgálószoftver telepítése parancssorból
Title: Az RMS kiszolgálószoftver telepítése parancssorból
ms:assetid: 'b55b1e2a-dd14-4168-a37f-9cdedbec660b'
ms:contentKeyID: 18122729
ms:mtpsurl: 'https://technet.microsoft.com/hu-hu/library/Cc747733(v=WS.10)'
---

Az RMS kiszolgálószoftver telepítése parancssorból
==================================================

A Service Pack 2 szervizcsomaggal kiegészített RMS (RMS SP2) parancssorból is telepíthető, így a telepítés automatizálható. A telepítés automatizálása az alábbi két mód egyikén történhet: a letöltött EXE fájlban lévő ügyfélszoftver felügyelet nélküli telepítésével vagy a letöltött EXE fájlban lévő MSI fájlok kicsomagolása után az RMS ügyfélszoftver telepítésével. a letöltött EXE fájl használatával történő telepítéshez a következő parancsot kell végrehajtani:

**objShell.run "WindowsRightsManagementServicesSP2-KB917275-Client-ENU.exe -override 1 /I MsDrmClient.msi REBOOT=ReallySuppress /q -override 2 /I RmClientBackCompat.msi REBOOT=ReallySuppress /q"**

A Windows® Installer (.msi) fájlok telepítéséhez először ki kell csomagolni azokat az RMS SP2 letöltött EXE fájljából. Az msdrmclient.msi és az RmClientBackCompat.msi fájl kibontásához a következő parancsot kell végrehajtani a parancssorból:

**WindowsRightsManagementServiceSP2-KB917275-Server-ENU.exe /X:C:\\***telepítés\_helye*

Az .msi fájlok kibontása után a következő parancsot használhatja az RMS telepítéséhez:

**msiexec.exe /I MSDrmClient.msi /qn ALLUSERS=2 /m MSIDHOG /lei naplófájl.log DISPLYPAGE="NO" TARGETDIR=c:\\***telepítés\_helye*

**msiexec.exe /I RMClientBackCompat.msi /qn ALLUSERS=2 /m MSIDHOG /lei naplófájl.log DISPLYPAGE="NO" TARGETDIR=c:\\***telepítés\_helye*

A következő táblázat a parancsok szintaxisát ismerteti.

###  

<p> </p>
<table style="border:1px solid black;">
<colgroup>
<col width="50%" />
<col width="50%" />
</colgroup>
<thead>
<tr class="header">
<th>Paraméter</th>
<th>Meghatározás</th>
</tr>
</thead>
<tbody>
<tr class="odd">
<td style="border:1px solid black;"><p><strong>/I MSDrmClient.msi</strong> vagy <strong>/I RMClientBackCompat.msi</strong></p></td>
<td style="border:1px solid black;"><p>Kötelező. A telepítendő terméket adja meg.</p></td>
</tr>  
<tr class="even">
<td style="border:1px solid black;"><p><strong>/qn</strong></p></td>
<td style="border:1px solid black;"><p>Nem kötelező. Csendes, felhasználói közbeavatkozás nélküli telepítést ír elő.</p></td>
</tr>  
<tr class="odd">
<td style="border:1px solid black;"><p><strong>/lei</strong> <em>naplófájl.log</em></p></td>
<td style="border:1px solid black;"><p>Nem kötelező. A naplófájlt adja meg, amelybe a telepítő bejegyzi a hiba- és az állapotüzeneteket.</p></td>
</tr>  
<tr class="even">
<td style="border:1px solid black;"><p><strong>DISPLAYPAGE=&quot;NO&quot;</strong></p></td>
<td style="border:1px solid black;"><p>Nem kötelező. Azt adja meg, hogy a telepítés után ne jelenjen meg a <strong>Globális felügyelet</strong> oldal.</p></td>
</tr>  
<tr class="odd">
<td style="border:1px solid black;"><p><strong>TARGETDIR=c:\</strong><em>telepítés_helye</em></p></td>
<td style="border:1px solid black;"><p>Nem kötelező. A Service Pack 2 szervizcsomaggal kiegészített RMS (RMS SP2) telepítési helyét adja meg. Ha nincs megadva a hely, a program az alapértelmezett telepítési helyet használja.</p></td>
</tr>  
</tbody>  
</table>
  
| ![](images/Cc747733.note(WS.10).gif)Megjegyzés:                                                                                                                                                             |  
|------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|  
| Bármelyik telepítési módszer választásakor biztosítani kell mindkét .msi fájl sikeres telepítését. Ha olyan hiba fordul elő, amely megakadályozza az MSDrmClient.msi telepítését, az RMClientBackCompat.msi fájlt nem szabad telepíteni. |
