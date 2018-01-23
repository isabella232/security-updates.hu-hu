---
TOCTitle: Jogmegadási sablon hozzáadása
Title: Jogmegadási sablon hozzáadása
ms:assetid: '1a5555cd-6d39-4078-a879-4106864674be'
ms:contentKeyID: 18122447
ms:mtpsurl: 'https://technet.microsoft.com/hu-hu/library/Cc720206(v=WS.10)'
---

Jogmegadási sablon hozzáadása
=============================

A művelet végrehajtásához helyben kell bejelentkeznie a felügyeleti webhelyre olyan tartományi felhasználói fiókkal, amely a Rendszergazdák csoport tagja az elérni kívánt számítógépen. A Tartománygazdák csoport tagjai is végrehajthatják ezt a műveletet. Biztonsági szempontból ajánlott a műveletet a **Futtatás másként** parancs segítségével végrehajtani.

A **Globális felügyelet** lap megnyitásához kattintson a **Start** gombra, és válassza a **Minden program**, a **Windows RMS**, majd a **Windows RMS felügyeleti webhely** parancsot.

Jogmegadási sablon hozzáadása
-----------------------------

#### Jogmegadási sablon hozzáadása

1.  Nyissa meg a **Globális felügyelet** lapot, majd keresse meg azt a webhelyet, amelyhez jogmegadási sablonokat szeretne hozzáadni, és kattintson a mellette látható **A webhelyen működő RMS felügyelete** hivatkozásra.

2.  A **Felügyeleti hivatkozások** csoportban kattintson a **Jogmegadási sablonok** hivatkozásra.

3.  A **Nyelv** listán jelölje ki, hogy milyen nyelvű sablont kíván használni.

4.  Kattintson a **Jogmegadási sablon hozzáadása** elemre.

5.  A **Sablon azonosítása** csoportban adja meg a sablon nevét, leírását és jogkérési URL-címét.

6.  A **Felhasználók és csoportok** csoport **Felhasználók és csoportok hozzáadása** mezőjébe írja be a hozzáadni kívánt felhasználó vagy csoport érvényes e-mail címét, és kattintson a **Hozzáadás** gombra. Ismételje meg a műveletet minden hozzáadni kívánt felhasználó vagy csoport esetében.

7.  A **Jelenlegi felhasználók és csoportok** listában jelölje ki annak a felhasználónak vagy csoportnak az e-mail címét, amelynek jogokat szeretne megadni.

8.  Jelölje be a kiválasztott felhasználónak vagy csoportnak megadni kívánt jogokhoz tartozó négyzeteket. Adja meg a megfelelő jogokat a többi felhasználónak és csoportnak is.

9.  A **Lejárati szabályzat** csoportban válasszon a három lejárati beállítás közül, majd adja meg a lejárat dátumát vagy időpontját. Ha szükséges, jelölje be **A tartalom használati licenceit** kezdetű beállítást, és adja meg, hány naponként kell megújítani a licenceket.

10. A **Kiterjesztett szabályzat** csoportban található négy beállítás közül adja meg a szükségeseket. Ha az **Alkalmazásspecifikus adatok betartatása** beállítást választotta, adja meg a betartatni kívánt adatok nevét és értékét, majd kattintson a **Hozzáadás** gombra.

11. Ha engedélyezni kívánja a visszavonást, a **Visszavonási szabályzat** csoportban jelölje be a **Visszavonás megkövetelése** négyzetet, majd hajtsa végre a következő műveleteket:

    1.  Az **URL vagy UNC** mezőbe írja be azt az URL-címet, ahol a visszavonási listát tartalmazó fájl közzé van téve. Ha a nem csatlakozó és a külső felhasználókkal is foglalkoznia kell, a megadott URL-címnek elérhetőnek kell lennie a vállalati hálózatból és az internetről egyaránt.

    2.  A **Visszavonási lista frissítési időköze** mezőbe írja be, hogy hány napig marad érvényes a visszavonási lista. Ha valamelyik felhasználónál olyan visszavonási lista található, amely korábbi, mint az itt megadott érték, a felhasználónak be kell szereznie a lista frissített példányát, hogy felhasználhassa annak tartalmát.

    3.  A **Nyilvános kulcs fájlja** mezőbe írja be a visszavonási lista nyilvános kulcsát tartalmazó fájl elérési útját és nevét, vagy a **Tallózás** gombra kattintva keresse meg a megfelelő fájlt. A fájlról a további tudnivalókat lásd a témakör „Aláírás beszúrása a visszavonási listába” című pontjában.

    > [!CAUTION]  
    > A visszavonás megvalósításakor a kellő körültekintéssel kell eljárnia. A megadott frissítési időközönként rendszeresen meg kell újítania a visszavonási listát, ellenkező esetben ugyanis automatikusan érvényét veszti, ami megakadályozza, hogy a felhasználók igénybe vegyék azt a tartalmat, amelyhez szükség van az adott listára. Ennek elkerülése érdekében gondosan mérlegelje, hogy milyen időközt állít be a visszavonási lista frissítésére. A további tudnivalókat lásd „[A visszavonás kezelése](https://technet.microsoft.com/df732a7d-1fb0-4845-87ca-fab4bc5f98a0)” pontban.

12. Kattintson a **Küldés** gombra.

A visszavonásról a további tudnivalókat lásd a témakör „[A visszavonás kezelése](https://technet.microsoft.com/df732a7d-1fb0-4845-87ca-fab4bc5f98a0)” című pontjában.

A visszavonási beállítások megadásával kapcsolatos szempontokat lásd: „[Visszavonási szabályzatok definiálása](https://technet.microsoft.com/e2fffe9f-def7-439b-a8aa-43f8a065813d)”.

Az eljárás végrehajtását „[A jogmegadási sablonok létrehozása és módosítása](https://technet.microsoft.com/6014176f-ef71-4d29-b3e3-da129c18563d)” pont ismerteti.