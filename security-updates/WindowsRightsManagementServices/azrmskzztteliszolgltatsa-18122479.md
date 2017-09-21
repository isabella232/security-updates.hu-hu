---
TOCTitle: Az RMS közzétételi szolgáltatása
Title: Az RMS közzétételi szolgáltatása
ms:assetid: '4c0c8fe3-695c-4b2c-a2d3-cab9b52bbb25'
ms:contentKeyID: 18122479
ms:mtpsurl: 'https://technet.microsoft.com/hu-hu/library/Cc720267(v=WS.10)'
---

Az RMS közzétételi szolgáltatása
================================

A közzétételi szolgáltatás, amely a közzétételi licenceket állítja ki, az RMS legfelső szintű fürtjén, illetve bármelyik csak licencelő fürtön fut. A közzétételi licencek azokat a szabályokat határozzák meg, amelyek szerint kiállíthatók a használati licencek.

A közzétételi szolgáltatás alkalmazásfájlja, a Publish.asmx, az IIS szolgáltatás Licensing virtuális könyvtárában található.

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
