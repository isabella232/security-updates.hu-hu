---
TOCTitle: Az RMS számára szükséges fiókok és engedélyek
Title: Az RMS számára szükséges fiókok és engedélyek
ms:assetid: '07a51daa-6823-41e6-b453-92f1a0592361'
ms:contentKeyID: 18122434
ms:mtpsurl: 'https://technet.microsoft.com/hu-hu/library/Cc720178(v=WS.10)'
---

Az RMS számára szükséges fiókok és engedélyek
=============================================

A következő táblázatban azok a felhasználói jogok és engedélyek szerepelnek, amelyekre az RMS telepítéséhez és felügyeletéhez szükség van.


<p> </p> 
<table style="border:1px solid black;">
<colgroup>
<col width="50%" />
<col width="50%" />
</colgroup>
<thead>
<tr class="header">
<th style="border:1px solid black;" >Tevékenység</th>
<th style="border:1px solid black;" >Felhasználói fiók és az engedélyek</th>
</tr>
</thead>
<tbody>
<tr class="odd">
<td style="border:1px solid black;">Az RMS telepítése</td>
<td style="border:1px solid black;">Olyan fiókkal kell bejelentkezni, amely tagja a helyi Rendszergazdák csoportnak.</td>
</tr>
<tr class="even">
<td style="border:1px solid black;">Az RMS létesítése</td>
<td style="border:1px solid black;">Olyan fiókkal kell bejelentkezni, amely tagja a helyi Rendszergazdák csoportnak. Emellett a fióknak olyan SQL bejelentkezési nevet kell használnia, amely az SQL Server adatbázisnál rendelkezik a System Administrator (Rendszergazda) szerepkörrel, hogy az RMS elő tudja készíteni a szükséges adatbázisokat.
A létesítés során meg kell adni az RMS szolgáltatásfiókját, amelyet azt megelőzően létre kell hozni. A felhasználói fióknak szokásos tartományi felhasználói fióknak kell lennie, amely nem rendelkezik további engedélyekkel. Ez a fiók az RMS szolgáltatás csoport tagjává válik, és ez az a fiók, amellyel szokásos esetben az RMS fut.
Olyan egykiszolgálós telepítéseknél, amelyekben az adatbázis a legfelső szintű tanúsítási kiszolgálón fut, a Helyi rendszerfiókot is megadhatja. Biztonsági megfontolásokból azonban azt ajánljuk, hogy mindig adja meg az RMS szolgáltatásfiókját, ne használja a Helyi rendszerfiókot. Ha az adatbázis külön kiszolgálón van, feltétlenül meg kell adni az RMS szolgáltatásfiókját.</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;">Az RMS felügyelete</td>
<td style="border:1px solid black;">Olyan fiókkal kell bejelentkezni, amely tagja a helyi Rendszergazdák csoportnak. A biztonsági beállítások testreszabásával kezelhető a felügyeleti weblapokhoz való hozzáférés.</td>
</tr>
</tbody>
</table>
  
> [!NOTE]
> Az RMS kiszolgálóra való bejelentkezéshez használt fióknak semmilyen további tartományi tagsággal sem kell rendelkeznie, nem kell például a Tartománygazdák közé tartoznia. Vannak azonban olyan felügyeleti műveletek (például a szolgáltatás kapcsolódási pontjának regisztrálása és a biztonsági szabályzat módosítása), amelyeket csak további jogokkal rendelkező fiókkal lehet végrehajtani.
