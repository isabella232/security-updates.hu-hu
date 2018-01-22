---
TOCTitle: 'A naplózás be- és kikapcsolása'
Title: 'A naplózás be- és kikapcsolása'
ms:assetid: '50ccd827-2d39-41e7-a395-3d5f5836869b'
ms:contentKeyID: 18122581
ms:mtpsurl: 'https://technet.microsoft.com/hu-hu/library/Cc747565(v=WS.10)'
---

A naplózás be- és kikapcsolása
==============================

Az aktuális fürt vagy kiszolgáló naplózását a **Naplózási beállítások** lapon kapcsolhatja be és ki. A naplózás kikapcsolása után az RMS-webszolgáltatások nem küldenek naplózási adatokat a naplózási üzenetsorba. A naplózás kikapcsolása egyúttal leállítja a naplózási figyelőszolgáltatást is. A naplózás nem kapcsolható ki a Windows Server 2003 Szolgáltatások nevű felügyeleti eszközével.

Az RMS-naplókat az üzenetsor-kezelés szolgáltatás küldi az adatbázis-kiszolgálóra. Ha az adatbázis-kiszolgálóval nincs kapcsolat, az üzenetsor-kezelés szolgáltatás a kapcsolat létrejöttéig egy helyi gyorsítótárban tárolja a naplófájlokat. Amikor első alkalommal engedélyezi a naplózást, ellenőrizze, hogy az RMS-kiszolgáló kapcsolódik-e az adatbázis-kiszolgálóhoz, és hogy az adatbázis szolgáltatás el van-e indítva. Ha adatbázis-kiszolgálóként SQL Server kiszolgálót használ, az alábbi lépésekkel ellenőrizheti, hogy a rendszer átvezeti-e a naplókat az adatbázisba.

-   Az SQL Server Enterprise Manager programjában keresse meg a naplózási adatbázist, bontsa ki a **Databases (Adatbázisok)** ágat, majd azt az adatbázist, amely az RMS naplózási adatbázisát tartalmazza.
-   Kattintson a naplózási adatbázisra, majd a **Tables** (Táblák) elemre, kattintson jobb oldali egérgombbal a **DRMS\_log\_master** táblára, és válassza az **Open table - return all rows** (Tábla megnyitása - összes sor megjelenítése) parancsot. Ha már készít naplófájlokat a szolgáltatás, itt megjelenik legalább egy naplófájl.
