---
TOCTitle: '7. lépés: Frissítések jóváhagyása és központi telepítése'
Title: '7. lépés: Frissítések jóváhagyása és központi telepítése'
ms:assetid: '38db25a9-6702-4e43-b536-764e8814afc6'
ms:contentKeyID: 18129697
ms:mtpsurl: 'https://technet.microsoft.com/hu-hu/library/Cc720504(v=WS.10)'
---

7. lépés: Frissítések jóváhagyása és központi telepítése
========================================================

Ebben a lépésben a tesztcsoportban lévő ügyfélszámítógépek bármelyikére alkalmazható frissítést kell jóváhagynia. Az ebben a csoportban elhelyezkedő számítógépek a következő 24 órában kapcsolatot fognak létesíteni a WSUS-kiszolgálóval, így ezen idő eltelte után a WSUS jelentéskészítő szolgáltatásával meghatározható, hogy a rendszer sikeresen telepítette-e a frissítéseket a számítógépekre. Amennyiben a tesztelés rendben zajlik, a vállalat vagy a hálózat többi számítógépére vonatkozóan is jóváhagyhatja a frissítést.

Az 7. lépésben a következő műveleteket kell végrehajtani:

-   Frissítés jóváhagyása és központi telepítése
-   A Frissítések állapota jelentés ellenőrzése

**Frissítés jóváhagyása és központi telepítése**
1.  A WSUS-konzol eszköztárán kattintson a **Frissítések** gombra. A program alapértelmezés szerint csak azon fontos és biztonsági frissítéseket jeleníti meg, amelyek ügyfélszámítógépeken történő keresését engedélyezték. Használja az alapértelmezett szűrőt.

2.  Jelölje ki a frissítések listájában a telepítésre jóváhagyni kívánt frissítéseket (a kijelölt frissítések adatai a **Részletek** lapon láthatók). Ha több egymás után következő frissítést szeretne kijelölni, tartsa lenyomva a SHIFT billentyűt, és úgy kattintson az egyes frissítésekre. A CTRL billentyűt lenyomva tartva több, nem egymás után álló frissítést jelölhet ki.

3.  Kattintson a **Frissítési feladatok** csoport **Jóváhagyás módosítása** elemére. Megjelenik a **Frissítések jóváhagyása** párbeszédpanel.

4.  A **Kijelölt frissítések jóváhagyási beállításainak csoportosítása** listában kattintson a tesztcsoport **Jóváhagyás** oszlopában látható **Telepítés** elemre, majd az **OK** gombra.

> [!NOTE]  
> A frissítések jóváhagyása során számos más lehetőség is rendelkezésre áll, például határidő beállítása és a frissítések eltávolítása. Mindezekről a „Microsoft Windows Server Update Services Operations Guide” (Használati útmutató a Microsoft Windows Server Update Services szolgáltatáshoz) című (angol nyelvű) szakmai dokumentációban olvashat részletesen. 

24 óra elteltével a WSUS jelentéskészítő szolgáltatásával meghatározható, hogy a rendszer sikeresen telepítette-e a frissítéseket a számítógépekre.

**A Frissítések állapota jelentés ellenőrzése**
1.  Kattintson a WSUS-konzol eszköztárán lévő **Jelentések** gombra.

2.  Kattintson a **Jelentések** lap **Frissítések állapota** elemére.

3.  A frissítések listájának szűréséhez adja meg a **Nézet** csoportban a szűrés feltételeit, majd kattintson az **Alkalmaz** gombra.

4.  Amennyiben számítógépcsoport, majd számítógép szerint kívánja megtekinteni egy adott frissítés állapotát, szükség szerint bontsa ki a frissítésnézetet.

5.  A Frissítések állapota jelentés kinyomtatásához kattintson a **Feladatok** csoport **Jelentés nyomtatása** elemére.

Ha a program rendben telepítette a frissítéseket a tesztcsoport számítógépeire, a vállalat vagy a hálózat többi számítógépére vonatkozóan is jóváhagyhatja a frissítéseket.
