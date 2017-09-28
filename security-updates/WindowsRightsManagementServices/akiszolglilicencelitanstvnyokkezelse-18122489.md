---
TOCTitle: A kiszolgálói licencelői tanúsítványok kezelése
Title: A kiszolgálói licencelői tanúsítványok kezelése
ms:assetid: '549979ad-13ee-4abc-8281-3e002a5a9561'
ms:contentKeyID: 18122489
ms:mtpsurl: 'https://technet.microsoft.com/hu-hu/library/Cc720272(v=WS.10)'
---

A kiszolgálói licencelői tanúsítványok kezelése
===============================================

A kiszolgálói licencelői tanúsítványok megadott idő után lejárnak. Ez az időtartam általában egy év. A kiszolgálói licencelői tanúsítvány megújításához helyi rendszergazdaként kell bejelentkeznie. A legfelső szintű tanúsítási fürt kiszolgálói licencelői tanúsítványának megújításakor az RMS megújítási kérelmet küld a Microsoft igénylési szolgáltatásnak. A licenckiszolgáló tanúsítványának megújításakor az RMS a megújítási kérelmet a lejáró tanúsítványt kiállító, legfelső szintű tanúsítási kiszolgálónak küldi.

Az RMS három eseményt jegyez be a Rendszer eseménynaplóba, ezeket figyelemmel kell kísérnie. Ezek az események tájékoztatják arról, hogy a kiszolgálói licencelői tanúsítvány megújítási dátuma közeleg, vagy már lejárt a tanúsítvány. A következő táblázat az események azonosítóját és nevét adja meg.

###  

<p> </p>
<table style="border:1px solid black;">
<colgroup>
<col width="33%" />
<col width="33%" />
<col width="33%" />
</colgroup>
<thead>
<tr class="header">
<th>Eseményazonosító</th>
<th>Eseménynév</th>
<th>Eseménytípus</th>
</tr>
</thead>
<tbody>
<tr class="odd">
<td style="border:1px solid black;"><p>16</p></td>
<td style="border:1px solid black;"><p>LicensorCertExpiresInOneMonthEvent</p></td>
<td style="border:1px solid black;"><p>Figyelem! A szolgáltatás rendben folytatja a működést.</p></td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><p>17</p></td>
<td style="border:1px solid black;"><p>LicensorCertExpiresInOneWeekEvent</p></td>
<td style="border:1px solid black;"><p>Figyelem! A szolgáltatás rendben folytatja a működést.</p></td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><p>18</p></td>
<td style="border:1px solid black;"><p>LicensorCertExpiredEvent</p></td>
<td style="border:1px solid black;"><p>Hiba. A szolgáltatás nem áll rendelkezésre.</p></td>
</tr>
</tbody>
</table>
