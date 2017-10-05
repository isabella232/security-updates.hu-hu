---
TOCTitle: Az RMS előtanúsításai szolgáltatása
Title: Az RMS előtanúsításai szolgáltatása
ms:assetid: '09957294-167f-4f98-88e9-ae90fbeb26c1'
ms:contentKeyID: 18122483
ms:mtpsurl: 'https://technet.microsoft.com/hu-hu/library/Cc720191(v=WS.10)'
---

Az RMS előtanúsításai szolgáltatása
===================================

Az előtanúsítási szolgáltatás csak az RMS legfelső szintű fürtjén fut. A szolgáltatás lehetővé teszi, hogy a kiszolgáló tartalomvédelmi fióktanúsítványt kérelmezzen egy felhasználó nevében, és egyéni alkalmazások fejlesztéséhez használható. Ezt a szolgáltatást például a Microsoft Exchange Server 2007 és a Microsoft Office SharePoint Server 2007 használja.

Az előtanúsítási szolgáltatás alkalmazásfájlja, a Precertification.asmx, az IIS szolgáltatás Certification virtuális könyvtárában található.

Az egyéni alkalmazások fejlesztéséről a további tudnivalókat tartalmaz az MSDN Library részben a Windows tartalomvédelmi szolgáltatások dokumentációja [http://go.microsoft.com/fwlink/?LinkId=32972](http://go.microsoft.com/fwlink/?linkid=32972).

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
