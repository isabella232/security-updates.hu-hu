---
TOCTitle: 'A bevezetés frissítése az RMS Service Pack 2 (SP2) csomaggal'
Title: 'A bevezetés frissítése az RMS Service Pack 2 (SP2) csomaggal'
ms:assetid: '27ee06a1-f467-4a6c-b662-45ddb5f8c13e'
ms:contentKeyID: 18122520
ms:mtpsurl: 'https://technet.microsoft.com/hu-hu/library/Cc720225(v=WS.10)'
---

A bevezetés frissítése az RMS Service Pack 2 (SP2) csomaggal
============================================================

Ez a rész a Microsoft® Windows® tartalomvédelmi szolgáltatások (RMS) Service Pack 2 (SP2) javítócsomag telepítéséhez nyújt segítséget a meglévő RMS rendszerrel rendelkező szervezeteknek. Csak azoknak a szervezeteknek szükséges végrehajtaniuk az RMS SP2 frissítést, amelyek már üzembe helyezték az RMS szolgáltatást. Azok a szervezetek, amelyek első alkalommal helyezik üzembe az RMS rendszert, a dokumentumgyűjtemény „RMS bevezetésének tervezése” ([http://go.microsoft.com/fwlink/?LinkId=74999](http://go.microsoft.com/fwlink/?linkid=74999)) és „RMS rendszer bevezetése” ([http://go.microsoft.com/fwlink/?LinkID=75000](http://go.microsoft.com/fwlink/?linkid=75000)) című részében megadott útmutatás szerint közvetlenül az RMS SP2 telepítését hajthatják végre.

Az RMS SP2 az RMS SP1 meglévő telepítésének eltávolítása nélkül telepíthető. Az RMS SP2 telepítőprogramja érzékeli az RMS SP1 telepítését, és szükség szerint felveszi a további szolgáltatásokat és beállításokat.

| ![](images/Cc720225.note(WS.10).gif)Megjegyzés:                                                                                                                                                                                                             |
|------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| Javítócsomag nélküli RMS-kiszolgálóról nem hajthatja végre az RMS SP2 verzióra való frissítést. Ha javítócsomag nélküli RMS-kiszolgálót használ, az RMS SP2 verzióra való frissítés előtt az RMS SP1 frissítést kell alkalmaznia. Az RMS-ügyfél tetszőleges előző verzióról frissíthető. |

**A témakör tartalma**

-   [Az RMS SP2 frissítés előkészítése](#bkmk_preparingforsp2update)
-   [Az RMS SP2 frissítés végrehajtása](#bkmk_performingsp2update)
-   [Fürtök frissítése](#bkmk_updateclusters)
-   [RMS-ügyfelek frissítése](#bkmk_updateclients)
-   [Együttműködés az RMS 1.0-s verziójával](#bkmk_interop)
-   [Az RMS SP2 eltávolítása](#bkmk_removingrms)

<span id="bkmk_PreparingForSP2Update"></span>
Az RMS SP2 frissítés előkészítése
---------------------------------

Az RMS SP2 frissítés kialakítása olyan, hogy megszakítás nélkül lehetővé teszi az RMS folyamatos működését. Az RMS fürtjének frissítése előtt azonban javasolt a következő műveletek végrehajtása:

-   Készítsen biztonsági másolatot a konfigurációs adatbázisról és az RMS titkos kulcsáról. A további tudnivalókat lásd a dokumentumgyűjteményben az RMS rendszer biztonsági mentésével foglalkozó témakört ([http://go.microsoft.com/fwlink/?LinkId=75001](http://go.microsoft.com/fwlink/?linkid=75001)).
-   Ha szoftver alapú titkos kulcsot használ, ügyeljen arra, hogy rendelkezzen az RMS titkos kulcsának jelszavával.
-   Készítsen biztonsági másolatot a naplózási adatbázisról, ha meg kívánja tartani a korábban rögzített statisztikai adatokat.
-   Ellenőrizze, hogy az ügyfélszámítógépeken és a kiszolgálókon telepítette az operációs rendszer legújabb fontos és biztonsági frissítéseit. Ehhez kattintson a **Start** gombra, válassza a **Windows Update** parancsot, és kövesse a képernyőn megjelenő utasításokat.

<span id="bkmk_PerformingSP2Update"></span>
Az RMS SP2 frissítés végrehajtása
---------------------------------

Amikor a Windows Rights Management Services Service Pack 2 érzékeli az RMS telepítését, a meglévő RMS SP1 alapján csak az új fájlokat veszi fel, illetve az RMS SP2 számára módosításra szorulókat cseréli le. Ha korábban már sikeresen futtatta az RMS rendszert, nem kell azt újból létesítenie, és további konfigurációs lépésekre sincs szükség az RMS SP2 telepítése után az RMS működésének folytatásához.

<span id="bkmk_UpdateClusters"></span>
Fürtök frissítése
-----------------

Ha az RMS telepítése fürtkonfigurációba történt, meg kell terveznie a fürtök frissítését, hogy a lehető legkisebb legyen a frissítés hatása a meglévő telepítésre. Érdemes megfontolni a következő ajánlásokat, amikor az RMS SP2 megvalósításának a szervezethez illeszkedő legjobb módszeréről dönt:

-   Gyakorlati tanács: az RMS SP2 telepítését egyidejűleg csak a fürt egy részén hajtsa végre, így a fürt frissítése jobban kézben tartható, és csökken a szolgáltatás teljesítménycsökkenésének valószínűsége a frissítés során.
-   Ha több RMS fürttel rendelkezik, először a legfelső szintű tanúsítási fürtöket kell frissíteni, majd ezután az aligényléssel létesített licencelési fürtöket.
-   Ha erdők közötti csoportbővítést használ, az erdőkben lévő fürtöket egymástól függetlenül frissítheti, és ez nem fogja korlátozni az RMS kiszolgálókat az erdők közötti csoporttagság bővítésében.
-   Az RMS SP2, RMS SP1 és az RMS 1.0-s verziójú kiszolgálója csak az Active Directory különböző erdőiben futva működhet együtt. Nem javasolt, hogy az RMS-kiszolgáló különböző verziói fussanak ugyanazon a fürtön.
-   Az RMS SP2 telepítőcsomagjával az RMS SP2 új üzembe helyezése is megvalósítható egy kiszolgálón, ehhez nincs szükség az RMS SP1 előzetes telepítésére.

<span id="bkmk_UpdateClients"></span>
RMS-ügyfelek frissítése
-----------------------

Az új RMS SP2 ügyfélszoftver elérhető a Windows Update paranccsal vagy a Microsoft letöltőközpontjából. Az RMS SP2 ügyféltelepítő csomagjával az RMS SP2 ügyfél új verziója telepíthető egy számítógépen, ehhez nincs szükség az RMS 1.0-s verziójú ügyfélszoftver előzetes telepítésére. Az RMS SP2 ügyfélszoftver visszafelé kompatibilis szolgáltatása lehetővé teszi az olyan RMS-kompatibilis alkalmazások használatát, amelyek az RMS 1.0-s verzióját igénylik.

Az RMS ügyfélszoftver frissítéséről és telepítéséről a további tudnivalókat lásd: Az RMS ügyfélszoftver terjesztése ([http://go.microsoft.com/fwlink/?LinkId=75070](http://go.microsoft.com/fwlink/?linkid=75070)).

<span id="bkmk_InterOp"></span>
Együttműködés az RMS 1.0-s verziójával
--------------------------------------

Mivel az RMS SP2 számos javítást és teljesítménynövelő továbbfejlesztést tartalmaz, a következő frissítési ciklus során mindenképpen érdemes telepíteni. Bár az RMS SP2 csomagot futtató kiszolgálók és ügyfelek tökéletesen együttműködnek az RMS SP2 javítócsomagot nem tartalmazó kiszolgálókkal és ügyfelekkel, tisztában kell lennie a vegyes környezetben előforduló következő működési különbségekkel:

-   Csak az RMS SP1 vagy újabb rendszert futtató kiszolgálók képesek a kapcsolat nélküli beiktatásra.
-   Csak az RMS SP1 vagy újabb rendszert futtató ügyfelek önaktiválóak..
-   A következő táblázat a vegyes környezetekben támogatott funkciókat mutatja be:

###  

<p> </p>
<table style="border:1px solid black;">
<colgroup>
<col width="25%" />
<col width="25%" />
<col width="25%" />
<col width="25%" />
</colgroup>
<thead>
<tr class="header">
<th>RMS kiszolgáló verziója</th>
<th>Az 1.0-s verziójú ügyfeleknél használható szolgáltatások</th>
<th>Az SP2 ügyfeleknél használható szolgáltatások</th>
<th>A vegyes ügyfelű környezetekben használható szolgáltatások</th>
</tr>
</thead>
<tbody>
<tr class="odd">
<td style="border:1px solid black;"><p>1.0</p></td>
<td style="border:1px solid black;"><p>Valamennyi előző szolgáltatás.</p>
<p>A kiszolgáló kapcsolat nélküli beiktatása nem lehetséges. A kiszolgálót az interneten keresztül kell beiktatni.</p>
<p>Nem önaktiváló ügyfelek.</p></td>
<td style="border:1px solid black;"><p>Valamennyi előző szolgáltatás.</p>
<p>A kiszolgáló kapcsolat nélküli beiktatása nem lehetséges.</p>
<p>Önaktiváló ügyfelek.</p></td>
<td style="border:1px solid black;"><p>Valamennyi előző szolgáltatás.</p>
<p>SP2 ügyfeleknél ezek önaktiválóak.</p>
<p>1.0-s ügyfeleknél ezeket az interneten keresztül kell aktiválni.</p></td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><p>SP2</p></td>
<td style="border:1px solid black;"><p>Valamennyi előző szolgáltatás.</p>
<p>Kiszolgáló kapcsolat nélküli beiktatása.</p>
<p>Nem önaktiváló ügyfelek.</p></td>
<td style="border:1px solid black;"><p>Valamennyi SP1 szolgáltatás.</p>
<p>Kiszolgáló kapcsolat nélküli beiktatása.</p>  
<p>Önaktiváló ügyfelek.</p>  
<p>Kiszolgálói kulcstároló.</p>
<p>A Microsoft SQL Server™ 2005 közvetlen támogatása.</p></td>
<td style="border:1px solid black;"><p>Valamennyi előző szolgáltatás az SP2 szolgáltatásaival kiegészítve.</p>
<p>Kiszolgáló kapcsolat nélküli beiktatása.</p>  
<p>SP2 ügyfeleknél ezek önaktiválóak.</p>
<p>1.0-s ügyfeleknél ezeket az interneten keresztül kell aktiválni.</p></td>
</tr>
</tbody>
</table>
<p> </p>

<span id="bkmk_RemovingRMS"></span>
Az RMS SP2 eltávolítása
-----------------------

Ha az RMS SP2 telepítése után az RMS kiszolgálóját a korábbi állapotába szeretné visszaállítani, a **Programok telepítése és törlése** segédprogramot használhatja a **Vezérlőpulton** az RMS SP2 eltávolításához.
