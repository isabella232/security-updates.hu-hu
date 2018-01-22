---
TOCTitle: Változtatások végrehajtása a konfigurációs adatbázisban
Title: Változtatások végrehajtása a konfigurációs adatbázisban
ms:assetid: '6a7bec73-09e4-4060-b551-5990836df4bc'
ms:contentKeyID: 18122609
ms:mtpsurl: 'https://technet.microsoft.com/hu-hu/library/Cc747606(v=WS.10)'
---

Változtatások végrehajtása a konfigurációs adatbázisban
=======================================================

A felügyeleti webhelyen keresztül végrehajtott konfigurációs változtatások a kiszolgáló vagy a fürt konfigurációs adatbázisában is érvényesülnek. Kifejezetten ajánljuk, hogy a konfigurációs beállításokat mindig a felügyeleti webhelyen módosítsa, kézzel ne módosítsa a konfigurációs adatbázis adatait. Az adatbázis kézi módosítására a következő két helyzetben lehet szükség:

-   **A naplózási adatbázis áthelyezése másik kiszolgálóra.** A naplózási adatbázis alapértelmezés szerint ugyanazon a kiszolgálón található, mint a konfigurációs adatbázis. Ha a naplózási adatbázist másik kiszolgálóra szeretné áthelyezni, a konfigurációs adatbázisban meg kell adnia a naplózási adatbázis új helyét. A naplózási adatbázis áthelyezéséről és a konfigurációs adatbázis megfelelő módosításáról „[A naplózási adatbázis áthelyezése](https://technet.microsoft.com/34ea8045-dc94-422e-9601-29927cfc1534)” című pont tartalmaz további tájékoztatást.

-   **A tartalomvédelmi fióktanúsítványokhoz kapcsolt felhasználói kulcsok eltávolítása**. Amikor eltávolít egy felhasználói fiókot az Active Directoryból, illetve kizár vagy visszavon egy tartalomvédelmi fióktanúsítványt a felügyeleti webhelyen, a tartalomvédelmi fióktanúsítványhoz tartozó felhasználói kulcsok nem törlődnek a konfigurációs adatbázisból. Az inaktív felhasználói kulcsokat kézzel kell eltávolítani a konfigurációs adatbázisból, egyrészt biztonsági okokból, másrészt hogy megkönnyítse az ügyféllicencek (CAL) számának nyilvántartását. A konfigurációs adatbázisban található felhasználói kulcsok eltávolításáról a „[Felhasználói fiókok törlése](https://technet.microsoft.com/bf73b141-d4d1-4807-a773-3aaff58b0db6)” című pont tartalmaz további tájékoztatást. Az ügyféllicencek nyilvántartásának részletes ismertetését lásd: „[A tartalomvédelmi fióktanúsítványok nyilvántartása](https://technet.microsoft.com/5bb0f3cf-fc44-4e60-a93f-c789d6f8a902)”.

Ha közvetlenül kell módosítania a konfigurációs adatbázist, forduljon az adatbázis-kiszolgáló rendszergazdájához.