---
TOCTitle: 'RMS-védelem eltávolítása tartalomból'
Title: 'RMS-védelem eltávolítása tartalomból'
ms:assetid: 'c30361e3-50d2-4474-a87d-d38de502cf9e'
ms:contentKeyID: 18122660
ms:mtpsurl: 'https://technet.microsoft.com/hu-hu/library/Cc747658(v=WS.10)'
---

RMS-védelem eltávolítása tartalomból
====================================

Időben el kell dönteni, hogy mely fájlokat kell helyreállítani, ezt ki és mikor hajtsa végre, hogy így minden fontos adat megőrizhető legyen, amikor befejeződik a leszerelési eljárás. Amikor az RMS-védelem az összes szükséges fájlból el lett távolítva, a kiszolgáló eltávolítható az infrastruktúrából.

Az RMS-védelem eltávolításának lépései a következők:

1.  A felhasználónak el kell távolítania az összes használati licencet a számítógépről. Ez biztosítja, hogy az RMS ügyfél a tartalom megnyitásakor a szükséges licenc beszerzéséhez a kiszolgálóhoz fordul. A használati licencek az ügyfélszámítógépen a %USERPROFILE%\\Local Settings\\Application Data\\Microsoft\\DRM mappában találhatók, és a fájlnevekben az EUL előtag szerepel.
2.  A leszerelési kiszolgálóhoz hozzáféréssel rendelkező felhasználó megkísérel megnyitni egy RMS-védelemmel ellátott fájlt.
3.  Az alkalmazás csatlakozik a leszerelési kiszolgálóhoz, és tartalomkulcsot kap.
4.  Ekkor megtörténik a tartalom visszafejtése, és az szerkeszthető, menthető, továbbítható vagy nyomtatható.
5.  A felhasználó RMS-védelem nélkül menti a tartalmat. Ezután az összes felhasználó az RMS kiszolgálóra való csatlakozás nélkül megnyithatja a tartalmat.
