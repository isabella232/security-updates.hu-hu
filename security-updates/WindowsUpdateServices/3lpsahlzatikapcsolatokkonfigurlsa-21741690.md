---
TOCTitle: '3. lépés: A hálózati kapcsolatok konfigurálása'
Title: '3. lépés: A hálózati kapcsolatok konfigurálása'
ms:assetid: '42a144c5-f08e-4a6e-b360-47ddea77bd24'
ms:contentKeyID: 21741690
ms:mtpsurl: 'https://technet.microsoft.com/hu-hu/library/Dd939815(v=WS.10)'
---

3. lépés: A hálózati kapcsolatok konfigurálása
==============================================

Ha befejezte a Windows Server Update Services 3.0 Service Pack 2 (WSUS 3.0 SP2) telepítését, automatikusan elindul a konfigurálási varázsló. A varázslót később is futtathatja, a WSUS felügyeleti konzol **Beállítások** lapjáról.

Mielőtt hozzálátna a konfiguráláshoz, tudnia kell a választ az alábbi kérdésekre:

1. Úgy van beállítva a kiszolgáló tűzfala, hogy az ügyfelek hozzá tudnak férni a kiszolgálóhoz?

2. Tud a számítógép kapcsolódni a felsőbb rétegbeli kiszolgálóhoz (például a Microsoft Update webhelyhez)?

3. Rendelkezésére áll az esetleges proxykiszolgáló neve és a hozzá szükséges felhasználói hitelesítő adatok?

A WSUS 3.0 SP2 szolgáltatás alapértelmezés szerint a Microsoft Update webhelyről tölti le a frissítéseket. Ha azonban proxykiszolgáló is működik a hálózaton, azt is beállíthatja, hogy a WSUS 3.0 SP2 a proxykiszolgálót használja. Ha vállalati tűzfal választja el egymástól a WSUS szolgáltatást és az internetet, lehetséges, hogy módosítani kell a tűzfal beállításait ahhoz, hogy a WSUS le tudja tölteni a frissítéseket.

 
<table style="border:1px solid black;">
<colgroup>
<col width="100%" />
</colgroup>
<thead>
<tr class="header">
<th style="border:1px solid black;" ><img src="images/Dd939815.note(WS.10).gif" />Megjegyzés</th>
</tr>
</thead>
<tbody>
<tr class="odd">
<td style="border:1px solid black;">Habár a Microsoft Update webhelyről csak működő internetkapcsolattal lehet frissítéseket letölteni, a WSUS szolgáltatással olyan hálózatokra is importálhatók a szükséges frissítések, amelyek nem férnek hozzá az internethez.
</td>
</tr>
</tbody>
</table>
 

A 3. lépésben a következő műveleteket kell végrehajtani:

-   A tűzfal beállítása
-   Annak meghatározása, hogy a kiszolgáló honnan töltse le a frissítéseket (a Microsoft Update webhelyről vagy egy másik WSUS-kiszolgálóról)
-   A proxykiszolgáló beállításainak módosítása, hogy a WSUS le tudja tölteni a frissítéseket

**A tűzfal beállításainak módosítása**
-   Ha vállalati tűzfal választja el egymástól a WSUS szolgáltatást és az internetet, lehetséges, hogy módosítani kell a tűzfal beállításait ahhoz, hogy a WSUS le tudja tölteni a frissítéseket. A frissítések Microsoft Update webhelyről történő letöltéséhez a WSUS-kiszolgáló a 80-as portot (HTTP) és a 443-as portot (HTTPS) használja. E két beállítás megváltoztatására nincs lehetőség.

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

 
<table style="border:1px solid black;">
<colgroup>
<col width="100%" />
</colgroup>
<thead>
<tr class="header">
<th style="border:1px solid black;" ><img src="images/Dd939815.note(WS.10).gif" />Megjegyzés</th>
</tr>
</thead>
<tbody>
<tr class="odd">
<td style="border:1px solid black;">A tűzfal beállítását célzó fenti műveletek a WSUS szolgáltatás és az internet közötti vállalati tűzfalra vonatkoznak. A WSUS-kiszolgálón nincs szükség a Windows tűzfal beállításainak módosítására, hiszen saját hálózati adatforgalmát teljes egészében a WSUS szolgáltatás kezdeményezi.
</td>
</tr>
</tbody>
</table>
 

Habár a Microsoft Update webhely és a WSUS szolgáltatás közötti kapcsolat megteremtéséhez a 80-as és a 443-as portnak nyitva kell lennie, egyéni port megadásával több WSUS-kiszolgáló is használhatja ugyanazt a portot.

A következő két művelet feltételezi, hogy a konfigurációs varázslót használja. E művelet későbbi része bemutatja, hogyan kell elindítani a WSUS felügyeleti beépülő modult és a kiszolgálót konfigurálni a Beállítások lapon.

**Annak meghatározása, hogy a kiszolgáló honnan töltse le a frissítéseket**
1.  A Microsoft Update szolgáltatásainak javítását célzó programhoz való csatlakozást követően kattintson a konfigurációs varázsló **Tovább** gombjára. Ezután megadhatja a felsőbb rétegbeli kiszolgálót.

2.  Ha azt választja, hogy a Microsoft Update webhelyről szinkronizál, nem kell mást tennie a Beállítások lapon. Kattintson a **Tovább** gombra, vagy válassza a **Proxykiszolgáló megadása** elemet a navigációs ablaktáblában.

3.  Ha úgy dönt, hogy egy másik WSUS-kiszolgálóról kíván szinkronizálni, meg kell adnia a kiszolgáló nevét és azt a portot, amelyen a kiszolgáló kommunikálni fog a felsőbb rétegbeli kiszolgálóval.

4.  Ha SSL-alapú titkosítást szeretne használni, jelölje be az **SSL használata a frissítési adatok szinkronizálásakor** jelölőnégyzetet. Ez esetben a kiszolgálók a 443-as portot használják a szinkronizálás során. (Ügyeljen arra, hogy mind ez a kiszolgáló, mind a felsőbb rétegbeli kiszolgáló támogassa az SSL használatát.)

5.  Ha ez a kiszolgáló a replikakiszolgáló, jelölje be az **Ez a felsőbb rétegbeli kiszolgáló replikája** jelölőnégyzetet.

6.  Ezzel befejeződött a felsőbb rétegbeli kiszolgáló konfigurálása. Kattintson a **Tovább** gombra, vagy válassza a **Proxykiszolgáló megadása** elemet a navigációs ablaktáblában.

**Proxykiszolgáló beállításainak megadása**
1.  Jelölje be a varázsló **Proxykiszolgáló megadása** lapján a **Proxykiszolgáló használata szinkronizáláskor** jelölőnégyzetét, és írja be a proxykiszolgáló nevét, illetve portszámát (alapértelmezés szerint 80) a megfelelő mezőkbe.

2.  Ha egyéni hitelesítő adatokkal szeretne kapcsolatot létesíteni a proxykiszolgálóval, jelölje be a **Csatlakozás a proxykiszolgálóhoz felhasználói hitelesítő adatokkal** jelölőnégyzetet, majd írja be a felhasználónevet, a tartományt és a felhasználói jelszót a megfelelő mezőbe. Ha engedélyezni szeretné az alapfokú hitelesítést a proxykiszolgálóval kapcsolatot létesítő felhasználó számára, jelölje be az **Alapfokú hitelesítés engedélyezése (jelszó küldése nem titkosított szövegben)** jelölőnégyzetet.

3.  Ezzel befejeződött a proxykiszolgáló konfigurálása. Kattintson a **Tovább** gombra a következő lapra történő továbblépéshez, ahol elkezdheti beállítani a szinkronizálási folyamatot.

A következő két művelet feltételezi, hogy a konfigurálást a WSUS felügyeleti beépülő modullal végzi. E két művelet bemutatja, hogyan kell elindítani a WSUS felügyeleti beépülő modult és a kiszolgálót konfigurálni a **Beállítások** lapon.

**A WSUS felügyeleti konzol elindítása**
-   A WSUS felügyeleti konzol elindításához mutasson a **Start** menü **Minden program** pontjára, majd a **Felügyeleti eszközök** pontra, és kattintson a **Microsoft Windows Server Update Services 3.0** parancsra.

 
<table style="border:1px solid black;">
<colgroup>
<col width="100%" />
</colgroup>
<thead>
<tr class="header">
<th style="border:1px solid black;" ><img src="images/Dd939815.note(WS.10).gif" />Megjegyzés</th>
</tr>
</thead>
<tbody>
<tr class="odd">
<td style="border:1px solid black;">A konzol összes szolgáltatásának használatához a WSUS-rendszergazdák vagy a helyi Rendszergazdák biztonsági csoport tagjaként kell bejelentkezni a WSUS szolgáltatást futtató kiszolgálón. A WSUS-jelentéskészítők biztonsági csoport tagjai olvasási jogosultsággal rendelkeznek a konzolhoz.
</td>
</tr>
</tbody>
</table>
 

**Frissítési forrás és proxykiszolgáló megadása**
1.  Kattintson a WSUS-konzol bal oldali ablaktáblájában a kiszolgáló neve alatt a **Beállítások**, majd a középső panelen a **Frissítés forrása és proxykiszolgáló** elemre.

    Ekkor megjelenik egy párbeszédpanel, amely a **Frissítés forrása** és a **Proxykiszolgáló** lapot tartalmazza.

2.  Válassza ki a **Frissítés forrása** lapon azt a helyet, ahonnan a kiszolgáló letölti a frissítéseket. Ha azt választja, hogy a Microsoft Update webhelyről szinkronizál (ez az alapértelmezett beállítás), nem kell mást tennie ezen az oldalon.

3.  Ha úgy dönt, hogy másik WSUS-kiszolgálóról kíván szinkronizálni, meg kell adnia azt a portot, amelyen a kiszolgálók kommunikálni fognak (az alapértelmezett a 80-as port). Ha nem az alapértelmezett portot használja, gondoskodnia kell arról, hogy mindkét kiszolgáló tudja használni a megadott portot.

4.  Azt is beállíthatja, hogy az SSL protokollal történjen a szinkronizálás a felsőbb rétegbeli WSUS-kiszolgálóról. Ez esetben a kiszolgálók a 443-as portot használják a felsőbb rétegbeli kiszolgálóról történő szinkronizálás során.

5.  Ha ez a kiszolgáló a másik WSUS-kiszolgáló replikája, jelölje be az **Ez a kiszolgáló a felsőbb rétegbeli kiszolgáló replikája** jelölőnégyzetet. Ebben az esetben csak a felsőbb rétegbeli WSUS-kiszolgálón kell jóváhagyni a frissítéseket.

6.  Jelölje be a **Proxykiszolgáló** lap **Proxykiszolgáló használata szinkronizáláskor** jelölőnégyzetét, és írja be a proxykiszolgáló nevét, illetve portszámát (alapértelmezés szerint 80) a megfelelő mezőkbe.

7.  Ha egyéni hitelesítő adatokkal szeretne kapcsolatot létesíteni a proxykiszolgálóval, jelölje be a **Csatlakozás a proxykiszolgálóhoz felhasználói hitelesítő adatokkal** jelölőnégyzetet, majd írja be a felhasználónevet, a tartományt és a felhasználói jelszót a megfelelő mezőbe. Ha engedélyezni szeretné az alapfokú hitelesítést a proxykiszolgálóval kapcsolatot létesítő felhasználó számára, jelölje be az **Alapfokú hitelesítés engedélyezése (jelszó küldése nem titkosított szövegben)** jelölőnégyzetet.

8.  A beállítások mentéséhez kattintson az **OK** gombra.

Következő lépés
---------------

[4. lépés: Frissítések és szinkronizálás konfigurálása](https://technet.microsoft.com/deeaa7e1-9b50-45cb-9537-d75f70de3405)

További források
----------------

[Részletes útmutató a Windows Server Update Services 3.0 SP2 telepítéséhez](https://technet.microsoft.com/4b504edc-93b3-45b0-a7e8-d0107f1a4442)
