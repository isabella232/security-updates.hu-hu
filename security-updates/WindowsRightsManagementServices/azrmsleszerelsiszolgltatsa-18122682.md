---
TOCTitle: Az RMS leszerelési szolgáltatása
Title: Az RMS leszerelési szolgáltatása
ms:assetid: '97677e3b-bc83-47ec-b6db-d326cd94566c'
ms:contentKeyID: 18122682
ms:mtpsurl: 'https://technet.microsoft.com/hu-hu/library/Cc747695(v=WS.10)'
---

Az RMS leszerelési szolgáltatása
================================

A leszerelési szolgáltatás olyan egyéni webszolgáltatás, amely az RMS szolgáltatással együtt települ. Egyaránt fut a legfelső szintű fürtön és a csak licencelő fürtökön. A szolgáltatás engedélyezése az RMS minden egyéb webszolgáltatásának a letiltását eredményezi.

A szolgáltatás az ügyfelektől érkező licenckérelmekre válaszul visszafejti a tartalomvédelemmel ellátott tartalom közzétételi licencében tárolt tartalomkulcsot, és elküldi ezt a kulcsot az ügyfélnek. Ez lehetővé teszi a tartalom RMS-védelem nélküli mentését. A leszerelési szolgáltatás minden hozzá beérkező ügyfélkérelmet naplóz, és a naplózási adatbázisban való rögzítésre elküldi ezeket a naplózási figyelőszolgáltatásnak.

A leszerelési szolgáltatás a felügyeleti webhely **Biztonsági beállítások** című oldalán engedélyezhető. A szolgáltatás engedélyezését követően a kiszolgáló nem állítható vissza a normál RMS-konfiguráció szerinti működésre.

A szolgáltatás engedélyezése után át kell állítani a decommission.asmx fájl tulajdonosi hozzáférés-szabályozási listáját (DACL) úgy, hogy hozzáférjen a vállalat minden olyan felhasználója, aki ezt a kiszolgálót használta tartalom licencelésére. Emellett olvasási és végrehajtási jogosultsággal fel kell venni az RMS szolgáltatás csoportot a tulajdonosi hozzáférés-szabályozási listába, hogy az RMS kezelni tudja a szolgáltatás működését. Miután minden, a kiszolgáló által közzétett tartalom védelmét sikerült megszüntetni, biztonsági másolatot kell készíteni a személyes kulcs adatairól, majd el lehet távolítani az RMS szolgáltatást a kiszolgálóról.

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
<td style="border:1px solid black;"><p>RENDSZER</p></td>
<td style="border:1px solid black;"><p>Teljes hozzáférés</p></td>
</tr>  
</tbody>  
</table>
