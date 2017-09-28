---
TOCTitle: Az RMS kulcsainak áttekintése
Title: Az RMS kulcsainak áttekintése
ms:assetid: 'b052305c-1db7-434a-bad9-26d704156776'
ms:contentKeyID: 18122733
ms:mtpsurl: 'https://technet.microsoft.com/hu-hu/library/Cc747729(v=WS.10)'
---

Az RMS kulcsainak áttekintése
=============================

A következő táblázat az RMS rendszerben használt kulcsokat mutatja be.

###  

<p> </p>
<table style="border:1px solid black;">
<colgroup>
<col width="50%" />
<col width="50%" />
</colgroup>
<thead>
<tr class="header">
<th>Kulcs</th>
<th>Rendeltetése</th>
</tr>
</thead>
<tbody>
<tr class="odd">
<td style="border:1px solid black;"><p>Kiszolgálói kulcsok</p></td>
<td style="border:1px solid black;"><p><strong>Nyilvános kulcs</strong></p>
<p>A közzétételi licencben szereplő tartalomkulcsot titkosítja, hogy csak az RMS kiszolgáló tudja beolvasni a tartalomkulcsot, és csak az tudjon használati licencet kiállítani az adott közzétételi licenc ellenében.</p>
<p><strong>Személyes kulcs</strong></p>
<p>Aláír minden, a kiszolgáló által kiállított tanúsítványt és licencet.</p></td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><p>Gépkulcsok</p></td>
<td style="border:1px solid black;"><p><strong>Nyilvános kulcs</strong></p>
<p>A tartalomvédelmi fióktanúsítvány személyes kulcsát titkosítja.</p>
<p><strong>Személyes kulcs</strong></p>
<p>A tartalomvédelmi fióktanúsítványt fejti vissza.</p></td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><p>Ügyfél-licencelői kulcsok</p></td>
<td style="border:1px solid black;"><p><strong>Nyilvános kulcs</strong></p>
<p>Az általa kiállított közzétételi licencek szimmetrikus tartalomkulcsát titkosítja.</p>
<p><strong>Személyes kulcs</strong></p>
<p>Aláírja azokat a közzétételi licenceket, amelyeket akkor állítanak ki, amikor a felhasználó nem kapcsolódik a hálózathoz.</p></td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><p>Felhasználói kulcsok</p></td>
<td style="border:1px solid black;"><p><strong>Nyilvános kulcs</strong></p>
<p>A használati licencben lévő tartalomkulcsot titkosítja,így csak az adott felhasználó tudja azt az RMS-védelemmel ellátott tartalmat az adott licenc segítségével használni.</p>
<p><strong>Személyes kulcs</strong></p>
<p>Lehetővé teszi a felhasználónak, hogy használja az RMS-védelemmel ellátott tartalmat.</p></td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><p>Tartalomkulcsok</p></td>
<td style="border:1px solid black;"><p>Az RMS-védelemmel ellátott tartalmat titkosítja, amikor a szerző közzéteszi azt.</p></td>
</tr>
</tbody>
</table>
