---
TOCTitle: Az RMS felügyeleti szolgáltatása
Title: Az RMS felügyeleti szolgáltatása
ms:assetid: '4bd3e142-f0f6-40e9-a160-deab28ce5b88'
ms:contentKeyID: 18122571
ms:mtpsurl: 'https://technet.microsoft.com/hu-hu/library/Cc747560(v=WS.10)'
---

Az RMS felügyeleti szolgáltatása
================================

A felügyeleti szolgáltatás az RMS legfelső szintű fürtjén, illetve bármelyik csak licencelő fürtön fut. A felügyeleti szolgáltatás működteti a felügyeleti webhelyet, módot adva ezzel az RMS kezelésére.

A felügyeleti szolgáltatás alkalmazásfájlja, a Default.aspx, az *RMS\_webhely*\\\_wmcs\\Admin virtuális könyvtárban található. Itt az *RMS\_webhely* annak a webhelynek a neve, amelyen az RMS létesítése történt.

A szolgáltatás alapértelmezett hozzáférési szabálygyűjteményét a következő táblázat szemlélteti:

###  

<p> </p>
<table style="border:1px solid black;">
<colgroup>
<col width="50%" />
<col width="50%" />
</colgroup>
<thead>
<tr class="header">
<th>Felhasználó vagy Csoport</th>
<th>Alapértelmezett engedély</th>
</tr>
</thead>
<tbody>
<tr class="odd">
<td style="border:1px solid black;"><p>Rendszergazdák</p></td>
<td style="border:1px solid black;"><p>Teljes hozzáférés</p></td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><p>RMS szolgáltatáscsoport</p></td>
<td style="border:1px solid black;"><p>Olvasás és végrehajtás</p></td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><p>RENDSZER</p></td>
<td style="border:1px solid black;"><p>Teljes hozzáférés</p></td>
</tr>
</tbody>
</table>
