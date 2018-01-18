---
TOCTitle: A jogmegadási sablonok létrehozása és módosítása
Title: A jogmegadási sablonok létrehozása és módosítása
ms:assetid: '6014176f-ef71-4d29-b3e3-da129c18563d'
ms:contentKeyID: 18122507
ms:mtpsurl: 'https://technet.microsoft.com/hu-hu/library/Cc720281(v=WS.10)'
---

A jogmegadási sablonok létrehozása és módosítása
================================================

Jogmegadási sablonok létrehozásakor vagy szerkesztésekor a következő elemeket adhatja meg:

-   **A jogmegadási sablon neve és leírása**. Emellett megadhat egy e-mail címet is, amelyen a felhasználók a sablonban biztosítottnál több jogot kérhetnek.
-   **Felhasználók és csoportok, akik és amelyek tagjai használati licencet szerezhetnek az ezzel a jogmegadási sablonnal közzétett tartalomhoz.** Annak megadásához, hogy tetszőleges felhasználó használati licencet szerezhessen a védett tartalomhoz, használja a **Bárki** csoportot, amely az RMS különleges csoportja. Úgy veheti fel ezt a speciális csoportot a sablonba, hogy a **Jogmegadási sablonok beállításai** lap **Felhasználók és csoportok hozzáadása** mezőjébe beírja a **Bárki** szót, majd rákattint a **Hozzáadás** gombra.
-   **Mindegyik felhasználónak vagy csoportnak megadott jogok.** A jogok közötti függőségi kapcsolatok miatt néhány jog automatikusan kijelölődik. Ha például kijelöli a **Szerkesztés** jogot, a **Megtekintés** és a **Mentés** jog is kijelölődik. A felsorolt és az XrML szókészletben megadott jogok közötti megfeleltetésről az „[RMS – a jogok és az XrML](https://technet.microsoft.com/7eb5cdd1-cd48-4b2b-96b6-fc74f7b42e7f)” című pontban olvashat.
-   **Lejárati szabályzat az adott jogmegadási sablonnal közzétett tartalomnál.** Alapértelmezés szerint a tartalom sohasem jár le. Ez azt jelenti, hogy a felhasználók bármikor szerezhetnek használati licencet. A lejárati szabályzat alábbi beállításai közül választhat:
    -   **Soha nem jár le a tartalom**. Ez az alapértelmezett beállítás. Ha ez a beállítás van kiválasztva, a felhasználó mindaddig hozzáférhet a tartalomhoz, amíg az megtalálható a számítógépen.
    -   **A tartalom lejárata**. Itt megadhatja a tartalom lejárati dátumát, ami azt jelenti, hogy a megadott használati licenc ezen a napon lejár, és ez után egyetlen felhasználó sem szerezhet használati licencet a tartalomhoz.
    -   **A tartalomhasználati licenc lejárata** *n* **nappal a közzététel után**. Itt megadhatja, hogy a közzétételt követően hány nap eltelte után nem szerezhető használati licenc a tartalomhoz.
    -   **A tartalom használati licenceit meg kell újítani** *n* **naponta**. Itt megadhatja, hogy a felhasználóknak milyen időközönként kell megújítaniuk használati licencüket a tartalomhoz. Ezt a szabályzatot az előzőekkel összhangban alkalmazhatja.
-   **Kiterjesztett szabályzat**. Az alábbi szabályzatok közül jelölhet be egyet vagy többet:
    -   **A szerző teljes körű, örökre szóló jogokat kap**. Ez a szabályzat örökös, nem korlátozott jogokat ad a szerzőnek. Ez a beállítás akkor is érvényes, ha a tartalom adott időpontban való lejáratát adta meg.
    -   **Az RMS-védelemmel ellátott tartalom megtekinthető megbízható böngészőkben**. Ez a szabályzat azt adja meg, hogy a tartalom megtekinthető-e megbízható böngészőkben, ha a tartalmat létrehozó RMS-kompatibilis alkalmazás szintén engedélyezi ezt. Ha nem jelöli be ezt a négyzetet, akkor a védett tartalmat a létrehozó alkalmazásban kell megtekinteni.
    -   **Új használati licenc szükséges a tartalom minden használata alkalmával**. Ez a szabályzat azt adja meg, hogy a felhasználóknak új használati licencet kell-e beszerezniük az ezzel a jogmegadási sablonnal közzétett tartalom minden használata alkalmával. Ha ez a szabályzat van kiválasztva, a felhasználó csak akkor érheti el a tartalmat, ha kapcsolódni tud az RMS kiszolgálóhoz.

    > [!CAUTION]  
    > Körültekintően járjon el, ha engedélyezi a **Új használati licenc szükséges a tartalom minden használata alkalmával** szabályzatot. Ez megköveteli, hogy a felhasználók minden alkalommal kapcsolódjanak a hálózathoz, amikor az ezzel a jogmegadási sablonnal közzétett tartalmat szeretnék elérni. Ha nem kapcsolódnak a hálózathoz, nem használhatják a tartalmat. Ha nem adja meg ezt a beállítást, a felhasználóknak csak egyszer, a tartalom első alkalommal való használatakor kell használati licencet beszerezniük. A felhasználók a licenc lejáratáig kapcsolat nélkül is újból használhatják azt. 

-   **Alkalmazásspecifikus adatok betartatása**. Ez a szabályzat az RMS-kompatibilis alkalmazásokra jellemző feltételek alapján testreszabott szabályzat kialakítását teszi lehetővé. A négyzet bejelölésekor írja be az alkalmazáshoz szükséges név-érték párt, majd a listára való felvételhez kattintson a **Hozzáadás** gombra.
-   **Visszavonási szabályzat a jogmegadási sablonhoz**. A **Visszavonás megkövetelése** jelölőnégyzet bejelölésével adhatja meg, hogy kötelező-e visszavonási listát használni. Ha megköveteli a visszavonást, visszavonási listát kell létrehoznia és fenntartania. A visszavonásról a további tudnivalókat lásd a témakör „[A visszavonás kezelése](https://technet.microsoft.com/df732a7d-1fb0-4845-87ca-fab4bc5f98a0)” című pontjában.
-   **Ügyfélhozzáférés-visszavonási lista**. Ez a tulajdonság a visszavonási lista URL-címét adja meg. A visszavonási listát URL-címmel elérhető webszolgáltatással teheti hozzáférhetővé. Amikor egy ügyfélszámítógép visszavonási listát megkövetelő, tartalomvédett tartalmat kísérel megnyitni, az RMS-kompatibilis alkalmazás először a helyi számítógépen keresi a visszavonási listát, és ha nem találja, a sablontulajdonságokban megadott URL-címet használja annak eléréséhez. Miután az RMS ügyfélszoftver a visszavonási URL-címre csatlakozott, ellenőrzi, hogy az OBJECT TYPE, az ID TYPE és az ID értéke a visszavonási lista ISSUER elemében megegyezik-e az RMS használati licencében lévővel. Az RMS ügyfélszoftver ezen kívül a visszavonási lista aláírásához használt nyilvános és személyes kulcsot is egyezteti. Ha valamelyik érték nem egyezik, nem veszi figyelembe a visszavonási listát.
-   **Visszavonási lista frissítési időköze**. Ez a tulajdonság a visszavonási lista érvényességi idejét adja meg. Ha az ügyfélszámítógépen lévő visszavonási lista régebbi a megadott időtartamnál, új lista letöltésére kerül sor.
-   **Nyilvános kulcs fájlja**. Ez a tulajdonság a visszavonási lista aláírásánál használt személyes kulcshoz tartozó nyilvános kulcsot tartalmazó fájl elérési útvonalát és nevét adja meg.
