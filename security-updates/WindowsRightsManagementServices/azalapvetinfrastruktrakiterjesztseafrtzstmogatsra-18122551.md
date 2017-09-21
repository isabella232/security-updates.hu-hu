---
TOCTitle: Az alapvető infrastruktúra kiterjesztése a fürtözés támogatására
Title: Az alapvető infrastruktúra kiterjesztése a fürtözés támogatására
ms:assetid: '78f0f2f0-a075-409c-9f46-26eb62d1d05b'
ms:contentKeyID: 18122551
ms:mtpsurl: 'https://technet.microsoft.com/hu-hu/library/Cc747567(v=WS.10)'
---

Az alapvető infrastruktúra kiterjesztése a fürtözés támogatására
================================================================

Ha nagyobb környezetben fürtökön vezeti be a rendszert, biztosítsa a fürtözés követelményeinek infrastrukturális feltételeit. A bevezetési tervnek a következő elemeket kell tartalmaznia.

DNS-regisztráció
----------------

Ügyeljen arra, hogy minden olyan DNS-regisztráció, amely az extranet irányában közzéteszi a virtuális IP-címet, megtörténjen az intranet irányában is.

Ha nincs DNS-regisztráció az intranet oldalán, sikertelenek lesznek a belső licenckérelmek. Ha nem módosíthatók a DNS-beállítások, a fürtbe tartozó minden kiszolgálón módosítani lehet az állomástáblát úgy, hogy a fürt URL-címét hozzárendelje a fürt virtuális IP-címéhez. A DNS-regisztrációt a fürt létesítése előtt kell végrehajtani. Ha már létesítette a szolgáltatást, el kell távolítani az RMS szolgáltatást a kiszolgálóról, és meg kell ismételni a létesítési folyamatot.

Terheléselosztás
----------------

A kérelmek fürtcsomópontok közötti elosztásához be kell állítani a terheléselosztás bevezetésének engedélyezéséhez szükséges hardvert és szoftvert, illetve szükség szerint működésbe kell állítani a hálózati terheléselosztási szolgáltatást vagy a hardveres terheléselosztót.
