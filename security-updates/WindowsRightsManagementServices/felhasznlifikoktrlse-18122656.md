---
TOCTitle: Felhasználói fiókok törlése
Title: Felhasználói fiókok törlése
ms:assetid: 'bf73b141-d4d1-4807-a773-3aaff58b0db6'
ms:contentKeyID: 18122656
ms:mtpsurl: 'https://technet.microsoft.com/hu-hu/library/Cc747653(v=WS.10)'
---

Felhasználói fiókok törlése
===========================

Amikor felhasználói fiókot töröl az Active Directoryból, a legfelső szintű tanúsítási fürt konfigurációs adatbázisában a felhasználói kulcstáblában lévő felhasználói tartalomvédelmi fióktanúsítvány bejegyzése nem törlődik automatikusan. Ezért a felhasználói kulcstábla mérete jelentősen megnövekedhet, ha új kulcsokat vesznek fel, de a régieket nem törlik.

A konfigurációs adatbázis karbantartásához olyan tárolt eljárást futtathat, amely a biztonsági azonosító (SID) alapján törli azt a felhasználói kulcsot, amelynek kapcsolódó felhasználói fiókját eltávolították az Active Directoryból. Másik megoldásként rendszeres időközönként olyan parancsfájlt futtathat, amely a konfigurációs adatbázisból törli azokat a felhasználói kulcsokat, amelyeknek nem felel meg SID azonosító az Active Directoryban. Ne feledje, hogy ez jelentős terhelést jelent az SQL Server és az Active Directory számára.
