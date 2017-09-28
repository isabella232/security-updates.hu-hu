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
<td style="border:1px solid black;">16</td>
<td style="border:1px solid black;">LicensorCertExpiresInOneMonthEvent</td>
<td style="border:1px solid black;">Figyelem! A szolgáltatás rendben folytatja a működést.</td>
</tr>
<tr class="even">
<td style="border:1px solid black;">17</td>
<td style="border:1px solid black;">LicensorCertExpiresInOneWeekEvent</td>
<td style="border:1px solid black;">Figyelem! A szolgáltatás rendben folytatja a működést.</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;">18</td>
<td style="border:1px solid black;">LicensorCertExpiredEvent</td>
<td style="border:1px solid black;">Hiba. A szolgáltatás nem áll rendelkezésre.</td>
</tr>
</tbody>
</table>
