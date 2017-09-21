---
TOCTitle: A naplózási adatbázis karbantartása
Title: A naplózási adatbázis karbantartása
ms:assetid: 'de55058b-0d1a-4997-8a45-e14678ddd13f'
ms:contentKeyID: 18122698
ms:mtpsurl: 'https://technet.microsoft.com/hu-hu/library/Cc747691(v=WS.10)'
---

A naplózási adatbázis karbantartása
===================================

A naplóbejegyzések közé tartoznak az RMS különböző műveleteihez (például felhasználói igénylésnél és használati licencek hozzárendelésénél) kiállított licencek másolatai. A legkedvezőtlenebb esetben, amikor minden naplóbejegyzés igénylés sikeres teljesítését vagy használati licenc kiállítását jelenti, az egyes bejegyzések mintegy 200 KB értékkel növelik a naplózási adatbázis méretét.

Példaként tegyük fel, hogy egy RMS-védelemmel ellátott e-mail üzenetet a vállalat összes alkalmazottjának elküldtek, ami 50 000 felhasználót jelent, és mindenki megnyitotta azt. Ha minden alkalmazott egy napon belül nyitotta meg az üzenetet, a naplózási adatbázis mérete 10 GB értékkel nő. A figyelőszolgáltatás beállítható úgy, hogy ne naplózza a tényleges XrML adatokat, így csökkenthető a naplózott adatok mennyisége.

Megfelelő parancsfájl létrehozásával a naplózási adatbázisból a régebbi adatok másodlagos adatbázisba archiválhatók. Az RMS Toolkit példákat tartalmaz a naplózási parancsfájlokra, amelyek ingyenesen letölthetők a [Microsoft webhelyéről](http://go.microsoft.com/fwlink/?linkid=26724) (http://go.microsoft.com/fwlink/?LinkId=26724).

A naplózási adatbázis méretnövekedését befolyásoló tényezők
-----------------------------------------------------------

A naplózási adatbázis méretének becslése a környezettől függ. A napló számos „indítási” bejegyzése előre látható, ilyenek a következők:

-   RMS kiszolgálói igénylés
-   Felhasználói igénylés (az egyes felhasználók által használt számítógépek egyedi kérelme)
-   Automatikus felhasználói kérelmek kapcsolat nélküli közzétételi tanúsítványokra

A kezdeti indítási bejegyzések után a naplózási adatbázis bejegyzéseinek döntő részét a védett tartalomhoz kiállított használati licencek adják. Az adatbázis méretnövekedését számos körülmény befolyásolja:

-   Új licenc kérelmezése a védett tartalom minden elérésénél. A védett dokumentumoknál nem ez az alapértelmezés szerinti módszer, de választható beállítás. Ennek megvalósításakor az adatbázis mérete gyorsabban fog növekedni.
-   Az egyes felhasználóknak naponta küldött védett e-mail üzenetek várható száma.
-   Az ezeket a védett e-mail üzeneteket elolvasó egyedi felhasználók várható száma.
-   A személyenként naponta előállított védett Microsoft Office 2003 (Word, PowerPoint és Excel) dokumentumok várható száma.
-   A védett dokumentumok címzettjeinek várható száma.

A naplózási adatbázis kezdeti mérete mintegy 1,7 MB lesz, amely az RMS kiszolgáló tanúsítási kérelmét tartalmazza. Valahányszor egy új felhasználó igénylésére kerül sor, az új felhasználó tartalomvédelmi fióktanúsítványt (RAC) és ügyfél-licencelői tanúsítvány (CLC) kap. Ez a két művelet a naplóba kerül, ami 0,06 MB méretnövekedést jelent. Amikor egy felhasználó sikeresen licencet szerez védett tartalomhoz, az adatbázis méretnövekedése 0,19 MB.

A becslés működésének érzékeléséhez vegyünk egy 5000 felhasználót tartalmazó szervezetet. Minden felhasználó egy számítógépen dolgozik, és a szervezet két RMS kiszolgálót működtet. A bevezetés után minden felhasználó naponta átlagosan egy, RMS-védelemmel ellátott e-mail üzenetet hoz létre, és azt öt felhasználónak küldi el. Emellett minden felhasználó naponta egy, RMS-védelemmel ellátott dokumentumot is létrehoz, amelyet három felhasználó nyit meg. A következő táblázat azt mutatja be, hogy ezek a tevékenységek várhatóan mennyivel növelik a naplózási adatbázis méretét.

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
<th>Művelet</th>
<th>Méretnövekedés</th>
<th>Halmozott naplóméret</th>
</tr>
</thead>
<tbody>
<tr class="odd">
<td style="border:1px solid black;"><p>RMS kiszolgáló sikeres létesítése</p></td>
<td style="border:1px solid black;"><p>1,7 MB</p></td>
<td style="border:1px solid black;"><p>1,7 MB</p></td>
</tr>  
<tr class="even">
<td style="border:1px solid black;"><p>5000 felhasználói igénylés (5000*0,06)</p></td>
<td style="border:1px solid black;"><p>300 MB</p></td>
<td style="border:1px solid black;"><p>301,7 MB</p></td>
</tr>  
<tr class="odd">
<td style="border:1px solid black;"><p>Hozzáférés védett e-mail üzenetekhez (25000*0,19)</p></td>
<td style="border:1px solid black;"><p>4750 MB</p></td>
<td style="border:1px solid black;"><p>5051,7 MB</p></td>
</tr>  
<tr class="even">
<td style="border:1px solid black;"><p>Hozzáférés védett dokumentumokhoz (15000*0,19)</p></td>
<td style="border:1px solid black;"><p>2850 MB</p></td>
<td style="border:1px solid black;"><p>7901,7 MB</p></td>
</tr>  
</tbody>  
</table>
  
A fentiek szerint az igénylés után a naplózási adatbázis mérete rögzített, ez mintegy 300 MB. A példa szerinti napi növekmény azonban 7,6 GB, amely megközelíti a Message Queuing alapértelmezés szerinti telepítésének 8 GB-os határértékét. Ha a naplózási adatbázis egy napnál hosszabb ideig elérhetetlenné válik, elkezdődhet a naplóbejegyzések elvesztése.
  
A naplózási adatbázis méretének szabályozása  
--------------------------------------------
  
A bevezetési tervnek megfelelő módszert kell tartalmaznia a naplózási adatbázis kezelésére. A leggyakrabban alkalmazott megoldások a következők.
  
-   **Tisztítás és archiválás**  
    Ez a módszer SQL Server parancsfájlok segítségével a bejegyzés létrehozása után adott idővel másodlagos adatbázisba archiválja a naplózási adatbázis kijelölt elemeit. Emellett a módszer kiszűri a felesleges adatokat is, így ezek nem fogják foglalni a helyet.  
-   **A naplózott adatok korlátozása**  
    A naplózási adatbázis három alapvető táblából áll. Ezek egyike a **DRMS\_Log\_Filter**, amely a naplószűrés engedélyezésekor a naplózni kívánt mezőket azonosítja.  
    A be/ki típusú táblabejegyzések megadják, hogy jelenleg mely mezőket naplóz az RMS kiszolgálón futó naplózási figyelőszolgáltatás. Ezek közül két, XrML vonatkozású mező előre tiltva van, mivel a licenckérelmi sorok méretének 99%-át ezek a mezők adják.  
    A **DRMS\_Config\_ServerName\_Port** adatbázis másik, **DRMS\_ClusterPolicies** táblája tartalmazza a **LoggingFiltering** mezőhöz tartozó **PolicyName** értéket. A **LoggingFiltering** (naplószűrés) alapértelmezés szerint nincs engedélyezve. Ha a **LoggingFiltering** értékét 1-re állítja, és újraindítja a naplózási figyelőszolgáltatást, a korábbi példában az adatbázis napi méretnövekedése a 7,6 GB értékről 160 MB-ra csökken.  
-   **A naplózási adatbázis áthelyezése**  
    A naplózási adatbázis méretnövekedésének kezelésére megoldást jelenthet, hogy egyszerűen áthelyezi egy olyan kiszolgálóra, amelyen több szabad lemezterület áll rendelkezésre. A naplózási adatbázis a konfigurációs adatbázisétól eltérő kiszolgálón is elhelyezkedhet. Az adatbázis másik kiszolgálóra való áthelyezése a következő lépésekkel hajtható végre:  
    1.  Állítsa le a naplózási figyelőszolgáltatást mindegyik RMS kiszolgálón.  
    2.  Másolja az adatbázist másik kiszolgálóra (vagy hozzon létre újat).  
    3.  Szerkessze a **DRMS\_Config\_ServerName\_Port** adatbázist: a **DRMS\_ClusterPolicies** táblában adja meg a **LoggingDatabaseName** (naplózási adatbázis neve) és a **LoggingDatabaseServer** (adatbázis-kiszolgáló neve) megfelelő értékét.  
    4.  A parancssorból az IISRESET.exe végrehajtásával indítsa újra az IIS szolgáltatást.
