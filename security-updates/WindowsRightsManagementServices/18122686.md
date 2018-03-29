---
TOCTitle: 'On-line közzététel'
Title: 'On-line közzététel'
ms:assetid: '962c4e83-cf34-4c61-9589-31d24b0299fb'
ms:contentKeyID: 18122686
ms:mtpsurl: 'https://technet.microsoft.com/hu-hu/library/Cc747694(v=WS.10)'
---

On-line közzététel
==================

Az alábbi ábra az on-line közzétételi folyamatot mutatja be.

![](images/Cc747694.897e47b6-fffe-4b11-bc9f-be58539b9f19(WS.10).gif)

Az on-line közzétételi folyamat a következő lépésekből áll:

1.  A tartalom szerzője létrehoz egy dokumentumot, majd az RMS-kompatibilis alkalmazás segítségével megadja a tartalom felhasználóit, valamint a használatra vonatkozó jogokat és feltételeket.

2.  Az RMS-kompatibilis alkalmazás előállít egy szimmetrikus tartalomkulcsot, majd közzétételi licencet kérelmez a tanúsítási kiszolgálótól vagy egy licenckiszolgálótól. A kérelem magában foglalja a tartalomkulcsot és a használatra vonatkozó beállításokat.

3.  A licenckiszolgáló előállítja a közzétételi licencet, titkosítja a tartalmat a kiszolgáló nyilvános kulcsával, majd visszaküldi a közzétételi licencet az RMS-kompatibilis alkalmazásnak.

4.  Az alkalmazás titkosítja a fájlt a tartalomkulccsal, és hozzáköti a közzétételi licencet a fájlhoz.

5.  A tartalom használójának számítógépén futó RMS-kompatibilis alkalmazás elküld a közzétételi licencet kibocsátó RMS kiszolgálónak egy használati licenc iránti kérelmet, amely tartalmazza a felhasználó tartalomvédelmi fióktanúsítványát.

6.  Az RMS kiszolgáló ellenőrzi a felhasználó hitelesítő adatainak érvényességét. Ha az érvényességi ellenőrzés sikeres, a kiszolgáló előállítja a használati licencet, és visszaküldi a tartalom használójának számítógépén futó RMS-kompatibilis alkalmazásnak.

7.  Az RMS-kompatibilis alkalmazás megnyitja a dokumentumot, és a használati licencben foglalt jogokat biztosítja a felhasználónak.