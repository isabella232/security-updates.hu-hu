---
TOCTitle: Az RMS tartalomkulcsai
Title: Az RMS tartalomkulcsai
ms:assetid: '63c814bf-2809-477e-a2db-d90370442075'
ms:contentKeyID: 18122514
ms:mtpsurl: 'https://technet.microsoft.com/hu-hu/library/Cc720284(v=WS.10)'
---

Az RMS tartalomkulcsai
======================

Amikor egy szerző RMS-védelemmel ellátott tartalmat tesz közzé, az RMS-kompatibilis alkalmazás létrehoz egy szimmetrikus tartalomkulcsot, és azzal titkosítja a tartalmat. Az RMS az Advanced Encryption Standard (AES) szabvány szerint hozza létre a tartalomkulcsot.

A tartalomkulcs belekerül a közzétételi licencbe, titkosítása a licencet kiállító RMS kiszolgáló nyilvános kulcsával történik.

Amikor az a kiszolgáló használati licenc iránti kérelmet kap, visszafejti a tartalomkulcsot a kiszolgáló személyes kulcsával, majd újra tikosítja a tartalmat a felhasználó személyes kulcsával (amelyet a kérelem részeként kap meg). Ezt követően belefoglalja a tartalomkulcsot a használati licencbe.
