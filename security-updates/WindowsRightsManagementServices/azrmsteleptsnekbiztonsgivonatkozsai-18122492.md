---
TOCTitle: Az RMS telepítésének biztonsági vonatkozásai
Title: Az RMS telepítésének biztonsági vonatkozásai
ms:assetid: '0a3d40b2-f27e-4e63-baff-a9c8433f5f91'
ms:contentKeyID: 18122492
ms:mtpsurl: 'https://technet.microsoft.com/hu-hu/library/Cc720192(v=WS.10)'
---

Az RMS telepítésének biztonsági vonatkozásai
============================================

Az RMS telepítője a bejelentkezett felhasználó hitelesítő adatait használja az RMS fájljainak telepítéséhez és konfigurálásához. Ezért a telepítési eljárást végrehajtó rendszergazdának olyan felhasználói fiókkal kell bejelentkeznie, amely tagja a helyi Rendszergazdák csoportnak. Az egyszámítógépes telepítések kivételével ennek a fióknak minden esetben egyúttal tartományi felhasználói fióknak kell lennie.

A telepítési folyamat során elindul a Windows Installer (Msiexec.exe) szolgáltatás. Ez a szolgáltatás örökli a szülő felhasználói tokenjét. Később, ha egyéni utófeldolgozási műveletek léteznek, az Msiexec.exe szolgáltatás a bejelentkezett felhasználó identitását használja. Ez attól függetlenül így történik, hogy a telepítést böngészőből vagy parancssorból indították el.

Az RMS telepítője a következő műveleteket hajtja végre:

-   A fájlok másolása a C:\\Program Files\\RMS mappába. Ez a mappa általában a Rendszergazdák és a Kiemelt felhasználók számára is hozzáférhető. A lemezegység és a fájlok helye beállítható a telepítés során.
-   A létesítési, azaz az RMS felügyeleti webhelyének létrehozása az alapértelmezés szerinti 5720-as számú porton. Ez a webhely a telepített fájlokra mutat.
-   A WMCSProvisioningAppPool alkalmazáskészlet létrehozása és társítása az RMS felügyeleti webhelyével. Az alkalmazáskészlet szolgáltatásfiókként a Hálózatszolgáltatások szolgáltatásfiókját használja.
-   A teljesítményszámlálók telepítése.
-   Olvasási és írási engedélyt ad az RMS szolgáltatás csoportnak a következő rendszerleíró kulcshoz.
    A Windows Server 2003 rendszer 32 bites verziójával működő számítógépeken:
    `HKEY_LOCAL_MACHINE\Software\Microsoft\DRMS\1.0`
    A Windows Server 2003 rendszer 64 bites verziójával működő számítógépeken:
    `HKEY_LOCAL_MACHINE\Software\WOW6432Node\Microsoft\DRMS\1.0`
