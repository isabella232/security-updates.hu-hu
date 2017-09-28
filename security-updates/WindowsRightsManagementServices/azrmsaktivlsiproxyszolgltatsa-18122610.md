---
TOCTitle: Az RMS aktiválási proxy szolgáltatása
Title: Az RMS aktiválási proxy szolgáltatása
ms:assetid: '6b9d33ef-466b-405b-a768-54e5615d6770'
ms:contentKeyID: 18122610
ms:mtpsurl: 'https://technet.microsoft.com/hu-hu/library/Cc747608(v=WS.10)'
---

Az RMS aktiválási proxy szolgáltatása
=====================================

Az RMS 1.0 verzió minden gépaktiválási kérelme az aktiválási proxy szolgáltatásán halad át, ami csak az RMS legfelső szintű fürtjén fut. Az ügyfélszámítógépek csak aktiválást követően használhatók az RMS szolgáltatással a tartalomvédelemmel ellátott tartalom közzétételére és használatára. A Service Pack 1 csomaggal frissített RMS ügyfélszoftver indításakor „önaktiváló”, így nincs szükség az aktiválási proxykiszolgáló vagy a Microsoft aktiválási szolgáltatásának használatára a kulcstároló és a géptanúsítvány előállításához.

Az aktiválási proxy szolgáltatás továbbítja az RMS 1.0-s verziójú ügyfelek gépaktiválási kérelmeit a Microsoft aktiválási szolgáltatásának, amely egy egyénileg előállított kulcstárolót és ennek megfelelő, az adott felhasználóra és számítógépre nézve egyedi RMS géptanúsítványt küld vissza. Az aktiválási proxy szolgáltatás ezt követően továbbítja ezeket a kérelmező ügyfélnek.

A fióktanúsítási szolgáltatás alkalmazásfájlja, az Activation.asmx, az IIS szolgáltatás Certification virtuális könyvtárában található. A szolgáltatás alapértelmezett hozzáférési szabálygyűjteményét a következő táblázat szemlélteti:

###  

 
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
<td style="border:1px solid black;">Rendszergazdák</td>
<td style="border:1px solid black;">Teljes hozzáférés</td>
</tr>
<tr class="even">
<td style="border:1px solid black;">Vendégek</td>
<td style="border:1px solid black;">Olvasás és végrehajtás</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;">RMS szolgáltatáscsoport</td>
<td style="border:1px solid black;">Olvasás és végrehajtás</td>
</tr>
<tr class="even">
<td style="border:1px solid black;">RENDSZER</td>
<td style="border:1px solid black;">Teljes hozzáférés</td>
</tr>
</tbody>
</table>
