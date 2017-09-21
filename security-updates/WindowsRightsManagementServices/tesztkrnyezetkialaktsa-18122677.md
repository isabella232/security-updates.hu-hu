---
TOCTitle: Tesztkörnyezet kialakítása
Title: Tesztkörnyezet kialakítása
ms:assetid: 'cdd96b05-49e2-4b6f-bfae-40b5c028ec66'
ms:contentKeyID: 18122677
ms:mtpsurl: 'https://technet.microsoft.com/hu-hu/library/Cc747673(v=WS.10)'
---

Tesztkörnyezet kialakítása
==========================

Az RMS együttműködik az Active Directory meglévő infrastruktúrájával és az adatbázis-kiszolgálókkal, például a Microsoft SQL Server™ 2000 rendszert futtatókkal. A kiegészítő összetevők kritikus természete miatt elszigetelt tesztkörnyezetben alaposan vizsgálni kell az RMS szolgáltatást, mielőtt bevezetnék azt a szervezetben. Ehhez az Active Directory és az adatbázis-kiszolgáló külön telepítése szükséges a tesztkörnyezetben.

Az RMS kiszolgáló legegyszerűbb konfigurációjából kell kiindulni, amikor az erdőben csak egy adatbázis-kiszolgáló és egy ügyfél szerepel. Az RMS alapvető működésének megismerése után a konfiguráció bővíthető, és az egyre jobban megközelítheti a szervezetben éles környezetben bevezetni kívánt topológiát, így szükség szerint további erdők vehetők fel és külső hozzáférés is használható. A tesztkörnyezetben nem kell feltétlenül szerepelni a teljes bevezetési terv minden redundáns elemének és a különböző helyeket egybefogó konfigurációknak, de legalább egyet tartalmaznia kell minden olyan összetevő kiszolgálójából, amelyet majd be kell vezetni.

A következő lista a tesztkörnyezet olyan minimális konfigurációját tartalmazza, amely alkalmas az RMS alapszintű konfigurációjának tesztelésére:

-   Egy tartományvezérlő, amelyen a Windows 2000 Server Service Pack 3 (SP3) vagy újabb csomaggal frissített verziója fut, valamint telepítve van az SQL Server 2000 SP3a csomaggal frissített verziója. Az SQL Server kezeli az RMS naplózási, konfigurációs és címtár-szolgáltatási adatbázisát. Ha az RMS és az adatbázis-kezelő azonos kiszolgálón fut, a szolgáltatás a Microsoft SQL Server 2000 Desktop Engine (MSDE 2000) Release A vagy az SQL Server adatbázis-kezelővel használható. Ha az adatbázis-támogatást egy távoli kiszolgáló biztosítja, az SQL Server adatbázis-kiszolgálóra van szükség. Az MSDE 2000 letölthető a Microsoft webhelyéről.

| ![](images/Cc747673.note(WS.10).gif)Megjegyzés:                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                       |
|----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| A tartományvezérlőn minimális követelmény a Windows 2000 Server Service Pack 3 (SP3) csomaggal frissített verziója, de az Active Directory csoportbehelyettesítésénél a teljesítményjavító szolgáltatások miatt a Windows Server 2003 rendszer javasolt. Az MSDE 2000 csak tesztkörnyezetben használható az RMS adatbázisaihoz, mivel az MSDE 2000 semmilyen hálózati csatlakozófelületet sem támogat. Emellett az MSDE 2000 használati feltételei továbbá megtiltják az SQL Server ügyféleszközeinek használatát az MSDE 2000 adatbázisok kezelésére. E korlátozás miatt nem fogja tudni megtekinteni a naplózott adatokat, és nem tudja módosítani a konfigurációs adatbázisban tárolt adatokat. |

-   Egy legfelső szintű tanúsítási kiszolgáló, amelyen Windows Server 2003 fut. Erre kell telepíteni és itt kell létesíteni az RMS szolgáltatást. A tesztelés során legfelső szintű tanúsítási fürt létrehozásához szükség szerint további kiszolgálók is felvehetők.
-   Egy Windows XP Professional rendszerű ügyfélszámítógép, amelyen telepítve van az RMS ügyfélszoftvere és egy RMS-kompatibilis alkalmazás.
-   Felhasználói fiókok, amelyek az Active Directoryban bejegyzett e-mail címmel rendelkeznek.

Az RMS alapvető infrastrukturális összetevőinek telepítéséről és konfigurálásáról, valamint az infrastrukturális követelmények éles környezetben való alkalmazásáról a tudnivalókat lásd a témakör „[Alapvető infrastruktúra kialakítása](https://technet.microsoft.com/3a0a3a47-e755-4455-bb22-0e05053723e4)" című pontjában.
