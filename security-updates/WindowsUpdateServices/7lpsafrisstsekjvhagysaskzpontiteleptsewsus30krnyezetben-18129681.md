---
TOCTitle: '7. lépés: A frissítések jóváhagyása és központi telepítése WSUS 3.0 környezetben'
Title: '7. lépés: A frissítések jóváhagyása és központi telepítése WSUS 3.0 környezetben'
ms:assetid: '88fac442-a9d3-4e74-92f6-3822b7237af1'
ms:contentKeyID: 18129681
ms:mtpsurl: 'https://technet.microsoft.com/hu-hu/library/Cc708475(v=WS.10)'
---

7. lépés: A frissítések jóváhagyása és központi telepítése WSUS 3.0 környezetben
================================================================================

Ebben a lépésben egy, a tesztcsoportban lévő ügyfélszámítógépek bármelyikére alkalmazható frissítést kell jóváhagynia. A ebbe a csoportba tartozó számítógépek a következő 24 órában kapcsolatot fognak létesíteni a WSUS-kiszolgálóval. Ezt követően a WSUS jelentéskészítő szolgáltatásával meghatározható, hogy a rendszer sikeresen telepítette-e a frissítéseket a számítógépekre. Amennyiben a tesztelés rendben zajlik, a vállalat vagy a hálózat többi számítógépére vonatkozóan is jóváhagyhatja a frissítéseket.

**Az 7. lépésben a következő műveleteket kell végrehajtani**:

-   Frissítés jóváhagyása és központi telepítése
-   A Frissítések állapota jelentés ellenőrzése

**Frissítés jóváhagyása és központi telepítése**
1.  A WSUS felügyeleti konzolon kattintson a **Frissítések** gombra. Ennek hatására megjelenik a frissítések összefoglalása az alapértelmezett nézetekben (a **Minden frissítés**, a **Fontos frissítések**, a **Biztonsági frissítések** és a **WSUS-frissítések** nézetben). Ebben a műveletsorban a **Minden frissítés** nézetet használja.

2.  Jelölje ki a frissítések listájában a telepítésre jóváhagyni kívánt frissítéseket (a kijelölt frissítések adatai a Frissítések panel legalsó ablaktábláján láthatók). Ha több egymás után következő frissítést szeretne kijelölni, tartsa lenyomva a **SHIFT** billentyűt, és úgy kattintson az egyes frissítésekre. A **CTRL** billentyűt lenyomva tartva több, nem egymás után álló frissítést jelölhet ki.

3.  Kattintson a jobb gombbal a kijelölt frissítésekre, majd kattintson a **Jóváhagyás** parancsra. Megjelenik a **Frissítések jóváhagyása** párbeszédpanel.

4.  Jelölje ki az egyik (például a **Teszt**) csoportot, és kattintson a bal oldalán látható nyílra. Megjelenik egy helyi menü, amely az alábbi lehetőségeket tartalmazza: **Telepítésre jóváhagyva**, **Eltávolításra jóváhagyva**, **Nincs jóváhagyva**, **Határidő**, **A szülővel azonos** és **Alkalmazás a gyermekekre**. Kattintson a **Telepítésre jóváhagyva** elemre, majd az **OK** gombra.

5.  Megjelenik a **Jóváhagyás állapota** ablak, amelyben a frissítések jóváhagyását befolyásoló különféle feladatok előrehaladása látható. Amikor befejezte a jóváhagyást, zárja be az ablakot a **Bezárás** gombra kattintva.

| ![](images/Cc708475.note(WS.10).gif)Megjegyzés:                                                          |
|---------------------------------------------------------------------------------------------------------------------------------------|
| A frissítések jóváhagyása során számos más lehetőség is rendelkezésre áll, például határidő beállítása és a frissítések eltávolítása. |

24 óra elteltével a WSUS jelentéskészítő szolgáltatásával meghatározható, hogy a rendszer sikeresen telepítette-e a frissítéseket a számítógépekre.

**A frissítések állapotának ellenőrzése**
1.  A WSUS felügyeleti konzolon kattintson a bal oldali ablaktáblán a **Jelentések** gombra.

2.  A **Jelentések** lapon több szabványos jelentések látható. Kattintson a **Frissítési állapot összegzése** jelentésre. Megjelenik a **Frissítési jelentések** ablak.

3.  A frissítések listájának szűréséhez adja meg a szűrés feltételeit (például **A frissítések belevétele ezekbe a besorolásokba**), majd kattintson az ablak eszköztárán a **Jelentés futtatása** gombra.

4.  Megjelenik a **Frissítési jelentések** ablaktábla. Az egyes frissítések állapotának ellenőrzéséhez jelölje ki az ablaktábla bal oldalán a kívánt frissítést. Ekkor a jelentéseket tartalmazó ablaktábla utolsó szakasza a frissítés állapotának összefoglalását fogja mutatni.

5.  A jelentést mentheti vagy kinyomtathatja az eszköztár megfelelő ikonjára kattintva.

Ha a program rendben telepítette a frissítéseket a tesztcsoport számítógépeire, a vállalat vagy a hálózat többi számítógépére vonatkozóan is jóváhagyhatja a frissítéseket.
