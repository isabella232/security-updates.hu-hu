---
TOCTitle: Az RMS jogmegadási sablonjaival kapcsolatos kérdések
Title: Az RMS jogmegadási sablonjaival kapcsolatos kérdések
ms:assetid: '01515f08-9844-4c1a-9ab5-a5a60a901b50'
ms:contentKeyID: 18122432
ms:mtpsurl: 'https://technet.microsoft.com/hu-hu/library/Cc720175(v=WS.10)'
---

Az RMS jogmegadási sablonjaival kapcsolatos kérdések
====================================================

Az RMS sablonjaival kapcsolatos kérdések
----------------------------------------

-   [Előírható-e egy alapértelmezett sablon a szervezetben létrehozott összes tartalomra, hogy így biztosítható legyen a jogok minimális készlete?](#bkmk_57)

-   [Hol találhatók az RMS szabályzati sablonjai?](#bkmk_58)

-   [A sablonok létrehozásakor felhasználói hivatkozási nevek és terjesztési listák kapcsolódnak ezekhez. A több részleggel rendelkező szervezetek hogyan biztosíthatnak olyan sablonokat, amelyek azonos alapvető jogokat tartalmaznak, de ezeket a tartalomtól függően különböző csoportoknak adják meg?](#bkmk_59)

-   [A dokumentumokhoz alkalmazott jogok rögzítettek? Ha a fájlok elküldése után a jogok módosítására lenne szükség, végrehajtható-e ez, feltéve, hogy a közzétételi licenc be van ágyazva a fájlba, azaz nem az RMS „szabályzati” kiszolgálóján található?](#bkmk_60)

#### Előírható-e egy alapértelmezett sablon a szervezetben létrehozott összes tartalomra, hogy így biztosítható legyen a jogok minimális készlete?

Igen. A Rights Management Services SDK készletének segítségével fejleszthető olyan egyéni alkalmazás, amellyel tetszőleges sablonok betartása megvalósítható. Az Office 2003 és újabb verziók jogkezelési megvalósítása azonban nem támogatja sablonok előírását a tartalomra.

#### Hol találhatók az RMS szabályzati sablonjai?

A sablonok helye az RMS-kompatibilis alkalmazástól függ. Az Office 2003 és újabb verziók esetében ezt a rendszerleíró adatbázis következő felhasználói beállítása adja meg:

**HKEY\_CURRENT\_USER\\Software\\Microsoft\\Office\\11.0\\Common\\DRM\\AdminTemplatePath**

vagy

**HKEY\_CURRENT\_USER\\Software\\Microsoft\\Office\\12.0\\Common\\DRM\\AdminTemplatePath** a Microsoft Office 2007 esetében

> [!NOTE]  
> Ha ez a bejegyzés az ügyfélgép helyi mappájára mutat, a sablonfájlokat az ügyfélgépre kell másolni. Ha hálózati megosztott mappára mutat, a felhasználó kapcsolat nélküli üzemmódjában nem lesz elérhető. 

#### A sablonok létrehozásakor felhasználói hivatkozási nevek és terjesztési listák kapcsolódnak ezekhez. A több részleggel rendelkező szervezetek hogyan biztosíthatnak olyan sablonokat, amelyek azonos alapvető jogokat tartalmaznak, de ezeket a tartalomtól függően különböző csoportoknak adják meg?

Erre a problémára két megoldás lehetséges:

-   Csak egy sablont hozzon létre (például „Vállalati – bizalmas” néven), amely a részleg összes alkalmazottjára érvényes, majd ezt a sablont használva egy e-mail üzenetben címezze azt adott személyeknek. A módszer előnye, hogy egyetlen sablon szükséges minden részlegnél az e-mail üzenethez, és azokra a felhasználókra korlátozható, akiknek elküldi az üzenetet. Hátránya az, hogy a csoporton kívül bárki, aki eredetileg megkapta, továbbra is elolvashatja azt.

-   Másik megoldásként hozzon létre több sablont, minden terjesztési listához egyet. Bár ez pontosabb szabályozást biztosít, de így az informatikai osztálynak több sablonnal kell foglalkoznia.

#### A dokumentumokhoz alkalmazott jogok rögzítettek? Ha a fájlok elküldése után a jogok módosítására lenne szükség, végrehajtható-e ez, feltéve, hogy a közzétételi licenc be van ágyazva a fájlba, azaz nem az RMS „szabályzati” kiszolgálóján található?

Igen, jogmegadási sablon használatakor ez lehetséges: Amikor jogmegadási sablon segítségével teszik közzé a tartalmat, a szabályzat definíciója a kiszolgálón marad, így azt a rendszergazda megváltoztathatja a tartalom közzététele után. Amikor egy felhasználó licencet kér a tartalomhoz, a licenc a kiszolgálón lévő aktuális szabályzatnak megfelelő jogokat adja meg. Ha a jogok megváltoznak a felhasználó használati licencének kiállítása után, a felhasználó a használati licenc kiállításakor érvényes jogokkal fog továbbra is rendelkezni. A tartalom közzététele után úgy tud másik jogmegadási sablont alkalmazni, hogy lejárati szabályzatot engedélyez a sablonra, és megadja a következő beállítást: **A tartalom használati licenceit n naponta meg kell újítani**. Az n helyére írja be, hogy hány nap eltelte után kell a felhasználónak új használati licencet kérelmeznie.
