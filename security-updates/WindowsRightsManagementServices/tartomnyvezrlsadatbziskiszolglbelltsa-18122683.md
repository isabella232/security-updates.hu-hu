---
TOCTitle: 'Tartományvezérlő és adatbázis-kiszolgáló beállítása'
Title: 'Tartományvezérlő és adatbázis-kiszolgáló beállítása'
ms:assetid: 'd20f8305-9f9e-4760-bfbf-82824db60d1f'
ms:contentKeyID: 18122683
ms:mtpsurl: 'https://technet.microsoft.com/hu-hu/library/Cc747681(v=WS.10)'
---

Tartományvezérlő és adatbázis-kiszolgáló beállítása
===================================================

Csak azt követően lehet legfelső szintű tanúsítási kiszolgálót vagy licenckiszolgálót telepíteni, ha ki van alakítva a működéséhez szükséges tartomány- és adatbázis-támogatás. Ehhez az Active Directory és egy adatbázis-kiszolgáló szükséges, amely az SQL Server 2000 Service Pack 3 (SP3) csomaggal frissített verziója vagy a Microsoft® SQL Server 2000 Desktop Engine (MSDE 2000) Release A lehet. Még ha futnak is már az éles környezetben a szükséges összetevők, az éles környezetet nem javasolt a tesztelés céljára használni.

A következő eljárás bemutatja, hogyan lehet kiszolgálóoldali tesztelés céljára elszigetelt hálózatban egyetlen számítógépet tartományvezérlőként és adatbázis-kiszolgálóként beállítani.

| ![](images/Cc747681.note(WS.10).gif)Megjegyzés:                                                                                                                                                                                                                                                                                             |
|--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| A példában az adatbázis-kiszolgáló a tartományvezérlőn fut. Éles környezetekben az az általános szabály, hogy tartományvezérlőn nem ajánlatos más összetevőket futtatni. A példában ugyanarra a számítógépre telepítjük az Active Directory szolgáltatást és az adatbázis-kiszolgálót, mert így a lehető legkevesebb számítógéppel kialakítható a teljes infrastruktúra. |

Ha adatbázis-kiszolgálóként az MSDE 2000 mellett dönt, ügyeljen arra, hogy ez semmilyen hálózati csatlakozófelületet sem támogat, és az MSDE 2000 használati feltételei megtiltják az SQL Server ügyféleszközeinek használatát az MSDE 2000 adatbázisok kezelésére. Ezt a korlátozást figyelembe véve nem áll majd módjában megtekinteni a naplózott adatokat, sem módosítani a konfigurációs adatbázisban tárolt adatokat. Emiatt az RMS adatbázisainak kezeléséhez az MSDE 2000 használata csak tesztkörnyezetben javasolt.

###  

<p> </p>
<table style="border:1px solid black;">
<colgroup>
<col width="33%" />
<col width="33%" />
<col width="33%" />
</colgroup>
<thead>
<tr class="header">
<th>Infrastrukturális összetevő</th>
<th>Tartományvezérlő és adatbázis-kiszolgáló beállításának lépései</th>
<th>Éles környezetben való bevezetéssel kapcsolatos megjegyzések</th>
</tr>
</thead>
<tbody>
<tr class="odd">
<td style="border:1px solid black;"><p>Operációs rendszer</p></td>
<td style="border:1px solid black;"><p>Telepítse a Windows 2000 Server SP3 vagy újabb verzióját vagy a Windows Server 2003 rendszert egy olyan számítógépre, amely megfelel az RMS hardverkövetelményeinek, de még nincs hálózathoz csatlakoztatva. A partíción az NTFS fájlrendszert használja.</p></td>
<td style="border:1px solid black;"><p>Kifejezetten ajánljuk, hogy mindig a legfrissebb szervizcsomagot használja, és telepítse a javításokat is. NTFS formátumú partíciókat használjon.</p></td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><p>Hálózati kapcsolat</p></td>
<td style="border:1px solid black;"><p>Létesítsen kapcsolatot egy olyan hálózattal, amelyen keresztül kapcsolódni lehet az internethez, de el van választva az éles környezettől.</p></td>
<td style="border:1px solid black;"><p>Az internetkapcsolatot megfelelő tűzfalnak kell védenie.</p></td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><p>IP-cím</p></td>
<td style="border:1px solid black;"><p>Adjon a számítógének egy statikus IP-címet.</p></td>
<td style="border:1px solid black;"><p>Kiszolgálókon mindig statikus IP-címet használjon.</p></td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><p>Az Active Directory</p></td>
<td style="border:1px solid black;"><p>Jelentkezzen be helyi rendszergazdaként.</p></td>
<td style="border:1px solid black;"><p> </p></td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><p> </p></td>
<td style="border:1px solid black;"><p>Kattintson a <strong>Start</strong> gombra, válassza a <strong>Futtatás</strong> parancsot, és írja be <code>dcpromo</code> parancsot a <strong>Megnyitás</strong> mezőbe, majd kattintson az <strong>OK</strong> gombra.</p></td>
<td style="border:1px solid black;"><p> </p></td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><p> </p></td>
<td style="border:1px solid black;"><p>Miután elindult az Active Directory telepítővarázslója, a lépéseket végrehajtva hozzon létre egy új tartományt egy új erdőben. Az alábbiak kivételével mindenhol fogadja el az alapértelmezett beállításokat:</p>
<p>Adja meg a tartománynevet (például contoso.com).</p>
<p>Engedélyezze a varázslónak, hogy konfigurálja a számítógépen a DNS szolgáltatást.</p>
<p>Válassza a <strong>Csak Windows 2000 kiszolgálókkal kompatibilis engedélyek</strong> beállítást, ha az összes tartományvezérlőn Windows 2000 vagy újabb rendszer fut.</p>
<p>Adjon meg egy nehezen feltörhető jelszót a helyi rendszergazdának.</p></td>
<td style="border:1px solid black;"><p>Ha új tartományokra van szükség az RMS megvalósításához, az Active Directoryban állítsa be ezeket.</p>
<p>Minden fiókot mindig nehezen feltörhető jelszóval kell védeni.</p></td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><p> </p></td>
<td style="border:1px solid black;"><p>Amikor a varázsló kéri, indítsa újra a számítógépet.</p></td>
<td style="border:1px solid black;"><p> </p></td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><p> </p></td>
<td style="border:1px solid black;"><p>Az <strong>Active Directory - felhasználók és számítógépek</strong> beépülő modul segítségével ellenőrizze működési szintet: ehhez kattintson a jobb oldali egérgombbal a tartomány nevére, válassza a <strong>Tulajdonságok</strong> parancsot, és nézze meg a <strong>Tartomány üzemmódja</strong> mező értékét. Ha nincsenek a Windows 2000 rendszerűnél korábbi tartományvezérlők, kattintson a <strong>Mód váltása</strong> gombra, és állítsa át a tartományt a <strong>Natív mód</strong> beállításra.</p>
<p>Megjegyzés: A Windows Server 2003 rendszeren a <strong>Tartomány üzemmódja</strong> beállítás helyett <strong>Tartomány működési szintje</strong> szerepel.</p></td>
<td style="border:1px solid black;"><p>Az optimális szintű védelem és a kezelhetőség feltétele, hogy az RMS támogatásához egységes Windows 2000 működési szintet használjon.</p></td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><p>Felhasználói fiókok</p></td>
<td style="border:1px solid black;"><p>Hozzon létre egy tartományi felhasználói fiókot az RMS szolgáltatásfiókjaként való használatra. Ez például a következő lehet: ContosoRMS@contoso.com. Nehezen feltörhető jelszót adjon meg. Feltétlenül adjon meg e-mail címet is a felhasználónak. Ha az e-mail cím nincs megadva az Active Directoryban, a felhasználó nem lesz képes licenceket és tanúsítványokat szerezni az RMS szolgáltatástól.</p>
<p>Megjegyzés: Az RMS szolgáltatásfiókja nem egyezhet meg az RMS telepítéséhez használt tartományi fiókkal.</p></td>
<td style="border:1px solid black;"><p>Hozzon létre külön fiókot az Active Directoryban az RMS szolgáltatásfiókjaként való használatra. E-mail címet is adjon meg. Ne adjon a fióknak semmilyen különleges engedélyt.</p></td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><p>SQL Server 2000</p></td>
<td style="border:1px solid black;"><p>Jelentkezzen be arra a kiszolgálóra, amelyen az adatbázis telepítését tervezi. Ha ez megegyezik a tartományvezérlővel, tartománygazdaként kell bejelentkeznie.</p></td>
<td style="border:1px solid black;"><p> </p></td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><p> </p></td>
<td style="border:1px solid black;"><p>Az adatbázis-kiszolgáló szoftverének telepítéséhez kövesse a termékhez kapott utasításokat.</p></td>
<td style="border:1px solid black;"><p> </p></td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><p> </p></td>
<td style="border:1px solid black;"><p>A telepítésnél alkalmazza a kiszolgálókkal kapcsolatos gyakorlati tanácsokat, azaz:</p>
<ul>
<li>Adjon nevet az adatbázis rendszergazdai fiókjának, és adja meg a szervezet nevét (például Contoso).<br />
<br />
</li>
<li>A rendszergazdánál nehezen feltörhető jelszót használjon.<br />
<br />
</li>
<li>Használja a beépített Windows-hitelesítés módszereit.<br />
<br />
</li>
</ul></td>
<td style="border:1px solid black;"><p>Ha egy mód van rá, a Windows-hitelesítési módot kell használni. Ha nem tudja ebben az üzemmódban futtatni az adatbázis-kiszolgálót, forduljon a tartománygazdához és az adatbázis-kiszolgáló rendszergazdájához, és beszélje meg velük, hogy milyen módosításokra lehet szükség az RMS beállításaiban.</p></td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><p> </p></td>
<td style="border:1px solid black;"><p>Ha nincs leállítva az adatbázis-szolgáltatás, állítsa azt le.</p></td>
<td style="border:1px solid black;"><p> </p></td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><p> </p></td>
<td style="border:1px solid black;"><p>Telepítse az adatbázis-kiszolgáló szoftverfrissítéseit. Ha ekkor jelszót kell megadni, a telepítésnél választott jelszót használja.</p></td>
<td style="border:1px solid black;"><p> </p></td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><p> </p></td>
<td style="border:1px solid black;"><p>Indítsa újra a számítógépet. Ellenőrizze, hogy elindult-e az adatbázis-szolgáltatás.</p></td>
<td style="border:1px solid black;"><p> </p></td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><p> </p></td>
<td style="border:1px solid black;"><p>Ellenőrizze, hogy a felhasználói fiókok érvényes e-mail címmel rendelkeznek-e az Active Directoryban.</p></td>
<td style="border:1px solid black;"><p> </p></td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><p> </p></td>
<td style="border:1px solid black;"><p>Ügyeljen arra, hogy az RMS felügyeletéért (és a legfelső szintű tanúsítási és a licenckiszolgálók létesítéséért) felelős tartományi felhasználó rendelkezzen a szükséges engedélyekkel az adatbázis-kiszolgálón. Ha adatbázis-kiszolgálóként SQL Server kiszolgálót használ, bejelentkezési azonosítót vehet fel ahhoz a felhasználóhoz, aki az <strong>SQL Server Enterprise Manager</strong> beépülő modult használja. A beépülő modulban bontsa ki a kiszolgáló és a kiszolgálócsoport ágát, majd a <strong>Security</strong> (Biztonság) elemet. Kattintson a <strong>Logins</strong> (Bejelentkezési nevek) elemre, hozzon létre új bejelentkezési nevet a tartományi felhasználó fiókjához, térjen át a <strong>Server Roles</strong> (Kiszolgálói szerepkörök) panellapra, és jelölje be a <strong>Server Administrators</strong> (Kiszolgálói rendszergazdák) négyzetet.</p></td>
<td style="border:1px solid black;"><p>Fontos: Minden olyan felhasználónak és csoportnak, aki vagy amely az RMS szolgáltatást licencszerzésre és tartalom közzétételére használja, e-mail címet kell beállítani az MMC Active Directory - felhasználók és számítógépek beépülő moduljában a <strong>Tulajdonságok</strong> párbeszédpanel <strong>Általános</strong> lapján.</p></td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><p>Internetkapcsolat</p>
<p>(nem kötelező)</p></td>
<td style="border:1px solid black;"><p>Ellenőrizze, hogy a böngésző és a kiszolgáló (esetleg a szükséges proxykiszolgáló), a TCP/IP és az LMHOSTS/HOSTS megfelelően be van-e állítva az internet eléréséhez. Tesztelje ezt a http://uddi.microsoft.com cím felkeresésével. Ha meg tudja nyitni ezt a lapot, az RMS kapcsolódni tud a Microsoft igénylési szolgáltatásához.</p></td>
<td style="border:1px solid black;"><p>A http://uddi.microsoft.com felkeresésével győződjön meg az internet elérhetőségéről.</p></td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><p>Szoftverfrissítések</p></td>
<td style="border:1px solid black;"><p>Töltse le és telepítse az adott számítógépen telepített szoftverek legújabb frissítéseit (ne feledkezzen meg a Windows www.microsoft.com webhelyen elérhető frissítéseiről sem).</p></td>
<td style="border:1px solid black;"><p>Mindig töltse le és telepítse a legújabb szervizcsomagokat.</p></td>
</tr>
</tbody>
</table>
  
A fenti lépések maradéktalan végrehajtása után készen áll a kezdeti telepítés (az előfeltételként szükséges szoftverek telepítését is beleértve) végrehajtására az RMS szolgáltatást futtató számítógépeken.
