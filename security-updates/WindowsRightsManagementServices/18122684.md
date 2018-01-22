---
TOCTitle: Jogmegadási sablon szerkesztése
Title: Jogmegadási sablon szerkesztése
ms:assetid: '9580b934-bd6f-4097-9d3c-4fc14a3147fa'
ms:contentKeyID: 18122684
ms:mtpsurl: 'https://technet.microsoft.com/hu-hu/library/Cc747684(v=WS.10)'
---

Jogmegadási sablon szerkesztése
===============================

A művelet végrehajtásához helyben kell bejelentkeznie a felügyeleti webhelyre olyan tartományi felhasználói fiókkal, amely a Rendszergazdák csoport tagja az elérni kívánt számítógépen. A Tartománygazdák csoport tagjai is végrehajthatják ezt a műveletet. Biztonsági szempontból ajánlott a műveletet a **Futtatás másként** parancs segítségével végrehajtani.

A **Globális felügyelet** lap megnyitásához kattintson a **Start** gombra, és válassza a **Minden program**, a **Windows RMS**, majd a **Windows RMS felügyeleti webhely** parancsot.

Jogmegadási sablon szerkesztése
-------------------------------

#### Jogmegadási sablon szerkesztése

1.  Nyissa meg a **Globális felügyelet** lapot, majd keresse meg azt a webhelyet, amelyen szerkeszteni szeretné a jogmegadási sablonokat, és kattintson a mellette látható **A webhelyen működő RMS felügyelete** hivatkozásra.

2.  A **Felügyeleti hivatkozások** csoportban kattintson a **Jogmegadási sablonok** hivatkozásra.

3.  **A sablon neve** listában kattintson a szerkeszteni kívánt sablon nevére.

4.  A **Sablon azonosítása** csoportban módosítsa szükség szerint **A sablon neve**, **A sablon leírása** és a **Jogkérelmező URL** mezőben szereplő adatokat.

5.  A **Felhasználók és csoportok** területen hajtsa végre a megfelelő műveletet:

    -   Ha új felhasználót vagy csoportot kíván hozzáadni, a **Felhasználók és csoportok hozzáadása** csoportban adja meg a felvenni kívánt felhasználó vagy csoport érvényes e-mail címét, kattintson a **Hozzáadás** gombra, majd a **Jelenlegi felhasználók és csoportok** listában jelölje ki a kívánt nevet. A **Jogok** csoportban jelölje be a választott felhasználónak vagy csoportnak megadni kívánt jogokhoz tartozó négyzeteket.

    -   Ha meglévő felhasználó vagy csoport jogait módosítja, jelölje ki a megfelelő nevet a **Jelenlegi felhasználók és csoportok** listában, majd jelölje be a megfelelő négyzeteket vagy törölje azok jelölését.

    -   Ha eltávolít egy csoportot vagy egy felhasználót, jelölje ki a megfelelő nevet a **Jelenlegi felhasználók és csoportok** listában, majd kattintson az **Eltávolítás** gombra.

6.  A **Lejárati szabályzat** csoportban szereplő adatok módosításával adja meg a tartalmi licencek lejáratának, illetve megújításának időpontját.

7.  A **Kiterjesztett szabályzat** csoportban szereplő adatok módosításával adja meg a tartalmi licencek megvalósításának módját, beleértve a szerzői jogok folytonosságát, a megbízható böngészők használhatóságát, a tartalom licenceinek folytonosságát, valamint az alkalmazásspecifikus adatok betartatását.

8.  A **Visszavonási szabályzat** csoportban határozza meg, hogy az adott sablon alapján létrehozott tartalomhoz szükség van-e visszavonási listára. Ha a **Visszavonás megkövetelése** beállítást választja, adja meg a következő beállításokat is:

    -   Az **URL** mezőbe írja be azt az URL-címet. ahol a visszavonási lista fájlja közzé van téve. Ha a nem csatlakozó és a külső felhasználókkal is foglalkoznia kell, a megadott URL-címnek elérhetőnek kell lennie a vállalati hálózatból és az internetről egyaránt. A további tudnivalókat lásd: „[A visszavonás megvalósítása](https://technet.microsoft.com/4735f060-7197-4ae2-830a-f91bcc4de30a)”.

    -   A **Visszavonási lista frissítési időköze** mezőbe írja be, hogy hány napig marad érvényes a visszavonási lista. Ha valamelyik felhasználónál olyan visszavonási lista található, amely korábbi, mint az itt megadott érték, a felhasználónak be kell szereznie a lista frissített példányát, hogy felhasználhassa annak tartalmát.
    
    -   A **Visszavonási lista nyilvános kulcsa** mezőbe írja be a visszavonási lista nyilvános kulcsát tartalmazó fájl elérési útját és nevét. A fájlról az „Aláírás beszúrása a visszavonási listába” című pont tartalmaz további tájékoztatást.

    > [!CAUTION]  
    > A visszavonás megvalósításakor a kellő körültekintéssel kell eljárnia. A megadott frissítési időközönként rendszeresen meg kell újítania a visszavonási listát, ellenkező esetben ugyanis automatikusan érvényét veszti, ami megakadályozza, hogy a felhasználók igénybe vegyék azt a tartalmat, amelyhez szükség van az adott listára. Ennek elkerülése érdekében gondosan mérlegelje, hogy milyen időközt állít be a visszavonási lista frissítésére vonatkozóan. A további tudnivalókat lásd: „[A visszavonás kezelése](https://technet.microsoft.com/df732a7d-1fb0-4845-87ca-fab4bc5f98a0)”.

9.  Kattintson a **Küldés** gombra.

Az eljárás végrehajtását „[A jogmegadási sablonok létrehozása és módosítása](https://technet.microsoft.com/6014176f-ef71-4d29-b3e3-da129c18563d)” pont ismerteti.