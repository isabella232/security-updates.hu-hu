---
TOCTitle: Az RMS licencelési szolgáltatása
Title: Az RMS licencelési szolgáltatása
ms:assetid: '5cad1baf-0304-4e82-b62d-83a4aac2140b'
ms:contentKeyID: 18122501
ms:mtpsurl: 'https://technet.microsoft.com/hu-hu/library/Cc720278(v=WS.10)'
---

Az RMS licencelési szolgáltatása
================================

A licencelő szolgáltatás, amely a használati licenceket állítja ki, az RMS legfelső szintű fürtjén, illetve bármelyik csak licencelő fürtön fut. A használati licencek lehetővé teszik a felhasználóknak, hogy használják a tartalomvédelemmel ellátott tartalmat.

A licencelési szolgáltatás alkalmazásfájlja, a License.asmx, az IIS szolgáltatás Licensing virtuális könyvtárában található.

| ![](images/Cc720278.note(WS.10).gif)Megjegyzés:                                                                                                                                                                                                                                                                                                                                                                                             |
|--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| Külön csak licencelési fürt üzembe helyezésével csökkenthető a legfelső szintű fürt által kiszolgálandó kérelmek száma. Egy osztály számára is üzembe helyezhető külön licenckiszolgáló vagy licencelési fürt, például azért, hogy az osztály saját jogmegadási sablonokat alakíthasson ki magának. Ezekről a kérdésekről a további tudnivalók a dokumentumgyűjtemény „RMS bevezetésének tervezése” részében „Az alapvető összetevők azonosítása” témakörben találhatók. |

A szolgáltatás alapértelmezett hozzáférési szabálygyűjteményét a következő táblázat szemlélteti:

###  

<p> </p>
<table style="border:1px solid black;">
<colgroup>
<col width="50%" />
<col width="50%" />
</colgroup>
<thead>
<tr class="header">
<th>Felhasználó vagy Csoport</th>
<th>Alapértelmezett engedély</th>
</tr>
</thead>
<tbody>
<tr class="odd">
<td style="border:1px solid black;"><p>Rendszergazdák</p></td>
<td style="border:1px solid black;"><p>Teljes hozzáférés</p></td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><p>RMS szolgáltatáscsoport</p></td>
<td style="border:1px solid black;"><p>Olvasás és végrehajtás</p></td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><p>RENDSZER</p></td>
<td style="border:1px solid black;"><p>Teljes hozzáférés</p></td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><p>Felhasználók</p></td>
<td style="border:1px solid black;"><p>Olvasás és végrehajtás</p></td>
</tr>
</tbody>
</table>
