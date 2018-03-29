---
TOCTitle: Több erdőt átfogó bevezetés tervezése
Title: Több erdőt átfogó bevezetés tervezése
ms:assetid: '2dfb40b7-95b1-4362-b32e-72867544b705'
ms:contentKeyID: 18122526
ms:mtpsurl: 'https://technet.microsoft.com/hu-hu/library/Cc720233(v=WS.10)'
---

Több erdőt átfogó bevezetés tervezése
=====================================

Ha több erdőt tartalmazó környezetben vezeti be az RMS szolgáltatást, el kell dönteni, hogy milyen támogatást kell nyújtani azoknak a felhasználóknak és csoportoknak, amelyek nem abba az erdőbe tartoznak, amelyben az RMS működik. Ezzel az a probléma, hogy a más erdőbe tartozó felhasználó- és csoportobjektumoknak általában nem felel meg objektum abban az erdőben, amelyben az RMS található. Ha úgy tervezi használni az RMS szolgáltatást, hogy a más erdőből származó felhasználókra és csoportokra korlátozza az engedélyeket, ennek megfelelően úgy kell konfigurálni az erdőt, hogy lehetővé tegye a másik erdőbe tartozó csoportok behelyettesítését.

Kétféleképpen alakítható ki a más erdőbe tartozó csoportok behelyettesítése az RMS számára:

-   Az RMS szolgáltatást be kell vezetni abban az erdőben, ahol a csoportokat definiálták, és ahol használni fogják a csoportok tagságának behelyettesítésére.

-   Szinkronizálni kell az erdők között a csoportdefiníciókat, mert így az RMS helyi telepítése minden felhasználónál meg tudja állapítani a teljes csoporttagságot. Ha a használati licencet kérelmező felhasználónak másik erdőben található a Windows-fiókja, akkor léteznie kell a helyi erdőben egy olyan kapcsolatobjektumnak, amely megjeleníti a felhasználó csoporttagságát. Metacímtárak, például a Microsoft® Identity Integration Server (MIIS) 2003 vagy az Identity Integration Feature Pack (IIFP) segítségével teljes körben szinkronizálhatók egymással a különböző erdők csoportobjektumai.

Ha az RMS szolgáltatást csak egy erdőben fogja használni, optimalizálhatja a használati licencek kiállítási eljárását az RMS konfigurációs adatbázisában lévő **MaxCrossForestCalls** fürtszabályzat módosításával. Ez a szabályzat azt adja meg, hogy egy csoport tagja hányszor léphet át erdők közötti határon. Az alapértelmezett érték 10. A 0 érték beállításához a következő SQL utasítás használható:

`update DRMS_ClusterPolicies set PolicyData=0 where PolicyName='MaxCrossForestCalls'`