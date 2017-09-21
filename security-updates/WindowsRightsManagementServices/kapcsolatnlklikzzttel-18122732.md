---
TOCTitle: Kapcsolat nélküli közzététel
Title: Kapcsolat nélküli közzététel
ms:assetid: 'f6384ed2-f917-442e-aa63-c1394a1c4d06'
ms:contentKeyID: 18122732
ms:mtpsurl: 'https://technet.microsoft.com/hu-hu/library/Cc747741(v=WS.10)'
---

Kapcsolat nélküli közzététel
============================

A kapcsolat nélküli közzététel abban különbözik az on-line közzétételtől, hogy az RMS-kompatibilis alkalmazás hogyan szerzi meg a közzétételi licencet.

A szerzők csak azt követően tehetnek közzé tartalmat kapcsolat nélkül, ha előbb ügyfél-licencelői tanúsítványt szereztek, amikor a hálózaton keresztül el tudták érni a legfelső szintű tanúsítási kiszolgálót.

A kapcsolat nélküli közzétételi folyamat a következő lépésekből áll:

1.  A szerző elkészíti a dokumentumot egy RMS-kompatibilis alkalmazással, majd megadja a tartalomra vonatkozó jogokat és feltételeket.
2.  Amikor a szerző menti a fájlt, az ügyfél-licencelői tanúsítvány lehetővé teszi a helyi számítógépnek vagy eszköznek, hogy kiállítsa és aláírja a fájl közzétételi licencét.
    A közzétételi licenc a tartalomkulcs két példányát tartalmazza: az egyik az ügyfél-licencelői tanúsítvány nyilvános kulcsával van titkosítva, a másik pedig az ügyfél licencelői tanúsítványt kiállító kiszolgáló nyilvános kulcsával. Tartalmazza a kiszolgáló URL-címét is. A két nyilvános kulcs és az URL-cím az ügyfél-licencelői tanúsítványból származik.
3.  A számítógép az ügyfél-licencelői tanúsítvány segítségével tulajdonosi licencet hoz létre. Ez olyan különleges használati licenc, amely lehetővé teszi a szerzőnek, hogy kapcsolat nélkül is használni tudja az RMS-védelemmel ellátott tartalmat. Az ügyfél-licencelői tanúsítvány a személyes kulcsával visszafejti a közzétételi licencben található szimmetrikus tartalomkulcsot, majd újra titkosítja, és elhelyezi a tulajdonosi licencben.
4.  Az alkalmazás titkosítja a fájlt a tartalomkulccsal, és hozzáköti a közzétételi licencet a fájlhoz. A fájl visszafejtésére alkalmas licencet csak a közzétételi licencet kiállító RMS kiszolgáló vagy egy megbízható közzétételi tartományba tartozó kiszolgáló állíthat ki.
