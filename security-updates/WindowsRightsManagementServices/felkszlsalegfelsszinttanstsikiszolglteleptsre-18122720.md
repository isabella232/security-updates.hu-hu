---
TOCTitle: Felkészülés a legfelső szintű tanúsítási kiszolgáló telepítésére
Title: Felkészülés a legfelső szintű tanúsítási kiszolgáló telepítésére
ms:assetid: 'ed51605e-8b17-4155-8d83-f6777f499b7b'
ms:contentKeyID: 18122720
ms:mtpsurl: 'https://technet.microsoft.com/hu-hu/library/Cc747726(v=WS.10)'
---

Felkészülés a legfelső szintű tanúsítási kiszolgáló telepítésére
================================================================

A példában bemutatott teszttelepítésben csak egy legfelső szintű tanúsítási kiszolgáló szerepel. Igény szerint további kiszolgálók is telepíthetők, akár legfelső szintű tanúsítási fürt részeként, akár önálló licencelési kiszolgáló fürtjeként. Az összes ilyen kiszolgálónak azonos az infrastrukturális beállítása, így mindegyik kiszolgálón az alább ismertetett eljárást kell végrehajtani.

A tartományvezérlő telepítése és az adatbázis-kiszolgálók beállítása (ezt az előző szakasz ismerteti), majd az alábbi táblázat lépéseinek végrehajtása után készen áll az RMS telepítésére.

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
<th>A kiszolgáló felkészítése az RMS telepítésére</th>
<th>Éles környezetben való bevezetéssel kapcsolatos megjegyzések</th>
</tr>
</thead>
<tbody>
<tr class="odd">
<td style="border:1px solid black;"><p>Operációs rendszer</p></td>
<td style="border:1px solid black;"><p>Telepítse a Windows Server 2003 rendszert egy olyan számítógépre, amely megfelel az RMS hardverkövetelményeinek, de még nincs hálózathoz csatlakoztatva. A partíción az NTFS fájlrendszert használja.</p></td>
<td style="border:1px solid black;"><p>Kifejezetten ajánljuk, hogy mindig a legfrissebb szervizcsomagot használja, és telepítse a javításokat is. NTFS formátumú partíciókat használjon.</p></td>
</tr>  
<tr class="even">
<td style="border:1px solid black;"><p>Internetkapcsolat</p>
<p>(nem kötelező)</p></td>
<td style="border:1px solid black;"><p>Létesítsen Ethernet-kapcsolatot egy olyan hálózattal, amelyen keresztül kapcsolódni lehet az internethez, de el van választva az éles környezettől. Ha a létesítési folyamat részeként az RMS kiszolgáló on-line igénylését kívánja végrehajtani, a kiszolgálónak internetkapcsolattal kell rendelkeznie.</p></td>
<td style="border:1px solid black;"><p>Az on-line igénylés használatakor az internetkapcsolatot megfelelő tűzfallal kell védeni.</p></td>
</tr>  
<tr class="odd">
<td style="border:1px solid black;"><p>IP-cím</p></td>
<td style="border:1px solid black;"><p>Adjon a számítógének egy statikus IP-címet.</p></td>
<td style="border:1px solid black;"><p>Kiszolgálókon mindig statikus IP-címet használjon.</p></td>
</tr>  
<tr class="even">
<td style="border:1px solid black;"><p>A számítógép csatlakoztatása a tartományhoz</p></td>
<td style="border:1px solid black;"><p>A számítógépen jelentkezzen be helyi rendszergazdaként. Kattintson a <strong>Start</strong> gombra, a jobb oldali egérgombbal a <strong>Sajátgép</strong> ikonra, válassza a <strong>Tulajdonságok</strong> parancsot, és a <strong>Számítógépnév</strong> panellapon kattintson a <strong>Módosítás</strong> gombra.</p></td>
<td style="border:1px solid black;"><p>Mindegyik kiszolgálón ugyanazt a tartományt használja.</p></td>
</tr>  
<tr class="odd">
<td style="border:1px solid black;"><p> </p></td>
<td style="border:1px solid black;"><p>Hagyja változatlanul a számítógép nevét, kattintson a <strong>Tartomány</strong> gombra, majd írja be a tartomány nevét (például Contoso.com), végül kattintson az <strong>OK</strong> gombra. Adja meg a tartományhoz való csatlakozásra módot adó hitelesítő adatokat, kattintson az <strong>OK</strong> gombra, majd amikor a rendszer kéri, indítsa újra a számítógépet. Amikor a számítógép újraindulása után a rendszer kéri a hitelesítő adatokat, adja meg a megfelelő tartományt, felhasználónevet és jelszót.</p></td>
<td style="border:1px solid black;"><p> </p></td>
</tr>  
<tr class="even">
<td style="border:1px solid black;"><p>Felhasználó és bejelentkezés</p></td>
<td style="border:1px solid black;"><p>Kattintson jobb oldali egérgombbal a <strong>Sajátgép</strong> ikonra, válassza a <strong>Kezelés</strong> parancsot, bontsa ki a <strong>Helyi felhasználók és csoportok</strong> ágat, kattintson a <strong>Csoportok</strong> elemre, majd kattintson duplán a <strong>Rendszergazdák</strong> csoportra.</p>
<p>Kattintson a <strong>Hozzáadás</strong> gombra, adja meg a felvenni kívánt felhasználói fiók nevét (például Mihaly@contoso.com), majd kattintson az <strong>OK</strong> gombra. Adjon rendszergazdai jogokat a felhasználói fióknak. Amikor a rendszer a hitelesítő adatokat kéri, adja meg a megfelelő fiók adatait, például Contoso\Rendszergazda.</p>
<p>Jelentkezzen be olyan tartományi felhasználóként, akinek rendszergazdai jogai vannak a számítógépen.</p></td>
<td style="border:1px solid black;"><p>Rendszergazdai jogok szükségesek ahhoz, hogy összetevőket lehessen a számítógéphez hozzáadni. A telepítés egyes lépései nem végezhetők el a helyi rendszergazdai fiókkal. Legalább egy olyan tartományi felhasználónak léteznie kell ezen a kiszolgálón, aki rendszergazda is. Az SQL Server ezenkívül System Administrator (Rendszergazda) jogokat követel meg az új adatbázisok létrehozásához.</p></td>
</tr>  
<tr class="odd">
<td style="border:1px solid black;"><p>Internetkapcsolat</p>
<p>(nem kötelező)</p></td>
<td style="border:1px solid black;"><p>A böngészőben a http://uddi.microsoft.com/ cím beírásával ellenőrizze az internetelérést. A Windows Server 2003 rendszerű számítógépeken előfordulhat, hogy módosítani kell az LMHOSTS és a HOSTS fájlt, hogy szerepeljen ezekben a tartományvezérlő.</p></td>
<td style="border:1px solid black;"><p>A http://uddi.microsoft.com webhely felkeresésével ellenőrizze az internet elérhetőségét.</p></td>
</tr>  
<tr class="even">
<td style="border:1px solid black;"><p>A Windows aktiválása</p></td>
<td style="border:1px solid black;"><p>Az aktiválási varázsló segítségével interneten keresztül aktiválja a Windows rendszert a Microsoftnál, de ez telefonon is végrehajtható. A Windows Server 2003 termék aktiválásáról a Windows Server 2003 súgójában talál további tájékoztatást.</p></td>
<td style="border:1px solid black;"><p>A Windows Server 2003 rendszert a telepítésétől számított 14 napon belül aktiválni kell.</p></td>
</tr>  
<tr class="odd">
<td style="border:1px solid black;"><p>Szoftverfrissítések</p></td>
<td style="border:1px solid black;"><p>Telepítse a számítógépen lévő szoftverek legújabb frissítéseit.</p></td>
<td style="border:1px solid black;"><p>Telepítse a legújabb szoftverfrissítéseket.</p></td>
</tr>  
<tr class="even">
<td style="border:1px solid black;"><p>Az Internet Explorer konfigurálása</p></td>
<td style="border:1px solid black;"><p>Az RMS webes felületet használ a felügyelethez. Néhány alapértelmezett biztonsági beállítás miatt egyes lapok esetleg nem jelennek meg. Az RMS felügyeleti webhelyén néhány lapon előugró ablakokban adhatók meg a konfigurációs beállítások.</p></td>
<td style="border:1px solid black;"><p> </p></td>
</tr>  
</tbody>  
</table>
  
Miután mindkét kiszolgálón végrehajtott minden fenti lépést, készen áll az RMS telepítésére és létesítésére a kiszolgálókon.
