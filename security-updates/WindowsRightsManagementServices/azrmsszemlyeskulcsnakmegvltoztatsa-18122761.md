---
TOCTitle: Az RMS személyes kulcsának megváltoztatása
Title: Az RMS személyes kulcsának megváltoztatása
ms:assetid: 'da32137e-394a-42b2-9552-ba20f4547c23'
ms:contentKeyID: 18122761
ms:mtpsurl: 'https://technet.microsoft.com/hu-hu/library/Cc747765(v=WS.10)'
---

Az RMS személyes kulcsának megváltoztatása
==========================================

A létesítés során az RMS létrehozza a kiszolgáló személyes kulcsát. Az RMS személyes kulcsa titkosított, tárolási helye a konfigurációs adatbázis. A személyes kulcsról készítsen biztonsági másolatot, és tárolja biztonságos helyen. Ezenkívül célszerű hardveres biztonsági modult is használni az RMS személyes kulcsának védelméhez, mivel a rendszer ezt a kulcsot használja az RMS kiszolgáló által védett teljes tartalom titkosítási sémájában. Ha az RMS személyes kulcsa megsérül, új személyes kulcs létrehozásához meg kell szüntetnie az RMS szolgáltatást a kiszolgálón, majd újból végre kell hajtani az RMS létesítését.

Ha a kiszolgálót tartalomvédelemre használta, értesíteni kell a tartalom tulajdonosait, és a tartalmat újból közzé kell tenni az új személyes kulccsal ellátott RMS kiszolgáló használatával. A sérült személyes kulccsal védett tartalom minden példányát meg kell semmisíteni, mivel ez a védelem már nem tekinthető megfelelőnek.

| ![](images/Cc747765.Important(WS.10).gif)Fontos:                                                                                                                                                                                              |
|----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| A kiszolgálónak meg kell ismételnie a létesítési műveletet, függetlenül attól, hogy megtörtént-e az igénylése a Microsoft igénylési szolgáltatással. Ha csak ismételt igénylést próbál végrehajtani az RMS kiszolgálónál, a rendszer az előző személyes kulcsot használja. |
