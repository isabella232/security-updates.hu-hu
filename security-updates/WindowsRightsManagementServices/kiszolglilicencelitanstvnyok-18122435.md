---
TOCTitle: Kiszolgálói licencelői tanúsítványok
Title: Kiszolgálói licencelői tanúsítványok
ms:assetid: '0b35fbcd-25a9-4587-898d-9a30fd1d3c5b'
ms:contentKeyID: 18122435
ms:mtpsurl: 'https://technet.microsoft.com/hu-hu/library/Cc720184(v=WS.10)'
---

Kiszolgálói licencelői tanúsítványok
====================================

A kiszolgálói licencelői tanúsítvány feljogosítja az RMS kiszolgálót tanúsítványok és licencek kiállítására. Az RMS bevezetésének első legfelső szintű tanúsítási kiszolgálójának létesítésekor ez kiszolgálói licencelői tanúsítványt szerez a Microsoft igénylési szolgáltatásától. A folyamat elnevezése igénylés. Ez a tanúsítvány tartalmazza a legfelső szintű tanúsítási kiszolgáló nyilvános kulcsát, illetve alá van írva az igénylési szolgáltatás személyes kulcsával. A legfelső szintű tanúsítási fürtbe felvett további kiszolgálók ugyanezt a tanúsítványt használják.

A létesítés során a fürt első licenckiszolgálója az RMS legfelső szintű tanúsítási kiszolgálójától vagy fürtjétől kap kiszolgálói licencelői tanúsítványt az aligénylésnek nevezett folyamat során. Ez a tanúsítvány tartalmazza a licenckiszolgáló nyilvános kulcsát, és alá van írva a legfelső szintű tanúsítási kiszolgáló vagy fürt személyes kulcsával. A licencelési fürthöz hozzáadott további kiszolgálók ugyanezt a tanúsítványt használják.

Az alábbi táblázat azokat a jogokat tartalmazza, amelyeket a kiszolgálók számára a kiszolgálói licencelői tanúsítványok adnak meg.

###  

 
<table style="border:1px solid black;">
<colgroup>
<col width="33%" />
<col width="33%" />
<col width="33%" />
</colgroup>
<thead>
<tr class="header">
<th>Kiállítási jogosultság</th>
<th>A legfelső szintű tanúsítási kiszolgáló részére kiállított kiszolgálói licencelői tanúsítvány</th>
<th>Licenckiszolgáló részére kiállított kiszolgálói licencelői tanúsítvány</th>
</tr>
</thead>
<tbody>
<tr class="odd">
<td style="border:1px solid black;">Tartalomvédelmi fióktanúsítványok</td>
<td style="border:1px solid black;">Igen</td>
<td style="border:1px solid black;">Nem</td>
</tr>
<tr class="even">
<td style="border:1px solid black;">Közzétételi licencek</td>
<td style="border:1px solid black;">Igen</td>
<td style="border:1px solid black;">Igen</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;">Használati licencek</td>
<td style="border:1px solid black;">Igen</td>
<td style="border:1px solid black;">Igen</td>
</tr>
<tr class="even">
<td style="border:1px solid black;">Alsóbb szintű kiszolgálói licencelői tanúsítványok</td>
<td style="border:1px solid black;">Igen</td>
<td style="border:1px solid black;">Nem</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;">Ügyfél licencelői tanúsítványok</td>
<td style="border:1px solid black;">Igen</td>
<td style="border:1px solid black;">Igen</td>
</tr>
</tbody>
</table>
  
| ![](images/Cc720184.note(WS.10).gif)Megjegyzés:                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                  |  
|-----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|  
| Az RMS működésének nem feltétele külön licenckiszolgálók vagy licencelési fürtök megléte, de ilyenek segítségével csökkenthető a legfelső szintű tanúsítási fürtre érkező licenckérelmek száma. Az is indokolhatja licenckiszolgálók létesítését, hogy egyes szervezeti egységeknek közvetlen szabályozási lehetőségre van szükségük a védett tartalom közzétételére vonatkozóan. Ilyen például az az eset, amikor a vállalat egészére vonatkozó szabályokat a legfelső szintű tanúsítási kiszolgáló vagy fürt jogmegadási sablonjai tartalmazzák, de ezekben nem szerepelnek egy adott részlegnél megkövetelt jogok. Ebben az esetben a részleg külön licenckiszolgáló vagy licencelési fürt üzembe helyezése után tárolhatja saját jogmegadási sablonjait, és kezelheti a licenckérelmeket. |
