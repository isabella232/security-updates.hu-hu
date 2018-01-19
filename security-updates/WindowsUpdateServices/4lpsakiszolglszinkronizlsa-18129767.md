---
TOCTitle: '4. lépés: A kiszolgáló szinkronizálása'
Title: '4. lépés: A kiszolgáló szinkronizálása'
ms:assetid: 'a5514e46-a50b-46a6-9e5b-33c87c5b7cef'
ms:contentKeyID: 18129767
ms:mtpsurl: 'https://technet.microsoft.com/hu-hu/library/Cc708523(v=WS.10)'
---

4. lépés: A kiszolgáló szinkronizálása
======================================

A hálózati kapcsolat beállítását követően letölthetők a szükséges frissítések. A Windows Server Update Services (WSUS) szolgáltatás alapértelmezés szerint az összes Microsoft-termékhez letölti a fontos és a biztonsági frissítéseket. A frissítések letöltéséhez *szinkronizálni* kell a WSUS-kiszolgálót.

A szinkronizálás során a kiszolgáló kapcsolatot létesít a Microsoft Update webhellyel, majd megállapítja, hogy az utolsó szinkronizálás óta közzétettek-e új frissítéseket. Mivel a WSUS-kiszolgálót most először szinkronizálja, valamennyi frissítés letölthetőként jelenik meg, így jóvá is hagyható telepítésre.

> [!NOTE]  
> Ebben a részben az alapbeállításokkal történő szinkronizálásról lesz szó, ám a WSUS megfelelő beállításaival minimalizálható például a szinkronizáláshoz szükséges sávszélesség. További információt a „Deploying Microsoft Windows Server Update Services” (A Microsoft Windows Server Update Services szolgáltatás központi telepítése) című (angol nyelvű) szakmai dokumentáció tartalmaz. 

**A WSUS-kiszolgáló szinkronizálása**
1.  A WSUS-konzol eszköztárán kattintson a **Beállítások** gombra, majd kattintson a **Szinkronizálási beállítások** hivatkozásra.

2.  A **Feladatok** területen kattintson a **Szinkronizálás** hivatkozásra.

A szinkronizálás befejezését követően a frissítések listájának megtekintéséhez kattintson a WSUS-konzol eszköztárának **Frissítések** elemére.
