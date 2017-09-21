---
TOCTitle: Az RMS konfigurációs adatbázisa
Title: Az RMS konfigurációs adatbázisa
ms:assetid: '769adbdc-f32f-464b-85c4-e8b160036187'
ms:contentKeyID: 18122631
ms:mtpsurl: 'https://technet.microsoft.com/hu-hu/library/Cc747634(v=WS.10)'
---

Az RMS konfigurációs adatbázisa
===============================

Az RMS adatbázis-kiszolgálót, például Microsoft® SQL Server vagy Microsoft SQL Server 2000 Desktop Engine (MSDE 2000) Release A, használ a konfigurációra és a szabályzatokra vonatkozó adatok tárolásához. Minden RMS kiszolgálóhoz vagy fürthöz egy konfigurációs adatbázis tartozik ,és ez tárolja, osztja meg és kéri le a konfigurációs és egyéb adatokat.

A legfelső szintű tanúsítási kiszolgáló vagy fürt konfigurációs adatbázisa tárolja a Windows felhasználói identitások és tartalomvédelmi fióktanúsítványaik listáját. A tanúsítvány kulcspárja az RMS kiszolgáló nyilvános kulcsával való titkosítás után kerül be az adatbázisba. A licenckiszolgálók konfigurációs adatbázisa nem tárolja ezeket az adatokat.

Az RMS szolgáltatás csoport Execute (Végrehajtási) engedélyekkel rendelkezik az adatbázis tárolt eljárásaihoz.

**Fontos   **Az MSDE 2000 csak tesztkörnyezetben használható az RMS adatbázisaihoz, mivel az MSDE 2000 semmilyen hálózati csatlakozófelületet sem támogat. Emellett az MSDE 2000 használati feltételei megtiltják az SQL Server ügyféleszközeinek használatát az MSDE 2000 adatbázisok kezelésére. Ezt a korlátozást figyelembe véve nem áll majd módjában megtekinteni a naplózott adatokat, sem módosítani a konfigurációs adatbázisban tárolt adatokat.
