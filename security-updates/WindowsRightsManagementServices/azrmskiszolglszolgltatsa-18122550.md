---
TOCTitle: Az RMS kiszolgálószolgáltatása
Title: Az RMS kiszolgálószolgáltatása
ms:assetid: '772d0a89-c9fb-4430-9434-38cd5add1e86'
ms:contentKeyID: 18122550
ms:mtpsurl: 'https://technet.microsoft.com/hu-hu/library/Cc747566(v=WS.10)'
---

Az RMS kiszolgálószolgáltatása
==============================

A kiszolgálószolgáltatás csak az RMS legfelső szintű fürtjén fut. A kiszolgálószolgáltatás az ügyfelek on-line közzététel segítségével benyújtott kérelmeit továbbítja kiszolgálói licencelői tanúsítvány lekéréséhez.

A kiszolgálószolgáltatás alkalmazásfájlja, a Server.asmx, az IIS szolgáltatás Certification virtuális könyvtárában található.

A szolgáltatás alapértelmezett hozzáférési szabálygyűjteményét a következő táblázat szemlélteti:

###  

 
<table style="border:1px solid black;">
<colgroup>
<col width="50%" />
<col width="50%" />
</colgroup>
<thead>
<tr class="header">
<th style="border:1px solid black;" >Felhasználó vagy Csoport</th>
<th style="border:1px solid black;" >Alapértelmezett engedély</th>
</tr>
</thead>
<tbody>
<tr class="odd">
<td style="border:1px solid black;">Rendszergazdák</td>
<td style="border:1px solid black;">Teljes hozzáférés</td>
</tr>
<tr class="even">
<td style="border:1px solid black;">RMS szolgáltatáscsoport</td>
<td style="border:1px solid black;">Olvasás és végrehajtás</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;">RENDSZER</td>
<td style="border:1px solid black;">Teljes hozzáférés</td>
</tr>
<tr class="even">
<td style="border:1px solid black;">Felhasználók</td>
<td style="border:1px solid black;">Olvasás és végrehajtás</td>
</tr>
</tbody>
</table>
