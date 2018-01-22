---
TOCTitle: '3. lépés: A hálózati kapcsolat beállítása a WSUS 3.0 szolgáltatásban'
Title: '3. lépés: A hálózati kapcsolat beállítása a WSUS 3.0 szolgáltatásban'
ms:assetid: 'dbc9d9f7-cf52-4539-9f9e-3e823273218a'
ms:contentKeyID: 18129921
ms:mtpsurl: 'https://technet.microsoft.com/hu-hu/library/Cc708602(v=WS.10)'
---

3. lépés: A hálózati kapcsolat beállítása a WSUS 3.0 szolgáltatásban
====================================================================

A WSUS 3.0 telepítése után automatikusan elindul a konfigurálási varázsló. Később is futtathatja, a WSUS 3.0 konzoljának **Beállítások** lapjáról.

Mielőtt hozzálátna a konfiguráláshoz, tudnia kell a választ az alábbi kérdésekre:

1. Úgy van beállítva a kiszolgáló tűzfala, hogy az ügyfelek hozzá tudnak férni a kiszolgálóhoz?

2. Tud a számítógép kapcsolódni a felsőbb rétegbeli kiszolgálóhoz (például a Microsoft Update webhelyhez)?

3. Rendelkezésére áll az esetleges proxykiszolgáló neve és a hozzá szükséges felhasználói hitelesítő adatok?

A szolgáltatás alapértelmezés szerint a Microsoft Update webhelyről tölti le a frissítéseket. Ha viszont proxykiszolgáló is működik a hálózaton, azt is beállíthatja, hogy a WSUS a proxykiszolgálót használja. Ha vállalati tűzfal választja el egymástól a WSUS szolgáltatást és az internetet, módosítani kellhet a tűzfal beállításait ahhoz, hogy a WSUS le tudja tölteni a frissítéseket.

> [!NOTE]  
> Habár a Microsoft Update webhelyről csak működő internetkapcsolattal lehet frissítéseket letölteni, a WSUS szolgáltatással olyan hálózatokra is importálhatók a szükséges frissítések, amelyek nem férnek hozzá az internethez. 

**Az 3. lépésben a következő műveleteket kell végrehajtani**:

-   A tűzfal beállítása
-   Annak meghatározása, hogy a kiszolgáló honnan töltse le a frissítéseket (a Microsoft Update webhelyről vagy egy másik WSUS-kiszolgálóról)
-   A proxykiszolgáló beállításainak módosítása, hogy a WSUS le tudja tölteni a frissítéseket

**A tűzfal beállításainak módosítása**
-   Ha vállalati tűzfal választja el egymástól a WSUS szolgáltatást és az internetet, módosítani kellhet a tűzfal beállításait ahhoz, hogy a WSUS le tudja tölteni a frissítéseket. A frissítések Microsoft Update webhelyről történő letöltéséhez a WSUS-kiszolgáló a 80-as portot (HTTP) és a 443-as portot (HTTPS) használja. E két beállítás megváltoztatására nincs lehetőség.

-   Ha a vállalaton belül csak bizonyos címek használhatják a 80-as és a 443-as portot, akkor az alábbi felsorolásban szereplő tartományokra korlátozhatja a hozzáférést, ezáltal a WSUS és az Automatikus frissítések szolgáltatás kapcsolatot létesíthet a Microsoft Update webhellyel.

    -   http://windowsupdate.microsoft.com
    -   http://\*.windowsupdate.microsoft.com
    -   https://\*.windowsupdate.microsoft.com
    -   http://\*.update.microsoft.com
    -   https://\*.update.microsoft.com
    -   http://\*.windowsupdate.com
    -   http://download.windowsupdate.com
    -   http://download.microsoft.com
    -   http://\*.download.windowsupdate.com
    -   http://wustat.windows.com
    -   http://ntservicepack.microsoft.com

> [!NOTE]  
> A tűzfal beállítását célzó fenti műveletek a WSUS szolgáltatás és az internet közötti vállalati tűzfalra vonatkoznak. A WSUS-kiszolgálón nincs szükség a Windows tűzfal beállításainak módosítására, hiszen saját hálózati adatforgalmát teljes egészében a WSUS szolgáltatás kezdeményezi. 

Habár a Microsoft Update webhely és a WSUS szolgáltatás közötti kapcsolat megteremtéséhez a 80-as és a 443-as portnak nyitva kell lennie, egyéni port megadásával több WSUS-kiszolgáló is használhatja ugyanazt a portot.

A következő két művelet feltételezi, hogy a konfigurációs varázslót használja. E művelet későbbi része bemutatja, hogyan kell elindítani a WSUS felügyeleti beépülő modult és a kiszolgálót konfigurálni a **Beállítások** oldalon.

**Annak meghatározása, hogy a kiszolgáló honnan töltse le a frissítéseket**
1.  A Microsoft Update szolgáltatásainak javítását célzó programhoz való csatlakozást követően válassza a konfigurációs varázsló **Tovább** gombját. Ezután megadhatja a felsőbb rétegbeli kiszolgálót.

2.  Ha azt választja, hogy a Microsoft Update webhelyről szinkronizál, nem kell mást tennie ezen az oldalon. Kattintson a **Tovább** gombra, vagy válassza a **Proxykiszolgáló megadása** elemet a bal oldali panelen.

3.  Ha úgy dönt, hogy másik WSUS-kiszolgálóról kíván szinkronizálni, meg kell adnia a kiszolgáló nevét és azt a portot, amelyen a kiszolgáló kommunikálni fog a felsőbb rétegbeli kiszolgálóval.

4.  Ha használni szeretné az SSL-titkosítást, jelölje be az **SSL használata a frissítési adatok szinkronizálásakor** jelölőnégyzetet. Ez esetben a kiszolgálók a 443-as portot használják a szinkronizálás során. (Ügyeljen arra, hogy mind ez a kiszolgáló, mind felsőbb rétegbeli kiszolgáló támogassa az SSL használatát.)

5.  Ha ez a kiszolgáló a replikakiszolgáló, jelölje be az **Ez a felsőbb rétegbeli kiszolgáló replikája** jelölőnégyzetet.

6.  Ezzel befejeződött a felsőbb rétegbeli kiszolgáló konfigurálása. Kattintson a **Tovább** gombra, vagy válassza a **Proxykiszolgáló megadása** elemet a bal oldali ablaktáblán.

**Proxykiszolgáló beállításainak megadása**
1.  Jelölje be a varázsló **Proxykiszolgáló megadása** oldalán a **Proxykiszolgáló használata szinkronizáláskor** jelölőnégyzetét, és írja be a proxykiszolgáló nevét, illetve portszámát (alapértelmezés szerint 80) a megfelelő mezőkbe.

2.  Ha egyéni hitelesítő adatokkal szeretne kapcsolatot létesíteni a proxykiszolgálóval, jelölje be a **Csatlakozás a proxykiszolgálóhoz felhasználói hitelesítő adatokkal** jelölőnégyzetet, majd írja be a felhasználónevet, a tartományt és a felhasználói jelszót a megfelelő mezőbe. Ha engedélyezni szeretné az alapfokú hitelesítést a proxykiszolgálóval kapcsolatot létesítő felhasználó számára, jelölje be az **Alapfokú hitelesítés engedélyezése (jelszó küldése nem titkosított szövegben)** jelölőnégyzetet.

3.  Ezzel befejeződött a proxykiszolgáló konfigurálása. Kattintson a **Tovább** gombra a következő oldalra történő továbblépéshez, ahol elkezdheti beállítani a szinkronizálási folyamatot.

A következő két művelet feltételezi, hogy a konfigurálást a WSUS felügyeleti beépülő modullal végzi. E két művelet bemutatja, hogyan kell elindítani a WSUS felügyeleti beépülő modult és a kiszolgálót konfigurálni a **Beállítások** oldalon.

**A WSUS felügyeleti konzol elindítása**
-   A WSUS felügyeleti konzol elindításához mutasson a **Start** menü **Minden program**, majd **Felügyeleti eszközök** pontjára, végül kattintson a **Microsoft Windows Server Update Services 3.0** parancsra.

> [!NOTE]  
> A WSUS-konzol összes szolgáltatását csak a WSUS-kiszolgáló WSUS-rendszergazdák csoportjának és helyi Rendszergazdák biztonsági csoportnak a tagjai használhatják. A WSUS-jelentéskészítők biztonsági csoport tagjainak ugyanakkor van olvasási engedélyük a felügyeleti konzolhoz. 

**Frissítési forrás és proxykiszolgáló megadása**
1.  Kattintson a WSUS-konzol bal oldali panelén, a kiszolgáló neve alatt a **Beállítások**, majd a középső panelen a **Frissítés forrása és proxykiszolgáló** lehetőségre.

2.  Megjelenik egy párbeszédpanel, amely a **Frissítés forrása** és a **Proxykiszolgáló** lapot tartalmazza.

3.  Válassza ki a **Frissítés forrása** lapon azt a helyet, ahonnan a kiszolgáló letölti a frissítéseket. Ha azt választja, hogy a Microsoft Update webhelyről szinkronizál (ez az alapértelmezett beállítás), nem kell mást tennie ezen az oldalon.

4.  Ha úgy dönt, hogy másik WSUS-kiszolgálóról kíván szinkronizálni, meg kell adnia azt a portot, amelyen a kiszolgálók kommunikálni fognak (az alapértelmezett a 80-as port). Ha nem az alapértelmezett portot használja, gondoskodnia kell arról, hogy mindkét kiszolgáló tudja használni a megadott portot.

5.  Azt is beállíthatja, hogy az SSL protokollal történjen a szinkronizálás a felsőbb rétegbeli WSUS-kiszolgálóról. Ez esetben a kiszolgálók a 443-as portot használják a felsőbb rétegbeli kiszolgálóról történő szinkronizálás során.

6.  Ha ez a kiszolgáló a másik WSUS-kiszolgáló replikája, jelölje be az **Ez a kiszolgáló a felsőbb rétegbeli kiszolgáló replikája** jelölőnégyzetet. Ebben az esetben csak a felsőbb rétegbeli WSUS-kiszolgálón kell jóváhagyni a frissítéseket.

7.  Jelölje be a **Proxykiszolgáló** lap **Proxykiszolgáló használata szinkronizáláskor** jelölőnégyzetét, és írja be a proxykiszolgáló nevét, illetve portszámát (alapértelmezés szerint 80) a megfelelő mezőkbe.

8.  Ha egyéni hitelesítő adatokkal szeretne kapcsolatot létesíteni a proxykiszolgálóval, jelölje be a **Csatlakozás a proxykiszolgálóhoz felhasználói hitelesítő adatokkal** jelölőnégyzetet, majd írja be a felhasználónevet, a tartományt és a felhasználói jelszót a megfelelő mezőbe. Ha engedélyezni szeretné az alapfokú hitelesítést a proxykiszolgálóval kapcsolatot létesítő felhasználó számára, jelölje be az **Alapfokú hitelesítés engedélyezése (jelszó küldése nem titkosított szövegben)** jelölőnégyzetet.

9.  A beállítások mentéséhez kattintson az **OK** gombra.
