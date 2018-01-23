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

 
<table style="border:1px solid black;">
<colgroup>
<col width="25%" />
<col width="25%" />
<col width="25%" />
<col width="25%" />
</colgroup>
<thead>
<tr class="header">
<th style="border:1px solid black;" >Név</th>
<th style="border:1px solid black;" >Adattípus</th>
<th style="border:1px solid black;" >NULL értékek</th>
<th style="border:1px solid black;" >Leírás</th>
</tr>
</thead>
<tbody>
<tr class="odd">
<td style="border:1px solid black;">i_LogID</td>
<td style="border:1px solid black;">int</td>
<td style="border:1px solid black;">IDENTITY (100,1) Nem NULL</td>
<td style="border:1px solid black;">A naplózási rekord egyedi azonosítója</td>
</tr>
<tr class="even">
<td style="border:1px solid black;">s_HostMachineName</td>
<td style="border:1px solid black;">nvarchar(64)</td>
<td style="border:1px solid black;">NULL</td>
<td style="border:1px solid black;">A rekordot generáló kiszolgáló</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;">s_HostMachineRequestId</td>
<td style="border:1px solid black;">nvarchar(64)</td>
<td style="border:1px solid black;">NULL</td>
<td style="border:1px solid black;">A kérelem azonosítója</td>
</tr>
<tr class="even">
<td style="border:1px solid black;">dt_RequestTime</td>
<td style="border:1px solid black;">datetime</td>
<td style="border:1px solid black;">NULL</td>
<td style="border:1px solid black;">A kérelem dátuma és időpontja</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;">s_RequestPath</td>
<td style="border:1px solid black;">nvarchar(128)</td>
<td style="border:1px solid black;">NULL</td>
<td style="border:1px solid black;">A kérelem URL-címe</td>
</tr>
<tr class="even">
<td style="border:1px solid black;">s_RequestType</td>
<td style="border:1px solid black;">nvarchar(64)</td>
<td style="border:1px solid black;">NULL</td>
<td style="border:1px solid black;">A kérelem típusa</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;">s_RequestUserAddress</td>
<td style="border:1px solid black;">nvarchar(32)</td>
<td style="border:1px solid black;">NULL</td>
<td style="border:1px solid black;">Az ügyfél IP-címe</td>
</tr>
<tr class="even">
<td style="border:1px solid black;">s_RequestUserAgent</td>
<td style="border:1px solid black;">nvarchar(128)</td>
<td style="border:1px solid black;">NULL</td>
<td style="border:1px solid black;">A ügyfél felhasználói ügynökének fejrésze</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;">s_AuthenticatedState</td>
<td style="border:1px solid black;">nvarchar(64)</td>
<td style="border:1px solid black;">NULL</td>
<td style="border:1px solid black;">A kérelem hitelesítési állapota</td>
</tr>
<tr class="even">
<td style="border:1px solid black;">s_SecureConnectionState</td>
<td style="border:1px solid black;">nvarchar(64)</td>
<td style="border:1px solid black;">NULL</td>
<td style="border:1px solid black;">A kérelem SSL-védelme</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;">s_AuthenticatedId</td>
<td style="border:1px solid black;">nvarchar(128)</td>
<td style="border:1px solid black;">NULL</td>
<td style="border:1px solid black;">A hitelesített felhasználó azonosítója</td>
</tr>
<tr class="even">
<td style="border:1px solid black;">s_ReceivedXrML</td>
<td style="border:1px solid black;">ntext</td>
<td style="border:1px solid black;">NULL</td>
<td style="border:1px solid black;">Az ügyféltől a kérelemben kapott XrML</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;">s_IssuedXrML</td>
<td style="border:1px solid black;">ntext</td>
<td style="border:1px solid black;">NULL</td>
<td style="border:1px solid black;">A kérelemben kiállított XrML-licenc</td>
</tr>
<tr class="even">
<td style="border:1px solid black;">s_Metadata</td>
<td style="border:1px solid black;">ntext</td>
<td style="border:1px solid black;">NULL</td>
<td style="border:1px solid black;">Metaadat</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;">s_SuccessOrFailure</td>
<td style="border:1px solid black;">nvarchar(32)</td>
<td style="border:1px solid black;">NULL</td>
<td style="border:1px solid black;">A kérelem sikeressége vagy sikertelensége</td>
</tr>
<tr class="even">
<td style="border:1px solid black;">s_ErrorInformation</td>
<td style="border:1px solid black;">ntext</td>
<td style="border:1px solid black;">NULL</td>
<td style="border:1px solid black;">Hibaadatok</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;">dt_LogCreateTime</td>
<td style="border:1px solid black;">datetime</td>
<td style="border:1px solid black;">Nem NULL</td>
<td style="border:1px solid black;">A bejegyzés létrehozásának időpontja</td>
</tr>
</tbody>
</table>
  
DRMS\_Log\_Detail  
-----------------
  
A következő táblázatban a naplózási rekordok további adatai szerepelnek. Az XrML-adatok jellemzően ebbe a táblába kerülnek.
  
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
<th style="border:1px solid black;" >Név</th>
<th style="border:1px solid black;" >Adattípus</th>
<th style="border:1px solid black;" >NULL értékek</th>
<th style="border:1px solid black;" >Leírás</th>
</tr>
</thead>
<tbody>
<tr class="odd">
<td style="border:1px solid black;">i_LogDetailID</td>
<td style="border:1px solid black;">int (PK)</td>
<td style="border:1px solid black;">IDENTITY(100,1)</td>
<td style="border:1px solid black;">Belső index</td>
</tr>
<tr class="even">
<td style="border:1px solid black;">i_LogID</td>
<td style="border:1px solid black;">int (külső kulcs)</td>
<td style="border:1px solid black;">Nem NULL (külső kulcs)</td>
<td style="border:1px solid black;">A szülő naplózási rekord azonosítója</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;">s_Name</td>
<td style="border:1px solid black;">nvarchar(128)</td>
<td style="border:1px solid black;">Nem NULL</td>
<td style="border:1px solid black;">A tulajdonság neve</td>
</tr>
<tr class="even">
<td style="border:1px solid black;">s_Value</td>
<td style="border:1px solid black;">ntext</td>
<td style="border:1px solid black;">NULL</td>
<td style="border:1px solid black;">A tulajdonság értéke</td>
</tr>
</tbody>
</table>
  
DRMS\_Log\_Filter  
-----------------
  
A következő táblázat azokat a mezőket tartalmazza, amelyeket a naplózásfigyelő szolgáltatás naplóz.
  
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
<th style="border:1px solid black;" >Név</th>
<th style="border:1px solid black;" >Adattípus</th>
<th style="border:1px solid black;" >NULL értékek</th>
<th style="border:1px solid black;" >Leírás</th>
</tr>
</thead>
<tbody>
<tr class="odd">
<td style="border:1px solid black;">i_ID</td>
<td style="border:1px solid black;">int</td>
<td style="border:1px solid black;">IDENTITY (100,1) Nem NULL</td>
<td style="border:1px solid black;">Belső index</td>
</tr>
<tr class="even">
<td style="border:1px solid black;">s_FieldName</td>
<td style="border:1px solid black;">nvarchar(255)</td>
<td style="border:1px solid black;">Nem NULL</td>
<td style="border:1px solid black;">A mező neve</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;">s_FieldDescription</td>
<td style="border:1px solid black;">nvarchar(1024)</td>
<td style="border:1px solid black;">NULL</td>
<td style="border:1px solid black;">A mező leírása</td>
</tr>
<tr class="even">
<td style="border:1px solid black;">i_IsIncluded</td>
<td style="border:1px solid black;">int</td>
<td style="border:1px solid black;">Nem NULL</td>
<td style="border:1px solid black;">Annak jelzése, hogy engedélyezve van-e a mező naplózása</td>
</tr>
</tbody>
</table>
