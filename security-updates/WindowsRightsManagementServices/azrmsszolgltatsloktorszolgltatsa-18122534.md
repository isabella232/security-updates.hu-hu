---
TOCTitle: Az RMS szolgáltatáslokátor szolgáltatása
Title: Az RMS szolgáltatáslokátor szolgáltatása
ms:assetid: '6f410cc9-5d5b-4df3-bf4f-7b13811eb52f'
ms:contentKeyID: 18122534
ms:mtpsurl: 'https://technet.microsoft.com/hu-hu/library/Cc747548(v=WS.10)'
---

Az RMS szolgáltatáslokátor szolgáltatása
========================================

A szolgáltatáslokátor szolgáltatás az RMS legfelső szintű fürtjén és a csak licencelő fürtökön fut. A szolgáltatáslokátor szolgáltatás teszi elérhetővé az Active Directory számára a fürt szolgáltatáskapcsolódási URL-címét, így azt az RMS-kompatibilis ügyfelek észlelni tudják.

A szolgáltatáslokátor szolgáltatás alkalmazásfájlja, a ServiceLocator.asmx, az IIS szolgáltatás Certification és Licensing virtuális könyvtárában található.

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
<tr class="even">
<td style="border:1px solid black;"><p>Felhasználók</p></td>
<td style="border:1px solid black;"><p>Olvasás és végrehajtás</p></td>
</tr>
</tbody>
</table>
