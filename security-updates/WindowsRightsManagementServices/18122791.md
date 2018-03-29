---
TOCTitle: A jogmegadási sablonok használata
Title: A jogmegadási sablonok használata
ms:assetid: 'ff4f1143-f6b9-4dd8-aa4c-c2cbbf6fdf06'
ms:contentKeyID: 18122791
ms:mtpsurl: 'https://technet.microsoft.com/hu-hu/library/Cc747804(v=WS.10)'
---

A jogmegadási sablonok használata
=================================

Miután létrehozta a jogmegadási sablont, annak a szerzők részére való eljuttatásának szabályozásával meghatározhatja, hogy miként alkalmazzák a sablont a szervezeten belül.

Az RMS a jogmegadási sablonokat a konfigurációs adatbázisban tárolja. Emellett minden jogmegadási sablon másolatát elhelyezi „[A jogmegadási sablonok helyének megadása](https://technet.microsoft.com/e1bee46d-33db-424f-ba45-1dcedcb883ab)” című témakörben ismertetett megosztott mappában is. A sablonok tárolására feltétlenül olyan, hálózatról is elérhető helyet válasszon, amely eleget tesz a szervezet biztonsági előírásainak. A sablonokat tároló megosztott mappákat ne az RMS által használt alapmappákban (ilyen például a Program Files vagy az IISRoot mappa) hozza létre.

Védett tartalom közzétételekor a szerzők az alkalmazni kívánt jogmegadási sablont a helyi számítógépen rendelkezésre állók közül választják. A jogmegadási sablonok hozzáférhetővé tételéhez a rendszergazdának a megosztott mappából telepítenie kell azokat a felhasználói gépekre.

Amikor egy felhasználó védett tartalmat kísérel meg használni, az RMS-kompatibilis alkalmazás a tartalom közzétételéhez használt jogmegadási sablon legfrissebb verzióját szerzi be a konfigurációs adatbázisból. Az RMS-kompatibilis alkalmazás ezután ennek beállításait alkalmazza a tartalomra. Amikor jogmegadási sablont módosít az RMS-kiszolgálón, az RMS megfelelően frissíti a sablont a konfigurációs adatbázisban és a megosztott mappában is (ha az RMS-kiszolgáló úgy van beállítva, hogy helyet kell megadni a jogmegadási sablonok példányainak tárolásához). Módosításuk után a jogmegadási sablonokat telepítse újból az ügyfélrendszereken, hogy a felhasználók számítógépein mindig a legfrissebb verzió álljon rendelkezésre.

Jogmegadási sablon törlésekor a rendszer eltávolítja azt a konfigurációs adatbázisból, valamint a törléskor a sablon tárolási helyeként megadott megosztott mappából is. A felhasználói számítógépeken viszont nem törlődik, ezt manuálisan kell végrehajtani. A törölt jogmegadási sablonokat minden felhasználói számítógépről el kell távolítani. Ha ezt nem hajtja végre, és a törölt jogmegadási sablont tartalom közzétételéhez használják, az RMS nem fog tudni használati licenceket kiállítani a tartalomhoz, mivel a megadott sablon már nem található a konfigurációs adatbázisban.

A jogmegadási sablonokkal való munka során a következő feladatokat kell végrehajtani:

-   **Meg kell adni egy megosztott mappát**. Az első jogmegadási sablon létrehozása előtt meg kell adnia az összes jogmegadási sablon tárolási helyeként szolgáló megosztott mappát. A további tudnivalókat lásd: „[A jogmegadási sablonok helyének megadása](https://technet.microsoft.com/e1bee46d-33db-424f-ba45-1dcedcb883ab)”.
-   **Létre kell hozni és módosítani kell a jogmegadási sablonokat**. A szervezetben a jogok kezeléséhez szükséges tetszőleges számú jogmegadási sablont létrehozhat. Jogmegadási sablon létrehozásakor a felhasználókat és a vonatkozó jogokat adja meg. Emellett azt is definiálja, hogy a jogmegadási sablont hogyan kell alkalmazni a tartalomra. Később, ha erre szükség van, módosíthatja a jogmegadási sablonokat. A további tudnivalókat lásd: „[A jogmegadási sablonok létrehozása és módosítása](https://technet.microsoft.com/6014176f-ef71-4d29-b3e3-da129c18563d)”.
-   **Ki kell osztani a jogmegadási sablonokat**. Ha egy szerző adott jogmegadási sablont szeretne alkalmazni a tartalomhoz, a jogmegadási sablon másolatának léteznie kell a számítógépén. A sablonok kiosztásával szabályozhatja, hogy adott szerzők milyen jogmegadási sablonokat használhatnak. A további tudnivalókat lásd: „[A jogmegadási sablonok kiosztása](https://technet.microsoft.com/ae6fa26f-d744-4ac9-9eb1-728ffab87bfe)”.
-   **Ki kell vonni a használatból a jogmegadási sablonokat**. A szükségtelenné vált jogmegadási sablont törölheti. Ennek végrehajtásakor a sablont a felhasználói számítógépekről is el kell távolítani, hogy a felhasználóknak ne okozzon problémát a kivont jogmegadási sablonnal közzétett tartalom használata. A további tudnivalókat lásd: „[A jogmegadási sablonok kivonása](https://technet.microsoft.com/32bf98c7-edda-4507-a4b8-4c11bddd6e60)”.
