---
TOCTitle: Az adatbázis méretnövekedésének becslése
Title: Az adatbázis méretnövekedésének becslése
ms:assetid: '87652cc2-b886-4797-8d40-356669768089'
ms:contentKeyID: 18122573
ms:mtpsurl: 'https://technet.microsoft.com/hu-hu/library/Cc747585(v=WS.10)'
---

Az adatbázis méretnövekedésének becslése
========================================

Az RMS adatbázisaihoz szükséges tárolási kapacitás becslésekor a kiindulási érték 10 MB, és ezt kell minden 500 felhasználónál 1 MB tárhellyel bővíteni az RMS konfigurációs adatbázisánál. A naplózási adatbázis a konfigurációs adatbázisétól eltérő kiszolgálón is elhelyezkedhet.

Az RMS naplózási szolgáltatásának használatakor a naplózási adatbázis méretnövekedése felhasználónként közelítőleg 1 MB a kezdeti felhasználótanúsítási szakaszban, amikor nagy mennyiségű naplóbejegyzésre kerül sor. Ha például a bevezetés 1000 felhasználót szolgál ki, a naplózási adatbázis 1 GB méretűre növekszik, amikor az RMS tanúsítási kiszolgálója az összes felhasználót aktiválja és tanúsítvánnyal látja el. A szokásos műveletek során a naplózási adatbázis méretnövekedése naponta és felhasználónként mintegy 200 KB (szakaszos bővítésnél további 1 MB számítható minden újonnan felvett felhasználóra).
