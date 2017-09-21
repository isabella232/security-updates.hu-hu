---
TOCTitle: 'Próbaüzemi RMS-bevezetés áttelepítése éles környezetbe'
Title: 'Próbaüzemi RMS-bevezetés áttelepítése éles környezetbe'
ms:assetid: 'ea151946-22fb-4cba-a3ef-fd7a4bf0d292'
ms:contentKeyID: 18122777
ms:mtpsurl: 'https://technet.microsoft.com/hu-hu/library/Cc747789(v=WS.10)'
---

Próbaüzemi RMS-bevezetés áttelepítése éles környezetbe
======================================================

Számos szervezet először próbaüzemben vezeti be az RMS szolgáltatást, mielőtt azt a teljes szervezetre alkalmazná. A próbaüzemnél általában korlátozva van a felhasználók száma, és a kiszolgálót erre kijelölt rendszergazda felügyeli, azaz az még nem része a vállalati IT-csoporthoz tartozó valamelyik adatközpontnak. Amikor a szervezet a próbaüzem befejezése után az adatközpontban valósítja meg az RMS szolgáltatást az összes ügyfél számára, új RMS kiszolgálók bevezetésére kerül sor a több felhasználó támogatásához.

Az RMS-védelemmel ellátott tartalom azonban a létrehozáskor használt RMS kiszolgálóhoz kötődik, így ha egy kiszolgálót áthelyeznek vagy lecserélnek, megfelelő lépéseket kell végrehajtani, hogy a próbaüzemi RMS kiszolgálókon titkosított tartalmat az éles környezet RMS kiszolgálói vissza tudják fejteni.

Ha az RMS szolgáltatást próbaüzemi környezetben vezette be, és ezt át szeretné helyezni éles környezetbe, a próbaüzem során védett tartalom integritásának megőrzése és a zökkenőmentes áttérés érdekében áttelepítési tervet kell készítenie, amely egyúttal a próbaüzem visszaállításának lehetőségét tartalmazza, ha az adatok helyreállítása válna szükségessé.

A következő lépések példaként szolgálnak, és az áttelepítési terv néhány nélkülözhetetlen elemét mutatják be; a tényleges áttérés egyéb követelményeket is támaszthat.

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
<th>Kiszolgáló</th>
<th>Lépés</th>
<th>Megjegyzések</th>
</tr>
</thead>
<tbody>
<tr class="odd">
<td style="border:1px solid black;"><p>Próbaüzem</p></td>
<td style="border:1px solid black;"><p>Készítse el az RMS konfigurációs adatbázisának biztonsági másolatát.</p></td>
<td style="border:1px solid black;"><p>Ez lehetővé teszi a próbaüzemi kiszolgáló visszaállítását, ha ez szükségessé válik.</p>
<p>A konfigurációs adatbázis tartalmazza az RMS személyes kulcsát.</p>
<p>Ismernie kell a személyes kulcs jelszavát.</p></td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><p>Próbaüzem</p></td>
<td style="border:1px solid black;"><p>Ha hardveres biztonsági modullal (HSM) védte az RMS személyes kulcsát, a gyártó által javasolt módon ennek konfigurációjáról is készítsen biztonsági másolatot.</p></td>
<td style="border:1px solid black;"><p>Az új kiszolgálón a HSM visszaállítására is sor fog kerülni.</p>
<p>Ügyeljen arra, hogy a HSM telepítéséhez és konfigurálásához szükséges valamennyi összetevő rendelkezésre álljon.</p></td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><p>Próbaüzem</p></td>
<td style="border:1px solid black;"><p>Exportálja a megbízható közzétételi tartományhoz tartozó fájlt.</p></td>
<td style="border:1px solid black;"><p>Ez lehetővé teszi más RMS kiszolgálónak az ezzel a kiszolgálóval létrehozott közzétételi licencek visszafejtését, valamint használati licencek kiállítását a védett tartalomhoz.</p>
<p>A megbízható közzétételi tartomány tartalmazza a kiszolgáló licencelői tanúsítványát, az RMS személyes kulcsát és az adott kiszolgálóval készített jogmegadási sablonokat.</p>
<p>A megbízható közzétételi tartományhoz tartozó fájl olyan XML fájl, amely a fájl létrehozásakor megadott nehezen feltörhető jelszóval van titkosítva. Erre a jelszóra szükség lesz a megbízható közzétételi tartományhoz tartozó fájl importálásakor is.</p></td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><p>Próbaüzem</p></td>
<td style="border:1px solid black;"><p>Exportálja a megbízható felhasználói tartományt.</p></td>
<td style="border:1px solid black;"><p>Ez lehetővé teszi más RMS kiszolgálónak használati licencek megadását olyan felhasználóknak, akik a tartalomvédelmi fióktanúsítványt (RAC) a próbaüzemi RMS kiszolgálótól kapták.</p>
<p>A megbízható felhasználói tartomány az adott kiszolgáló kiszolgálói licencelői tanúsítványának a másik RMS kiszolgálóra importálásával létesíthető.</p></td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><p>Éles környezet</p></td>
<td style="border:1px solid black;"><p>Készítse elő az új kiszolgálót a legfelső szintű tanúsítási kiszolgáló szerepre.</p></td>
<td style="border:1px solid black;"><p>Ellenőrizze az adatbázis-kiszolgáló elérhetőségét, valamint az IIS és a Message Queuing szolgáltatás telepítését.</p>
<p>Lehetőség szerint ugyanazt a kiszolgálónevet használja ennél a kiszolgálónál is.</p></td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><p>Éles környezet</p></td>
<td style="border:1px solid black;"><p>HSM használatakor telepítse a HSM modult, és állítsa vissza konfigurációját a próbaüzemi kiszolgálónál létrehozott biztonsági másolatból.</p></td>
<td style="border:1px solid black;"><p>Hozza létre az RMS személyes kulcsának visszafejtéséhez szükséges hitelesítő adatokat.</p></td>
</tr>  
<tr class="odd">
<td style="border:1px solid black;"><p>Éles környezet</p></td>
<td style="border:1px solid black;"><p>Telepítse az RMS rendszert.</p></td>
<td style="border:1px solid black;"><p>Az RMS ellenőrzi az összes szükséges szolgáltatás megfelelő telepítését és konfigurálását.</p></td>
</tr>  
<tr class="even">
<td style="border:1px solid black;"><p>Éles környezet</p></td>
<td style="border:1px solid black;"><p>Új személyes kulcs megadásával létesítsen RMS szolgáltatást. Ha on-line igénylést használ, a létesítési eljárás során az interneten keresztül a Microsoft igénylési szolgáltatásához kapcsolódva megtörténik a kiszolgáló tanúsítványigénylése. Ha a kiszolgálóról nem létesíthető internetkapcsolat, off-line igénylést kell használni.</p></td>
<td style="border:1px solid black;"><p>Ha a kiszolgáló neve nem egyezik meg a próbaüzemi kiszolgáló nevével, a fürt URL-címét a próbaüzemi kiszolgáló URL-címére állíthatja be.</p>
<p>Ha ezt nem hajtja végre, URL-átirányítást kell létesítenie a korábbi fürt URL-címéről az új fürt URL-címére, hogy a már létező tartalomhoz használati licencet szerezhessenek a felhasználók.</p></td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><p>Éles környezet</p></td>
<td style="border:1px solid black;"><p>Kapcsolat nélküli igénylés használatakor hajtsa végre a kézi igénylési eljárást az új RMS kiszolgálóra. A további tudnivalókat lásd a dokumentumgyűjtemény „RMS kiszolgáló működtetése” részében a „Legfelső szintű tanúsítási kiszolgáló kézi igénylése” témakörben.</p></td>
<td style="border:1px solid black;"><p>Az eljárás végrehajtásáig az RMS kiszolgáló nem használható.</p>
<p>Emellett addig az RMS felügyeleti webhely oldalai sem érhetők el.</p></td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><p>Éles környezet</p></td>
<td style="border:1px solid black;"><p>Importálja a 3. lépésben exportált megbízható közzétételi tartományhoz tartozó fájlt.</p></td>
<td style="border:1px solid black;"><p>A fájl sikeres importálásához az RMS-szolgáltatásfióknak olvasási engedéllyel kell rendelkeznie a fájl tárolási helyéhez.</p></td>
</tr>  
<tr class="odd">
<td style="border:1px solid black;"><p>Éles környezet</p></td>
<td style="border:1px solid black;"><p>Írja újból alá a megbízható közzétételi tartománnyal importált sablonokat.</p></td>
<td style="border:1px solid black;"><p>A sablonok aláírása a kiszolgáló személyes kulcsával történik. Mivel a kiszolgáló új személyes kulccsal rendelkezik, az érvényességhez újból alá kell írni a sablonokat. A további tudnivalókat lásd a dokumentumgyűjtemény „RMS kiszolgáló működtetése” részében a „Jogmegadási sablon újbóli aláírása” témakörben.</p></td>
</tr>  
<tr class="even">
<td style="border:1px solid black;"><p>Éles környezet</p></td>
<td style="border:1px solid black;"><p>Ossza ki a sablonokat a próbaüzemben használt ügyfélszámítógépeknek.</p></td>
<td style="border:1px solid black;"><p>A régi sablonokat el kell távolítani, és ezeket az ezzel a kiszolgálóval aláírt sablonokkal kell helyettesíteni.</p></td>
</tr>  
<tr class="odd">
<td style="border:1px solid black;"><p>Éles környezet</p></td>
<td style="border:1px solid black;"><p>Importálja a 4. lépésben exportált megbízható felhasználói tartományt.</p></td>
<td style="border:1px solid black;"><p>Ez lehetővé teszi a régi ügyfél-licencelői tanúsítványok és tartalomvédelmi fióktanúsítványok használatát.</p>
<p>Ha az áttelepítés során felhasználói fiókok erdők közötti áthelyezésére is sor kerül, ügyeljen a fiókok egyező SMTP proxybeállítására.</p></td>
</tr>
</tbody>
</table>
<p> </p>

Az éles környezet kiszolgálójának beállítása után ellenőrizze, hogy a próbaüzem felhasználói használni tudják-e az előzőleg védett levelezést. A szervezetben lévő felhasználók számának megfelelően igény szerint több RMS kiszolgálót is felvehet.
