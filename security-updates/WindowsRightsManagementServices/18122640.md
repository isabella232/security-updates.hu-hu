---
TOCTitle: A kiszolgálói licencelői tanúsítvány megújítása
Title: A kiszolgálói licencelői tanúsítvány megújítása
ms:assetid: 'affce9cf-8b46-4293-8e1c-ee06f2ca6537'
ms:contentKeyID: 18122640
ms:mtpsurl: 'https://technet.microsoft.com/hu-hu/library/Cc747636(v=WS.10)'
---

A kiszolgálói licencelői tanúsítvány megújítása
===============================================

A művelet végrehajtásához helyben kell bejelentkeznie a felügyeleti webhelyre olyan tartományi felhasználói fiókkal, amely a Rendszergazdák csoport tagja az elérni kívánt számítógépen. A Tartománygazdák csoport tagjai is végrehajthatják ezt a műveletet. Biztonsági szempontból ajánlott a műveletet a **Futtatás másként** parancs segítségével végrehajtani.

A **Globális felügyelet** lap megnyitásához kattintson a **Start** gombra, és válassza a **Minden program**, a **Windows RMS**, majd a **Windows RMS felügyeleti webhely** parancsot.

Ha a kapcsolat nélküli megújítás lehetőséget választotta és az internethez kapcsolódáshoz és kiszolgálói licencelői tanúsítvány igényléséhez fokozott böngésző biztonságra konfigurált számítógépet használ – például Windows Server 2003 rendszert vagy a Windows XP Service Pack 2 szervizcsomagot futtató számítógépet –, a kiszolgálói licencelői tanúsítvány letöltésének engedélyezéséhez ne feledje felvenni az Igénylési szolgáltatás webhely URL-címét a Megbízható helyek zónájába. Ez az URL-cím a https://activation.drm.microsoft.com.

Ha az igénylést kapcsolat nélküli hajtja végre, gondoskodjon arról, hogy a Microsoft igénylési szolgáltatáshoz igénylési kérelem küldésére használt számítógép tanúsítványtárolójában telepítve legyen a GTE Cyber Trust Root CA hitelesítésszolgáltató tanúsítványa. Ez a hitelesítésszolgáltató Windows Server 2003 rendszert futtató számítógépeken alapértelmezés szerint megbízhatónak van ítélve. Ha a számítógépen a Windows más változata fut, a hitelesítésszolgáltatót a Windows Update webhelyről a legújabb tanúsítvány frissítések telepítésével minősítheti megbízhatónak.

A kiszolgálói licencelői tanúsítvány megújítása
-----------------------------------------------

#### A kiszolgálói licencelői tanúsítvány megújítása

1.  Nyissa meg a **Globális felügyelet** lapot, majd keresse meg azt a webhelyet, amelyen tanúsítványt szeretne megújítani, és kattintson a mellette látható **A webhelyen működő RMS felügyelete** hivatkozásra.

2.  A **Felügyelet** oldalon kattintson a **Fürterőforrások** terület **Megújítás** gombjára. Megjelenik a Megújítás párbeszédpanel.

3.  Ha a kiszolgáló csatlakozik az internethez, válassza az **On-line** lehetőséget, majd kattintson a **Megújítás** gombra, így automatikusan megújítja a kiszolgálói licencelői tanúsítványt.

4.  Ha a kiszolgáló nem csatlakozik az internethez, válassza a **Kapcsolat nélkül** lehetőséget, majd kattintson az **Exportálás** gombra. Megjelenik a **Fájl letöltése** párbeszédpanel.

5.  Kattintson a **Mentés** gombra. Megjelenik a **Mentés másként** párbeszédpanel.

    > [!NOTE]  
    > A **Fájl letöltése** párbeszédpanelen kattintson a **Megnyitás** gombra. Ha a **Megnyitás** gombra kattint, egy hibaüzenet jelenik meg, és a kérelem fájl nem lesz mentve. 

6.  A megújítási kérelem fájlba exportálásához kattintson a **Mentés** gombra. A fájl alapértelmezés szerint az asztalra lesz mentve, és a *kiszolgáló\_neve*RenewalRequest.xml nevet kapja, ahol a *kiszolgáló\_neve* helyett az RMS-kiszolgáló neve szerepel. A fájl más helyre is menthető, ehhez a Mentés helye legördülő menüben adja meg a kívánt helyet. A **Fájlnév** mezőbe új nevet beírva az alapértelmezett fájlnév is módosítható.

7.  A megújítási kérelem fájl mentése után megjelenik **A letöltés befejeződött** párbeszédpanel. A **Megnyitás** gombra kattintva megtekintheti a fájlban található XML-kódot, ekkor módosításra nincs lehetősége. A fájlt tartalmazó mappa megnyitásához kattintson a **Mappa megnyitása** elemre. Ha befejezte a fájl tartalmának és helyének vizsgálatát, kattintson a **Bezárás** gombra.

8.  A megújítási kérelemfájlt helyezze át a kiszolgálóról egy internetkapcsolattal rendelkező számítógépre, majd lépjen az [Igénylési szolgáltatás webhelyére]() (https://go.microsoft.com/fwlink/?LinkId=25828).

9.  A webhely útmutatásait követve szerezzen be egy kiszolgálói licencelői tanúsítványt.

10. Helyezze vissza a kiszolgálói licencelői tanúsítvány erre a legfelső szintű tanúsítási kiszolgálóra.

11. Kattintson a **Fürterőforrások** terület **Megújítás** gombjára. A **Megújítás** párbeszédpanel jelenik meg.

12. A **Megújítás** párbeszédpanelen kattintson a **Tallózás** gombra, keresse meg a letöltött kiszolgálói licencelői tanúsítványt, majd kattintson az **Importálás** gombra.

13. Az **Igen** gombra kattintással kattintva erősítse meg, hogy ezt a tanúsítványt szeretné importálni.

14. A kiszolgálói licencelői tanúsítvány sikeres megújítását követően a **Fürterőforrások** területen a kiszolgálói licencelői tanúsítvány új lejárati dátuma lesz látható.

A kiszolgálói licencelői tanúsítványok megújításáról a további tudnivalókat lásd: „[A kiszolgálói licencelői tanúsítványok kezelése](https://technet.microsoft.com/549979ad-13ee-4abc-8281-3e002a5a9561)”.
