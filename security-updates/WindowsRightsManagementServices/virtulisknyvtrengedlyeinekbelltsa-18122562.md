---
TOCTitle: Virtuális könyvtár engedélyeinek beállítása
Title: Virtuális könyvtár engedélyeinek beállítása
ms:assetid: '45112111-9608-45b1-9a86-7b313d0a1579'
ms:contentKeyID: 18122562
ms:mtpsurl: 'https://technet.microsoft.com/hu-hu/library/Cc747549(v=WS.10)'
---

Virtuális könyvtár engedélyeinek beállítása
===========================================

Engedélyezése után a leszerelés szolgáltatásként érhető el. A leszerelési szolgáltatás azonban az IIS virtuális könyvtára, amelyhez hozzáférési engedélyek kapcsolódnak. A szolgáltatás használatához engedélyeket kell beállítani a virtuális könyvtáron és az adott fájlban (decommission.asmx) a felhasználók számára.

Alapértelmezés szerint a beépített Windows hitelesítés engedélyezve van a virtuális könyvtárhoz, de az adott fájlhoz csak a rendszer- és a rendszergazdai fiókok férhetnek hozzá. Amikor megadja az engedélyeket a decommission.asmx fájl tulajdonosi hozzáférés-szabályozási listájában, megbízható felhasználók adott csoportjának engedélyezheti a hozzáférést a tényleges RMS-védelem eltávolításához, illetve mindenki számára hozzáférhetővé teheti a szolgáltatást.

Mielőtt a felhasználók megkezdhetnék a leszerelési szolgáltatás használatát, a felhasználói alkalmazást úgy kell módosítani, hogy a használati licencek iránti kérelmek elküldhetők legyenek ebbe az új leszerelési adatcsatornába. Microsoft Office System 2003 rendszeren ez rendszerleíró bejegyzés felvételével hajtható végre a felhasználó számítógépén. Az Office 2003 használatakor az eljárás a következő:

1.  Nyissa meg a rendszerleíró adatbázis szerkesztőjét.
2.  Keresse meg a `HKEY_CURRENT_USER\Software\Microsoft\Office\11.0\Common\DRM` bejegyzést, és vegyen fel egy új, `Decommissioning` nevű kulcsot.
3.  A Decommissioning kulcsban vegye fel a következő új, **Karakterlánc** típusú bejegyzést, a *licenckiszolgáló* helyére írja az RMS kiszolgáló nevét.
    `http://`*licenckiszolgáló*`/_wmcs/licensing`
4.  Ezután kattintson a jobb oldali egérgombbal a bejegyzésre, válassza a **Módosítás** parancsot, és adja meg a leszerelési szolgáltatásra mutató értéket:
    `http://`*licenckiszolgáló*`/_wmcs/decommission`

> [!NOTE]  
> Ennél a kulcsnál több bejegyzés is szerepelhet, ha a szervezeten belül több RMS kiszolgáló van leszerelési üzemmódban. 
