---
TOCTitle: Visszavonás a jogmegadási sablonokban
Title: Visszavonás a jogmegadási sablonokban
ms:assetid: '287c5b92-fcb5-4295-9c2b-4e37e643beb2'
ms:contentKeyID: 18122522
ms:mtpsurl: 'https://technet.microsoft.com/hu-hu/library/Cc720226(v=WS.10)'
---

Visszavonás a jogmegadási sablonokban
=====================================

A visszavonási feltételek a jogmegadási sablonokban vannak megadva. A jogmegadási sablonokba beírt visszavonási feltételek a sablon alapján kiállított közzétételi licencekbe egy XrML REFRESH címke alatt kerülnek be. A kiszolgáló által ennek ellenében kiállított használati licencek is tartalmazzák a REFRESH címkét.

Az alábbi táblázatban a REFRESH címkében használat paraméterek olvashatók.

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
<th>Leírás</th>
</tr>
</thead>
<tbody>
<tr class="odd">
<td style="border:1px solid black;"><p>ID</p></td>
<td style="border:1px solid black;"><p>A visszavonási lista azonosítója.</p></td>
</tr>  
<tr class="even">
<td style="border:1px solid black;"><p>ADDRESS</p></td>
<td style="border:1px solid black;"><p>Az az URL-cím vagy UNC elérési út, ahonnan a visszavonási lista megszerezhető.</p></td>
</tr>  
<tr class="odd">
<td style="border:1px solid black;"><p>PUBLICKEY</p></td>
<td style="border:1px solid black;"><p>A visszavonási lista kiállítójának nyilvános kulcsa. A nyilvános kulcs megfelel a visszavonási lista aláírására használt személyes kulcsnak.</p></td>
</tr>  
<tr class="even">
<td style="border:1px solid black;"><p>INTERVALTIME</p></td>
<td style="border:1px solid black;"><p>A visszavonási lista maximális kora, napokban megadva. Ha a gyorsítótárban lévő visszavonási lista régebbi, mint az INTERVALTIME érték által megengedett időtartam, az RMS ügyfélszámítógépe beszerzi a visszavonási lista legfrissebb változatát az ADDRESS bejegyzésben megadott címről. Ez garantálja, hogy a használt visszavonási lista naprakész legyen.</p></td>
</tr>  
</tbody>  
</table>
  
A jogmegadási sablonok létrehozásáról a további tudnivalókat lásd a dokumentumgyűjtemény „RMS kiszolgáló működtetése” részében „A jogmegadási sablonok létrehozása és módosítása” témakörben.
