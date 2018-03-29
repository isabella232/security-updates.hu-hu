---
TOCTitle: Tartalomvédelmi fióktanúsítványok kizárása
Title: Tartalomvédelmi fióktanúsítványok kizárása
ms:assetid: 'e5cd9dec-ac29-437e-8515-dc697ec75edf'
ms:contentKeyID: 18122773
ms:mtpsurl: 'https://technet.microsoft.com/hu-hu/library/Cc747785(v=WS.10)'
---

Tartalomvédelmi fióktanúsítványok kizárása
==========================================

A művelet végrehajtásához helyben kell bejelentkeznie a felügyeleti webhelyre olyan tartományi felhasználói fiókkal, amely a Rendszergazdák csoport tagja az elérni kívánt számítógépen. A Tartománygazdák csoport tagjai is végrehajthatják ezt a műveletet. Biztonsági szempontból ajánlott a műveletet a **Futtatás másként** parancs segítségével végrehajtani.

A **Globális felügyelet** lap megnyitásához kattintson a **Start** gombra, és válassza a **Minden program**, a **Windows RMS**, majd a **Windows RMS felügyeleti webhely** parancsot.

Ezeket a feltételeket az ügyfél tartatja be akkor, amikor a használati licencet hozzáköti a védelemmel ellátott tartalomhoz.

Tartalomvédelmi fióktanúsítványok kizárása
------------------------------------------

#### Tartalomvédelmi fióktanúsítványok kizárása

1.  Nyissa meg a **Globális felügyelet** lapot, majd keresse meg azt a webhelyet, amelyen tartalomvédelmi fióktanúsítványokat szeretne kizárni, és kattintson a mellette látható **A webhelyen működő RMS felügyelete** hivatkozásra.

2.  A **Felügyeleti hivatkozások** csoportban kattintson a **Kizárási szabályzatok** hivatkozásra.

3.  A felhasználók tartalomvédelmi fióktanúsítványának kizárásához a tartalomvédelmi fióktanúsítvány kizárása csoportban kattintson az **Engedélyezés** elemre.

4.  Válassza ki a kizárni kívánt fióktanúsítvány meghatározásának módját:

    -   Ha a fióktanúsítványt a felhasználónév alapján szeretné kizárni, kattintson **A kizárandó tartalomvédelmi fióktanúsítvány felhasználóneve** beállításra, írja be a kizárni kívánt felhasználó nevét (a *felhasználónév*@*tartománynév*.com formában), majd kattintson a **Hozzáadás** gombra. Ezt a beállítást az Active Directory felhasználói fiókkal rendelkező belső felhasználók fióktanúsítványának kizárásához használja.

    -   Ha a fióktanúsítványt annak nyilvános kulcsa alapján szeretné kizárni, kattintson **A kizárandó tartalomvédelmi fióktanúsítvány nyilvánoskulcs-karakterlánca** beállításra, írja be a megfelelő tartalomvédelmi fióktanúsítvány nyilvános kulcsát, majd kattintson a **Hozzáadás** gombra. Ezt a beállítást az Active Directory felhasználói fiókkal nem rendelkező külső felhasználók fióktanúsítványának kizárásához használja.

    > [!NOTE]  
    > Ha törölni szeretne egy fióktanúsítványt a kizárási listáról, kattintson a listában a kizárt tartalomvédelmi fióktanúsítványra, majd **A kijelölt nyilvános kulcsok törlése a kizárási listáról** elemre. Az adott fióktanúsítvánnyal rendelkező felhasználó ezután kérhet licencet az RMS-védelemmel ellátott tartalomhoz az adott kiszolgálón.

    > [!NOTE]  
    > A tartalomvédelmi tanúsítványfiókok kizárásának letiltásához kattintson a **Letiltás** elemre.

Az eljárás végrehajtásáról a további tudnivalókat lásd: „[Tartalomvédelmi fióktanúsítványok kizárása](https://technet.microsoft.com/cba5e901-942c-4d06-9865-e6c4648c95e6)”.