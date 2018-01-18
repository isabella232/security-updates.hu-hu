---
TOCTitle: Az SMS vagy a Csoportházirend beállítása az ügyfelek központi telepítésére
Title: Az SMS vagy a Csoportházirend beállítása az ügyfelek központi telepítésére
ms:assetid: '9e37c27b-8cc1-40c6-adb7-0937aa64c8db'
ms:contentKeyID: 18122695
ms:mtpsurl: 'https://technet.microsoft.com/hu-hu/library/Cc747703(v=WS.10)'
---

Az SMS vagy a Csoportházirend beállítása az ügyfelek központi telepítésére
==========================================================================

Az RMS bevezetésekor a felhasználók számítógépére telepíteni kell egy RMS-kompatibilis alkalmazást, amelynek segítségével RMS-védelemmel ellátott tartalmat hozhatnak létre, illetve használhatnak.

Egy alkalmazás akkor RMS-kompatibilis, ha működésébe be van építve az RM-ügyfél. A Windows Vista® előtt az RMS ügyfélszoftver a Microsoft letöltési központjából külön letölthető Windows-összetevő. Ha nem szeretné minden ügyfélszámítógépre egyenként letölteni az ügyfélszoftvert, a Microsoft Systems Management Server (SMS), a Csoportházirend vagy parancsfájlok segítségével automatikusan telepítheti az ügyfélszámítógépekre az RMS ügyfélszoftverét.

> [!IMPORTANT]
> Az RMS ügyfélszoftver a Windows Vista operációs rendszerbe be lett építve. Ezért nincs szükség külön telepítésre.

Ha az SMS segítségével terjeszti az RMS ügyfélszoftverét, a következő lépéseket hajtsa végre:

-   Hozzon létre egy új csomagdefiníciós fájlt.
-   Bontsa ki a Windows Installer működéséhez szükséges fájlokat a WindowsRightsManagementServicesSP2-KB917275-Client-ENU.exe fájlból. Ehhez először mentse a WindowsRightsManagementServicesSP2-KB917275-Client-ENU.exe fájlt. Ne telepítse a fájlt. Példaként a fájl tárolási helye legyen a c:\\mappa\_neve. Nyissa meg a parancssori ablakot, és írja be a következő parancsot:
    `c:\folder_name\WindowsRightsManagementServicesSP2-KB917275-Client-ENU.exe /x/t:c:\folder_name`
    Ez a parancs kibontja az MSDrmClient.msi és az RMClientBackCompat.msi fájlt az .exe fájlból, és ezeket a *c:\\mappa\_neve* mappába helyezi.
-   Használja a Windows Installer fájljait a csomagdefiníció alapjaként és forrásként.
-   Hirdesse meg a hálózaton a csomagok elérhetőségét.

> [!NOTE]
> A szoftver telepítéséhez rendszergazdai jogok szükségesek. Előfordulhat, hogy a szervezet biztonsági szabályzatának előírásai miatt rendszergazdának kell telepítenie az RMS ügyfélszoftvert.

Az SMS használatával történő szoftverterjesztésről lásd a Systems Management Server 2003 Concepts, Planning, and Deployment Guide című kézikönyvet ([http://go.microsoft.com/](http://go.microsoft.com/fwlink/?linkid=17401)).(http://go.microsoft.com/fwlink/?LinkID=17401)

Ügyfélszoftvernek a Csoportházirend használatával történő telepítéséről a Csoportházirend alapú szoftverterjesztés témaköreiben talál további tudnivalókat ([(http://go.microsoft.com/fwlink/?LinkID=17401)](http://go.microsoft.com/fwlink/?linkid=38997)).
