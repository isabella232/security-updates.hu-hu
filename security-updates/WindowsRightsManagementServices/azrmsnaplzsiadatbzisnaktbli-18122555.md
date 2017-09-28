---
TOCTitle: Az RMS naplózási adatbázisának táblái
Title: Az RMS naplózási adatbázisának táblái
ms:assetid: '7ab2104c-b12d-4807-8a4b-bcabb145ff9b'
ms:contentKeyID: 18122555
ms:mtpsurl: 'https://technet.microsoft.com/hu-hu/library/Cc747569(v=WS.10)'
---

Az RMS naplózási adatbázisának táblái
=====================================

Ez a szakasz az RMS naplózási adatbázisának tábláit ismerteti.

DRMS\_Log\_Master
-----------------

A következő táblázat minden naplózási rekordhoz tartalmaz egy bejegyzést.

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
<td style="border:1px solid black;"><p>i_LogID</p></td>
<td style="border:1px solid black;"><p>int</p></td>
<td style="border:1px solid black;"><p>IDENTITY (100,1) Nem NULL</p></td>
<td style="border:1px solid black;"><p>A naplózási rekord egyedi azonosítója</p></td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><p>s_HostMachineName</p></td>
<td style="border:1px solid black;"><p>nvarchar(64)</p></td>
<td style="border:1px solid black;"><p>NULL</p></td>
<td style="border:1px solid black;"><p>A rekordot generáló kiszolgáló</p></td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><p>s_HostMachineRequestId</p></td>
<td style="border:1px solid black;"><p>nvarchar(64)</p></td>
<td style="border:1px solid black;"><p>NULL</p></td>
<td style="border:1px solid black;"><p>A kérelem azonosítója</p></td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><p>dt_RequestTime</p></td>
<td style="border:1px solid black;"><p>datetime</p></td>
<td style="border:1px solid black;"><p>NULL</p></td>
<td style="border:1px solid black;"><p>A kérelem dátuma és időpontja</p></td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><p>s_RequestPath</p></td>
<td style="border:1px solid black;"><p>nvarchar(128)</p></td>
<td style="border:1px solid black;"><p>NULL</p></td>
<td style="border:1px solid black;"><p>A kérelem URL-címe</p></td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><p>s_RequestType</p></td>
<td style="border:1px solid black;"><p>nvarchar(64)</p></td>
<td style="border:1px solid black;"><p>NULL</p></td>
<td style="border:1px solid black;"><p>A kérelem típusa</p></td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><p>s_RequestUserAddress</p></td>
<td style="border:1px solid black;"><p>nvarchar(32)</p></td>
<td style="border:1px solid black;"><p>NULL</p></td>
<td style="border:1px solid black;"><p>Az ügyfél IP-címe</p></td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><p>s_RequestUserAgent</p></td>
<td style="border:1px solid black;"><p>nvarchar(128)</p></td>
<td style="border:1px solid black;"><p>NULL</p></td>
<td style="border:1px solid black;"><p>A ügyfél felhasználói ügynökének fejrésze</p></td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><p>s_AuthenticatedState</p></td>
<td style="border:1px solid black;"><p>nvarchar(64)</p></td>
<td style="border:1px solid black;"><p>NULL</p></td>
<td style="border:1px solid black;"><p>A kérelem hitelesítési állapota</p></td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><p>s_SecureConnectionState</p></td>
<td style="border:1px solid black;"><p>nvarchar(64)</p></td>
<td style="border:1px solid black;"><p>NULL</p></td>
<td style="border:1px solid black;"><p>A kérelem SSL-védelme</p></td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><p>s_AuthenticatedId</p></td>
<td style="border:1px solid black;"><p>nvarchar(128)</p></td>
<td style="border:1px solid black;"><p>NULL</p></td>
<td style="border:1px solid black;"><p>A hitelesített felhasználó azonosítója</p></td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><p>s_ReceivedXrML</p></td>
<td style="border:1px solid black;"><p>ntext</p></td>
<td style="border:1px solid black;"><p>NULL</p></td>
<td style="border:1px solid black;"><p>Az ügyféltől a kérelemben kapott XrML</p></td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><p>s_IssuedXrML</p></td>
<td style="border:1px solid black;"><p>ntext</p></td>
<td style="border:1px solid black;"><p>NULL</p></td>
<td style="border:1px solid black;"><p>A kérelemben kiállított XrML-licenc</p></td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><p>s_Metadata</p></td>
<td style="border:1px solid black;"><p>ntext</p></td>
<td style="border:1px solid black;"><p>NULL</p></td>
<td style="border:1px solid black;"><p>Metaadat</p></td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><p>s_SuccessOrFailure</p></td>
<td style="border:1px solid black;"><p>nvarchar(32)</p></td>
<td style="border:1px solid black;"><p>NULL</p></td>
<td style="border:1px solid black;"><p>A kérelem sikeressége vagy sikertelensége</p></td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><p>s_ErrorInformation</p></td>
<td style="border:1px solid black;"><p>ntext</p></td>
<td style="border:1px solid black;"><p>NULL</p></td>
<td style="border:1px solid black;"><p>Hibaadatok</p></td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><p>dt_LogCreateTime</p></td>
<td style="border:1px solid black;"><p>datetime</p></td>
<td style="border:1px solid black;"><p>Nem NULL</p></td>
<td style="border:1px solid black;"><p>A bejegyzés létrehozásának időpontja</p></td>
</tr>
</tbody>
</table>
  
DRMS\_Log\_Detail  
-----------------
  
A következő táblázatban a naplózási rekordok további adatai szerepelnek. Az XrML-adatok jellemzően ebbe a táblába kerülnek.
  
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
<td style="border:1px solid black;"><p>i_LogDetailID</p></td>
<td style="border:1px solid black;"><p>int (PK)</p></td>
<td style="border:1px solid black;"><p>IDENTITY(100,1)</p></td>
<td style="border:1px solid black;"><p>Belső index</p></td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><p>i_LogID</p></td>
<td style="border:1px solid black;"><p>int (külső kulcs)</p></td>
<td style="border:1px solid black;"><p>Nem NULL (külső kulcs)</p></td>
<td style="border:1px solid black;"><p>A szülő naplózási rekord azonosítója</p></td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><p>s_Name</p></td>
<td style="border:1px solid black;"><p>nvarchar(128)</p></td>
<td style="border:1px solid black;"><p>Nem NULL</p></td>
<td style="border:1px solid black;"><p>A tulajdonság neve</p></td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><p>s_Value</p></td>
<td style="border:1px solid black;"><p>ntext</p></td>
<td style="border:1px solid black;"><p>NULL</p></td>
<td style="border:1px solid black;"><p>A tulajdonság értéke</p></td>
</tr>
</tbody>
</table>
  
DRMS\_Log\_Filter  
-----------------
  
A következő táblázat azokat a mezőket tartalmazza, amelyeket a naplózásfigyelő szolgáltatás naplóz.
  
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
<td style="border:1px solid black;"><p>i_ID</p></td>
<td style="border:1px solid black;"><p>int</p></td>
<td style="border:1px solid black;"><p>IDENTITY (100,1) Nem NULL</p></td>
<td style="border:1px solid black;"><p>Belső index</p></td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><p>s_FieldName</p></td>
<td style="border:1px solid black;"><p>nvarchar(255)</p></td>
<td style="border:1px solid black;"><p>Nem NULL</p></td>
<td style="border:1px solid black;"><p>A mező neve</p></td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><p>s_FieldDescription</p></td>
<td style="border:1px solid black;"><p>nvarchar(1024)</p></td>
<td style="border:1px solid black;"><p>NULL</p></td>
<td style="border:1px solid black;"><p>A mező leírása</p></td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><p>i_IsIncluded</p></td>
<td style="border:1px solid black;"><p>int</p></td>
<td style="border:1px solid black;"><p>Nem NULL</p></td>
<td style="border:1px solid black;"><p>Annak jelzése, hogy engedélyezve van-e a mező naplózása</p></td>
</tr>
</tbody>
</table>
