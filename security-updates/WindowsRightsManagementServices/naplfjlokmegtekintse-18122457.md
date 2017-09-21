---
TOCTitle: Naplófájlok megtekintése
Title: Naplófájlok megtekintése
ms:assetid: '2dc9ed54-76d8-4721-ba93-194845de726a'
ms:contentKeyID: 18122457
ms:mtpsurl: 'https://technet.microsoft.com/hu-hu/library/Cc720228(v=WS.10)'
---

Naplófájlok megtekintése
========================

Az RMS bevezetésének módjától függően a naplófájlok tárolása az SQL Server vagy a Microsoft SQL Server 2000 Desktop Engine (MSDE 2000) Release A adatbázis-kiszolgálón történik. A naplófájlokban rögzített adatok mennyiségének csökkentésére szűrőket alkalmazhat. Erről az SQL Server Enterprise Manager súgójában tájékozódhat.

A naplóbejegyzések átlagos mérete 300 bájt. Az alábbi táblázat a naplóban szereplő mezőket ismerteti.

###  

<p> </p>
<table style="border:1px solid black;">
<colgroup>
<col width="50%" />
<col width="50%" />
</colgroup>
<thead>
<tr class="header">
<th>Mező</th>
<th>Leírás</th>
</tr>
</thead>
<tbody>
<tr class="odd">
<td style="border:1px solid black;"><p>HostMachineName</p></td>
<td style="border:1px solid black;"><p>A kérelmet kezelő számítógép.</p></td>
</tr>  
<tr class="even">
<td style="border:1px solid black;"><p>HostMachineRequestId</p></td>
<td style="border:1px solid black;"><p>Egyedien azonosítja az adott kérelmet az adott számítógépen. A HostMachineName és a HostMachineRequestId érték együttesen egyedien azonosítja a kérelmet a fürtön belül.</p></td>
</tr>  
<tr class="odd">
<td style="border:1px solid black;"><p>RequestTime</p></td>
<td style="border:1px solid black;"><p>A kérelem fogadásának ideje az egyetemes koordinált idő (greenwich-i idő) szerint.</p></td>
</tr>  
<tr class="even">
<td style="border:1px solid black;"><p>RequestPath</p></td>
<td style="border:1px solid black;"><p>Az .asmx fájl relatív URL-címe, például: /_wmcs/licensing/License.asmx.</p></td>
</tr>  
<tr class="odd">
<td style="border:1px solid black;"><p>RequestType</p></td>
<td style="border:1px solid black;"><p>A hívott webes metódus neve, például: AcquireLicense.</p></td>
</tr>  
<tr class="even">
<td style="border:1px solid black;"><p>RequestUserAddress</p></td>
<td style="border:1px solid black;"><p>A kérelmező forrás IP-címe.</p></td>
</tr>  
<tr class="odd">
<td style="border:1px solid black;"><p>RequestUserAgent</p></td>
<td style="border:1px solid black;"><p>A HTTP-fejrész felhasználói ügynök értéke.</p></td>
</tr>  
<tr class="even">
<td style="border:1px solid black;"><p>AuthenticatedState</p></td>
<td style="border:1px solid black;"><p>A HTTP-kapcsolat hitelesítettségéről tájékoztat (True/False).</p></td>
</tr>  
<tr class="odd">
<td style="border:1px solid black;"><p>SecureConnectionState</p></td>
<td style="border:1px solid black;"><p>Megadja, hogy a kapcsolat SSL-kapcsolat-e (True/False).</p></td>
</tr>  
<tr class="even">
<td style="border:1px solid black;"><p>AuthenticatedId</p></td>
<td style="border:1px solid black;"><p>A hitelesített kérelmek bejelentkezési neve. Üres, ha AuthenticatedState=False.</p></td>
</tr>  
<tr class="odd">
<td style="border:1px solid black;"><p>ReceivedXrMLDocument</p></td>
<td style="border:1px solid black;"><p>A kérelmezőtől érkezett XrML-dokumentum.</p></td>
</tr>  
<tr class="even">
<td style="border:1px solid black;"><p>ReceivedXrMLDocumentIssuerChain</p></td>
<td style="border:1px solid black;"><p>A fogadott XrML-dokumentum kiállítói lánca.</p></td>
</tr>  
<tr class="odd">
<td style="border:1px solid black;"><p>IssuedXrMLDocument</p></td>
<td style="border:1px solid black;"><p>A kérelmezőnek visszaküldött XrML-dokumentum.</p></td>
</tr>  
<tr class="even">
<td style="border:1px solid black;"><p>IssuedXrMLDocumentIssuerChain</p></td>
<td style="border:1px solid black;"><p>A kiadott XrML-dokumentum kiállítói lánca.</p></td>
</tr>  
<tr class="odd">
<td style="border:1px solid black;"><p>SuccessOrFailure</p></td>
<td style="border:1px solid black;"><p>Megadja, hogy sikeres volt-e a kérelem (Succeeded/Failed).</p></td>
</tr>  
<tr class="even">
<td style="border:1px solid black;"><p>Metaadat</p></td>
<td style="border:1px solid black;"><p>A metaadatok mezője.</p></td>
</tr>  
<tr class="odd">
<td style="border:1px solid black;"><p>ErrorInformation</p></td>
<td style="border:1px solid black;"><p>Hiba esetén a hibát leíró üzenet.</p></td>
</tr>  
</tbody>  
</table>
