---
TOCTitle: A normál működés biztonsági vonatkozásai
Title: A normál működés biztonsági vonatkozásai
ms:assetid: '98f3d584-6320-4aa1-9959-7133cfdb6df7'
ms:contentKeyID: 18122602
ms:mtpsurl: 'https://technet.microsoft.com/hu-hu/library/Cc747609(v=WS.10)'
---

A normál működés biztonsági vonatkozásai
========================================

Az RMS telepítése és létesítése után az RMS webszolgáltatásai IIS-alkalmazásokként működnek, és így különböző rendszererőforrásokat érnek el, amelyek megkövetelik a hitelesítést és az engedélyezést. A hitelesítést mindegyik rendszererőforrás megköveteli, és nem is lehet mást beállítani. Az oldal hátralévő része az RMS engedélyezési szerkezetét mutatja be.

Az RMS webszolgáltatásai egy IIS-alkalmazáskészlet környezetében futnak. Az IIS mindegyik alkalmazáskészlete egy egyedi identitás, amely megfelelhet egy tartományi felhasználói fióknak, egy helyi felhasználói fióknak, a helyi Hálózati szolgáltatásfióknak, illetve a Helyi rendszerfióknak. Ezek a fiókok mind különböző engedélyekkel rendelkeznek a rendszeren belül. Az RMS létesítésekor választani lehet, hogy az RMS webszolgáltatásai a helyi rendszerfiókkal vagy egy tartományi felhasználói fiókkal fussanak-e. Ezt követően ez a fiók lesz az RMS alkalmazáskészletének az identitása. A Globális felügyeleti webhely alkalmazáskészlete a „DRMS Application Pool” nevet viseli. A létesített webhely alkalmazáskészletének „\_DRMSAppPool1” a neve. Az RMS naplózási szolgáltatása külön Windows-szolgáltatásként fut az RMS alkalmazáskészlete identitásaként megadott felhasználói fiókkal.

Az RMS webszolgáltatásai többféle erőforrást érnek el, így a rendszeren található fájlokat és mappákat, adatbázisokat és tárolt eljárásokat az adatbázis-kiszolgálón, a helyi rendszerleíró adatbázist, az Active Directoryt, a programkód gyorsítótárát, a memóriát és a rendszeren futó más folyamatokat. Az RMS naplózási szolgáltatásának a helyi rendszer naplózási várólistáját is el kell érnie. Ezeknek az erőforrásoknak mindnek saját tulajdonosi hozzáférés-szabályozási listája (DACL) van, amely meghatározza, hogy ki jogosult hozzáférni az erőforráshoz, és hogy mit csinálhat vele.

Az engedélyek kiosztásának és a szolgáltatásfiókok kezelésének megkönnyítése érdekében az RMS által a létesítés során létrehozott RMS szolgáltatás csoport minden szükséges engedélyt megkap. Mivel az RMS szolgáltatásfiókja tagja ennek a csoportnak, így minden olyan engedélyt megkap, amellyel ez a csoport rendelkezik.

Az alábbi lista összefoglalja az RMS szolgáltatás csoport számára megadott engedélyeket:

-   Olvasási engedély a virtuális gyökérkönyvtárakhoz
-   Írási engedély a programkód gyorsítótárának könyvtárához
-   Írási engedély a rendszer ideiglenes könyvtárához
-   Írási engedély a naplózási várólistához
-   Olvasási engedély az Active Directoryhoz

Ha adatbázis-kiszolgálóként a Microsoft SQL Server 2000 rendszert használja, ügyeljen arra, hogy ez némileg eltérően osztja ki az engedélyeket, mint a Windows Server 2003. Az RMS létesítése bejelentkezési adatokat hoz létre az RMS szolgáltatásfiókja számára az SQL Server kiszolgálón. Ha úgy döntött, hogy a helyi rendszerfiókkal létesíti az RMS szolgáltatást, az SQL Server bejelentkezési neve a *TARTOMÁNY\\számítógép\_neve* formátumban jön létre, ahol *TARTOMÁNY* azt az Active Directory-tartományt jelöli, amelynek a számítógép tagja, míg a *számítógép\_neve* a kiszolgáló neve. Létrejön egy rms\_service nevű SQL szerepkör is, amely minden szükséges engedélyt megkap. Az RMS szolgáltatásfiókjának bejelentkezési neve bekerül ebbe a csoportba. Maga az RMS szolgáltatásfiókja semmilyen engedélyt sem kap.

Az SQL Server emellett minden adatbázishoz hozzárendel egy adatbázis-tulajdonost (DBO). Az adatbázis-tulajdonos hozzárendelésére a létesítés során kerül sor az alábbiak szerint:

-   A konfigurációs adatbázis tulajdonosi jogát az RMS létesítésekor használt tartományi fiók kapja meg.
-   A címtár-szolgáltatási és a naplózási adatbázis tulajdonosi jogát az RMS szolgáltatásfiókja kapja meg.

Az RMS tervezése során a biztonsági szempontokra való figyelemmel, gondosan választottuk meg, hogy az RMS milyen engedélyeket hozzon létre a különböző erőforrásokhoz. Elméletileg nem létezhet olyan ok, amely miatt módosítani kellene azokat az engedélyeket, amelyeket a létesítési folyamat az erőforrásokhoz kiosztott. Ha a létesítést követően módosítani kell a szolgáltatásfiókként használt felhasználói fiókot vagy annak jelszavát, ez az RMS Globális felügyelet weblapján végrehajtható. A további tudnivalókat lásd a dokumentumgyűjtemény „RMS kiszolgáló működtetése” részében „Az RMS szolgáltatásfiók megváltoztatása” témakörben.
