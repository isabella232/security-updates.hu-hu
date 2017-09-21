---
TOCTitle: Az RMS fürttel szembeni követelményeinek tervezése
Title: Az RMS fürttel szembeni követelményeinek tervezése
ms:assetid: 'ec4023eb-4d39-4551-9789-c8a2d973a55b'
ms:contentKeyID: 18122779
ms:mtpsurl: 'https://technet.microsoft.com/hu-hu/library/Cc747792(v=WS.10)'
---

Az RMS fürttel szembeni követelményeinek tervezése
==================================================

Ha fürtben vezeti be az RMS szolgáltatást, feltétlenül gondolja át, hogyan nyújt megoldást az alábbi helyzetekre, amennyiben azok fennállnak az adott szervezetnél.

###  

<p> </p>
<table style="border:1px solid black;">
<colgroup>
<col width="50%" />
<col width="50%" />
</colgroup>
<thead>
<tr class="header">
<th>Helyzet</th>
<th>Javaslat</th>
</tr>
</thead>
<tbody>
<tr class="odd">
<td style="border:1px solid black;"><p>Nagy számú asztali gép használja az RMS szolgáltatást.</p></td>
<td style="border:1px solid black;"><p>A Windows Update, parancsfájl vagy szoftverterjesztő módszer, például a Systems Management Server (SMS) vagy a Csoportházirend segítségével telepítheti és aktiválhatja a Microsoft Windows tartalomvédelmi szolgáltatások ügyfélszoftverét.</p></td>
</tr>  
<tr class="even">
<td style="border:1px solid black;"><p>Az ügyfelek sok kérelmet nyújtanak be.</p></td>
<td style="border:1px solid black;"><p>Ossza el a terhelést a fürt számítógépei között egy terheléselosztó kiszolgáló, a hálózati terheléselosztási szolgáltatás (NLB) vagy hardveres terheléselosztás segítségével.</p></td>
</tr>  
<tr class="odd">
<td style="border:1px solid black;"><p>Két olyan hálózati kártya, amelyek virtuális IP-címzés segítségével az extranetes és az intranetes kérelmeket egyaránt kiszolgálják.</p></td>
<td style="border:1px solid black;"><p>Ügyeljen arra, hogy minden olyan DNS-regisztráció, amely az extranet irányában közzéteszi a virtuális IP-címet, megtörténjen az intranet irányában is.</p>
<p>Ha nincs DNS-regisztráció az intranet oldalán, sikertelenek lesznek a használati licenc iránti belső kérelmek. Ha nem módosíthatók a DNS erőforrásrekordjai, a fürtbe tartozó minden kiszolgálón módosítani lehet az állomástáblát úgy, hogy a fürt URL-címét hozzárendelje a fürt virtuális IP-címéhez. A DNS-regisztrációnak még az RMS létesítése előtt meg kell történnie. Ha már létesítette az RMS szolgáltatást, előbb meg kell szüntetni, majd meg kell ismételni a létesítési folyamatot.</p></td>
</tr>
</tbody>
</table>
