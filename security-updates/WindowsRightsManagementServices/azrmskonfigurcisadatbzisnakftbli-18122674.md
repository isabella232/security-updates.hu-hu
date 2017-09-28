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
<td style="border:1px solid black;">ID</td>
<td style="border:1px solid black;">int</td>
<td style="border:1px solid black;">IDENTITY (100,1) Nem NULL</td>
<td style="border:1px solid black;">Belső index</td>
</tr>
<tr class="even">
<td style="border:1px solid black;">Név</td>
<td style="border:1px solid black;">nvarchar(256)</td>
<td style="border:1px solid black;">Nem NULL</td>
<td style="border:1px solid black;">Az alkalmazás neve</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;">VersionMinMajor</td>
<td style="border:1px solid black;">int</td>
<td style="border:1px solid black;">NULL</td>
<td style="border:1px solid black;">Az alkalmazás legkisebb fő verziószáma</td>
</tr>
<tr class="even">
<td style="border:1px solid black;">VersionMinMinor</td>
<td style="border:1px solid black;">int</td>
<td style="border:1px solid black;">NULL</td>
<td style="border:1px solid black;">Az alkalmazás legkisebb alverziószáma</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;">VersionMinBuild</td>
<td style="border:1px solid black;">int</td>
<td style="border:1px solid black;">NULL</td>
<td style="border:1px solid black;">Az alkalmazás legkisebb buildszáma</td>
</tr>
<tr class="even">
<td style="border:1px solid black;">VersionMinRevision</td>
<td style="border:1px solid black;">int</td>
<td style="border:1px solid black;">NULL</td>
<td style="border:1px solid black;">Az alkalmazás legkisebb változatszáma</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;">VersionMaxMajor</td>
<td style="border:1px solid black;">int</td>
<td style="border:1px solid black;">NULL</td>
<td style="border:1px solid black;">Az alkalmazás legnagyobb fő verziószáma</td>
</tr>
<tr class="even">
<td style="border:1px solid black;">VersionMaxMinor</td>
<td style="border:1px solid black;">int</td>
<td style="border:1px solid black;">NULL</td>
<td style="border:1px solid black;">Az alkalmazás legnagyobb alverziószáma</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;">VersionMaxBuild</td>
<td style="border:1px solid black;">int</td>
<td style="border:1px solid black;">NULL</td>
<td style="border:1px solid black;">Az alkalmazás legnagyobb buildszáma</td>
</tr>
<tr class="even">
<td style="border:1px solid black;">VersionMaxRevision</td>
<td style="border:1px solid black;">int</td>
<td style="border:1px solid black;">NULL</td>
<td style="border:1px solid black;">Az alkalmazás legnagyobb változatszáma</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;">Leírás</td>
<td style="border:1px solid black;">nvarchar(256)</td>
<td style="border:1px solid black;">NULL</td>
<td style="border:1px solid black;">Az alkalmazás leírása</td>
</tr>
<tr class="even">
<td style="border:1px solid black;">dt_DateUpdated</td>
<td style="border:1px solid black;">datetime</td>
<td style="border:1px solid black;">NULL</td>
<td style="border:1px solid black;">A frissítés időpontja</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;">dt_DateCreated</td>
<td style="border:1px solid black;">datetime</td>
<td style="border:1px solid black;">NULL</td>
<td style="border:1px solid black;">A létrehozás időpontja</td>
</tr>
</tbody>
</table>
  
DRMS\_AsynchronousQueue  
-----------------------
  
A következő táblázat az üzenetsorral kapcsolatos adatokat sorolja fel.
  
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
<td style="border:1px solid black;">AsyncQueueID</td>
<td style="border:1px solid black;">Int (PK)</td>
<td style="border:1px solid black;">IDENTITY (100,1) Nem NULL</td>
<td style="border:1px solid black;">Belső index</td>
</tr>
<tr class="even">
<td style="border:1px solid black;">QueueName</td>
<td style="border:1px solid black;">nvarchar(256)</td>
<td style="border:1px solid black;">Nem NULL</td>
<td style="border:1px solid black;">Az üzenetsor elérési útja</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;">DateUpdated</td>
<td style="border:1px solid black;">datetime</td>
<td style="border:1px solid black;">NULL</td>
<td style="border:1px solid black;">A frissítés időpontja</td>
</tr>
<tr class="even">
<td style="border:1px solid black;">DateCreated</td>
<td style="border:1px solid black;">datetime</td>
<td style="border:1px solid black;">NULL</td>
<td style="border:1px solid black;">A létrehozás időpontja</td>
</tr>
</tbody>
</table>
  
DRMS\_CaType  
------------
  
A következő táblázat az ügyfélnek kiállított tanúsítvány típúsával kapcsolatos adatokat tartalmazza.
  
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
<td style="border:1px solid black;">ID</td>
<td style="border:1px solid black;">Int (PK)</td>
<td style="border:1px solid black;">Nem NULL</td>
<td style="border:1px solid black;">A tanúsítvány azonosítója</td>
</tr>
<tr class="even">
<td style="border:1px solid black;">TypeName</td>
<td style="border:1px solid black;">nvarchar(256)</td>
<td style="border:1px solid black;">Nem NULL</td>
<td style="border:1px solid black;">Desktop, MobileDevice vagy Server</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;">DateUpdated</td>
<td style="border:1px solid black;">datetime</td>
<td style="border:1px solid black;">NULL</td>
<td style="border:1px solid black;">A frissítés időpontja</td>
</tr>
<tr class="even">
<td style="border:1px solid black;">DateCreated</td>
<td style="border:1px solid black;">datetime</td>
<td style="border:1px solid black;">NULL</td>
<td style="border:1px solid black;">A létrehozás időpontja</td>
</tr>
</tbody>
</table>
  
DRMS\_ClusterConfiguration  
--------------------------
  
A következő táblázat a DRMS\_LicensorCertificate táblában lévő aktuális kiszolgálói licencelői tanúsítvány adatait tartalmazza.
  
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
<td style="border:1px solid black;">CurrentLicensorCertID</td>
<td style="border:1px solid black;">int (külső kulcs)</td>
<td style="border:1px solid black;">NULL</td>
<td style="border:1px solid black;">Az aktív licencelői tanúsítvány</td>
</tr>
<tr class="even">
<td style="border:1px solid black;">DateUpdated</td>
<td style="border:1px solid black;">datetime</td>
<td style="border:1px solid black;">NULL</td>
<td style="border:1px solid black;">A frissítés időpontja</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;">DateCreated</td>
<td style="border:1px solid black;">datetime</td>
<td style="border:1px solid black;">NULL</td>
<td style="border:1px solid black;">A létrehozás időpontja</td>
</tr>
</tbody>
</table>
  
DRMS\_ClusterPolicies  
---------------------
  
A következő táblázat a fürt szabályzatait tároló helyekre vonatkozó adatokat sorolja fel.
  
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
<td style="border:1px solid black;">PolicyID</td>
<td style="border:1px solid black;">Int (PK)</td>
<td style="border:1px solid black;">IDENTITY (100,1) Nem NULL</td>
<td style="border:1px solid black;">A szabályzat azonosítója</td>
</tr>
<tr class="even">
<td style="border:1px solid black;">PolicyName</td>
<td style="border:1px solid black;">nvarchar(64)</td>
<td style="border:1px solid black;">Nem NULL</td>
<td style="border:1px solid black;">A szabályzat neve</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;">PolicyData</td>
<td style="border:1px solid black;">sql_variant</td>
<td style="border:1px solid black;">NULL</td>
<td style="border:1px solid black;">A szabályzat adata</td>
</tr>
<tr class="even">
<td style="border:1px solid black;">DateUpdated</td>
<td style="border:1px solid black;">datetime</td>
<td style="border:1px solid black;">NULL</td>
<td style="border:1px solid black;">A frissítés időpontja</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;">DateCreated</td>
<td style="border:1px solid black;">datetime</td>
<td style="border:1px solid black;">NULL</td>
<td style="border:1px solid black;">A létrehozás időpontja</td>
</tr>
</tbody>
</table>
  
DRMS\_ClusterServer  
-------------------
  
A következő táblázat a fürtbe tartozó kiszolgálókra vonatkozó adatokat sorolja fel.
  
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
<td style="border:1px solid black;">ServerID</td>
<td style="border:1px solid black;">Int (PK)</td>
<td style="border:1px solid black;">IDENTITY (100,1) Nem NULL</td>
<td style="border:1px solid black;">A kiszolgáló azonosítója</td>
</tr>
<tr class="even">
<td style="border:1px solid black;">ServerName.</td>
<td style="border:1px solid black;">nvarchar(256)</td>
<td style="border:1px solid black;">Nincs megadva</td>
<td style="border:1px solid black;">A kiszolgáló számítógépneve</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;">DateUpdated</td>
<td style="border:1px solid black;">datetime</td>
<td style="border:1px solid black;">NULL</td>
<td style="border:1px solid black;">A frissítés időpontja</td>
</tr>
<tr class="even">
<td style="border:1px solid black;">DateCreated</td>
<td style="border:1px solid black;">datetime</td>
<td style="border:1px solid black;">NULL</td>
<td style="border:1px solid black;">A létrehozás időpontja</td>
</tr>
</tbody>
</table>
  
DRMS\_GICExclusionList  
----------------------
  
A következő táblázat a kizárt tartalomvédelmi fióktanúsítványokra vonatkozó adatokat tartalmazza.
  
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
<td style="border:1px solid black;">PublicKeyIndex</td>
<td style="border:1px solid black;">Int (PK)</td>
<td style="border:1px solid black;">IDENTITY (100,1) Nem NULL</td>
<td style="border:1px solid black;">Belső index</td>
</tr>
<tr class="even">
<td style="border:1px solid black;">PublicKey</td>
<td style="border:1px solid black;">PublicKey</td>
<td style="border:1px solid black;">Nem NULL</td>
<td style="border:1px solid black;">A nyilvános kulcs bájtjai</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;">UserID</td>
<td style="border:1px solid black;">int</td>
<td style="border:1px solid black;">NULL</td>
<td style="border:1px solid black;">A felhasználóazonosító indexe</td>
</tr>
<tr class="even">
<td style="border:1px solid black;">ExpirationDate</td>
<td style="border:1px solid black;">datetime</td>
<td style="border:1px solid black;">NULL</td>
<td style="border:1px solid black;">A tartalomvédelmi fióktanúsítvány lejáratának dátuma</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;">Leírás</td>
<td style="border:1px solid black;">nvarchar(256)</td>
<td style="border:1px solid black;">NULL</td>
<td style="border:1px solid black;">A kizárt tartalomvédelmi fióktanúsítvány kulcsához társított NAME (név) érték</td>
</tr>
<tr class="even">
<td style="border:1px solid black;">dt_DateUpdated</td>
<td style="border:1px solid black;">datetime</td>
<td style="border:1px solid black;">Nem NULL</td>
<td style="border:1px solid black;">A frissítés időpontja</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;">dt_DateCreated</td>
<td style="border:1px solid black;">datetime</td>
<td style="border:1px solid black;">Nem NULL</td>
<td style="border:1px solid black;">A létrehozás időpontja</td>
</tr>
</tbody>
</table>
  
DRMS\_LicensorCertificate  
-------------------------
  
A következő táblázat az aktív kiszolgálói licencelői tanúsítványra vonatkozó adatokat tartalmazza.
  
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
<td style="border:1px solid black;">i_CertID</td>
<td style="border:1px solid black;">Int (PK)</td>
<td style="border:1px solid black;">IDENTITY (100,1) Nem NULL</td>
<td style="border:1px solid black;">A szabályzat azonosítója</td>
</tr>
<tr class="even">
<td style="border:1px solid black;">s_CertGUIDType</td>
<td style="border:1px solid black;">nvarchar(64)</td>
<td style="border:1px solid black;">Nem NULL</td>
<td style="border:1px solid black;">A kulcspár-azonosító típusa</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;">s_CertGUID</td>
<td style="border:1px solid black;">nvarchar(128)</td>
<td style="border:1px solid black;">Nem NULL</td>
<td style="border:1px solid black;">A kulcspár-azonosító GUID azonosítója</td>
</tr>
<tr class="even">
<td style="border:1px solid black;">i_CertificateID</td>
<td style="border:1px solid black;">int (külső kulcs)</td>
<td style="border:1px solid black;">Nem NULL</td>
<td style="border:1px solid black;">Az aktuális tanúsítványra hivatkozó mutató</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;">dt_DateUpdated</td>
<td style="border:1px solid black;">datetime</td>
<td style="border:1px solid black;">NULL</td>
<td style="border:1px solid black;">A frissítés időpontja</td>
</tr>
<tr class="even">
<td style="border:1px solid black;">dt_DateCreated</td>
<td style="border:1px solid black;">datetime</td>
<td style="border:1px solid black;">NULL</td>
<td style="border:1px solid black;">A létrehozás időpontja</td>
</tr>
</tbody>
</table>
  
DRMS\_LicensorPrivateKey  
------------------------
  
A következő táblázat az aktív kiszolgálói licencelői tanúsítvány személyes kulcsára vonatkozó adatokat tartalmazza.
  
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
<td style="border:1px solid black;">PrivateKeyID</td>
<td style="border:1px solid black;">Int (PK)</td>
<td style="border:1px solid black;">IDENTITY (100,1) Nem NULL</td>
<td style="border:1px solid black;">Belső index</td>
</tr>
<tr class="even">
<td style="border:1px solid black;">CertGUIDType</td>
<td style="border:1px solid black;">nvarchar(64)</td>
<td style="border:1px solid black;">Nem NULL</td>
<td style="border:1px solid black;">A kulcspár-azonosító típusa</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;">CertGUID</td>
<td style="border:1px solid black;">nvarchar(128)</td>
<td style="border:1px solid black;">Nem NULL</td>
<td style="border:1px solid black;">A kulcspár-azonosító GUID azonosítója</td>
</tr>
<tr class="even">
<td style="border:1px solid black;">PrivateKey</td>
<td style="border:1px solid black;">varbinary(2048)</td>
<td style="border:1px solid black;">NULL</td>
<td style="border:1px solid black;">A kulcs bináris leképezése</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;">CSP</td>
<td style="border:1px solid black;">nvarchar(512)</td>
<td style="border:1px solid black;">NULL</td>
<td style="border:1px solid black;">A kriptográfiai szolgáltató (CSP) neve</td>
</tr>
<tr class="even">
<td style="border:1px solid black;">CSPType</td>
<td style="border:1px solid black;">int</td>
<td style="border:1px solid black;">NULL</td>
<td style="border:1px solid black;">A CSP típusa</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;">KeyContainerName</td>
<td style="border:1px solid black;">nvarchar(512)</td>
<td style="border:1px solid black;">Nincs megadva</td>
<td style="border:1px solid black;">A kulcstároló neve</td>
</tr>
<tr class="even">
<td style="border:1px solid black;">KeyNumber</td>
<td style="border:1px solid black;">int</td>
<td style="border:1px solid black;">NULL</td>
<td style="border:1px solid black;">A kulcs száma</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;">DateUpdated</td>
<td style="border:1px solid black;">datetime</td>
<td style="border:1px solid black;">NULL</td>
<td style="border:1px solid black;">A frissítés időpontja</td>
</tr>
<tr class="even">
<td style="border:1px solid black;">DateCreated</td>
<td style="border:1px solid black;">datetime</td>
<td style="border:1px solid black;">NULL</td>
<td style="border:1px solid black;">A létrehozás időpontja</td>
</tr>
</tbody>
</table>
  
DRMS\_PassportDenyList  
----------------------
  
A következő táblázat azokról a Microsoft® .NET Passport-fiókokról tartalmaz adatokat, amelyektől meg kell tagadni a licencet.
  
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
<td style="border:1px solid black;">DenyID</td>
<td style="border:1px solid black;">Int (PK)</td>
<td style="border:1px solid black;">IDENTITY (100,1) Nem NULL</td>
<td style="border:1px solid black;">Belső index</td>
</tr>
<tr class="even">
<td style="border:1px solid black;">DenyAddressPattern</td>
<td style="border:1px solid black;">nvarchar(500)</td>
<td style="border:1px solid black;">Nem NULL</td>
<td style="border:1px solid black;">Felhasználónév/tartománynév</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;">DateUpdated</td>
<td style="border:1px solid black;">datetime</td>
<td style="border:1px solid black;">NULL</td>
<td style="border:1px solid black;">A frissítés időpontja</td>
</tr>
<tr class="even">
<td style="border:1px solid black;">DateCreated</td>
<td style="border:1px solid black;">datetime</td>
<td style="border:1px solid black;">NULL</td>
<td style="border:1px solid black;">A létrehozás időpontja</td>
</tr>
</tbody>
</table>
  
DRMS\_Plugin  
------------
  
A következő táblázat a beépülő modulokkal kapcsolatos adatokat sorolja fel.
  
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
<td style="border:1px solid black;">PluginID</td>
<td style="border:1px solid black;">Int</td>
<td style="border:1px solid black;">IDENTITY (100,1) Nem NULL</td>
<td style="border:1px solid black;">Belső index</td>
</tr>
<tr class="even">
<td style="border:1px solid black;">PluginTypeID</td>
<td style="border:1px solid black;">int (külső kulcs)</td>
<td style="border:1px solid black;">NULL</td>
<td style="border:1px solid black;">A beépülő modul típusa</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;">NameSpace</td>
<td style="border:1px solid black;">nvarchar(128)</td>
<td style="border:1px solid black;">Nem NULL</td>
<td style="border:1px solid black;">A beépülő modul névtere</td>
</tr>
<tr class="even">
<td style="border:1px solid black;">PluginName</td>
<td style="border:1px solid black;">nvarchar(128)</td>
<td style="border:1px solid black;">Nem NULL</td>
<td style="border:1px solid black;">A beépülő modul neve</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;">Ordinal</td>
<td style="border:1px solid black;">Int</td>
<td style="border:1px solid black;">Nem NULL</td>
<td style="border:1px solid black;">A beépülő modul végrehajtási sorszáma</td>
</tr>
<tr class="even">
<td style="border:1px solid black;">Path</td>
<td style="border:1px solid black;">nvarchar(512)</td>
<td style="border:1px solid black;">Nem NULL</td>
<td style="border:1px solid black;">A DLL-fájl elérési útja</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;">ObjectTypeName</td>
<td style="border:1px solid black;">nvarchar(50)</td>
<td style="border:1px solid black;">NULL</td>
<td style="border:1px solid black;">Használaton kívül</td>
</tr>
<tr class="even">
<td style="border:1px solid black;">DebugMode</td>
<td style="border:1px solid black;">int</td>
<td style="border:1px solid black;">NULL</td>
<td style="border:1px solid black;">Megadja, hogy hibakereső módban fusson-e a beépülő modul</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;">PublicKey</td>
<td style="border:1px solid black;">PublicKey</td>
<td style="border:1px solid black;">NULL</td>
<td style="border:1px solid black;">A beépülő modul nyilvános kulcsa</td>
</tr>
<tr class="even">
<td style="border:1px solid black;">Version</td>
<td style="border:1px solid black;">nvarchar(64)</td>
<td style="border:1px solid black;">NULL</td>
<td style="border:1px solid black;">A beépülő modul verziószáma</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;">DateUpdated</td>
<td style="border:1px solid black;">datetime</td>
<td style="border:1px solid black;">NULL</td>
<td style="border:1px solid black;">A frissítés időpontja</td>
</tr>
<tr class="even">
<td style="border:1px solid black;">DateCreated</td>
<td style="border:1px solid black;">datetime</td>
<td style="border:1px solid black;">NULL</td>
<td style="border:1px solid black;">A létrehozás időpontja</td>
</tr>
</tbody>
</table>
  
DRMS\_AllowedPluginVersions  
---------------------------
  
A következő táblázat az RMS rendszerben megengedett beépülő modulok verzióira vonatkozó adatokat tartalmazza.
  
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
<td style="border:1px solid black;">RowID</td>
<td style="border:1px solid black;">int</td>
<td style="border:1px solid black;">Nem NULL</td>
<td style="border:1px solid black;">Belső index</td>
</tr>
<tr class="even">
<td style="border:1px solid black;">PluginID</td>
<td style="border:1px solid black;">int</td>
<td style="border:1px solid black;">IDENTITY (100,1) Nem NULL</td>
<td style="border:1px solid black;">Belső index</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;">VersionInfo</td>
<td style="border:1px solid black;">nvarchar(64)</td>
<td style="border:1px solid black;">Nincs megadva</td>
<td style="border:1px solid black;">A beépülő modul verziószáma</td>
</tr>
</tbody>
</table>
  
DRMS\_PluginProperties  
----------------------
  
A következő táblázat a beépülő modul tulajdonságaira vonatkozó adatokat tartalmazza.
  
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
<td style="border:1px solid black;">PropertyID</td>
<td style="border:1px solid black;">int</td>
<td style="border:1px solid black;">IDENTITY (100,1) Nem NULL</td>
<td style="border:1px solid black;">Belső index</td>
</tr>
<tr class="even">
<td style="border:1px solid black;">PluginID</td>
<td style="border:1px solid black;">int (külső kulcs)</td>
<td style="border:1px solid black;">NULL</td>
<td style="border:1px solid black;">Annak a beépülő modulnak az azonosítója, amelyhez a tulajdonság tartozik</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;">PropertyName</td>
<td style="border:1px solid black;">nvarchar(256)</td>
<td style="border:1px solid black;">Nem NULL</td>
<td style="border:1px solid black;">Az adott konfigurációs adatot tartalmazó tulajdonság neve</td>
</tr>
<tr class="even">
<td style="border:1px solid black;">PropertyValue</td>
<td style="border:1px solid black;">text</td>
<td style="border:1px solid black;">Nem NULL</td>
<td style="border:1px solid black;">Az adott konfigurációs adatot tartalmazó tulajdonság értéke</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;">DateUpdated</td>
<td style="border:1px solid black;">datetime</td>
<td style="border:1px solid black;">NULL</td>
<td style="border:1px solid black;">A frissítés időpontja</td>
</tr>
<tr class="even">
<td style="border:1px solid black;">DateCreated</td>
<td style="border:1px solid black;">datetime</td>
<td style="border:1px solid black;">NULL</td>
<td style="border:1px solid black;">A létrehozás időpontja</td>
</tr>
</tbody>
</table>
  
DRMS\_PluginType  
----------------
  
A következő táblázat a beépülő modul típusára vonatkozó adatokat tartalmazza.
  
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
<td style="border:1px solid black;">PluginTypeID</td>
<td style="border:1px solid black;">Int (PK)</td>
<td style="border:1px solid black;">Nem NULL</td>
<td style="border:1px solid black;">Belső index</td>
</tr>
<tr class="even">
<td style="border:1px solid black;">PluginTypeName</td>
<td style="border:1px solid black;">nvarchar(256)</td>
<td style="border:1px solid black;">Nem NULL</td>
<td style="border:1px solid black;">A beépülő modul neve</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;">DateUpdated</td>
<td style="border:1px solid black;">datetime</td>
<td style="border:1px solid black;">NULL</td>
<td style="border:1px solid black;">A frissítés időpontja</td>
</tr>
<tr class="even">
<td style="border:1px solid black;">DateCreated</td>
<td style="border:1px solid black;">datetime</td>
<td style="border:1px solid black;">NULL</td>
<td style="border:1px solid black;">A létrehozás időpontja</td>
</tr>
</tbody>
</table>
  
DRMS\_RightsTemplate  
--------------------
  
A következő táblázat a jogmegadási sablonokra vonatkozó adatokat tartalmazza.
  
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
<td style="border:1px solid black;">Guid</td>
<td style="border:1px solid black;">nvarchar(128) (PK)</td>
<td style="border:1px solid black;">Nem NULL</td>
<td style="border:1px solid black;">A jogmegadási sablon GUID azonosítója</td>
</tr>
<tr class="even">
<td style="border:1px solid black;">TemplateData</td>
<td style="border:1px solid black;">ntext</td>
<td style="border:1px solid black;">Nem NULL</td>
<td style="border:1px solid black;">Ez a mező tartalmazza az XrML sablon adatait.</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;">DateUpdated</td>
<td style="border:1px solid black;">datetime</td>
<td style="border:1px solid black;">NULL</td>
<td style="border:1px solid black;">A frissítés időpontja</td>
</tr>
<tr class="even">
<td style="border:1px solid black;">DateCreated</td>
<td style="border:1px solid black;">datetime</td>
<td style="border:1px solid black;">NULL</td>
<td style="border:1px solid black;">A létrehozás időpontja</td>
</tr>
</tbody>
</table>
  
DRMS\_TrustedCertificateAuthorities  
-----------------------------------
  
A következő táblázat a megbízható hitelesítésszolgáltatókra vonatkozó adatokat tartalmazza.
  
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
<td style="border:1px solid black;">ID</td>
<td style="border:1px solid black;">Int (PK)</td>
<td style="border:1px solid black;">IDENTITY (1,1) Nem NULL</td>
<td style="border:1px solid black;">Belső index</td>
</tr>
<tr class="even">
<td style="border:1px solid black;">CertificateID</td>
<td style="border:1px solid black;">int (külső kulcs)</td>
<td style="border:1px solid black;">Nem NULL</td>
<td style="border:1px solid black;">A tanúsítvány azonosítója</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;">CertificateGUID</td>
<td style="border:1px solid black;">nvarchar(128)</td>
<td style="border:1px solid black;">Nem NULL</td>
<td style="border:1px solid black;">A tanúsítvány GUID azonosítója</td>
</tr>
<tr class="even">
<td style="border:1px solid black;">CaTypeID</td>
<td style="border:1px solid black;">int (külső kulcs)</td>
<td style="border:1px solid black;">Nem NULL</td>
<td style="border:1px solid black;">A hitelesítésszolgáltató típusa</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;">DateUpdated</td>
<td style="border:1px solid black;">datetime</td>
<td style="border:1px solid black;">NULL</td>
<td style="border:1px solid black;">A frissítés időpontja</td>
</tr>
<tr class="even">
<td style="border:1px solid black;">DateCreated</td>
<td style="border:1px solid black;">datetime</td>
<td style="border:1px solid black;">NULL</td>
<td style="border:1px solid black;">A létrehozás időpontja</td>
</tr>
</tbody>
</table>
  
DRMS\_TrustedEmailDomains  
-------------------------
  
A következő táblázat az RMS környezetbe tartozó email tartományokra vonatkozó adatokat sorolja fel.
  
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
<td style="border:1px solid black;">Azonosító</td>
<td style="border:1px solid black;">int (PK)</td>
<td style="border:1px solid black;">IDENTITY (100,1) Nem NULL</td>
<td style="border:1px solid black;">Belső index</td>
</tr>
<tr class="even">
<td style="border:1px solid black;">i_TrustedIdentityDomainID</td>
<td style="border:1px solid black;">int (külső kulcs)t</td>
<td style="border:1px solid black;">NULL</td>
<td style="border:1px solid black;">Belső index</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;">s_EmailDomainName</td>
<td style="border:1px solid black;">nvarchar(256)</td>
<td style="border:1px solid black;">NULL</td>
<td style="border:1px solid black;">A megbízható felhasználói tartományokra érvényes e-mail tartománynevek</td>
</tr>
</tbody>
</table>
  
DRMS\_TrustedIdentityDomain  
---------------------------
  
A következő táblázat a megbízható felhasználói tartományokra és a megbízható közzétételi tartományokra vonatkozó adatokat sorolja fel.
  
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
<td style="border:1px solid black;">i_TrustedIdentityDomainID</td>
<td style="border:1px solid black;">Int (PK)</td>
<td style="border:1px solid black;">IDENTITY (100,1) Nem NULL</td>
<td style="border:1px solid black;">Belső index</td>
</tr>
<tr class="even">
<td style="border:1px solid black;">s_DomainType</td>
<td style="border:1px solid black;">nvarchar(64)</td>
<td style="border:1px solid black;">NULL</td>
<td style="border:1px solid black;">A tartomány típusa</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;">CertGUIDType</td>
<td style="border:1px solid black;">nvarchar(64)</td>
<td style="border:1px solid black;">Nem NULL</td>
<td style="border:1px solid black;">A tanúsítvány GUID azonosítójának típusa</td>
</tr>
<tr class="even">
<td style="border:1px solid black;">CertGUID</td>
<td style="border:1px solid black;">nvarchar(128)</td>
<td style="border:1px solid black;">Nem NULL</td>
<td style="border:1px solid black;">A tanúsítvány GUID azonosítója</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;">i_CertificateID</td>
<td style="border:1px solid black;">int (külső kulcs)</td>
<td style="border:1px solid black;">NULL</td>
<td style="border:1px solid black;">A tanúsítvány azonosítója</td>
</tr>
<tr class="even">
<td style="border:1px solid black;">i_allowSID</td>
<td style="border:1px solid black;">int</td>
<td style="border:1px solid black;">Nem NULL</td>
<td style="border:1px solid black;">A tartomány SID azonosítója</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;">S_friendlyname</td>
<td style="border:1px solid black;">nvarchar(255)</td>
<td style="border:1px solid black;">NULL</td>
<td style="border:1px solid black;">A tanúsítvány rövid neve</td>
</tr>
<tr class="even">
<td style="border:1px solid black;">dt_DateUpdated</td>
<td style="border:1px solid black;">datetime</td>
<td style="border:1px solid black;">NULL</td>
<td style="border:1px solid black;">A frissítés időpontja</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;">dt_DateCreated</td>
<td style="border:1px solid black;">datetime</td>
<td style="border:1px solid black;">NULL</td>
<td style="border:1px solid black;">A létrehozás időpontja</td>
</tr>
</tbody>
</table>
  
DRMS\_XrML\_Certificate  
-----------------------
  
A következő táblázat azoknak az XrML kiszolgálói licencelői tanúsítványoknak az adatait tartalmazza, amelyekre a DRMS\_LicensorCertificate tábla hivatkozik. A tanúsítványláncot is hozzárendeli a tanúsítványhoz.
  
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
<td style="border:1px solid black;">i_CertificateID</td>
<td style="border:1px solid black;">Int (PK)</td>
<td style="border:1px solid black;">IDENTITY (100,1) Nem NULL</td>
<td style="border:1px solid black;">Az aktuális tanúsítványra hivatkozó mutató</td>
</tr>
<tr class="even">
<td style="border:1px solid black;">s_Certificate</td>
<td style="border:1px solid black;">ntext</td>
<td style="border:1px solid black;">Nem NULL</td>
<td style="border:1px solid black;">Az aktuális tanúsítványra hivatkozó mutató</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;">i_ParentCertificateID</td>
<td style="border:1px solid black;">int (külső kulcs)</td>
<td style="border:1px solid black;">NULL</td>
<td style="border:1px solid black;">Az aktuális tanúsítványra hivatkozó mutató</td>
</tr>
</tbody>
</table>
