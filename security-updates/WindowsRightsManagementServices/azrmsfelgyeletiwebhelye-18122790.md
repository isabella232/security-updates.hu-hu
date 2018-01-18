---
TOCTitle: Az RMS felügyeleti webhelye
Title: Az RMS felügyeleti webhelye
ms:assetid: 'f003c1d9-9a17-4e50-9e1e-5d67677552a0'
ms:contentKeyID: 18122790
ms:mtpsurl: 'https://technet.microsoft.com/hu-hu/library/Cc747796(v=WS.10)'
---

Az RMS felügyeleti webhelye
===========================

Minden legfelső szintű és csak licencelő fürthöz felügyeleti webhely tartozik, amely az RMS kezelésére használható. Ez a webhely csak az éppen felügyelt RMS kiszolgálóról, illetve távoli asztali kapcsolaton keresztül érhető el.

Ez a témakör a felügyeleti webhely szolgáltatásait ismerteti. A webhely RMS felügyeletére való használatára vonatkozó utasítások a dokumentumgyűjtemény „RMS kiszolgáló működtetése” című részében az „RMS – Útmutató” és „Az RMS kezelése” című témakörben találhatók.

**Megjegyzés   **A fürtök konfigurálása globális művelet. A fürtök konfigurálása bármely olyan kiszolgáló felügyeleti webhelyéről végrehajtható, amely az adott fürtbe tartozik.

A **Globális felügyelet** lapon a következő műveletek hajthatók végre:

-   RMS létesítése adott webhelyen.

-   Kiszolgáló létesítése és felvétele fürtbe

-   RMS eltávolítása adott webhelyről.

-   A fürtök felügyeleti lapjainak megnyitása

Nyissa meg a fürt **Felügyelet** lapját a következő feladatok végrehajtásához:

-   **Fürtadatok megtekintése**Megtekinthetők a fürt különböző adatai, így például a telepítési URL-cím, a kiszolgáló URL-címe, a tanúsítvány neve, a konfigurációs adatbázis kiszolgálója, a konfigurációs adatbázis neve, valamint a tanúsítvány lejáratának dátuma.

-   **A kiszolgálói licencelői tanúsítvány igénylése vagy megújítása.**Igényelhető vagy megújítható a fürt kiszolgálói licencelői tanúsítványa.

-   **Bizalmi szabályzatok kialakítása.**A hivatkozásra kattintva megnyithatja a Bizalmi szabályzatok weblapot, ahol megbízható felhasználói tartományokat és megbízható közzétételi tartományokat vehet fel vagy távolíthat el. A megbízható felhasználói tartományok kizárási listáján felhasználókat vehet vagy távolíthat el. Fájlba exportálhatja kiszolgálói licencelői tanúsítványát más RMS-telepítésbe való importáláshoz.

-   **Jogmegadási sablonok konfigurálása.**A hivatkozásra kattintva megnyithatja a Jogmegadási sablonok weblapot, ahol létrehozhatja és módosíthatja a vállalatnál használt jogmegadási sablonokat.

-   **A naplózás konfigurálása.**A hivatkozásra kattintva megnyithatja a Naplózási beállítások weblapot, ahol ki- és bekapcsolhatja a naplózást, majd megtekintheti a naplózási kiszolgálót és az adatbázist.

-   **A fürt extranetes URL-címének megadása.**A hivatkozásra kattintva megnyithatja A fürt extranetes URL-címének megadása weblapot, ahol megadhatja azt az URL-címet, amelyikről az extranetről elérhetők a legfelső szintű fürt tanúsítási szolgáltatásai.

-   **Az RMS proxybeállításainak megadása.**A hivatkozásra kattintva megnyithatja az RMS proxybeállításai weblapot, ahol megadhatja proxyykiszolgáló címét, a hitelesítés típusát, valamint a felhasználónevet. Az RMS kiszolgáló ezeket használja, amikor proxykiszolgálón keresztül kell kapcsolódnia az internethez.

-   **A kiosztott tartalomvédelmi fióktanúsítványok számának ellenőrzése.**A hivatkozásra kattintva megnyithatja a Tartalomvédelmi fióktanúsítványok nyilvántartása weblapot, amelyen megtekintheti, hogy hány licencet állított ki a legfelső szintű fürt. Ennek alapján megbecsülheti, hogy hány ügyféllicencre van szükség.

-   **A biztonsági beállítások kezelése.**A hivatkozásra kattintva megnyithatja a Biztonsági beállítások weblapot, amelyen a felügyelői csoport tagságát kezelheti. A csoport tagjai teljes jogosultsággal rendelkeznek minden licenccel ellátott tartalomhoz, valamint átállíthatják a személyes kulcs jelszavát.

-   **A fióktanúsítási beállítások megtekintése és konfigurálása.**A hivatkozásra kattintva megnyithatja a Tanúsítási beállítások weblapot, amelyen megadhatja a tanúsítványok érvényességi időtartamát, valamint a rendszergazda elérhetőségét.

-   **A kizárási szabályzatok engedélyezése.**A hivatkozásra kattintva megnyithatja a Kizárási szabályzatok weblapot, amelyen a kulcstároló verzióján, a Windows verzióján, a fióktanúsítványokon és az alkalmazásokon alapuló kizárási szabályzatokat engedélyezhet.

-   **A szolgáltatás kapcsolódási pontjának regisztrálása.**A hivatkozásra kattintva megnyithatja a Szolgáltatás kapcsolódási pontja weblapot, amelyen regisztrálhatja a fürt szolgáltatáskapcsolódási pontját, illetve törölheti annak bejegyzését.

A Microsoft Management Console (MMC) segítségével további műveleteket is végrehajthatnak a rendszergazdák, többek között figyelemmel követhetik az eseményeket, illetve kezelhetik az Active Directoryt, az Internet Information Services (IIS) szolgáltatást és az SQL Server kiszolgálót.