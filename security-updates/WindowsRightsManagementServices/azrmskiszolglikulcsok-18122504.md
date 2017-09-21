---
TOCTitle: Az RMS kiszolgálói kulcsok
Title: Az RMS kiszolgálói kulcsok
ms:assetid: '5f4100a1-9aa5-42af-85c8-4bc691022f06'
ms:contentKeyID: 18122504
ms:mtpsurl: 'https://technet.microsoft.com/hu-hu/library/Cc720280(v=WS.10)'
---

Az RMS kiszolgálói kulcsok
==========================

Minden RMS kiszolgáló rendelkezik egy 1024 bites RSA-kulcspárral.

A kiszolgáló nyilvános kulcsával van titkosítva a közzétételi licencben szereplő tartalomkulcs, hogy csak az RMS kiszolgáló tudja beolvasni a tartalomkulcsot, és csak az tudjon használati licencet kiállítani az adott közzétételi licenc ellenében. A kiszolgáló licencelői tanúsítványa tartalmazza a kiszolgáló nyilvános kulcsát.

A kiszolgáló személyes kulcsával van aláírva minden, a kiszolgáló által kiállított tanúsítvány és licenc.

A kiszolgáló személyes kulcsának védelme
----------------------------------------

Alapértelmezés szerint a létesítés során létrejön a kiszolgáló személyes kulcsa, majd titkosított formában tárolódik az RMS adatbázisában. De a létesítés során megadható egy, már a kiszolgálóra telepített kriptográfiai szolgáltató (CSP) is.

A CSP kétféleképpen használható:

-   Választhat a kiszolgálóval alapértelmezés szerint települő szoftveres CSP-megvalósítások közül.
    vagy
-   Használhat a kiszolgálóra telepített, nem a Microsofttól származó szoftveres szolgáltatót is.

| ![](images/Cc720280.note(WS.10).gif)Megjegyzés:                                                                                          |
|-----------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| Ha hardveres biztonsági modult kíván használni, ügyeljen rá, hogy olyan kriptográfiai szolgáltatót (CSP) válasszon, amely támogatja a hardveres biztonsági modulokat. |

Ha úgy dönt, hogy CSP segítségével védi a kiszolgáló személyes kulcsát, az RMS konfigurációs adatbázisa tárolja a szolgáltató és a kulcstároló nevét.
