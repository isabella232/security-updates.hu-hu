---
TOCTitle: Visszavonási szabályzatok definiálása
Title: Visszavonási szabályzatok definiálása
ms:assetid: 'e2fffe9f-def7-439b-a8aa-43f8a065813d'
ms:contentKeyID: 18122770
ms:mtpsurl: 'https://technet.microsoft.com/hu-hu/library/Cc747782(v=WS.10)'
---

Visszavonási szabályzatok definiálása
=====================================

A szervezeti visszavonási szabályzatok definiálása gondos mérlegelést és tervezést igényel, mivel a visszavonás ugyan a védett tartalom nagyobb biztonságát nyújtja, de befolyásolhatja a felhasználók tartalomelérését is. Az RMS bevezetéséhez a visszavonási szabályzatok a felügyeleti webhelyen adhatók meg.

Visszavonás külső féllel
------------------------

Mivel az RMS-telepítés legfelső szintű tanúsítási kiszolgálójának licencelői tanúsítványát a Microsoft igénylési szolgáltatás állította ki, a Microsoft visszavonhatja a kiszolgálói licencelői tanúsítványt. Ezt azonban csak akkor teszi meg a Microsoft, ha erre bírósági végzés kötelezi.

A Microsoft igénylési szolgáltatása mellett külső fél is kijelölhető egy RMS kiszolgáló licencelői tanúsítványának visszavonására. Ez a harmadik fél lehet egy külső entitás, illetve egy nyilvános vagy személyes kulcspár, amelyet a rendszergazda állít elő a szervezet nevében. A megadott külső fél személyes kulcsa aláírhat egy olyan visszavonási listát, amely visszavonja a kiszolgálói licencelői tanúsítványt. A harmadik fél megadása nyilvános kulcsával az RMS létesítése során történik. A kiszolgáló jogmegadási sablonjai úgy is definiálhatók, hogy lehetővé tegyék a külső felek számára az RMS-telepítéssel kiadott tartalom, alkalmazási jegyzékfájlok, licencek és tanúsítványok visszavonását. A további tudnivalókat lásd: „[A jogmegadási sablonok létrehozása és módosítása](https://technet.microsoft.com/6014176f-ef71-4d29-b3e3-da129c18563d)”.

> [!IMPORTANT]  
> Ha a legfelső szintű tanúsítási kiszolgáló licencelői tanúsítványának visszavonásához saját kulcspár előállítása mellett dönt, ügyeljen ennek biztonságos helyen való tárolására. 

A kiszolgálói licencelői tanúsítvány visszavonása fontos döntés, mert ezzel az RMS-telepítéssel kiadott összes tanúsítvány és licenc érvénytelenné válik. A kiszolgálói licencelői tanúsítványok visszavonásáról a további tudnivalókat lásd: „[Kiszolgálói licencelői tanúsítványok visszavonása](https://technet.microsoft.com/8020861d-d196-4431-8282-044675ef5616)”.

A visszavonási listák érvénybe léptetésének megfontolása
--------------------------------------------------------

Ha egy adott védett tartalom esetében szükséges a visszavonás, a jogok megadásakor minden, az ügyfélszámítógépen regisztrált visszavonási listát használ a program, és ha teljesül egy megadott feltétel, foganatosítja is őket. Éppen ezért legyen körültekintő a visszavonás megvalósításakor, mivel ennek eredményeként regisztrált visszavonási listák jöhetnek létre az ügyfélszámítógépeken, és ezek a tervezettnél szélesebb kört érinthetnek. A sablonok konfigurálásáról a további tudnivalókat lásd: „[A jogmegadási sablonok létrehozása és módosítása](https://technet.microsoft.com/6014176f-ef71-4d29-b3e3-da129c18563d)”.

A biztonság és a használhatóság egyensúlya
------------------------------------------

Amikor visszavonási szabályzatot ad meg a jogmegadási sablonokban, mérlegelje a dokumentumok nagyobb biztonságának követelményét és annak lehetőségét, hogy a felhasználók problémákba ütközhetnek a tartalom használatakor.

Ezt mutatja be a következő példa. Egy jogmegadási sablonban a visszavonási lista beállítása részeként frissítési időközt is megad a visszavonási listához. A kérdéses jogmegadási sablon használatával közzétett tartalom eléréséhez a felhasználó számítógépén visszavonási listának kell léteznie, és ez nem lehet régebbi a megadott frissítési időköznél. Ha például a frissítési időköz 10 nap, a visszavonási lista nem lehet tíz napnál régebbi. Ha nincs visszavonási lista az ügyfélszámítógépen, vagy ha ennek létrehozási dátuma a frissítési időköznél régebbi, az RMS-kompatibilis alkalmazás a legfrissebb visszavonási listát tölti le a használati licencben megadott helyről. A hálózatra nem csatlakozó felhasználó azonban nem tudja lekérni az aktuális visszavonási listát, így a tartalmat sem használhatja.

A következő javaslatok segíthetnek a probléma megoldásában:

-   Kellő körültekintéssel adja meg a visszavonási lista frissítési időközét, és biztosítsa, hogy a friss visszavonási lista mindig könnyen hozzáférhető legyen a felhasználók számára.
-   A visszavonási listákat a vállalati hálózaton belülről és kívülről is elérhető URL-címen tárolja.
-   A Microsoft® Systems Management Server (SMS) vagy hasonló szolgáltatással rendszeres időközönként (például minden éjjel) tegye közzé az összes ügyfélszámítógépen a visszavonási listák frissített példányait.
-   A visszavonást csak olyan típusú dokumentumoknál követelje meg, amelyek bizalmas jellege ezt valóban indokolja.
