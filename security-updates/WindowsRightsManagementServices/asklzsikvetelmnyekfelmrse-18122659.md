---
TOCTitle: A skálázási követelmények felmérése
Title: A skálázási követelmények felmérése
ms:assetid: '89f0138c-946d-47d7-a286-041d4d9606a8'
ms:contentKeyID: 18122659
ms:mtpsurl: 'https://technet.microsoft.com/hu-hu/library/Cc747663(v=WS.10)'
---

A skálázási követelmények felmérése
===================================

Amikor arról dönt, hogy egy vagy több kiszolgálót helyezzen-e üzembe, azt kell felmérnie, hogy hány felhasználó fogja igénybe venni az RMS rendszert, és hány fájlt kell védelemmel ellátni.

Ezzel megkapja az átlagos felhasználási igényt. A rendszert a csúcsfelhasználás követelményeire kell méretezni, ami nagyjából az átlagos igény háromszorosát jelenti.

A döntésnél figyelembe kell venni a vállalatnak a hibatűréssel és a szolgáltatások rendelkezésre állásával kapcsolatos előírásait is.

A teljesítmény viszonyítási alapjának megállapításához az RMS rendszert kétprocesszoros, 2,4 GHz-es, 1 GB memóriát tartalmazó Pentium 4 kiszolgálón tesztelték. Ebben a konfigurációban az RMS kiszolgáló másodpercenként körülbelül 50 licencet állított ki.

Az alábbi számadatok segítséget nyújtanak az RMS rendszerrel szembeni felhasználási követelmények megbecsléséhez a kapacitástervezés során.

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
<th>Tranzakció</th>
<th>Előfordulás</th>
<th>Az ügyféltől a kiszolgáló felé irányuló sávszélesség-felhasználás (KB)</th>
<th>A kiszolgálótól az ügyfél felé irányuló sávszélesség-felhasználás (KB)</th>
</tr>
</thead>
<tbody>
<tr class="odd">
<td style="border:1px solid black;"><p>Licenckérelem</p></td>
<td style="border:1px solid black;"><p>Felhasználónként és védeni kívánt anyagonként egyszer</p></td>
<td style="border:1px solid black;"><p>64</p></td>
<td style="border:1px solid black;"><p>18</p></td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><p>Tartalomvédelmi fióktanúsítvány</p></td>
<td style="border:1px solid black;"><p>Csak az RMS inicializálásakor</p></td>
<td style="border:1px solid black;"><p>12</p></td>
<td style="border:1px solid black;"><p>16</p></td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><p>Az ügyfelek igénylési folyamata</p></td>
<td style="border:1px solid black;"><p>Csak az RMS inicializálásakor</p></td>
<td style="border:1px solid black;"><p>17</p></td>
<td style="border:1px solid black;"><p>16</p></td>
</tr>
</tbody>
</table>
  
Ezenkívül az Active Directory-lekérdezésekkel járó forgalom is hatással van a hálózat átbocsátóképességére. Ez azonban általában nem jelentős tényező, ha a globáliskatalógus-kiszolgálók közvetlen közelében telepítik az RMS kiszolgálókat. Ez alól az az eset jelent kivételt, ha adott hely valamennyi globáliskatalógus-kiszolgálója leáll, így feladatátvétellel másik hely kiszolgálóit kell használni olyan kapcsolaton keresztül, amelynek kapacitása nem éri el az előzőét.
  
A következő táblázatban az RMS-tranzakciók sávszélesség-felhasználásra vonatkozó adatai olvashatók, amelyek alapján felmérhető, hogy mekkora hatást fejt ki az Active Directory-lekérdezések forgalma az adott hálózatra.
  
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
<th>Tranzakció</th>
<th>Az RMS szolgáltatástól a globális katalógus felé irányuló sávszélesség-felhasználás (bájt)</th>
<th>A globális katalógus felől az RMS felé irányuló sávszélesség-felhasználás (bájt)</th>
</tr>
</thead>
<tbody>
<tr class="odd">
<td style="border:1px solid black;"><p>Az RMS kapcsolatlétesítése (ldap_bind)</p></td>
<td style="border:1px solid black;"><p>1600</p></td>
<td style="border:1px solid black;"><p>200</p></td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><p>Az RMS csoporttagság-vizsgálata (ldap_search)</p></td>
<td style="border:1px solid black;"><p>200</p></td>
<td style="border:1px solid black;"><p>100</p></td>
</tr>
</tbody>
</table>
  
A táblázatok adatainak használatánál ügyeljen arra, hogy az értékeket az adott bevezetés környezetének megfelelően alkalmazza. Ha például egy felhasználó 15 csoportnak tagja, az RMS keresési kérelme 200 bájtot vesz igénybe, a globális katalógus válasza pedig 1500 (100 x 15) bájtot.
  
A kapacitástervezésnek a várható tartalomlicenc-kérelmek számán kell alapulnia, mivel ezek jelentik az RMS által végrehajtott műveletek túlnyomó többségét. A lemezegység bemeneti/kimeneti sebessége és átbocsátóképessége nem döntő tényező az RMS szempontjából, mivel a licenckérelmek nem tartalmaznak sok adatot, és ezekhez többnyire a gyorsítótár is elegendő.
  
A kiszolgáló átbocsátóképességének legfontosabb változója a processzorterhelés, így döntő jelentősége van a megfelelő processzor kiválasztásának. Az RMS kiszolgálók memóriaigénye a kiszolgálóra háruló terheléssel együtt nő, míg végül meghaladja a kiszolgáló átbocsátóképességét. Amikor ez bekövetkezik, az Internet Information Services (IIS) a memóriában várólistába helyezi a bejövő kérelmeket, amíg a kiszolgáló fel nem tudja dolgozni őket. Az IIS-ben beállítható várólistakorlát elérésekor megszűnik a kérelmek sorba állítása: amikor a várólista eléri a meghatározott maximális méretet, a kiszolgáló elutasítja a kérelmeket.
  
Az RMS adott terhelési mintának megfelelő működéséhez szükséges memóriaigénynek teljes egészében bele kell férnie a fizikai memória méretébe. A memória teljes méretére mindennél nagyobb hatással van a csoportbehelyettesítéshez kapcsolódó gyorsítótárazás. Az RMS szolgáltatást futtató kiszolgálókon legalább 1 GB RAM ajánlott.
  
Adott idő alatt minden RMS kiszolgáló meghatározott számú ügyfélkérelem kezelésére képes (másodpercenként körülbelül 30–50 licenc). Ebből következően a fürtbe tartozó kiszolgálók számának bővülése lineárisan növeli a fürt licenckiállítási kapacitását, valamint fokozza a megbízhatóságot. Így a méretezésnél nemcsak az egyes kiszolgálókra kell figyelemmel lenni, hanem az üzembe helyezett kiszolgálók számára is. A következő konfigurációs példák bemutatják, hogyan használhatók ezek a becsült értékek az RMS bevezetés skálázási követelményeinek kiszámításához.
  
-   Kis terhelésű konfiguráció  
    Vannak szervezetek, amelyeknél az RMS szolgáltatásnak viszonylag kis felhasználási igényt kell kielégítenie. Vegyünk például egy olyan szervezetet, ahol az 5000 felhasználó 10 százaléka használja rendszeresen az RMS szolgáltatást e-mail üzenetek tartalmának védelmére. Becslésként feltehetjük, hogy egy átlagos felhasználó óránként 3 e-mailt lát el védelemmel. Ebből kiindulva az RMS kiszolgálóknak óránként 1500 licencet kell kiállítaniuk, amely másodpercenként 0,42 licencet jelent. Ez az átlagos felhasználási igényt adja meg. Ha ezt megszorozzuk hárommal, megkapjuk a csúcsterhelést, amely másodpercenként 1,26 licenc.  
    Ez viszonylag kis terhelést jelent. Ennél a szervezetnél elég egyetlen RMS kiszolgálót üzembe helyezni.  
-   Közepes terhelésű konfiguráció  
    Sok olyan szervezet van, amelyben viszonylag sok, közepes felhasználási igényű felhasználócsoport található. Vegyünk például egy olyan szervezetet, ahol a 40 000 felhasználó 50 százaléka használja rendszeresen az RMS szolgáltatást tartalomvédelemre. Becslésként feltehetjük, hogy egy átlagos felhasználó óránként 7 e-mailt és 1 dokumentumot vagy más fájlt lát el védelemmel. Ebből kiindulva az RMS kiszolgálóknak óránként 160 000 licencet kell kiállítaniuk, amely másodpercenként 44,4 licencet jelent. Ez az átlagos felhasználási igényt adja meg. Ha ezt megszorozzuk hárommal, megkapjuk a csúcsterhelést, amely másodpercenként 133,2 licenc.  
    Ez az eredmény azt jelenti, hogy a felhasználás mértéke mérsékelten magas, a jelenlegi felhasználói igény kielégítéséhez 3 RMS kiszolgáló elég, 6 RMS kiszolgáló pedig a jelenlegi igények kielégítésén túlmenően a növekedésre is rendelkezik tartalékokkal.  
-   Nagy terhelésű konfiguráció  
    A nagyobb szervezeteknél gyakran előfordul, hogy nagyon sok, nagy felhasználási igényű felhasználócsoport található. Vegyünk például egy olyan szervezetet, ahol a 150 000 felhasználó 70 százaléka használja rendszeresen az RMS szolgáltatást tartalomvédelemre. Becslésként feltehetjük, hogy egy átlagos felhasználó óránként 15 e-mailt és 3 dokumentumot vagy más fájlt lát el védelemmel. Ebből kiindulva az RMS kiszolgálóknak óránként 1 890 000 licencet kell kiállítaniuk, amely másodpercenként 525 licencet jelent. Ez az átlagos felhasználási igényt adja meg. Ha ezt megszorozzuk hárommal, megkapjuk a csúcsterhelést, amely másodpercenként 1575 licenc.  
    Ez az eredmény azt jelenti, hogy a felhasználás mértéke nagyon magas, a jelenlegi felhasználói igény kielégítéséhez 32 RMS kiszolgáló elég, 51 RMS kiszolgáló pedig a jelenlegi igények kielégítésén túlmenően a növekedésre is rendelkezik tartalékokkal.
  
Ha a számítások eredménye másodpercenként 30–50 további licenc kiállítását jelzi, általában újabb RMS kiszolgáló beállítására van szükség.
