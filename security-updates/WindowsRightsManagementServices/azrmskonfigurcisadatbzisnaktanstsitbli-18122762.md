---
TOCTitle: Az RMS konfigurációs adatbázisának tanúsítási táblái
Title: Az RMS konfigurációs adatbázisának tanúsítási táblái
ms:assetid: 'd392663a-1a46-42f6-a71d-f0f2c1843566'
ms:contentKeyID: 18122762
ms:mtpsurl: 'https://technet.microsoft.com/hu-hu/library/Cc747760(v=WS.10)'
---

Az RMS konfigurációs adatbázisának tanúsítási táblái
====================================================

Ez a rész az RMS konfigurációs adatbázisának tanúsítási tábláit ismerteti. A táblák azoknak a tartalomvédelmi fióktanúsítványoknak az adatait tartalmazzák, amelyeket az adott telepítés felhasználói részére kibocsátott a szolgáltatás.

UD\_Machines
------------

A következő táblázat a számítógépek hardverazonosítóira vonatkozó adatokat tartalmazza.

###  

<p> </p>
<table style="border:1px solid black;">
<colgroup>
<col width="25%" />
<col width="25%" />
<col width="25%" />
<col width="25%" />
</colgroup>
<thead>
<tr class="header">
<th>Név</th>
<th>Adattípus</th>
<th>NULL értékek</th>
<th>Leírás</th>
</tr>
</thead>
<tbody>
<tr class="odd">
<td style="border:1px solid black;"><p>i_MachineId</p></td>
<td style="border:1px solid black;"><p>int</p></td>
<td style="border:1px solid black;"><p>IDENTITY (1,1) Nem NULL</p></td>
<td style="border:1px solid black;"><p>Belső index</p></td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><p>b_PubKeyHash</p></td>
<td style="border:1px solid black;"><p>binary(20)</p></td>
<td style="border:1px solid black;"><p>(20) Nem NULL</p></td>
<td style="border:1px solid black;"><p>A hardverazonosító kivonata</p></td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><p>dt_CreateDate</p></td>
<td style="border:1px solid black;"><p>datetime</p></td>
<td style="border:1px solid black;"><p>Nem NULL</p></td>
<td style="border:1px solid black;"><p>A dátum és időpont, amikor a bejegyzés bekerült a táblába</p></td>
</tr>
</tbody>
</table>
  
UD\_PassportAuthIdentities  
--------------------------
  
A következő táblázat a felhasználók Microsoft® .NET Passport adatairól tájékoztat.
  
###  

<p> </p>
<table style="border:1px solid black;">
<colgroup>
<col width="25%" />
<col width="25%" />
<col width="25%" />
<col width="25%" />
</colgroup>
<thead>
<tr class="header">
<th>Név</th>
<th>Adattípus</th>
<th>NULL értékek</th>
<th>Leírás</th>
</tr>
</thead>
<tbody>
<tr class="odd">
<td style="border:1px solid black;"><p>i_UserId</p></td>
<td style="border:1px solid black;"><p>int</p></td>
<td style="border:1px solid black;"><p>Nem NULL</p></td>
<td style="border:1px solid black;"><p>Belső index</p></td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><p>i64_Puid</p></td>
<td style="border:1px solid black;"><p>bigint</p></td>
<td style="border:1px solid black;"><p>(50) NULL</p></td>
<td style="border:1px solid black;"><p>.NET Passport-felhasználóazonosító</p></td>
</tr>
</tbody>
</table>
  
UD\_UserMachine  
---------------
  
A következő táblázat a tanúsítvánnyal ellátott felhasználók és a hozzájuk tartozó számítógép adatait felelteti meg egymásnak.
  
###  

<p> </p>
<table style="border:1px solid black;">
<colgroup>
<col width="25%" />
<col width="25%" />
<col width="25%" />
<col width="25%" />
</colgroup>
<thead>
<tr class="header">
<th>Név</th>
<th>Adattípus</th>
<th>NULL értékek</th>
<th>Leírás</th>
</tr>
</thead>
<tbody>
<tr class="odd">
<td style="border:1px solid black;"><p>i_MachineId</p></td>
<td style="border:1px solid black;"><p>int</p></td>
<td style="border:1px solid black;"><p>Nem NULL</p></td>
<td style="border:1px solid black;"><p>Belső index</p></td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><p>i_UserId</p></td>
<td style="border:1px solid black;"><p>int</p></td>
<td style="border:1px solid black;"><p>Nem NULL</p></td>
<td style="border:1px solid black;"><p>Belső index</p></td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><p>dt_CreateDate</p></td>
<td style="border:1px solid black;"><p>datetime</p></td>
<td style="border:1px solid black;"><p>Nem NULL</p></td>
<td style="border:1px solid black;"><p>A dátum és időpont, amikor a bejegyzés bekerült a táblába</p></td>
</tr>
</tbody>
</table>
  
UD\_Users  
---------
  
A következő táblázat a felhasználói adatokkal kapcsolatos információkat tartalmazza.
  
###  

<p> </p>
<table style="border:1px solid black;">
<colgroup>
<col width="25%" />
<col width="25%" />
<col width="25%" />
<col width="25%" />
</colgroup>
<thead>
<tr class="header">
<th>Név</th>
<th>Adattípus</th>
<th>NULL értékek</th>
<th>Leírás</th>
</tr>
</thead>
<tbody>
<tr class="odd">
<td style="border:1px solid black;"><p>i_UserId</p></td>
<td style="border:1px solid black;"><p>int</p></td>
<td style="border:1px solid black;"><p>IDENTITY (1,1) Nem NULL</p></td>
<td style="border:1px solid black;"><p>Belső index</p></td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><p>b_KeyData</p></td>
<td style="border:1px solid black;"><p>varbinary(2000)</p></td>
<td style="border:1px solid black;"><p>(2000) Nem NULL</p></td>
<td style="border:1px solid black;"><p>A felhasználó nyilvános és személyes kulcsának titkosított változata</p></td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><p>i_KeyDataLength</p></td>
<td style="border:1px solid black;"><p>int</p></td>
<td style="border:1px solid black;"><p>Nem NULL</p></td>
<td style="border:1px solid black;"><p>A felhasználó nyilvános és személyes kulcsa titkosítatlan változatának hossza</p></td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><p>b_PublicKey</p></td>
<td style="border:1px solid black;"><p>PublicKey</p></td>
<td style="border:1px solid black;"><p>Nem NULL</p></td>
<td style="border:1px solid black;"><p>A felhasználó nyilvános kulcsa</p></td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><p>i_EncryptionDbId</p></td>
<td style="border:1px solid black;"><p>int</p></td>
<td style="border:1px solid black;"><p>Nem NULL</p></td>
<td style="border:1px solid black;"><p>A nyilvános-személyes kulcspár titkosítására használt licencelői tanúsítványra mutató hivatkozás</p></td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><p>s_Certificate</p></td>
<td style="border:1px solid black;"><p>ntext</p></td>
<td style="border:1px solid black;"><p>Nincs megadva</p></td>
<td style="border:1px solid black;"><p>Használaton kívül</p></td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><p>dt_Expiration</p></td>
<td style="border:1px solid black;"><p>datetime</p></td>
<td style="border:1px solid black;"><p>Nem NULL</p></td>
<td style="border:1px solid black;"><p>A felhasználói kulcs lejáratának dátuma</p></td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><p>dt_TemporaryExpiration</p></td>
<td style="border:1px solid black;"><p>datetime</p></td>
<td style="border:1px solid black;"><p>Nem NULL</p></td>
<td style="border:1px solid black;"><p>A dátum és időpont, amikor lejár a kulcs ideiglenes használhatósága</p></td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><p>f_Modified</p></td>
<td style="border:1px solid black;"><p>bit</p></td>
<td style="border:1px solid black;"><p>Nem NULL</p></td>
<td style="border:1px solid black;"><p>Használaton kívül</p></td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><p>i_Quota</p></td>
<td style="border:1px solid black;"><p>int</p></td>
<td style="border:1px solid black;"><p>Nem NULL</p></td>
<td style="border:1px solid black;"><p>A felhasználó kvótájának aktuális szintje</p></td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><p>i_WaitDays</p></td>
<td style="border:1px solid black;"><p>int</p></td>
<td style="border:1px solid black;"><p>Nem NULL</p></td>
<td style="border:1px solid black;"><p>Azoknak a napoknak a száma, ahány nap múlva sikeresek lehetnek a további, kvóta iránti kérelmek</p></td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><p>dt_LastConsumption</p></td>
<td style="border:1px solid black;"><p>datetime</p></td>
<td style="border:1px solid black;"><p>Nem NULL</p></td>
<td style="border:1px solid black;"><p>A dátum és időpont, amikor a felhasználó utoljára kapott további tanúsítványt</p></td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><p>dt_CreateDate</p></td>
<td style="border:1px solid black;"><p>datetime</p></td>
<td style="border:1px solid black;"><p>Nem NULL</p></td>
<td style="border:1px solid black;"><p>A dátum és időpont, amikor a bejegyzés bekerült a táblába</p></td>
</tr>
</tbody>
</table>
  
UD\_Windows AuthIdentities  
--------------------------
  
A következő táblázat a Windows által hitelesített és tanúsítvánnyal ellátott összes felhasználó adatait tartalmazza.
  
###  

<p> </p>
<table style="border:1px solid black;">
<colgroup>
<col width="25%" />
<col width="25%" />
<col width="25%" />
<col width="25%" />
</colgroup>
<thead>
<tr class="header">
<th>Név</th>
<th>Adattípus</th>
<th>NULL értékek</th>
<th>Leírás</th>
</tr>
</thead>
<tbody>
<tr class="odd">
<td style="border:1px solid black;"><p>i_UserId</p></td>
<td style="border:1px solid black;"><p>int</p></td>
<td style="border:1px solid black;"><p>Nem NULL</p></td>
<td style="border:1px solid black;"><p>Belső index</p></td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><p>s_Sid</p></td>
<td style="border:1px solid black;"><p>Sid</p></td>
<td style="border:1px solid black;"><p>Nem NULL</p></td>
<td style="border:1px solid black;"><p>A felhasználó biztonsági azonosítója (SID)</p></td>
</tr>
</tbody>
</table>
