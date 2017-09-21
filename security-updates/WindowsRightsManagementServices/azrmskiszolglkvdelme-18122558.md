---
TOCTitle: Az RMS kiszolgálók védelme
Title: Az RMS kiszolgálók védelme
ms:assetid: '7e6c4d3a-6cfb-4e96-9dda-ead83f961a6e'
ms:contentKeyID: 18122558
ms:mtpsurl: 'https://technet.microsoft.com/hu-hu/library/Cc747574(v=WS.10)'
---

Az RMS kiszolgálók védelme
==========================

Az RMS-kiszolgálókon található felhasználói fiókok és biztonsági beállítások kezelésekor vegye figyelembe a következő ajánlásokat:

-   Az RMS felügyeletéhez használt webhely virtuális könyvtárai a helyi rendszergazdák hozzáférését korlátozó tulajdonosi hozzáférés-vezérlési listával (DACL) rendelkeznek. A helyi rendszergazdák tagok felvételével és eltávolításával, valamint a felügyeleti weblapokon található hozzáférés-szabályozási bejegyzések (ACE) beállításával új biztonsági csoportokat hozhatnak létre a hozzáférés még körültekintőbb vezérléséhez.
-   A nagyobb biztonság érdekében változtassa meg a Biztonsági beállítások weblap (SecurityPolicy.aspx) DACL-beállításait. A létesítés lehetővé tételéhez az alapértelmezés szerinti ACE teljes ellenőrzést engedélyez az RMS létesítésének végrehajtásához használt fiók számára. A létesítés befejezése után célszerű valamilyen egyéni vagy korlátozott biztonsági csoportra módosítani az ACE beállítását.
-   Az egyes RMS-kiszolgálók engedélyei és jogosultságai mellett külön figyelmet kell fordítani a létfontosságú szerepet betöltő konfigurációs adatbázis védelmi követelményeire. A további tudnivalókat lásd: „[A konfigurációs adatbázis védelme](https://technet.microsoft.com/e023b96f-81d0-45fb-8cc5-becaf6d47ae1)”.

Ha további tájékoztatást szeretne kapni a Microsoft SQL Server™ biztonságos használatával kapcsolatban, nézze át az **SQL Server Security** (Az SQL Server biztonsága) weblapot a [Microsoft webhelyén](http://www.microsoft.com/) (http://www.microsoft.com/).

A Microsoft Windows Server 2003 termékcsalád operációs rendszereivel működő számítógépek biztonságos használatáról a „Windows Server 2003 Security Guide” (Windows Server 2003 biztonsági útmutató) című kiadványból tájékozódhat, amely a [Microsoft webhelyén](http://www.microsoft.com/) (http://www.microsoft.com/) található letöltőközpontból tölthető le.
