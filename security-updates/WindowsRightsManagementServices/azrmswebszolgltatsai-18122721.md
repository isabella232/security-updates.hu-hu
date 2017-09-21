---
TOCTitle: Az RMS webszolgáltatásai
Title: Az RMS webszolgáltatásai
ms:assetid: 'ed8dbb2e-0590-4502-afc4-54f66b96d515'
ms:contentKeyID: 18122721
ms:mtpsurl: 'https://technet.microsoft.com/hu-hu/library/Cc747728(v=WS.10)'
---

Az RMS webszolgáltatásai
========================

Az RMS biztosítja az RMS rendszer kiszolgáló összetevőjét. Alapvető funkciói Microsoft® ASP.NET webszolgáltatások készleteként vannak megvalósítva, amelyek a Microsoft® Internet Information Services (IIS) rendszeren futnak. Az RMS webszolgáltatások a SOAP felületen vagy a .NET Remoting eljárással érhetők el.

A webszolgáltatások a következőket biztosítják:

-   Kiszolgálók aligénylése
-   Megbízható entitások fióktanúsítása
-   Tartalomvédelemmel ellátott adatok licencelése
-   Az RMS felügyeleti funkciói

A következő táblázat az RMS webszolgáltatásait ismerteti.

###  

<p> </p>
<table style="border:1px solid black;">
<colgroup>
<col width="50%" />
<col width="50%" />
</colgroup>
<thead>
<tr class="header">
<th>Szolgáltatás</th>
<th>Leírás</th>
</tr>
</thead>
<tbody>
<tr class="odd">
<td style="border:1px solid black;"><p>Aligénylés</p></td>
<td style="border:1px solid black;"><p>Alsóbb szintű kiszolgálói licencelői tanúsítványokat nyújt a csak licencelésre szolgáló fürtökön lévő kiszolgálóknak. Ezek a tanúsítványok közzétételi és használati licencek kiállítását teszik lehetővé a csak licencelésre szolgáló fürt számára.</p></td>
</tr>  
<tr class="even">
<td style="border:1px solid black;"><p>Fióktanúsítás</p></td>
<td style="border:1px solid black;"><p>Tartalomvédelmi fióktanúsítványokat állít ki a felhasználóknak. Ezekre a tanúsítványokra van szükségük a felhasználóknak, hogy védelemmel ellátott tartalom elkészítésére és használatára alkalmas közzétételi és használati licenceket szerezhessenek.</p></td>
</tr>  
<tr class="odd">
<td style="border:1px solid black;"><p>Aktiválási proxy</p></td>
<td style="border:1px solid black;"><p>Ez a szolgáltatás az RMS 1.0-s verziójú ügyfélszoftverrel való kompatibilitás miatt maradt meg. Továbbítja a gépaktiválási kérelmeket a Microsoft aktiválási szolgáltatásának, és visszaküldi az RMS 1.0-s verziójú ügyfeleknek a kulcstárolókat és az RMS géptanúsítványokat. Ezt a szolgáltatást nem használják a Service Pack 1 (SP1) vagy újabb javítócsomaggal bővített RMS-ügyfelek.</p></td>
</tr>  
<tr class="even">
<td style="border:1px solid black;"><p>Közzététel</p></td>
<td style="border:1px solid black;"><p>Közzétételi licenceket állít ki, amelyek alapján a szerzők védelemmel ellátott tartalmat hozhatnak létre és terjeszthetnek. Ez a szolgáltatás állítja ki az ügyfél-licencelői tanúsítványokat is: így a felhasználók úgy tehetnek közzé védelemmel ellátott tartalmat, hogy kapcsolódnának az RMS belső hálózatához.</p></td>
</tr>  
<tr class="odd">
<td style="border:1px solid black;"><p>Licencelés</p></td>
<td style="border:1px solid black;"><p>Használati licenceket állít ki, amelyek alapján a felhasználók védelemmel ellátott tartalmat használhatnak.</p></td>
</tr>  
<tr class="even">
<td style="border:1px solid black;"><p>Felügyelet</p></td>
<td style="border:1px solid black;"><p>Lehetővé teszi a rendszergazdának az RMS kezelését.</p></td>
</tr>  
<tr class="odd">
<td style="border:1px solid black;"><p>DrmRemote</p></td>
<td style="border:1px solid black;"><p>A .NET Remoting elérhetővé tételével lehetővé teszi a webszolgáltatásoknak az egymás közötti és az RMS rendszer más összetevőivel való kommunikációt.</p></td>
</tr>  
<tr class="even">
<td style="border:1px solid black;"><p>Leszerelés</p></td>
<td style="border:1px solid black;"><p>Eltávolítja a-védelemmel ellátott tartalom védelmét, és visszaküldi a tartalmat az ügyfélnek. A szolgáltatás települ az RMS telepítésekor, de amíg a rendszergazda nem engedélyezi, nem felel meg neki virtuális gyökér az IIS szolgáltatásban. A szolgáltatás engedélyezése az összes többi szolgáltatás letiltását eredményezi.</p></td>
</tr>  
</tbody>  
</table>
  
Az RMS a webszolgáltatásokon kívül a naplózási figyelőszolgáltatást is telepíti. Mindegyik webszolgáltatás a naplózási várólistába küldi a naplózott adatokat. A naplózási figyelőszolgáltatás ezt követően továbbítja az adatokat a várólistából a naplózási adatbázisba.
  
A webszolgáltatásokat megvalósító alkalmazások az IIS virtuális könyvtáraiban találhatók. Ezeket a virtuális könyvtárakat minden RMS kiszolgálóra telepíti a rendszer a létesítéskor kijelölt webhely alá.
  
A hitelesítés és a hozzáférés minden virtuális könyvtárra külön beállítható. Emellett az egyes webszolgáltatásokhoz való hozzáférés is különállóan konfigurálható. A virtuális könyvtárakra és a webszolgáltatásokra vonatkozó biztonsági beállításokról a további tudnivalókat lásd: [Internet Information Services](https://technet.microsoft.com/bd4dc69f-1e4e-4e95-9ae2-c925d8a14d4c).
  
Az egyes webszolgáltatási összetevőkről a további tudnivalókat lásd: [Az RMS szoftveres összetevői](https://technet.microsoft.com/e38a840e-f390-48fd-8354-50108a64f5ca).
