---
TOCTitle: Az RMS naplózási adatbázisa
Title: Az RMS naplózási adatbázisa
ms:assetid: '8ba147f3-16e4-4d9a-ac8f-f05ba2ba11bb'
ms:contentKeyID: 18122664
ms:mtpsurl: 'https://technet.microsoft.com/hu-hu/library/Cc747669(v=WS.10)'
---

Az RMS naplózási adatbázisa
===========================

Az RMS telepítője legfelső szintű tanúsítási vagy licencelési fürtönként telepít egy naplózási adatbázist az adatbázis-kiszolgáló ugyanazon példányára, amelyen a konfigurációs adatbázis fut. A telepítő egy, a naplózásra szolgáló saját várólistát is létrehoz a Message Queuing szolgáltatásban. A naplózási figyelőszolgáltatás ebből a várólistából továbbítja az adatokat a naplózási adatbázisba.

Az RMS szolgáltatás csoport Execute (Végrehajtási) engedélyekkel rendelkezik a naplózási adatbázis tárolt eljárásaihoz.

A naplózási figyelőszolgáltatás hatalmas mennyiségű adatot küld a naplózási adatbázisba, ezért a rendszergazdák szűrők létrehozásával beállíthatják, hogy a naplózási adatbázis csak azokat az információkat tárolja, amelyekre az adott szervezetnek szüksége van.
