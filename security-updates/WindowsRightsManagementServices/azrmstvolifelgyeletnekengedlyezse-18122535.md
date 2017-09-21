---
TOCTitle: Az RMS távoli felügyeletének engedélyezése
Title: Az RMS távoli felügyeletének engedélyezése
ms:assetid: '00f17054-5f5d-47e2-89c1-7a593b930bb3'
ms:contentKeyID: 18122535
ms:mtpsurl: 'https://technet.microsoft.com/hu-hu/library/Cc720181(v=WS.10)'
---

Az RMS távoli felügyeletének engedélyezése
==========================================

Az RMS távoli felügyeletéhez használt számítógépen az Internet Explorer 6.0 vagy újabb webböngészőnek telepítve kell lennie.

Az RMS távoli felügyeletének engedélyezése
------------------------------------------

#### Az RMS távoli felügyeletének engedélyezése

1.  Jelentkezzen be arra a kiszolgálóra, amelyen engedélyezni kívánja a távoli felügyeletet.

2.  A **Felügyeleti eszközök** segédprogramban nyissa meg az **Internet Information Services (IIS) kezelője** beépülő modult.

3.  Bontsa ki az RMS-szolgáltatást tartalmazó webhelynek megfelelő elemet.

4.  Kattintson jobb oldali egérgombbal a **\_wmcs** mappára, és válassza a **Tulajdonságok** parancsot. A **Könyvtárbiztonság** panellap **Biztonságos kommunikáció** csoportjában kattintson a **Szerkesztés** gombra, majd a **Biztonságos csatorna szükséges** beállításra, végül az **OK** gombra. Ezzel bekapcsolja a Secure Sockets Layer (SSL) védelmet az RMS webszolgáltatásaira. Ha tájékoztatást szeretne kapni arról, hogyan kezelhetők a webhelyek az IIS használatával, olvassa el az IIS súgóját.

    | ![](images/Cc720181.Important(WS.10).gif)Fontos:                                                                                                                                                                                                                                                                     |
    |---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
    | Az RMS webszolgáltatások az SSL segítségével további védelemben részesíthetők, ami lehetővé teszi az RMS felügyeleti webhelyének HTTP protokollal, távolról történő elérését. Ha azt tervezi, hogy engedélyezi az SSL-protokollt az RMS webszolgáltatásaira vonatkozóan, szerezzen be és telepítsen egy érvényes SSL webkiszolgálói tanúsítványt. |

5.  Kattintson jobb oldali egérgombbal az **Admin** mappára, és válassza a **Tulajdonságok** parancsot. A **Könyvtárbiztonság** panellap **IP-cím és tartománynév korlátozása** csoportjában kattintson a **Szerkesztés** gombra, majd az **IP-címek korlátozása** csoportban kattintson a **Hozzáférés engedélyezve** beállításra. Ezzel engedélyezheti az összes számítógép számára a webhelyre irányuló kapcsolatok kérését.
