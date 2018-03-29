---
TOCTitle: 'Kulcstároló-verziók kizárása'
Title: 'Kulcstároló-verziók kizárása'
ms:assetid: 'e287f026-aab2-43ab-93bc-48087da82f36'
ms:contentKeyID: 18122703
ms:mtpsurl: 'https://technet.microsoft.com/hu-hu/library/Cc747700(v=WS.10)'
---

Kulcstároló-verziók kizárása
============================

Az ügyfelekhez rendelt kulcstároló-verziók használatával zárhatja ki a korábbi verziókat, így biztosíthatja, hogy az ügyfelek az RMS kulcstároló szoftver megfelelő verzióját használják. A szolgáltatás engedélyezésekor a kulcstároló minimális verzióját adja meg, amelyet a Microsoft aktiválási szolgáltatása írt alá. Ezután minden olyan fürt felügyeleti webhelyén engedélyezi a kulcstároló verzióinak kizárását, ahol érvénybe szeretné léptetni. A rendszer ekkor minden tanúsítási és licenckérelmet megvizsgál, hogy eleget tesz-e a kulcstároló minimális verziójára vonatkozó feltételnek.

Ha engedélyezte a kulcstároló verzióján alapuló kizárást, a kulcstároló megadott értékénél korábbi verziót használó ügyfelek nem szerezhetnek be tartalomvédelmi fióktanúsítványt vagy használati licencet, mert kérelmeik el lesznek utasítva. Ezek az ügyfelek az RMS ügyfélszoftver új verziójának telepítésével kaphatnak a szoftver aktuális verzióját használó új kulcstárolót.

A Service Pack 1 (SP1) RMS ügyfele 5.0.0.0 vagy nagyobb verziószámú kulcstárolót használ. Ha erre a minimális verzióra állítja be a kulcstároló-kizárást, a szervezetben található RMS ügyfeleknek az SP1 RMS ügyfélre kell frissíteniük a szoftvert ahhoz, hogy használhassák az RMS-védelemmel ellátott tartalmat.

A tartalomhoz korábban kiadott licenccel, de kizárt kulcstárolóval rendelkező felhasználó új kulcstároló beszerzése nélkül továbbra is használhatja az adott tartalmat.
