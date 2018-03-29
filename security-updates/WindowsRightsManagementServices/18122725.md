---
TOCTitle: Legfelső szintű tanúsítási kiszolgáló kézi igénylése
Title: Legfelső szintű tanúsítási kiszolgáló kézi igénylése
ms:assetid: 'aecdebb5-b28b-4b58-937a-392bb6ce9643'
ms:contentKeyID: 18122725
ms:mtpsurl: 'https://technet.microsoft.com/hu-hu/library/Cc747727(v=WS.10)'
---

Legfelső szintű tanúsítási kiszolgáló kézi igénylése
====================================================

A művelet végrehajtásához helyben kell bejelentkeznie a felügyeleti webhelyre olyan tartományi felhasználói fiókkal, amely a Rendszergazdák csoport tagja az elérni kívánt számítógépen. A Tartománygazdák csoport tagjai is végrehajthatják ezt a műveletet. Biztonsági szempontból ajánlott a műveletet a Futtatás másként parancs segítségével végrehajtani.

A **Globális felügyelet** lap megnyitásához kattintson a **Start** gombra, és válassza a **Minden program**, a **Windows RMS**, majd a **Windows RMS felügyeleti webhely** parancsot.

Ha az igénylést kapcsolat nélküli hajtja végre, gondoskodjon arról, hogy az RMS ügyfelek az igénylés befejeződéséig ne próbáljanak licencekért az RMS-kiszolgálóhoz kapcsolódni. Ha az RMS ügyfelek nem igényelt RMS-kiszolgálóhoz próbálnak kapcsolódni, a webszolgáltatások olyan hibaállapotba kerülnek, amely használhatatlanná teszi azokat. Ha nem tudja biztosítani, hogy az ügyfelek ne kapcsolódjanak az RMS-kiszolgálóhoz, a legjobb, ha az igénylést követően az IIS alaphelyzetbe állításával megszünteti az esetlegesen bekövetkező hibaállapotokat.

Ha a kapcsolat nélküli igénylési lehetőséget választotta és az internethez kapcsolódáshoz és kiszolgálói licencelői tanúsítvány igényléséhez fokozott böngésző biztonságra konfigurált számítógépet használ – például Windows Server 2003 rendszert vagy a Windows XP Service Pack 2 szervizcsomagot futtató számítógépet –, a kiszolgálói licencelői tanúsítvány letöltésének engedélyezéséhez ne feledje felvenni az Igénylési szolgáltatás webhely URL-címét a Megbízható helyek zónájába. Ez az URL-cím a https://activation.drm.microsoft.com.

Ha az igénylést kapcsolat nélküli hajtja végre, gondoskodjon arról, hogy a Microsoft igénylési szolgáltatáshoz igénylési kérelem küldésére használt számítógép tanúsítványtárolójában telepítve legyen a GTE Cyber Trust Root CA hitelesítésszolgáltató tanúsítványa. Ez a hitelesítésszolgáltató Windows Server 2003 rendszert futtató számítógépeken alapértelmezés szerint megbízhatónak van ítélve. Ha a számítógépen a Windows más változata fut, a hitelesítésszolgáltatót a Windows Update webhelyről a legújabb tanúsítvány frissítések telepítésével minősítheti megbízhatónak.

Legfelső szintű tanúsítási kiszolgáló kézi igénylése
----------------------------------------------------

#### Legfelső szintű tanúsítási kiszolgáló kézi igénylése

1.  Miután telepítette az RMS-szolgáltatást arra a kiszolgálóra, amelyet legfelső szintű tanúsítási kiszolgálónak szán, nyissa meg a **Globális felügyelet** lapot, majd keresse meg azt a webhelyet, amelyre szeretne legfelső szintű tanúsítási kiszolgálói licencelői tanúsítványt importálni, és kattintson a mellette látható **A webhelyen működő RMS felügyelete** hivatkozásra.

2.  Kattintson a **Fürterőforrások** terület **Megújítás** gombjára. Megjelenik az **Igénylés** párbeszédpanel.

3.  Válassza a **Kapcsolat nélkül** lehetőséget, majd kattintson az **Exportálás** gombra. Megjelenik a **Fájl letöltése** párbeszédpanel.

4.  Kattintson a **Mentés** gombra. Megjelenik a **Mentés másként** párbeszédpanel.

    > [!NOTE]  
    > A **Fájl letöltése** párbeszédpanelen kattintson a **Megnyitás** gombra. Ha a **Megnyitás** gombra kattint, egy hibaüzenet jelenik meg, és a kérelem fájl nem lesz mentve.

5.  Az igénylési kérelem fájlba exportálásához kattintson a **Mentés** gombra. A fájlt alapértelmezés szerint az asztalra menti a rendszer, és a *kiszolgáló\_neve*EnrollRequest.xml nevet kapja, ahol a *kiszolgáló\_neve* helyett az RMS-kiszolgáló neve szerepel. A fájl más helyre is menthető, ehhez a **Mentés helye** lenyitható listán adja meg a kívánt helyet. A **Fájlnév** mezőbe új nevet beírva az alapértelmezett fájlnév is módosítható.

6.  Az igénylési kérelem fájl mentése után megjelenik **A letöltés befejeződött** párbeszédpanel. A **Megnyitás** gombra kattintva megtekintheti a fájlban található XML-kódot, ekkor módosításra nincs lehetősége. A fájlt tartalmazó mappa megnyitásához kattintson a **Mappa megnyitása** elemre. Ha befejezte a fájl tartalmának és helyének vizsgálatát, kattintson a **Bezárás** gombra.

7.  Az igénylési kérelemfájlt helyezze át a kiszolgálóról egy internetkapcsolattal rendelkező számítógépre, majd lépjen az [Igénylési szolgáltatás webhelyére]().

8.  A webhely útmutatásait követve szerezzen be egy kiszolgálói licencelői tanúsítványt.

9.  Helyezze vissza a kiszolgálói licencelői tanúsítvány erre a legfelső szintű tanúsítási kiszolgálóra.

10. Kattintson a **Fürterőforrások** terület **Megújítás** gombjára. Megjelenik az **Igénylés** párbeszédpanel.

11. Az **Igénylés** párbeszédpanelen kattintson a **Tallózás** gombra, keresse meg a letöltött kiszolgálói licencelői tanúsítványt, majd kattintson az **Importálás** gombra.

12. Az **Igen** gombra kattintással kattintva erősítse meg, hogy ezt a tanúsítványt szeretné importálni.

13. A **Fürterőforrások** területen a kiszolgálói licencelői tanúsítvány lesz látható.