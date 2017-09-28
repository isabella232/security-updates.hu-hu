---
TOCTitle: Az RMS konfigurációs adatbázisának fő táblái
Title: Az RMS konfigurációs adatbázisának fő táblái
ms:assetid: '8f9e15a2-92bc-41f7-a4fd-329567afb142'
ms:contentKeyID: 18122674
ms:mtpsurl: 'https://technet.microsoft.com/hu-hu/library/Cc747676(v=WS.10)'
---

Az RMS konfigurációs adatbázisának fő táblái
============================================

Ez a rész az RMS konfigurációs adatbázisának fő tábláit ismerteti.

DRMS\_ApplicationExclusionList
------------------------------

A következő táblázat a kizárt alkalmazásokkal kapcsolatos adatokat tartalmazza.

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
<td style="border:1px solid black;"><p>ID</p></td>
<td style="border:1px solid black;"><p>int</p></td>
<td style="border:1px solid black;"><p>IDENTITY (100,1) Nem NULL</p></td>
<td style="border:1px solid black;"><p>Belső index</p></td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><p>Név</p></td>
<td style="border:1px solid black;"><p>nvarchar(256)</p></td>
<td style="border:1px solid black;"><p>Nem NULL</p></td>
<td style="border:1px solid black;"><p>Az alkalmazás neve</p></td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><p>VersionMinMajor</p></td>
<td style="border:1px solid black;"><p>int</p></td>
<td style="border:1px solid black;"><p>NULL</p></td>
<td style="border:1px solid black;"><p>Az alkalmazás legkisebb fő verziószáma</p></td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><p>VersionMinMinor</p></td>
<td style="border:1px solid black;"><p>int</p></td>
<td style="border:1px solid black;"><p>NULL</p></td>
<td style="border:1px solid black;"><p>Az alkalmazás legkisebb alverziószáma</p></td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><p>VersionMinBuild</p></td>
<td style="border:1px solid black;"><p>int</p></td>
<td style="border:1px solid black;"><p>NULL</p></td>
<td style="border:1px solid black;"><p>Az alkalmazás legkisebb buildszáma</p></td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><p>VersionMinRevision</p></td>
<td style="border:1px solid black;"><p>int</p></td>
<td style="border:1px solid black;"><p>NULL</p></td>
<td style="border:1px solid black;"><p>Az alkalmazás legkisebb változatszáma</p></td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><p>VersionMaxMajor</p></td>
<td style="border:1px solid black;"><p>int</p></td>
<td style="border:1px solid black;"><p>NULL</p></td>
<td style="border:1px solid black;"><p>Az alkalmazás legnagyobb fő verziószáma</p></td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><p>VersionMaxMinor</p></td>
<td style="border:1px solid black;"><p>int</p></td>
<td style="border:1px solid black;"><p>NULL</p></td>
<td style="border:1px solid black;"><p>Az alkalmazás legnagyobb alverziószáma</p></td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><p>VersionMaxBuild</p></td>
<td style="border:1px solid black;"><p>int</p></td>
<td style="border:1px solid black;"><p>NULL</p></td>
<td style="border:1px solid black;"><p>Az alkalmazás legnagyobb buildszáma</p></td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><p>VersionMaxRevision</p></td>
<td style="border:1px solid black;"><p>int</p></td>
<td style="border:1px solid black;"><p>NULL</p></td>
<td style="border:1px solid black;"><p>Az alkalmazás legnagyobb változatszáma</p></td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><p>Leírás</p></td>
<td style="border:1px solid black;"><p>nvarchar(256)</p></td>
<td style="border:1px solid black;"><p>NULL</p></td>
<td style="border:1px solid black;"><p>Az alkalmazás leírása</p></td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><p>dt_DateUpdated</p></td>
<td style="border:1px solid black;"><p>datetime</p></td>
<td style="border:1px solid black;"><p>NULL</p></td>
<td style="border:1px solid black;"><p>A frissítés időpontja</p></td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><p>dt_DateCreated</p></td>
<td style="border:1px solid black;"><p>datetime</p></td>
<td style="border:1px solid black;"><p>NULL</p></td>
<td style="border:1px solid black;"><p>A létrehozás időpontja</p></td>
</tr>
</tbody>
</table>
  
DRMS\_AsynchronousQueue  
-----------------------
  
A következő táblázat az üzenetsorral kapcsolatos adatokat sorolja fel.
  
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
<td style="border:1px solid black;"><p>AsyncQueueID</p></td>
<td style="border:1px solid black;"><p>Int (PK)</p></td>
<td style="border:1px solid black;"><p>IDENTITY (100,1) Nem NULL</p></td>
<td style="border:1px solid black;"><p>Belső index</p></td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><p>QueueName</p></td>
<td style="border:1px solid black;"><p>nvarchar(256)</p></td>
<td style="border:1px solid black;"><p>Nem NULL</p></td>
<td style="border:1px solid black;"><p>Az üzenetsor elérési útja</p></td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><p>DateUpdated</p></td>
<td style="border:1px solid black;"><p>datetime</p></td>
<td style="border:1px solid black;"><p>NULL</p></td>
<td style="border:1px solid black;"><p>A frissítés időpontja</p></td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><p>DateCreated</p></td>
<td style="border:1px solid black;"><p>datetime</p></td>
<td style="border:1px solid black;"><p>NULL</p></td>
<td style="border:1px solid black;"><p>A létrehozás időpontja</p></td>
</tr>
</tbody>
</table>
  
DRMS\_CaType  
------------
  
A következő táblázat az ügyfélnek kiállított tanúsítvány típúsával kapcsolatos adatokat tartalmazza.
  
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
<td style="border:1px solid black;"><p>ID</p></td>
<td style="border:1px solid black;"><p>Int (PK)</p></td>
<td style="border:1px solid black;"><p>Nem NULL</p></td>
<td style="border:1px solid black;"><p>A tanúsítvány azonosítója</p></td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><p>TypeName</p></td>
<td style="border:1px solid black;"><p>nvarchar(256)</p></td>
<td style="border:1px solid black;"><p>Nem NULL</p></td>
<td style="border:1px solid black;"><p>Desktop, MobileDevice vagy Server</p></td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><p>DateUpdated</p></td>
<td style="border:1px solid black;"><p>datetime</p></td>
<td style="border:1px solid black;"><p>NULL</p></td>
<td style="border:1px solid black;"><p>A frissítés időpontja</p></td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><p>DateCreated</p></td>
<td style="border:1px solid black;"><p>datetime</p></td>
<td style="border:1px solid black;"><p>NULL</p></td>
<td style="border:1px solid black;"><p>A létrehozás időpontja</p></td>
</tr>
</tbody>
</table>
  
DRMS\_ClusterConfiguration  
--------------------------
  
A következő táblázat a DRMS\_LicensorCertificate táblában lévő aktuális kiszolgálói licencelői tanúsítvány adatait tartalmazza.
  
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
<td style="border:1px solid black;"><p>CurrentLicensorCertID</p></td>
<td style="border:1px solid black;"><p>int (külső kulcs)</p></td>
<td style="border:1px solid black;"><p>NULL</p></td>
<td style="border:1px solid black;"><p>Az aktív licencelői tanúsítvány</p></td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><p>DateUpdated</p></td>
<td style="border:1px solid black;"><p>datetime</p></td>
<td style="border:1px solid black;"><p>NULL</p></td>
<td style="border:1px solid black;"><p>A frissítés időpontja</p></td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><p>DateCreated</p></td>
<td style="border:1px solid black;"><p>datetime</p></td>
<td style="border:1px solid black;"><p>NULL</p></td>
<td style="border:1px solid black;"><p>A létrehozás időpontja</p></td>
</tr>
</tbody>
</table>
  
DRMS\_ClusterPolicies  
---------------------
  
A következő táblázat a fürt szabályzatait tároló helyekre vonatkozó adatokat sorolja fel.
  
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
<td style="border:1px solid black;"><p>PolicyID</p></td>
<td style="border:1px solid black;"><p>Int (PK)</p></td>
<td style="border:1px solid black;"><p>IDENTITY (100,1) Nem NULL</p></td>
<td style="border:1px solid black;"><p>A szabályzat azonosítója</p></td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><p>PolicyName</p></td>
<td style="border:1px solid black;"><p>nvarchar(64)</p></td>
<td style="border:1px solid black;"><p>Nem NULL</p></td>
<td style="border:1px solid black;"><p>A szabályzat neve</p></td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><p>PolicyData</p></td>
<td style="border:1px solid black;"><p>sql_variant</p></td>
<td style="border:1px solid black;"><p>NULL</p></td>
<td style="border:1px solid black;"><p>A szabályzat adata</p></td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><p>DateUpdated</p></td>
<td style="border:1px solid black;"><p>datetime</p></td>
<td style="border:1px solid black;"><p>NULL</p></td>
<td style="border:1px solid black;"><p>A frissítés időpontja</p></td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><p>DateCreated</p></td>
<td style="border:1px solid black;"><p>datetime</p></td>
<td style="border:1px solid black;"><p>NULL</p></td>
<td style="border:1px solid black;"><p>A létrehozás időpontja</p></td>
</tr>
</tbody>
</table>
  
DRMS\_ClusterServer  
-------------------
  
A következő táblázat a fürtbe tartozó kiszolgálókra vonatkozó adatokat sorolja fel.
  
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
<td style="border:1px solid black;"><p>ServerID</p></td>
<td style="border:1px solid black;"><p>Int (PK)</p></td>
<td style="border:1px solid black;"><p>IDENTITY (100,1) Nem NULL</p></td>
<td style="border:1px solid black;"><p>A kiszolgáló azonosítója</p></td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><p>ServerName.</p></td>
<td style="border:1px solid black;"><p>nvarchar(256)</p></td>
<td style="border:1px solid black;"><p>Nincs megadva</p></td>
<td style="border:1px solid black;"><p>A kiszolgáló számítógépneve</p></td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><p>DateUpdated</p></td>
<td style="border:1px solid black;"><p>datetime</p></td>
<td style="border:1px solid black;"><p>NULL</p></td>
<td style="border:1px solid black;"><p>A frissítés időpontja</p></td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><p>DateCreated</p></td>
<td style="border:1px solid black;"><p>datetime</p></td>
<td style="border:1px solid black;"><p>NULL</p></td>
<td style="border:1px solid black;"><p>A létrehozás időpontja</p></td>
</tr>
</tbody>
</table>
  
DRMS\_GICExclusionList  
----------------------
  
A következő táblázat a kizárt tartalomvédelmi fióktanúsítványokra vonatkozó adatokat tartalmazza.
  
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
<td style="border:1px solid black;"><p>PublicKeyIndex</p></td>
<td style="border:1px solid black;"><p>Int (PK)</p></td>
<td style="border:1px solid black;"><p>IDENTITY (100,1) Nem NULL</p></td>
<td style="border:1px solid black;"><p>Belső index</p></td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><p>PublicKey</p></td>
<td style="border:1px solid black;"><p>PublicKey</p></td>
<td style="border:1px solid black;"><p>Nem NULL</p></td>
<td style="border:1px solid black;"><p>A nyilvános kulcs bájtjai</p></td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><p>UserID</p></td>
<td style="border:1px solid black;"><p>int</p></td>
<td style="border:1px solid black;"><p>NULL</p></td>
<td style="border:1px solid black;"><p>A felhasználóazonosító indexe</p></td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><p>ExpirationDate</p></td>
<td style="border:1px solid black;"><p>datetime</p></td>
<td style="border:1px solid black;"><p>NULL</p></td>
<td style="border:1px solid black;"><p>A tartalomvédelmi fióktanúsítvány lejáratának dátuma</p></td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><p>Leírás</p></td>
<td style="border:1px solid black;"><p>nvarchar(256)</p></td>
<td style="border:1px solid black;"><p>NULL</p></td>
<td style="border:1px solid black;"><p>A kizárt tartalomvédelmi fióktanúsítvány kulcsához társított NAME (név) érték</p></td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><p>dt_DateUpdated</p></td>
<td style="border:1px solid black;"><p>datetime</p></td>
<td style="border:1px solid black;"><p>Nem NULL</p></td>
<td style="border:1px solid black;"><p>A frissítés időpontja</p></td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><p>dt_DateCreated</p></td>
<td style="border:1px solid black;"><p>datetime</p></td>
<td style="border:1px solid black;"><p>Nem NULL</p></td>
<td style="border:1px solid black;"><p>A létrehozás időpontja</p></td>
</tr>
</tbody>
</table>
  
DRMS\_LicensorCertificate  
-------------------------
  
A következő táblázat az aktív kiszolgálói licencelői tanúsítványra vonatkozó adatokat tartalmazza.
  
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
<td style="border:1px solid black;"><p>i_CertID</p></td>
<td style="border:1px solid black;"><p>Int (PK)</p></td>
<td style="border:1px solid black;"><p>IDENTITY (100,1) Nem NULL</p></td>
<td style="border:1px solid black;"><p>A szabályzat azonosítója</p></td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><p>s_CertGUIDType</p></td>
<td style="border:1px solid black;"><p>nvarchar(64)</p></td>
<td style="border:1px solid black;"><p>Nem NULL</p></td>
<td style="border:1px solid black;"><p>A kulcspár-azonosító típusa</p></td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><p>s_CertGUID</p></td>
<td style="border:1px solid black;"><p>nvarchar(128)</p></td>
<td style="border:1px solid black;"><p>Nem NULL</p></td>
<td style="border:1px solid black;"><p>A kulcspár-azonosító GUID azonosítója</p></td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><p>i_CertificateID</p></td>
<td style="border:1px solid black;"><p>int (külső kulcs)</p></td>
<td style="border:1px solid black;"><p>Nem NULL</p></td>
<td style="border:1px solid black;"><p>Az aktuális tanúsítványra hivatkozó mutató</p></td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><p>dt_DateUpdated</p></td>
<td style="border:1px solid black;"><p>datetime</p></td>
<td style="border:1px solid black;"><p>NULL</p></td>
<td style="border:1px solid black;"><p>A frissítés időpontja</p></td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><p>dt_DateCreated</p></td>
<td style="border:1px solid black;"><p>datetime</p></td>
<td style="border:1px solid black;"><p>NULL</p></td>
<td style="border:1px solid black;"><p>A létrehozás időpontja</p></td>
</tr>
</tbody>
</table>
  
DRMS\_LicensorPrivateKey  
------------------------
  
A következő táblázat az aktív kiszolgálói licencelői tanúsítvány személyes kulcsára vonatkozó adatokat tartalmazza.
  
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
<td style="border:1px solid black;"><p>PrivateKeyID</p></td>
<td style="border:1px solid black;"><p>Int (PK)</p></td>
<td style="border:1px solid black;"><p>IDENTITY (100,1) Nem NULL</p></td>
<td style="border:1px solid black;"><p>Belső index</p></td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><p>CertGUIDType</p></td>
<td style="border:1px solid black;"><p>nvarchar(64)</p></td>
<td style="border:1px solid black;"><p>Nem NULL</p></td>
<td style="border:1px solid black;"><p>A kulcspár-azonosító típusa</p></td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><p>CertGUID</p></td>
<td style="border:1px solid black;"><p>nvarchar(128)</p></td>
<td style="border:1px solid black;"><p>Nem NULL</p></td>
<td style="border:1px solid black;"><p>A kulcspár-azonosító GUID azonosítója</p></td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><p>PrivateKey</p></td>
<td style="border:1px solid black;"><p>varbinary(2048)</p></td>
<td style="border:1px solid black;"><p>NULL</p></td>
<td style="border:1px solid black;"><p>A kulcs bináris leképezése</p></td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><p>CSP</p></td>
<td style="border:1px solid black;"><p>nvarchar(512)</p></td>
<td style="border:1px solid black;"><p>NULL</p></td>
<td style="border:1px solid black;"><p>A kriptográfiai szolgáltató (CSP) neve</p></td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><p>CSPType</p></td>
<td style="border:1px solid black;"><p>int</p></td>
<td style="border:1px solid black;"><p>NULL</p></td>
<td style="border:1px solid black;"><p>A CSP típusa</p></td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><p>KeyContainerName</p></td>
<td style="border:1px solid black;"><p>nvarchar(512)</p></td>
<td style="border:1px solid black;"><p>Nincs megadva</p></td>
<td style="border:1px solid black;"><p>A kulcstároló neve</p></td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><p>KeyNumber</p></td>
<td style="border:1px solid black;"><p>int</p></td>
<td style="border:1px solid black;"><p>NULL</p></td>
<td style="border:1px solid black;"><p>A kulcs száma</p></td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><p>DateUpdated</p></td>
<td style="border:1px solid black;"><p>datetime</p></td>
<td style="border:1px solid black;"><p>NULL</p></td>
<td style="border:1px solid black;"><p>A frissítés időpontja</p></td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><p>DateCreated</p></td>
<td style="border:1px solid black;"><p>datetime</p></td>
<td style="border:1px solid black;"><p>NULL</p></td>
<td style="border:1px solid black;"><p>A létrehozás időpontja</p></td>
</tr>
</tbody>
</table>
  
DRMS\_PassportDenyList  
----------------------
  
A következő táblázat azokról a Microsoft® .NET Passport-fiókokról tartalmaz adatokat, amelyektől meg kell tagadni a licencet.
  
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
<td style="border:1px solid black;"><p>DenyID</p></td>
<td style="border:1px solid black;"><p>Int (PK)</p></td>
<td style="border:1px solid black;"><p>IDENTITY (100,1) Nem NULL</p></td>
<td style="border:1px solid black;"><p>Belső index</p></td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><p>DenyAddressPattern</p></td>
<td style="border:1px solid black;"><p>nvarchar(500)</p></td>
<td style="border:1px solid black;"><p>Nem NULL</p></td>
<td style="border:1px solid black;"><p>Felhasználónév/tartománynév</p></td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><p>DateUpdated</p></td>
<td style="border:1px solid black;"><p>datetime</p></td>
<td style="border:1px solid black;"><p>NULL</p></td>
<td style="border:1px solid black;"><p>A frissítés időpontja</p></td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><p>DateCreated</p></td>
<td style="border:1px solid black;"><p>datetime</p></td>
<td style="border:1px solid black;"><p>NULL</p></td>
<td style="border:1px solid black;"><p>A létrehozás időpontja</p></td>
</tr>
</tbody>
</table>
  
DRMS\_Plugin  
------------
  
A következő táblázat a beépülő modulokkal kapcsolatos adatokat sorolja fel.
  
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
<td style="border:1px solid black;"><p>PluginID</p></td>
<td style="border:1px solid black;"><p>Int</p></td>
<td style="border:1px solid black;"><p>IDENTITY (100,1) Nem NULL</p></td>
<td style="border:1px solid black;"><p>Belső index</p></td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><p>PluginTypeID</p></td>
<td style="border:1px solid black;"><p>int (külső kulcs)</p></td>
<td style="border:1px solid black;"><p>NULL</p></td>
<td style="border:1px solid black;"><p>A beépülő modul típusa</p></td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><p>NameSpace</p></td>
<td style="border:1px solid black;"><p>nvarchar(128)</p></td>
<td style="border:1px solid black;"><p>Nem NULL</p></td>
<td style="border:1px solid black;"><p>A beépülő modul névtere</p></td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><p>PluginName</p></td>
<td style="border:1px solid black;"><p>nvarchar(128)</p></td>
<td style="border:1px solid black;"><p>Nem NULL</p></td>
<td style="border:1px solid black;"><p>A beépülő modul neve</p></td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><p>Ordinal</p></td>
<td style="border:1px solid black;"><p>Int</p></td>
<td style="border:1px solid black;"><p>Nem NULL</p></td>
<td style="border:1px solid black;"><p>A beépülő modul végrehajtási sorszáma</p></td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><p>Path</p></td>
<td style="border:1px solid black;"><p>nvarchar(512)</p></td>
<td style="border:1px solid black;"><p>Nem NULL</p></td>
<td style="border:1px solid black;"><p>A DLL-fájl elérési útja</p></td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><p>ObjectTypeName</p></td>
<td style="border:1px solid black;"><p>nvarchar(50)</p></td>
<td style="border:1px solid black;"><p>NULL</p></td>
<td style="border:1px solid black;"><p>Használaton kívül</p></td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><p>DebugMode</p></td>
<td style="border:1px solid black;"><p>int</p></td>
<td style="border:1px solid black;"><p>NULL</p></td>
<td style="border:1px solid black;"><p>Megadja, hogy hibakereső módban fusson-e a beépülő modul</p></td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><p>PublicKey</p></td>
<td style="border:1px solid black;"><p>PublicKey</p></td>
<td style="border:1px solid black;"><p>NULL</p></td>
<td style="border:1px solid black;"><p>A beépülő modul nyilvános kulcsa</p></td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><p>Version</p></td>
<td style="border:1px solid black;"><p>nvarchar(64)</p></td>
<td style="border:1px solid black;"><p>NULL</p></td>
<td style="border:1px solid black;"><p>A beépülő modul verziószáma</p></td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><p>DateUpdated</p></td>
<td style="border:1px solid black;"><p>datetime</p></td>
<td style="border:1px solid black;"><p>NULL</p></td>
<td style="border:1px solid black;"><p>A frissítés időpontja</p></td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><p>DateCreated</p></td>
<td style="border:1px solid black;"><p>datetime</p></td>
<td style="border:1px solid black;"><p>NULL</p></td>
<td style="border:1px solid black;"><p>A létrehozás időpontja</p></td>
</tr>
</tbody>
</table>
  
DRMS\_AllowedPluginVersions  
---------------------------
  
A következő táblázat az RMS rendszerben megengedett beépülő modulok verzióira vonatkozó adatokat tartalmazza.
  
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
<td style="border:1px solid black;"><p>RowID</p></td>
<td style="border:1px solid black;"><p>int</p></td>
<td style="border:1px solid black;"><p>Nem NULL</p></td>
<td style="border:1px solid black;"><p>Belső index</p></td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><p>PluginID</p></td>
<td style="border:1px solid black;"><p>int</p></td>
<td style="border:1px solid black;"><p>IDENTITY (100,1) Nem NULL</p></td>
<td style="border:1px solid black;"><p>Belső index</p></td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><p>VersionInfo</p></td>
<td style="border:1px solid black;"><p>nvarchar(64)</p></td>
<td style="border:1px solid black;"><p>Nincs megadva</p></td>
<td style="border:1px solid black;"><p>A beépülő modul verziószáma</p></td>
</tr>
</tbody>
</table>
  
DRMS\_PluginProperties  
----------------------
  
A következő táblázat a beépülő modul tulajdonságaira vonatkozó adatokat tartalmazza.
  
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
<td style="border:1px solid black;"><p>PropertyID</p></td>
<td style="border:1px solid black;"><p>int</p></td>
<td style="border:1px solid black;"><p>IDENTITY (100,1) Nem NULL</p></td>
<td style="border:1px solid black;"><p>Belső index</p></td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><p>PluginID</p></td>
<td style="border:1px solid black;"><p>int (külső kulcs)</p></td>
<td style="border:1px solid black;"><p>NULL</p></td>
<td style="border:1px solid black;"><p>Annak a beépülő modulnak az azonosítója, amelyhez a tulajdonság tartozik</p></td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><p>PropertyName</p></td>
<td style="border:1px solid black;"><p>nvarchar(256)</p></td>
<td style="border:1px solid black;"><p>Nem NULL</p></td>
<td style="border:1px solid black;"><p>Az adott konfigurációs adatot tartalmazó tulajdonság neve</p></td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><p>PropertyValue</p></td>
<td style="border:1px solid black;"><p>text</p></td>
<td style="border:1px solid black;"><p>Nem NULL</p></td>
<td style="border:1px solid black;"><p>Az adott konfigurációs adatot tartalmazó tulajdonság értéke</p></td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><p>DateUpdated</p></td>
<td style="border:1px solid black;"><p>datetime</p></td>
<td style="border:1px solid black;"><p>NULL</p></td>
<td style="border:1px solid black;"><p>A frissítés időpontja</p></td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><p>DateCreated</p></td>
<td style="border:1px solid black;"><p>datetime</p></td>
<td style="border:1px solid black;"><p>NULL</p></td>
<td style="border:1px solid black;"><p>A létrehozás időpontja</p></td>
</tr>
</tbody>
</table>
  
DRMS\_PluginType  
----------------
  
A következő táblázat a beépülő modul típusára vonatkozó adatokat tartalmazza.
  
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
<td style="border:1px solid black;"><p>PluginTypeID</p></td>
<td style="border:1px solid black;"><p>Int (PK)</p></td>
<td style="border:1px solid black;"><p>Nem NULL</p></td>
<td style="border:1px solid black;"><p>Belső index</p></td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><p>PluginTypeName</p></td>
<td style="border:1px solid black;"><p>nvarchar(256)</p></td>
<td style="border:1px solid black;"><p>Nem NULL</p></td>
<td style="border:1px solid black;"><p>A beépülő modul neve</p></td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><p>DateUpdated</p></td>
<td style="border:1px solid black;"><p>datetime</p></td>
<td style="border:1px solid black;"><p>NULL</p></td>
<td style="border:1px solid black;"><p>A frissítés időpontja</p></td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><p>DateCreated</p></td>
<td style="border:1px solid black;"><p>datetime</p></td>
<td style="border:1px solid black;"><p>NULL</p></td>
<td style="border:1px solid black;"><p>A létrehozás időpontja</p></td>
</tr>
</tbody>
</table>
  
DRMS\_RightsTemplate  
--------------------
  
A következő táblázat a jogmegadási sablonokra vonatkozó adatokat tartalmazza.
  
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
<td style="border:1px solid black;"><p>Guid</p></td>
<td style="border:1px solid black;"><p>nvarchar(128) (PK)</p></td>
<td style="border:1px solid black;"><p>Nem NULL</p></td>
<td style="border:1px solid black;"><p>A jogmegadási sablon GUID azonosítója</p></td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><p>TemplateData</p></td>
<td style="border:1px solid black;"><p>ntext</p></td>
<td style="border:1px solid black;"><p>Nem NULL</p></td>
<td style="border:1px solid black;"><p>Ez a mező tartalmazza az XrML sablon adatait.</p></td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><p>DateUpdated</p></td>
<td style="border:1px solid black;"><p>datetime</p></td>
<td style="border:1px solid black;"><p>NULL</p></td>
<td style="border:1px solid black;"><p>A frissítés időpontja</p></td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><p>DateCreated</p></td>
<td style="border:1px solid black;"><p>datetime</p></td>
<td style="border:1px solid black;"><p>NULL</p></td>
<td style="border:1px solid black;"><p>A létrehozás időpontja</p></td>
</tr>
</tbody>
</table>
  
DRMS\_TrustedCertificateAuthorities  
-----------------------------------
  
A következő táblázat a megbízható hitelesítésszolgáltatókra vonatkozó adatokat tartalmazza.
  
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
<td style="border:1px solid black;"><p>ID</p></td>
<td style="border:1px solid black;"><p>Int (PK)</p></td>
<td style="border:1px solid black;"><p>IDENTITY (1,1) Nem NULL</p></td>
<td style="border:1px solid black;"><p>Belső index</p></td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><p>CertificateID</p></td>
<td style="border:1px solid black;"><p>int (külső kulcs)</p></td>
<td style="border:1px solid black;"><p>Nem NULL</p></td>
<td style="border:1px solid black;"><p>A tanúsítvány azonosítója</p></td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><p>CertificateGUID</p></td>
<td style="border:1px solid black;"><p>nvarchar(128)</p></td>
<td style="border:1px solid black;"><p>Nem NULL</p></td>
<td style="border:1px solid black;"><p>A tanúsítvány GUID azonosítója</p></td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><p>CaTypeID</p></td>
<td style="border:1px solid black;"><p>int (külső kulcs)</p></td>
<td style="border:1px solid black;"><p>Nem NULL</p></td>
<td style="border:1px solid black;"><p>A hitelesítésszolgáltató típusa</p></td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><p>DateUpdated</p></td>
<td style="border:1px solid black;"><p>datetime</p></td>
<td style="border:1px solid black;"><p>NULL</p></td>
<td style="border:1px solid black;"><p>A frissítés időpontja</p></td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><p>DateCreated</p></td>
<td style="border:1px solid black;"><p>datetime</p></td>
<td style="border:1px solid black;"><p>NULL</p></td>
<td style="border:1px solid black;"><p>A létrehozás időpontja</p></td>
</tr>
</tbody>
</table>
  
DRMS\_TrustedEmailDomains  
-------------------------
  
A következő táblázat az RMS környezetbe tartozó email tartományokra vonatkozó adatokat sorolja fel.
  
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
<td style="border:1px solid black;"><p>Azonosító</p></td>
<td style="border:1px solid black;"><p>int (PK)</p></td>
<td style="border:1px solid black;"><p>IDENTITY (100,1) Nem NULL</p></td>
<td style="border:1px solid black;"><p>Belső index</p></td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><p>i_TrustedIdentityDomainID</p></td>
<td style="border:1px solid black;"><p>int (külső kulcs)t</p></td>
<td style="border:1px solid black;"><p>NULL</p></td>
<td style="border:1px solid black;"><p>Belső index</p></td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><p>s_EmailDomainName</p></td>
<td style="border:1px solid black;"><p>nvarchar(256)</p></td>
<td style="border:1px solid black;"><p>NULL</p></td>
<td style="border:1px solid black;"><p>A megbízható felhasználói tartományokra érvényes e-mail tartománynevek</p></td>
</tr>
</tbody>
</table>
  
DRMS\_TrustedIdentityDomain  
---------------------------
  
A következő táblázat a megbízható felhasználói tartományokra és a megbízható közzétételi tartományokra vonatkozó adatokat sorolja fel.
  
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
<td style="border:1px solid black;"><p>i_TrustedIdentityDomainID</p></td>
<td style="border:1px solid black;"><p>Int (PK)</p></td>
<td style="border:1px solid black;"><p>IDENTITY (100,1) Nem NULL</p></td>
<td style="border:1px solid black;"><p>Belső index</p></td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><p>s_DomainType</p></td>
<td style="border:1px solid black;"><p>nvarchar(64)</p></td>
<td style="border:1px solid black;"><p>NULL</p></td>
<td style="border:1px solid black;"><p>A tartomány típusa</p></td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><p>CertGUIDType</p></td>
<td style="border:1px solid black;"><p>nvarchar(64)</p></td>
<td style="border:1px solid black;"><p>Nem NULL</p></td>
<td style="border:1px solid black;"><p>A tanúsítvány GUID azonosítójának típusa</p></td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><p>CertGUID</p></td>
<td style="border:1px solid black;"><p>nvarchar(128)</p></td>
<td style="border:1px solid black;"><p>Nem NULL</p></td>
<td style="border:1px solid black;"><p>A tanúsítvány GUID azonosítója</p></td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><p>i_CertificateID</p></td>
<td style="border:1px solid black;"><p>int (külső kulcs)</p></td>
<td style="border:1px solid black;"><p>NULL</p></td>
<td style="border:1px solid black;"><p>A tanúsítvány azonosítója</p></td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><p>i_allowSID</p></td>
<td style="border:1px solid black;"><p>int</p></td>
<td style="border:1px solid black;"><p>Nem NULL</p></td>
<td style="border:1px solid black;"><p>A tartomány SID azonosítója</p></td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><p>S_friendlyname</p></td>
<td style="border:1px solid black;"><p>nvarchar(255)</p></td>
<td style="border:1px solid black;"><p>NULL</p></td>
<td style="border:1px solid black;"><p>A tanúsítvány rövid neve</p></td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><p>dt_DateUpdated</p></td>
<td style="border:1px solid black;"><p>datetime</p></td>
<td style="border:1px solid black;"><p>NULL</p></td>
<td style="border:1px solid black;"><p>A frissítés időpontja</p></td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><p>dt_DateCreated</p></td>
<td style="border:1px solid black;"><p>datetime</p></td>
<td style="border:1px solid black;"><p>NULL</p></td>
<td style="border:1px solid black;"><p>A létrehozás időpontja</p></td>
</tr>
</tbody>
</table>
  
DRMS\_XrML\_Certificate  
-----------------------
  
A következő táblázat azoknak az XrML kiszolgálói licencelői tanúsítványoknak az adatait tartalmazza, amelyekre a DRMS\_LicensorCertificate tábla hivatkozik. A tanúsítványláncot is hozzárendeli a tanúsítványhoz.
  
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
<td style="border:1px solid black;"><p>i_CertificateID</p></td>
<td style="border:1px solid black;"><p>Int (PK)</p></td>
<td style="border:1px solid black;"><p>IDENTITY (100,1) Nem NULL</p></td>
<td style="border:1px solid black;"><p>Az aktuális tanúsítványra hivatkozó mutató</p></td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><p>s_Certificate</p></td>
<td style="border:1px solid black;"><p>ntext</p></td>
<td style="border:1px solid black;"><p>Nem NULL</p></td>
<td style="border:1px solid black;"><p>Az aktuális tanúsítványra hivatkozó mutató</p></td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><p>i_ParentCertificateID</p></td>
<td style="border:1px solid black;"><p>int (külső kulcs)</p></td>
<td style="border:1px solid black;"><p>NULL</p></td>
<td style="border:1px solid black;"><p>Az aktuális tanúsítványra hivatkozó mutató</p></td>
</tr>
</tbody>
</table>
