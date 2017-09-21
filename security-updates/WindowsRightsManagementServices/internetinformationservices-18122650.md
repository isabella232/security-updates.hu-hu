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

<p> </p>
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
<td style="border:1px solid black;"><p>_wmcs</p></td>
<td style="border:1px solid black;"><p>Ez az RMS-fürt felügyeleti virtuális könyvtára.</p></td>
<td style="border:1px solid black;"><p>Nincs ilyen.</p></td>
</tr>  
<tr class="even">
<td style="border:1px solid black;"><p>Certification</p></td>
<td style="border:1px solid black;"><p>Ez a virtuális könyvtár az RMS tanúsítási műveleteihez szükséges szolgáltatásokat tartalmazza.</p></td>
<td style="border:1px solid black;"><p>Nincs ilyen.</p></td>
</tr>  
<tr class="odd">
<td style="border:1px solid black;"><p> </p></td>
<td style="border:1px solid black;"><p>Aktiválási proxy</p></td>
<td style="border:1px solid black;"><p>Activation.asmx</p></td>
</tr>  
<tr class="even">
<td style="border:1px solid black;"><p> </p></td>
<td style="border:1px solid black;"><p>Fióktanúsítás</p></td>
<td style="border:1px solid black;"><p>Certification.asmx</p></td>
</tr>  
<tr class="odd">
<td style="border:1px solid black;"><p> </p></td>
<td style="border:1px solid black;"><p>Előtanúsítás</p></td>
<td style="border:1px solid black;"><p>Precertification.asmx</p></td>
</tr>  
<tr class="even">
<td style="border:1px solid black;"><p> </p></td>
<td style="border:1px solid black;"><p>Szolgáltatáslokátor</p></td>
<td style="border:1px solid black;"><p>ServiceLocator.asmx</p></td>
</tr>  
<tr class="odd">
<td style="border:1px solid black;"><p> </p></td>
<td style="border:1px solid black;"><p>Kiszolgáló</p></td>
<td style="border:1px solid black;"><p>Server.asmx</p></td>
</tr>  
<tr class="even">
<td style="border:1px solid black;"><p> </p></td>
<td style="border:1px solid black;"><p>Kiszolgálótanúsítás</p></td>
<td style="border:1px solid black;"><p>ServerCertification.asmx</p></td>
</tr>  
<tr class="odd">
<td style="border:1px solid black;"><p> </p></td>
<td style="border:1px solid black;"><p>Mobil eszköz tanúsítása</p></td>
<td style="border:1px solid black;"><p>MobileDeviceCertfication.asmx</p></td>
</tr>  
<tr class="even">
<td style="border:1px solid black;"><p> </p></td>
<td style="border:1px solid black;"><p>Igénylés</p></td>
<td style="border:1px solid black;"><p>SubEnrollService.asmx</p></td>
</tr>  
<tr class="odd">
<td style="border:1px solid black;"><p>Licencing</p></td>
<td style="border:1px solid black;"><p>Ez a virtuális könyvtár az RMS licencelési műveleteihez szükséges szolgáltatásokat tartalmazza.</p></td>
<td style="border:1px solid black;"><p>Nincs ilyen.</p></td>
</tr>  
<tr class="even">
<td style="border:1px solid black;"><p> </p></td>
<td style="border:1px solid black;"><p>Licencelés</p></td>
<td style="border:1px solid black;"><p>License.asmx</p></td>
</tr>  
<tr class="odd">
<td style="border:1px solid black;"><p> </p></td>
<td style="border:1px solid black;"><p>Közzététel</p></td>
<td style="border:1px solid black;"><p>Publish.asmx</p></td>
</tr>  
<tr class="even">
<td style="border:1px solid black;"><p> </p></td>
<td style="border:1px solid black;"><p>Kiszolgáló</p></td>
<td style="border:1px solid black;"><p>Server.asmx</p></td>
</tr>  
<tr class="odd">
<td style="border:1px solid black;"><p> </p></td>
<td style="border:1px solid black;"><p>Szolgáltatáslokátor</p></td>
<td style="border:1px solid black;"><p>ServiceLocator.asmx</p></td>
</tr>  
<tr class="even">
<td style="border:1px solid black;"><p>Admin</p></td>
<td style="border:1px solid black;"><p>Ez a virtuális könyvtár az RMS felügyeletéhez szükséges szolgáltatásokat tartalmazza.</p></td>
<td style="border:1px solid black;"><p>Nincs ilyen.</p></td>
</tr>  
<tr class="odd">
<td style="border:1px solid black;"><p> </p></td>
<td style="border:1px solid black;"><p>Felügyelet</p></td>
<td style="border:1px solid black;"><p>AdminSvc.asmx</p></td>
</tr>  
<tr class="even">
<td style="border:1px solid black;"><p>A DrmRemote</p></td>
<td style="border:1px solid black;"><p>A .NET Remoting felület</p></td>
<td style="border:1px solid black;"><p>Nincs ilyen.</p></td>
</tr>  
<tr class="odd">
<td style="border:1px solid black;"><p>DirectoryServices</p></td>
<td style="border:1px solid black;"><p>Ez a DrmRemote alkönyvtára</p></td>
<td style="border:1px solid black;"><p>Nincs ilyen.</p></td>
</tr>  
</tbody>  
</table>
  
| ![](images/Cc747649.note(WS.10).gif)Megjegyzés:                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                     |  
|----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|  
| A felügyeleti szolgáltatás szigorúbb korlátozás alá esik a többi webszolgáltatásnál, mert az általa biztosított felület lehetővé teszi az RMS konfigurálását. Ezért a felhasználók csoportja nem kap hozzáférést a felügyeleti szolgáltatáshoz. Ezenkívül az IP-szűrés engedélyezve van, hogy az oldalak csak a helyi számítógépről legyenek elérhetők. A DirectoryServices virtuális könyvtár vendégfelhasználóknak nem teszi lehetővé a hozzáférést. A szolgáltatáslokátor szolgáltatás a Hálózati szolgáltatás fióknak is teljes jogosultságot ad. Licenckiszolgáló létesítéséhez módosítani kell az alapértelmezett hozzáférés-szabályozási bejegyzéseket (ACE), hogy engedélyezzék a hozzáférést az RMS rendszergazdájának. |
