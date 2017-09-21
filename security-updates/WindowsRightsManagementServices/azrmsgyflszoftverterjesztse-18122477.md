---
TOCTitle: Az RMS ügyfélszoftver terjesztése
Title: Az RMS ügyfélszoftver terjesztése
ms:assetid: '4b8dd930-4105-4e73-918c-12d2b05d5fb5'
ms:contentKeyID: 18122477
ms:mtpsurl: 'https://technet.microsoft.com/hu-hu/library/Cc720266(v=WS.10)'
---

Az RMS ügyfélszoftver terjesztése
=================================

Az RMS ügyfélszoftver be van építve a Windows Vista® operációs rendszerbe, így az RMS ügyfélszoftvert már nem kell külön telepíteni. A Windows Vista előtti operációs rendszerek esetén szükség van az RMS ügyfélszoftver telepítésére és aktiválására.

Az aktiválási eljárás kulcstárolót és géptanúsítványt létesít a jelenleg bejelentkezett felhasználóhoz. Az aktiválás helyi művelet, és nem igényel hálózati kapcsolatot. A sikeres aktiválás után, amikor kompatibilis alkalmazás először kér licenchasználatot, a felhasználó felhasználói tanúsítványhoz jut. Az RMS ügyfélszoftver a Csoportházirend, a Windows Update vagy rendszergazdai parancsfájl segítségével telepíthető a szervezet egyes ügyfélszámítógépeire.

| ![](images/Cc720266.note(WS.10).gif)Megjegyzés:                                                                                                                                                                                                                                                               |
|--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| A terjesztési módszertől függetlenül az RMS ügyfélszoftver az RMS kiszolgálóval történő kommunikációhoz portot használ, alapértelmezés szerint ez a 80-as vagy a 443-as port. Biztosítani kell, hogy az ügyfélszámítógép ezeken a portokon képes legyen kimeneti kérelmeket küldeni az RMS legfelső szintű és a csak licencelő fürtjeihez. |

**A Csoportházirend használata**

Ha a szervezetben szoftver terjesztéséhez a Csoportházirend szolgáltatást használják, ez a magasabb szintű rendszerjogosultságokkal használható az RMS ügyfélszoftver terjesztéséhez is. Ha az RMS ügyfélszoftvert így terjesztik, a felhasználóknak nem szükséges rendszergazdai engedélyekkel rendelkezniük, és a telepítést végrehajthatják a **VezérlőpultProgramok telepítése és törlése** segédprogramjával vagy a tartalomvédelemmel ellátott tartalom megnyitásával egy RMS-kompatibilis alkalmazásban.

**Terjesztés a Windows Update segítségével**

A Windows Update az RMS ügyfélszoftver telepítésének legegyszerűbb módját kínálja. Ennek a módszernek az az előnye, hogy a felhasználóknak ismerős mechanizmust használ, de megköveteli, hogy az RMS ügyfele a számítógépen helyi rendszergazdai jogosultsággal rendelkezzen.

**Terjesztés parancsfájlon alapuló telepítéssel**

Az ügyfélszoftver telepítése a legjobban úgy tartható kézben, hogy letölti a szoftvert, majd parancsfájl futtatásával a telepítési folyamat valamennyi lépésében meggyőződik annak épségéről. Ilyen parancsfájl megírható és indító parancsfájlként hozzárendelhető a Csoportházirend-objektumhoz (GPO). Ennél a módszernél nem szükséges, hogy a felhasználó helyi rendszergazda legyen a számítógépen, az RMS ügyfélszoftver pedig újraindításkor automatikusan telepítődik.

        ```
Az RMS ügyfélszoftver Csoportházirend alkalmazásával való terjesztéséről az alapvető tudnivalókat [Az SMS vagy a Csoportházirend beállítása az ügyfelek központi telepítésére](https://technet.microsoft.com/9e37c27b-8cc1-40c6-adb7-0937aa64c8db) című rész tartalmazza.

Az RMS ügyfélszoftver bevezetésének eljárását [Az RMS-ügyfél bevezetése](https://technet.microsoft.com/c84f1724-cf71-4385-9003-ff68bc23c927) című rész ismerteti.
