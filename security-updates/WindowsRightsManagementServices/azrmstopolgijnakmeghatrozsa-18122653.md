---
TOCTitle: Az RMS topológiájának meghatározása
Title: Az RMS topológiájának meghatározása
ms:assetid: 'bf516f7d-b3a1-4e7f-971f-bfab1db41812'
ms:contentKeyID: 18122653
ms:mtpsurl: 'https://technet.microsoft.com/hu-hu/library/Cc747651(v=WS.10)'
---

Az RMS topológiájának meghatározása
===================================

Az RMS alapszintű topológiájánál az egyes Active Directory-erdőkben az RMS legfelső szintű tanúsítási kiszolgálója vagy fürtje az RMS valamennyi szolgáltatását biztosítja a szervezet számára. Ez az RMS-topológia nagy és kis méretű szervezeteknél egyaránt jól működik. Az RMS elosztott topológiájánál egy vagy több licenckiszolgáló (más néven részlegszintű licenckiszolgáló) a licencelési szolgáltatások egy részét vagy egészét biztosítja az adott szervezeti egység adott felhasználói és csoportjai számára. Bár továbbra is a legfelső szintű tanúsítási kiszolgáló (vagy fürt) biztosítja a fióktanúsítási és az aktiválási proxy szolgáltatást a szervezet egészének, az elosztott RMS-topológia olyan szervezeteknél hasznos, ahol nagyon eltérő licencelési szükségletek jelentkeznek, és amelyek a szervezeti egységekre lebontva szeretnék szabályozni az RMS használatát.

Annak ellenére, hogy az RMS csak két alapvető topológiában használható, a topológiák nagyon eltérő összetevőkből épülhetnek fel. A szervezetnél szükséges összetevők definiálásához és az RMS megfelelő topológiájának kialakításához a következő lépéseket kell végrehajtani:

-   Mérje fel a szervezet szükségleteit és céljait.
-   Állapítsa meg, mire kell használni a tartalomvédelmet.
-   A forgalomban és a terhelésben várható szabályszerűségek elemzése alapján döntsön a szolgáltatás megfelelő szintjéről.

A topológia meghatározása és a terv kivitelezéséhez szükséges döntések meghozatala iteratív eljárás részét képezik, amely az RMS bevezetésének teljes tervezési folyamatára jellemző.

A témakör tartalma:

-   [Az alapvető összetevők azonosítása](https://technet.microsoft.com/c9ec225b-0e51-42f5-aff6-0aecb62e3b27)
-   [A topológiai célok megállapítása](https://technet.microsoft.com/8275a04d-3e5b-40b0-be9d-2f31b7aeca6b)
-   [Az RMS rendszer hatókörének meghatározása](https://technet.microsoft.com/4b5fe1be-643e-47c4-bf9b-50d1e97108fb)
-   [A skálázási követelmények felmérése](https://technet.microsoft.com/89f0138c-946d-47d7-a286-041d4d9606a8)
-   [Redundancia és terheléselosztás biztosítása](https://technet.microsoft.com/162d547c-78a7-4848-b43e-58e481832af2)
-   [Az áttelepítési követelmények felmérése](https://technet.microsoft.com/cec07f45-dc52-4004-860b-5cc33e5fc209)
-   [Az adatbázis-kiszolgáló infrastruktúrájának tervezése](https://technet.microsoft.com/b12354bd-3143-4d1f-b5aa-450c4550653c)
-   [Több erdőt átfogó bevezetés tervezése](https://technet.microsoft.com/2dfb40b7-95b1-4362-b32e-72867544b705)
-   [Külső RMS-felhasználók tervezése](https://technet.microsoft.com/107e1338-4dcf-4ed5-a49d-e875cc883db1)
-   [Alapszintű RMS-topológia tervezése](https://technet.microsoft.com/fec3201e-201f-4faf-910e-fa44132af83d)
-   [Elosztott RMS-topológia tervezése](https://technet.microsoft.com/8773a1e0-6ac3-41f5-9866-5890cef08d04)
