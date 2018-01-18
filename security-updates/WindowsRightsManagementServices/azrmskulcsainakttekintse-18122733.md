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
<th style="border:1px solid black;" >Kulcs</th>
<th style="border:1px solid black;" >Rendeltetése</th>
</tr>
</thead>
<tbody>
<tr class="odd">
<td style="border:1px solid black;">Kiszolgálói kulcsok</td>
<td style="border:1px solid black;"><strong>Nyilvános kulcs</strong>
A közzétételi licencben szereplő tartalomkulcsot titkosítja, hogy csak az RMS kiszolgáló tudja beolvasni a tartalomkulcsot, és csak az tudjon használati licencet kiállítani az adott közzétételi licenc ellenében.
<strong>Személyes kulcs</strong>
Aláír minden, a kiszolgáló által kiállított tanúsítványt és licencet.</td>
</tr>
<tr class="even">
<td style="border:1px solid black;">Gépkulcsok</td>
<td style="border:1px solid black;"><strong>Nyilvános kulcs</strong>
A tartalomvédelmi fióktanúsítvány személyes kulcsát titkosítja.
<strong>Személyes kulcs</strong>
A tartalomvédelmi fióktanúsítványt fejti vissza.</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;">Ügyfél-licencelői kulcsok</td>
<td style="border:1px solid black;"><strong>Nyilvános kulcs</strong>
Az általa kiállított közzétételi licencek szimmetrikus tartalomkulcsát titkosítja.
<strong>Személyes kulcs</strong>
Aláírja azokat a közzétételi licenceket, amelyeket akkor állítanak ki, amikor a felhasználó nem kapcsolódik a hálózathoz.</td>
</tr>
<tr class="even">
<td style="border:1px solid black;">Felhasználói kulcsok</td>
<td style="border:1px solid black;"><strong>Nyilvános kulcs</strong>
A használati licencben lévő tartalomkulcsot titkosítja,így csak az adott felhasználó tudja azt az RMS-védelemmel ellátott tartalmat az adott licenc segítségével használni.
<strong>Személyes kulcs</strong>
Lehetővé teszi a felhasználónak, hogy használja az RMS-védelemmel ellátott tartalmat.</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;">Tartalomkulcsok</td>
<td style="border:1px solid black;">Az RMS-védelemmel ellátott tartalmat titkosítja, amikor a szerző közzéteszi azt.</td>
</tr>
</tbody>
</table>
