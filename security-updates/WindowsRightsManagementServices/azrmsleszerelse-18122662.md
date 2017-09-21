---
TOCTitle: Az RMS leszerelése
Title: Az RMS leszerelése
ms:assetid: '8b563c25-17cd-4b9b-ae42-695497ab6439'
ms:contentKeyID: 18122662
ms:mtpsurl: 'https://technet.microsoft.com/hu-hu/library/Cc747665(v=WS.10)'
---

Az RMS leszerelése
==================

A művelet végrehajtásához helyben kell bejelentkeznie a felügyeleti webhelyre olyan tartományi felhasználói fiókkal, amely a Rendszergazdák csoport tagja az elérni kívánt számítógépen. A Tartománygazdák csoport tagjai is végrehajthatják ezt a műveletet. Biztonsági szempontból ajánlott a műveletet a **Futtatás másként** parancs segítségével végrehajtani.

A **Globális felügyelet** lap megnyitásához kattintson a **Start** gombra, és válassza a **Minden program**, a **Windows RMS**, majd a **Windows RMS felügyeleti webhely** parancsot.

| ![](images/Cc747665.Warning(WS.10).gif)Figyelmeztetés:                            |
|----------------------------------------------------------------------------------------------------------------|
| A leszerelt kiszolgálókon nem állítható vissza a szabványos RMS-konfiguráció. Ez a művelet nem vonható vissza. |

| ![](images/Cc747665.Warning(WS.10).gif)Figyelmeztetés:                                                                                |
|--------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| Az RMS leszerelése után újabb RMS példány csak akkor telepíthető, ha előbb a Programok telepítése és törlése segédprogrammal teljesen eltávolítja a szolgáltatást. |

Az RMS leszerelése
------------------

#### Az RMS leszerelése

1.  Jelentkezzen be arra a kiszolgálóra, amelyen az RMS leszerelését tervezi.

2.  A **Globális felügyelet** weblapon kattintson **A webhelyen működő RMS felügyelete** hivatkozásra.

3.  A **Felügyeleti kezdőlap** lapon kattintson a **Biztonsági beállítások** hivatkozásra.

4.  **Az RMS leszerelése** csoportban jelölje be **Az RMS-telepítés leszerelésének engedélyezése** négyzetet, és kattintson a **Leszerelés** gombra.

5.  Amikor a program kéri, az **OK** gombra kattintva erősítse meg, hogy véglegesen le szeretné szerelni az RMS-telepítést.
