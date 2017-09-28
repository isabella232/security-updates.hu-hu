---
TOCTitle: Internet Information Services
Title: Internet Information Services
ms:assetid: 'bd4dc69f-1e4e-4e95-9ae2-c925d8a14d4c'
ms:contentKeyID: 18122650
ms:mtpsurl: 'https://technet.microsoft.com/hu-hu/library/Cc747649(v=WS.10)'
---

Internet Information Services
=============================

Az RMS elsődleges szolgáltatásai ASP .NET-webszolgáltatások formájában vannak megvalósítva. Ezek a webszolgáltatások a Microsoft® Internet Information Services (IIS) szolgáltatáson futnak. A kiszolgáló létesítése során az RMS virtuális könyvtárakat hoz létre az IIS szolgáltatásban. A webszolgáltatások alkalmazásfájljai a virtuális könyvtárakba vannak telepítve.

A kiszolgáló létesítésekor a kiszolgálón létező webhelyek listájából kiválasztható az a webhely, amelyen el kívánja helyezni a virtuális könyvtárakat. A kiszolgáló létesítése előtt érdemes lehet létrehozni egy külön webhelyet az RMS számára. Ekkor az RMS-telepítésre jellemző hitelesítési és hozzáférési korlátozásokat állíthat be.

A webszolgáltatások fájljainak és a virtuális könyvtáraknak a tulajdonosi hozzáférés-szabályozási listája (DACL) alapértelmezés szerint megakadályozza, hogy illetéktelenek hozzáférhessenek a funkcióikhoz. A következő hozzáférés-szabályozási bejegyzések (ACE) vannak ezekre beállítva:

-   A Rendszergazdák csoport teljes jogosultsággal rendelkezik.
-   A helyi rendszer teljes jogosultsággal rendelkezik.
-   Az RMS szolgáltatás csoport Olvasás és végrehajtás engedéllyel rendelkezik
-   A vendégek és a felhasználók engedélyei: Olvasás és végrehajtás, Mappa tartalmának listázása, Olvasás.
-   A névtelen hozzáférés le van tiltva.

Az alábbi táblázat az IIS szolgáltatásban létrejövő virtuális könyvtárakat, valamint a virtuális könyvtárakba telepített szolgáltatásokat sorolja fel.

###  

 
<table style="border:1px solid black;">
<colgroup>
<col width="33%" />
<col width="33%" />
<col width="33%" />
</colgroup>
<thead>
<tr class="header">
<th>Virtuális könyvtár</th>
<th>Szolgáltatás</th>
<th>Webszolgáltatási fájl</th>
</tr>
</thead>
<tbody>
<tr class="odd">
<td style="border:1px solid black;">_wmcs</td>
<td style="border:1px solid black;">Ez az RMS-fürt felügyeleti virtuális könyvtára.</td>
<td style="border:1px solid black;">Nincs ilyen.</td>
</tr>
<tr class="even">
<td style="border:1px solid black;">Certification</td>
<td style="border:1px solid black;">Ez a virtuális könyvtár az RMS tanúsítási műveleteihez szükséges szolgáltatásokat tartalmazza.</td>
<td style="border:1px solid black;">Nincs ilyen.</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"> </td>
<td style="border:1px solid black;">Aktiválási proxy</td>
<td style="border:1px solid black;">Activation.asmx</td>
</tr>
<tr class="even">
<td style="border:1px solid black;"> </td>
<td style="border:1px solid black;">Fióktanúsítás</td>
<td style="border:1px solid black;">Certification.asmx</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"> </td>
<td style="border:1px solid black;">Előtanúsítás</td>
<td style="border:1px solid black;">Precertification.asmx</td>
</tr>
<tr class="even">
<td style="border:1px solid black;"> </td>
<td style="border:1px solid black;">Szolgáltatáslokátor</td>
<td style="border:1px solid black;">ServiceLocator.asmx</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"> </td>
<td style="border:1px solid black;">Kiszolgáló</td>
<td style="border:1px solid black;">Server.asmx</td>
</tr>
<tr class="even">
<td style="border:1px solid black;"> </td>
<td style="border:1px solid black;">Kiszolgálótanúsítás</td>
<td style="border:1px solid black;">ServerCertification.asmx</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"> </td>
<td style="border:1px solid black;">Mobil eszköz tanúsítása</td>
<td style="border:1px solid black;">MobileDeviceCertfication.asmx</td>
</tr>
<tr class="even">
<td style="border:1px solid black;"> </td>
<td style="border:1px solid black;">Igénylés</td>
<td style="border:1px solid black;">SubEnrollService.asmx</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;">Licencing</td>
<td style="border:1px solid black;">Ez a virtuális könyvtár az RMS licencelési műveleteihez szükséges szolgáltatásokat tartalmazza.</td>
<td style="border:1px solid black;">Nincs ilyen.</td>
</tr>
<tr class="even">
<td style="border:1px solid black;"> </td>
<td style="border:1px solid black;">Licencelés</td>
<td style="border:1px solid black;">License.asmx</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"> </td>
<td style="border:1px solid black;">Közzététel</td>
<td style="border:1px solid black;">Publish.asmx</td>
</tr>
<tr class="even">
<td style="border:1px solid black;"> </td>
<td style="border:1px solid black;">Kiszolgáló</td>
<td style="border:1px solid black;">Server.asmx</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"> </td>
<td style="border:1px solid black;">Szolgáltatáslokátor</td>
<td style="border:1px solid black;">ServiceLocator.asmx</td>
</tr>
<tr class="even">
<td style="border:1px solid black;">Admin</td>
<td style="border:1px solid black;">Ez a virtuális könyvtár az RMS felügyeletéhez szükséges szolgáltatásokat tartalmazza.</td>
<td style="border:1px solid black;">Nincs ilyen.</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"> </td>
<td style="border:1px solid black;">Felügyelet</td>
<td style="border:1px solid black;">AdminSvc.asmx</td>
</tr>
<tr class="even">
<td style="border:1px solid black;">A DrmRemote</td>
<td style="border:1px solid black;">A .NET Remoting felület</td>
<td style="border:1px solid black;">Nincs ilyen.</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;">DirectoryServices</td>
<td style="border:1px solid black;">Ez a DrmRemote alkönyvtára</td>
<td style="border:1px solid black;">Nincs ilyen.</td>
</tr>
</tbody>
</table>
  
| ![](images/Cc747649.note(WS.10).gif)Megjegyzés:                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                     |  
|----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|  
| A felügyeleti szolgáltatás szigorúbb korlátozás alá esik a többi webszolgáltatásnál, mert az általa biztosított felület lehetővé teszi az RMS konfigurálását. Ezért a felhasználók csoportja nem kap hozzáférést a felügyeleti szolgáltatáshoz. Ezenkívül az IP-szűrés engedélyezve van, hogy az oldalak csak a helyi számítógépről legyenek elérhetők. A DirectoryServices virtuális könyvtár vendégfelhasználóknak nem teszi lehetővé a hozzáférést. A szolgáltatáslokátor szolgáltatás a Hálózati szolgáltatás fióknak is teljes jogosultságot ad. Licenckiszolgáló létesítéséhez módosítani kell az alapértelmezett hozzáférés-szabályozási bejegyzéseket (ACE), hogy engedélyezzék a hozzáférést az RMS rendszergazdájának. |
