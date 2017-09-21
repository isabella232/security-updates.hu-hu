---
TOCTitle: Az RMS üzembe helyezésével kapcsolatos kérdések
Title: Az RMS üzembe helyezésével kapcsolatos kérdések
ms:assetid: '5559ae65-77ae-4e0b-bfd8-3512409ed29b'
ms:contentKeyID: 18122497
ms:mtpsurl: 'https://technet.microsoft.com/hu-hu/library/Cc720274(v=WS.10)'
---

Az RMS üzembe helyezésével kapcsolatos kérdések
===============================================

Az RMS üzembe helyezésével kapcsolatos kérdések
-----------------------------------------------

-   [Van-e valamilyen előírás az Exchange verziójára, ha az RMS rendszerhez használt biztonsági hitelesítő adatok globális címlisták?](#bkmk_20)
-   [Mi az SQL Server szerepe az RMS rendszerben?](#bkmk_21)
-   [Az RMS használatához a legfelső szintű fürtjével megegyező tartományhoz kell-e kapcsolni a felhasználó számítógépét?](#bkmk_22)
-   [Ha egy felhasználó szegélyhálózatban kívánja elhelyezni az RMS kiszolgálót, az ezzel való kommunikációhoz mely portoknak kell megnyitva lenniük az internet, illetve az intranet felé néző tűzfalon?](#bkmk_23)
-   [Hogyan történik az alsóbb szintű licenckiszolgálók igénylése csak licencelésre szolgáló fürtben, és van-e valamilyen teendő az ügyfelekkel, hogy tudomást szerezzenek az alsóbb szintű licenckiszolgálókról?](#bkmk_24)
-   [Mi az előnye a csak licencelésre szolgáló fürt használatának?](#bkmk_25)
-   [Hogyan távolítható el teljesen az RMS telepítése?](#bkmk_26)
-   [Miután eltávolítottam az RMS rendszert a Programok telepítése és törlése segédprogrammal, szükség van-e további fájlok törlésére?](#bkmk_27)
-   [Használható-e az RMS FAT fájlrendszerrel?](#bkmk_28)
-   [Milyen jellemző hardverkonfiguráció javasolt az RMS adatbázis-kiszolgálójánál?](#bkmk_29)
-   [Milyen hatással van a csoportbehelyettesítésnél a globális katalógus használata a globáliskatalógus-kiszolgáló teljesítményére?](#bkmk_30)
-   [Szükséges-e módosítani a sémákat az Active Directory címtárban az RMS működéséhez?](#bkmk_31)
-   [Átkerül-e automatikusan a szolgáltatás kapcsolódási pontja (SCP) az RMS fürt telepítési tartományának különböző tartományvezérlőire?](#bkmk_32)
-   [Hogyan telepíthető és konfigurálható az RMS ügyfélszoftvere, ha a felhasználók nem rendelkeznek rendszergazdai jogokkal?](#bkmk_33)
-   [Mit jelen az RMS skálázhatósága?](#bkmk_35)
-   [Használhatók-e az RMS rendszerben hardveres biztonsági modulok (HSM) az RMS kulcsainak védelméhez?](#bkmk_36)

<span id="BKMK_20"></span>
#### Van-e valamilyen előírás az Exchange verziójára, ha az RMS rendszerhez használt biztonsági hitelesítő adatok globális címlisták?

Az RMS az Active Directory szolgáltatástól függ, az Exchange rendszertől nem. Az Exchange 5.5-ös verziója azonban saját címtárat tart fenn, és nem használja az Active Directoryt. Ügyeljen arra, hogy az Active Directory valamennyi felhasználó- és csoportobjektuma érvényes e-mail attribútummal rendelkezzen, amely tartalmazza a teljesen megadott tartománynevet. Ez automatikusan megtörténik az Exchange 2000 vagy újabb verzió használatakor.

<span id="BKMK_21"></span>
#### Mi az SQL Server szerepe az RMS rendszerben?

Az RMS adatbázist használ a szolgáltatás következő adatainak tárolásához: valamennyi konfigurációs adat, a rendszer résztvevőire vonatkozó adatok, az összes naplózási adat és az Active Directory-gyorsítótár. Az RMS rendszert teljes körűen tesztelték az SQL Server 2000 és az SQL Server 2005 kiszolgálóval.

<span id="BKMK_22"></span>
#### Az RMS használatához a legfelső szintű fürtjével megegyező tartományhoz kell-e kapcsolni a felhasználó számítógépét?

Nem szükséges, hogy a felhasználó számítógépe az RMS fürtjével azonos tartomány tagja legyen, de a számítógépnek meg kell tudni találnia az RMS fürtöt. Ennek legegyszerűbb módja az Active Directory lekérdezése szolgáltatáskapcsolódási ponton (SCP) keresztül. Emellett az ügyfélgép rendszerleíró beállításaival is megadható az RMS fürt helye, így nincs szükség az Active Directory használatára. A pontos beállítások az RMS-kompatibilis alkalmazástól függően változnak.

<span id="BKMK_23"></span>
#### Ha egy felhasználó szegélyhálózatban kívánja elhelyezni az RMS kiszolgálót, az ezzel való kommunikációhoz mely portoknak kell megnyitva lenniük az internet, illetve az intranet felé néző tűzfalon?

A belső felhasználóknak el kell érniük az RMS kiszolgálókat, amelyek tartalomvédelmi fióktanúsítványokat (RAC) és használati licenceket állítanak ki. Az RMS kiszolgáló alapértelmezés szerint a HTTP (80-as TCP port) vagy a HTTPS (443-as TCP port) protokollt figyeli attól függően, hogy be van-e állítva az SSL használata, így ezeknek a portoknak kell megnyitva lenniük az internet felé néző tűzfalon. A tartomány tagkiszolgálóihoz további portok megnyitására is szükség lehet az intranet felé néző tűzfalon.

<span id="BKMK_24"></span>
#### Hogyan történik az alsóbb szintű licenckiszolgálók igénylése csak licencelésre szolgáló fürtben, és van-e valamilyen teendő az ügyfelekkel, hogy tudomást szerezzenek az alsóbb szintű licenckiszolgálókról?

A legfelső szintű fürtön a vállalat első RMS kiszolgálójának létrehozásakor ez kiszolgálói licencelői tanúsítványt szerez a Microsoft igénylési szolgáltatásától. További RMS kiszolgáló telepítésekor és létesítésekor azt a legfelső szintű fürthöz kapcsolhatja, vagy alsóbb szintű kiszolgálóként igényelheti egy csak licencelésre szolgáló fürtön. Utóbbi esetben a kiszolgáló igénylési kérelmet küld az RMS legfelső szintű fürtjébe. Az RMS-kompatibilis alkalmazások adják meg, hogy az ügyfélalkalmazás hol keresi a csak licencelésre szolgáló fürtöt. Az Office 2003 például RMS-kompatibilis alkalmazás, amely alapértelmezés szerint a legfelső szintű fürtöt várja. Ez a rendszerleíró bejegyzésekkel felülírható, így az alkalmazás keresni fogja az új, alsóbb szintű, csak licencelésre szolgáló fürtöt.

<span id="BKMK_25"></span>
#### Mi az előnye az alsóbb szintű, csak licencelésre szolgáló fürt használatának?

Az egyik előny, hogy így elkülöníthetők a szervezeten belüli részlegek. Ha az RMS fürtök között nincs kialakítva megbízható közzétételi tartomány, a tartalmat csak adott licenckiszolgálót elérők használhatják. Ily módon például a jogi osztály mindenki mást kizárhat titkosított e-mail üzeneteinek olvasásából. Emellett számos egyéb beállítás is megadható a csak licencelésre szolgáló fürtön, például jogmegadási sablonok, naplózás, felügyelői csoporttagság és kizárási szabályzatok.

<span id="BKMK_26"></span>
#### Hogyan távolítható el teljesen az RMS telepítése?

A teljes eltávolítás a következő lépések végrehajtásával történhet.

**Az RMS telepítésének eltávolítása**
1.  Az RMS felügyeleti webhelyén távolítsa el az RMS fürt szolgáltatáskapcsolódási pontját (SCP).

2.  A kiszolgálón lévő RMS megszüntetéséhez a **Globális felügyelet** lapon kattintson **A webhelyen működő RMS eltávolítása** hivatkozásra. Először a csak licencelésre szolgáló fürtökön aligényléssel létesített kiszolgálókat kell megszüntetni, és ezután következhetnek a legfelső szintű fürt kiszolgálói.

3.  A **Vezérlőpulton** a **Programok telepítése és törlése** segédprogrammal távolítsa el a **Tartalomvédelmi szolgáltatások** rendszert.

4.  Az adatbázis-kiszolgálón távolítsa el az RMS még fellelhető adatbázisait.

5.  Az adatbázis-kiszolgálón távolítsa el az RMS szolgáltatásfiókját a jogosult bejelentkezők listájáról, majd távolítsa el magát a fiókot az Active Directoryból.

6.  Ha az RMS ügyfeleken Windows XP vagy Windows 2000 operációs rendszer fut, az ügyfélszámítógépeken távolítsa el az RMS ügyfélszoftverét.

| ![](images/Cc720274.Important(WS.10).gif)Fontos:                                                                                                                                                 |
|-------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| Az eljárás végrehajtása után többé nem fog tudni tartalomvédelemmel ellátott dokumentumot megnyitni. A teljes eltávolítása előtt az RMS leszerelésére van szükség, ha az RMS rendszerrel értékes adatok védelmére került sor. |

<span id="BKMK_27"></span>
#### Miután eltávolítottam az RMS rendszert a Programok telepítése és törlése segédprogrammal, szükség van-e további fájlok törlésére?

Bár ez nem szükséges, de törölheti a kulcstárolót a %rendszergyökér%\\system32 útvonalon.

<span id="BKMK_28"></span>
#### Használható-e az RMS FAT fájlrendszerrel?

Igen, az RMS működőképes FAT fájlrendszert használó számítógépeken is, bár az NTFS fájlrendszer ajánlott.

<span id="BKMK_29"></span>
#### Milyen jellemző hardverkonfiguráció javasolt az RMS adatbázis-kiszolgálójánál?

A naplózási adatbázis mérete gyorsan növekszik, különösen olyan környezetekben, ahol jelentős az RMS használata. Ha adatbázis-kiszolgálóként SQL Server kiszolgálót kíván használni, Windows 2000 Advanced Server rendszeren az SQL Server 2000 Enterprise Edition vagy az SQL Server 2005 Enterprise Edition választható, illetve a Windows Server 2003 Enterprise Edition használható aktív-készenléti konfigurációban egy fürtben. Ebben az esetben a javasolt kiépítés: RAID-1 naplózási lemezek és a RAID-5 adatlemezek, valamint legalább 512 MB memória. A processzor legalább 1,4 GHz-es Pentium III legyen. A célra rendelt adatbázis-kiszolgálókon nem követelmény a többprocesszoros kialakítás.

<span id="BKMK_30"></span>
#### Milyen hatással van a csoportbehelyettesítésnél a globális katalógus használata a globáliskatalógus-kiszolgáló teljesítményére?

Az RMS kiszolgálója a csoportbehelyettesítési listákat gyorsítótárba helyezi, így ez nem jelenthet nagyobb terhelést a globáliskatalógus-kiszolgálóra. A csoporttagság gyakori frissítése növeli a globáliskatalógus-kiszolgáló igénybevételét, de az új csoportlisták beszerzésének időtúllépése rendszerleíró beállításban megadható. Nagy csoportok gyakori behelyettesítése csökkenti a teljesítményt. A további tudnivalókat lásd a dokumentumgyűjtemény „RMS kiszolgáló működtetése” részében „Az Active Directory-gyorsítótár beállításainak módosítása” témakörben.

<span id="BKMK_31"></span>
#### Szükséges-e módosítani a sémákat az Active Directory címtárban az RMS működéséhez?

Az RMS csak abban az esetben tudja behelyettesíteni közzétételi licencben megadott csoport tagságát a másik erdőből, ha egy, a távoli erdőben lévő csoportot leképező kapcsolatobjektum létezik a helyi Active Directory-erdőben. Az RMS ebben az esetben le tudja kérdezni a kapcsolatobjektum attribútumait, és így észlelheti, hogy az objektum egy másik erdőben található csoportot képvisel.

Ennek végrehajtásához az Active Directoryban szükség van a Microsoft Exchange Server 2003 vagy újabb verzió msExchOriginatingForest sémaattribútumára. Ez az attribútum alapértelmezés szerint települ az Active Directory sémájába, ha az erdőben van az Exchange Server 2003 rendszert futtató kiszolgáló. Az attribútumra minden olyan Active Directory-séma erdejében szükség van, amely részt fog venni az RMS szolgáltatásban. Ha nem használja az Exchange Server 2003 kiszolgálót, külön is telepítheti a sémát az Active Directory szerkezetébe az RMS felügyeleti eszközkészletével.

<span id="BKMK_32"></span>
#### Átkerül-e automatikusan a szolgáltatás kapcsolódási pontja (SCP) az RMS kiszolgáló telepítési tartományának különböző tartományvezérlőire?

Adott erdő első RMS kiszolgálójának létesítése után be kell azt jegyezni az Active Directoryba olyan tartományi fiók használatával, amelynek engedélyei lehetővé teszik tárolóobjektum létrehozását az Active Directory-erdő Configuration tárolójában lévő Services tároló alatt. A beépített Vállalati rendszergazdák biztonsági csoport például olyan fiók, amely rendelkezik a szükséges engedélyekkel. Ez létrehozza a szolgáltatás kapcsolódási pontját (SCP). Mivel ez a Services tárolóban található, az Active Directory replikálja ezt a beállítást az erdő valamennyi tartományvezérlőjére.

<span id="BKMK_33"></span>
#### Hogyan telepíthető és konfigurálható az RMS ügyfélszoftvere, ha a felhasználók nem rendelkeznek rendszergazdai jogokkal?

Az RMS ügyfélszoftvere egy Windows Installer fájl, és bevezetéséhez szoftverterjesztési infrastruktúra használható, ilyen például a Systems Management Server 2003. Az RMS ügyfélszoftverének terjesztése megoldható egy csoportházirend-objektummal (GPO) is, amely rendszergazdai jogokkal rendelkező szolgáltatásfiókot használ. Ha az RMS ügyfél operációs rendszere a Windows Vista, az RMS ügyfélszoftverének külön telepítésére nincs szükség, mivel az az operációs rendszer beépített része.

<span id="BKMK_35"></span>
#### Mit jelen az RMS skálázhatósága?

Az RMS helyhez nem kötött webszolgáltatás, így a többi webhelyhez vagy webszolgáltatáshoz hasonlóan megoldható a fürtözés és a terheléselosztás. Az RMS teljesítményét leginkább a processzor rendelkezésre állása határozza meg, így processzorok felvételével javítható a teljesítmény.

<span id="BKMK_36"></span>
#### Használhatók-e az RMS rendszerben hardveres biztonsági modulok (HSM) az RMS kulcsainak védelméhez?

Igen, az RMS együttműködik a CAPI-kompatibilis hardveres biztonsági modulokkal, ilyen például az nCipher.
