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
<td style="border:1px solid black;">i_MachineId</td>
<td style="border:1px solid black;">int</td>
<td style="border:1px solid black;">IDENTITY (1,1) Nem NULL</td>
<td style="border:1px solid black;">Belső index</td>
</tr>
<tr class="even">
<td style="border:1px solid black;">b_PubKeyHash</td>
<td style="border:1px solid black;">binary(20)</td>
<td style="border:1px solid black;">(20) Nem NULL</td>
<td style="border:1px solid black;">A hardverazonosító kivonata</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;">dt_CreateDate</td>
<td style="border:1px solid black;">datetime</td>
<td style="border:1px solid black;">Nem NULL</td>
<td style="border:1px solid black;">A dátum és időpont, amikor a bejegyzés bekerült a táblába</td>
</tr>
</tbody>
</table>
  
UD\_PassportAuthIdentities  
--------------------------
  
A következő táblázat a felhasználók Microsoft® .NET Passport adatairól tájékoztat.
  
###  

 
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
<td style="border:1px solid black;">i_UserId</td>
<td style="border:1px solid black;">int</td>
<td style="border:1px solid black;">Nem NULL</td>
<td style="border:1px solid black;">Belső index</td>
</tr>
<tr class="even">
<td style="border:1px solid black;">i64_Puid</td>
<td style="border:1px solid black;">bigint</td>
<td style="border:1px solid black;">(50) NULL</td>
<td style="border:1px solid black;">.NET Passport-felhasználóazonosító</td>
</tr>
</tbody>
</table>
  
UD\_UserMachine  
---------------
  
A következő táblázat a tanúsítvánnyal ellátott felhasználók és a hozzájuk tartozó számítógép adatait felelteti meg egymásnak.
  
###  

 
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
<td style="border:1px solid black;">i_MachineId</td>
<td style="border:1px solid black;">int</td>
<td style="border:1px solid black;">Nem NULL</td>
<td style="border:1px solid black;">Belső index</td>
</tr>
<tr class="even">
<td style="border:1px solid black;">i_UserId</td>
<td style="border:1px solid black;">int</td>
<td style="border:1px solid black;">Nem NULL</td>
<td style="border:1px solid black;">Belső index</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;">dt_CreateDate</td>
<td style="border:1px solid black;">datetime</td>
<td style="border:1px solid black;">Nem NULL</td>
<td style="border:1px solid black;">A dátum és időpont, amikor a bejegyzés bekerült a táblába</td>
</tr>
</tbody>
</table>
  
UD\_Users  
---------
  
A következő táblázat a felhasználói adatokkal kapcsolatos információkat tartalmazza.
  
###  

 
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
<td style="border:1px solid black;">i_UserId</td>
<td style="border:1px solid black;">int</td>
<td style="border:1px solid black;">IDENTITY (1,1) Nem NULL</td>
<td style="border:1px solid black;">Belső index</td>
</tr>
<tr class="even">
<td style="border:1px solid black;">b_KeyData</td>
<td style="border:1px solid black;">varbinary(2000)</td>
<td style="border:1px solid black;">(2000) Nem NULL</td>
<td style="border:1px solid black;">A felhasználó nyilvános és személyes kulcsának titkosított változata</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;">i_KeyDataLength</td>
<td style="border:1px solid black;">int</td>
<td style="border:1px solid black;">Nem NULL</td>
<td style="border:1px solid black;">A felhasználó nyilvános és személyes kulcsa titkosítatlan változatának hossza</td>
</tr>
<tr class="even">
<td style="border:1px solid black;">b_PublicKey</td>
<td style="border:1px solid black;">PublicKey</td>
<td style="border:1px solid black;">Nem NULL</td>
<td style="border:1px solid black;">A felhasználó nyilvános kulcsa</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;">i_EncryptionDbId</td>
<td style="border:1px solid black;">int</td>
<td style="border:1px solid black;">Nem NULL</td>
<td style="border:1px solid black;">A nyilvános-személyes kulcspár titkosítására használt licencelői tanúsítványra mutató hivatkozás</td>
</tr>
<tr class="even">
<td style="border:1px solid black;">s_Certificate</td>
<td style="border:1px solid black;">ntext</td>
<td style="border:1px solid black;">Nincs megadva</td>
<td style="border:1px solid black;">Használaton kívül</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;">dt_Expiration</td>
<td style="border:1px solid black;">datetime</td>
<td style="border:1px solid black;">Nem NULL</td>
<td style="border:1px solid black;">A felhasználói kulcs lejáratának dátuma</td>
</tr>
<tr class="even">
<td style="border:1px solid black;">dt_TemporaryExpiration</td>
<td style="border:1px solid black;">datetime</td>
<td style="border:1px solid black;">Nem NULL</td>
<td style="border:1px solid black;">A dátum és időpont, amikor lejár a kulcs ideiglenes használhatósága</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;">f_Modified</td>
<td style="border:1px solid black;">bit</td>
<td style="border:1px solid black;">Nem NULL</td>
<td style="border:1px solid black;">Használaton kívül</td>
</tr>
<tr class="even">
<td style="border:1px solid black;">i_Quota</td>
<td style="border:1px solid black;">int</td>
<td style="border:1px solid black;">Nem NULL</td>
<td style="border:1px solid black;">A felhasználó kvótájának aktuális szintje</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;">i_WaitDays</td>
<td style="border:1px solid black;">int</td>
<td style="border:1px solid black;">Nem NULL</td>
<td style="border:1px solid black;">Azoknak a napoknak a száma, ahány nap múlva sikeresek lehetnek a további, kvóta iránti kérelmek</td>
</tr>
<tr class="even">
<td style="border:1px solid black;">dt_LastConsumption</td>
<td style="border:1px solid black;">datetime</td>
<td style="border:1px solid black;">Nem NULL</td>
<td style="border:1px solid black;">A dátum és időpont, amikor a felhasználó utoljára kapott további tanúsítványt</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;">dt_CreateDate</td>
<td style="border:1px solid black;">datetime</td>
<td style="border:1px solid black;">Nem NULL</td>
<td style="border:1px solid black;">A dátum és időpont, amikor a bejegyzés bekerült a táblába</td>
</tr>
</tbody>
</table>
  
UD\_Windows AuthIdentities  
--------------------------
  
A következő táblázat a Windows által hitelesített és tanúsítvánnyal ellátott összes felhasználó adatait tartalmazza.
  
###  

 
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
<td style="border:1px solid black;">i_UserId</td>
<td style="border:1px solid black;">int</td>
<td style="border:1px solid black;">Nem NULL</td>
<td style="border:1px solid black;">Belső index</td>
</tr>
<tr class="even">
<td style="border:1px solid black;">s_Sid</td>
<td style="border:1px solid black;">Sid</td>
<td style="border:1px solid black;">Nem NULL</td>
<td style="border:1px solid black;">A felhasználó biztonsági azonosítója (SID)</td>
</tr>
</tbody>
</table>
