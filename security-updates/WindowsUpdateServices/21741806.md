---
TOCTitle: '7. lépés: A WSUS frissítéseinek jóváhagyása és központi telepítése'
Title: '7. lépés: A WSUS frissítéseinek jóváhagyása és központi telepítése'
ms:assetid: 'c4e58e17-d5e3-4194-8f26-b459e0c03b86'
ms:contentKeyID: 21741806
ms:mtpsurl: 'https://technet.microsoft.com/hu-hu/library/Dd939909(v=WS.10)'
---

7. lépés: A WSUS frissítéseinek jóváhagyása és központi telepítése
==================================================================

Ebben a lépésben a tesztcsoport bármely számítógépének frissítését hagyhatja jóvá a Windows Server Update Services 3.0 Service Pack 2 (WSUS 3.0 SP2) szolgáltatáshoz. A csoportban lévő számítógépek automatikusan felveszik a kapcsolatot a WSUS-kiszolgálóval az elkövetkező 24 órában a frissítés beszerzése érdekében. A WSUS jelentési szolgáltatásával megállapíthatja, hogy a frissítések központi telepítése megtörtént-e a tesztszámítógépeken. Ha a tesztek sikeresen befejeződtek, jóváhagyhatja a frissítéseket a szervezet megfelelő számítógépcsoportjaihoz.

Az 7. lépés műveletei
---------------------

-   Frissítés jóváhagyása és központi telepítése
-   Frissítés állapotának ellenőrzése

**Frissítés jóváhagyása és központi telepítése**
1.  A WSUS felügyeleti konzolon kattintson a **Frissítések** elemre. Ekkor megjelenik a frissítések állapotának összegzése a **Minden frissítés**, **Fontos frissítések**, **Biztonsági frissítések** és **WSUS-frissítések** formájában.

2.  A **Minden frissítés** csoportban kattintson a **Számítógépekre telepítendő frissítések** elemre.

3.  A frissítések listájában jelölje ki azokat a frissítéseket, amelyeket jóvá kíván hagyni a teszteléshez létrehozott számítógépcsoporton való telepítéshez. A kijelölt frissítések adatai a Frissítések panel legalsó ablaktábláján láthatók. Ha több egymás után következő frissítést szeretne kijelölni, tartsa lenyomva a **SHIFT** billentyűt, és úgy kattintson az egyes frissítésekre. A **CTRL** billentyűt lenyomva tartva több, nem egymás után álló frissítést jelölhet ki.

4.  Kattintson a jobb gombbal a kijelölt frissítésekre, majd kattintson a **Jóváhagyás** parancsra.

5.  A **Frissítések jóváhagyása** párbeszédpanelen jelölje ki a tesztcsoportot, majd kattintson a lefelé mutató nyílra.

6.  Kattintson a **Telepítésre jóváhagyva** elemre, majd az **OK** gombra.

7.  Ekkor megjelenik a Jóváhagyás állapota ablak, amelyben a frissítés jóváhagyását érintő feladatok előrehaladása látható. A jóváhagyás befejeződésekor kattintson a **Bezárás** gombra.

24 óra elteltével a WSUS jelentéskészítő szolgáltatásával megállapítható, hogy a rendszer sikeresen telepítette-e a frissítéseket a tesztcsoport számítógépeire.

**A frissítések állapotának ellenőrzése**
1.  A WSUS felügyeleti konzol navigációs ablaktáblájában kattintson a **Jelentések** elemre.

2.  A **Jelentések** lapon kattintson a **Frissítési állapot összegzése** jelentésre. Ekkor megnyílik a **Frissítési jelentés** ablak.

3.  A frissítések listájának szűréséhez adja meg a szűrés feltételeit (például **A frissítések belevétele ezekbe a besorolásokba**), majd kattintson az ablak eszköztárán a **Jelentés futtatása** gombra.

4.  Megjelenik a **Frissítési jelentések** ablaktábla. Az egyes frissítések állapotának ellenőrzéséhez jelölje ki az ablaktábla bal oldalán a kívánt frissítést. Ekkor a jelentéseket tartalmazó ablaktábla utolsó szakasza a frissítés állapotának összefoglalását fogja mutatni.

5.  A jelentést mentheti vagy kinyomtathatja az eszköztár megfelelő ikonjára kattintva.

6.  A frissítések tesztelése után jóváhagyhatja a frissítéseknek a szervezet megfelelő számítógépcsoportjain való telepítését.

További források
----------------

[Részletes útmutató a Windows Server Update Services 3.0 SP2 telepítéséhez](https://technet.microsoft.com/4b504edc-93b3-45b0-a7e8-d0107f1a4442)

További tudnivalók a WSUS 3.0 SP2 szolgáltatás használatáról:

A WSUS központi telepítési útmutatója a [http://go.microsoft.com/fwlink/?LinkId=139832](http://go.microsoft.com/fwlink/?linkid=139832) webhelyen

A WSUS használati útmutatója a [http://go.microsoft.com/fwlink/?LinkId=139838](http://go.microsoft.com/fwlink/?linkid=139838) webhelyen
