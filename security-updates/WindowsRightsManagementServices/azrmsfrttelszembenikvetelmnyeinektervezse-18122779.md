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
<td style="border:1px solid black;">Nagy számú asztali gép használja az RMS szolgáltatást.</td>
<td style="border:1px solid black;">A Windows Update, parancsfájl vagy szoftverterjesztő módszer, például a Systems Management Server (SMS) vagy a Csoportházirend segítségével telepítheti és aktiválhatja a Microsoft Windows tartalomvédelmi szolgáltatások ügyfélszoftverét.</td>
</tr>
<tr class="even">
<td style="border:1px solid black;">Az ügyfelek sok kérelmet nyújtanak be.</td>
<td style="border:1px solid black;">Ossza el a terhelést a fürt számítógépei között egy terheléselosztó kiszolgáló, a hálózati terheléselosztási szolgáltatás (NLB) vagy hardveres terheléselosztás segítségével.</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;">Két olyan hálózati kártya, amelyek virtuális IP-címzés segítségével az extranetes és az intranetes kérelmeket egyaránt kiszolgálják.</td>
<td style="border:1px solid black;">Ügyeljen arra, hogy minden olyan DNS-regisztráció, amely az extranet irányában közzéteszi a virtuális IP-címet, megtörténjen az intranet irányában is.
Ha nincs DNS-regisztráció az intranet oldalán, sikertelenek lesznek a használati licenc iránti belső kérelmek. Ha nem módosíthatók a DNS erőforrásrekordjai, a fürtbe tartozó minden kiszolgálón módosítani lehet az állomástáblát úgy, hogy a fürt URL-címét hozzárendelje a fürt virtuális IP-címéhez. A DNS-regisztrációnak még az RMS létesítése előtt meg kell történnie. Ha már létesítette az RMS szolgáltatást, előbb meg kell szüntetni, majd meg kell ismételni a létesítési folyamatot.</td>
</tr>
</tbody>
</table>
