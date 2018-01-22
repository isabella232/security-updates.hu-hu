---
TOCTitle: A tanúsítási és a licencelési szolgáltatás beállítása az első kiszolgálón
Title: A tanúsítási és a licencelési szolgáltatás beállítása az első kiszolgálón
ms:assetid: 'cce29a2f-984f-48ed-9187-0eb68286ec5b'
ms:contentKeyID: 18122752
ms:mtpsurl: 'https://technet.microsoft.com/hu-hu/library/Cc747756(v=WS.10)'
---

A tanúsítási és a licencelési szolgáltatás beállítása az első kiszolgálón
=========================================================================

Az RMS erőben való kialakításának első lépése egy kiszolgáló telepítése és létesítése. Az első bevezetett kiszolgáló lesz a legfelső szintű tanúsítási kiszolgáló. Ez a kiszolgáló biztosítja a tanúsítás és a licencelés feltételeit, egykiszolgálós konfigurációban önmagában is használható, de lehet a legfelső szintű tanúsítási fürt első kiszolgálója is.

A további RMS kiszolgálók telepítéshez és a létesítéshez szükséges szerepkörök, engedélyek és jogok
---------------------------------------------------------------------------------------------------

Az RMS telepítéséhez helyi rendszergazdai jogokkal rendelkező fiókkal kell bejelentkezni. Emellett egy tartományba is be kell jelentkezni egy érvényes tartományi fiókkal, hogy az Active Directory hitelesíthesse az RMS szolgáltatást. Ha olyan környezetben vezeti be az RMS szolgáltatást, amelyben az Active Directory tartomány működési szintje natív Windows 2000 működési szinten áll, előfordulhat, hogy az RMS nem tudja beolvasni az Active Directory-objektumok memberOf attribútumának értékét, amikor megpróbálja behelyettesíteni a csoportok tagságát. Az RMS akkor tudja olvasni a memberOf attribútumot, ha az RMS szolgáltatásfiókja olyan tartományi fiókot használ, amely tagja az adott erdőben működő, a Windows 2000 előtti rendszerekkel kompatibilis beépített hozzáférési csoportnak. Ha rejtett tagságú csoportokat vezetett be, akkor az RMS szolgáltatásfiókjánál olyan engedélyeket is meg adni, amelyek engedélyezik a rejtett tagság olvasását.

> [!NOTE]  
> Az RMS szolgáltatásfiókja nem egyezhet meg az RMS telepítéséhez használt tartományi fiókkal. 

Az első kiszolgáló telepítésének és létesítésének folyamata
-----------------------------------------------------------

Az RMS kiszolgáló bevezetése két lépésből áll. Először az RMS kiszolgálószoftverét, valamint az összes kiegészítő szoftvert (például IIS, Message Queuing és ASP.NET) kell telepíteni. A további tudnivalókat lásd a dokumentumgyűjtemény „RMS kiszolgáló működtetése” részében „A Service Pack 1 csomaggal frissített RMS telepítése” témakörben.

> [!NOTE]  
> Az RMS telepítése parancssorból is végrehajtható. A további tudnivalókat lásd a dokumentumgyűjtemény „RMS kiszolgáló működtetése” részében „Az RMS telepítése a parancssorból” témakörben. 

Miután telepítette az RMS szolgáltatást egy kiszolgálóra, létesítenie kell a szolgáltatást az adott kiszolgáló egyik webhelyén való használatra. A webhely létesítésekor a webhely számos beállítása módosul, és virtuális könyvtárak jönnek létre. Ezekről a változtatásokról a további tudnivalókat lásd a dokumentumgyűjtemény „RMS műszaki források” részében az „Internet Information Services” témakörben.

Használhatja az IIS alapértelmezett webhelyét, de új webhelyet is létrehozhat. Ha nem az alapértelmezett webhelyen szeretné létesíteni az RMS szolgáltatást, akkor azt a webhelyet még a létesítési folyamat elindítás előtt létre kell hoznia. Ha az alapértelmezett webhelyet más célokra használja, feltétlenül új helyet kell létrehoznia az RMS számára, hogy az alapértelmezett webhely megőrizhesse alapértelmezett konfigurációját.

Amikor a **Start** menü **Windows RMS felügyeleti webhely** parancsát választja, a **Globális felügyelet** lap jelenik meg. Erről az oldalról indítható el valamelyik webhelyen a létesítési folyamat. Az első RMS kiszolgáló létesítéséhez a következő adatokra van szükség:

-   Az RMS konfigurációs, naplózási és címtár-szolgáltatási adatbázis céljára használt adatbázis nevének megadása.
    Ha az SQL Server példányának neve nem egyezik meg a helyi kiszolgáló nevével, akkor azt távoli SQL Server-példányként kell beállítani még abban az esetben is, ha minden ugyanarra a kiszolgálóra van telepítve.
    A létesítés során a jelenleg bejelentkezett felhasználói fióknak engedéllyel kell rendelkeznie adatbázis létrehozására az adatbázis-kiszolgálón.
-   Az RMS szolgáltatásfiókjaként használt fiók megadása. Helyi konfigurációnál használható a Helyi rendszerfiók, ezt azonban nem ajánljuk, mert biztonsági problémákat okozhat, ha egy szolgáltatás a helyi rendszerével egyenértékű engedélyekkel fut.
    Távoli SQL Server példányt vagy egynél több RMS kiszolgálót tartalmazó telepítésnél tartományi fiókot kell megadni. Az erre a célra használt tartományi fióknak Active Directory keresési engedélyekkel kell rendelkeznie. Ezt a fiókot használja a létesítési folyamat az IIS alkalmazáskészlet létrehozására, amely alatt a felügyeleti konzol fut. Ha nem frissítést hajt végre vagy nem létező adatbázist használ, az RMS szolgáltatásfiókjának adatbázis-létrehozási engedélyekkel kell rendelkeznie. Ha létező adatbázisokat használ, a fióknak olvasási és írási engedélyekkel kell rendelkeznie az RMS mindegyik adatbázisához.
-   A webhely elérésére használt URL-cím megadása. Ennek alapértelmezett értéke annak a webhelynek a neve, amelyen a létesítés történik (ha például az IIS alapértelmezett telepítését futtató kiszolgálót létesít, akkor Alapértelmezett webhely). Más webhelyre mutató egyéni URL-címet is megadhat, például terheléselosztó URL-címét, illetve olyat, amely egyaránt lehetővé teszi az intranetes és az internetes elérést. Ellenőriznie kell az egyéni URL működését, és fel kell vennie a webhely nevét a DNS szolgáltatásba, mert a **Globális felügyelet** és a **Létesítés** oldal csak így találja meg a virtuális gyökereket. Ha egy internetről is elérhető telepítés URL-címét adja meg, biztosítsa annak a feltételeit, hogy az új URL-cím az internetről és a vállalati hálózatról egyaránt elérhető legyen.
-   Válassza ki a legfelső szintű telepítés igénylésre használt személyes kulcsának védelmére használt módszert. Az alapértelmezés a szoftveres titkosítás használata, ekkor a titkosított személyes kulcsot az RMS konfigurációs adatbázisa tárolja. Ha az alapértelmezett konfigurációt használja, nehezen feltörhető jelszót kell megadnia az adatbázisban tárolt érték titkosításához.
    Ha viszont a számítógépen hardveres biztonsági modul (HSM) van telepítve és konfigurálva, választhatja a hardveres biztonsági modullal használandó kriptográfiai szolgáltatót (CSP) is. Ekkor a személyes kulcsot hardver, például intelligens kártya tárolja. Az RMS teljes RSA-szolgáltatót igényel, ezért csak az ilyen szolgáltatók szerepelnek a kriptográfiai szolgáltatók listáján. Az RMS személyes kulcsának védelmére kifejezetten javasolt a HSM használata.
    Ha azt választotta, hogy szoftveres kriptográfiai szolgáltatóval, jelszóval védi az RMS személyes kulcsát, azt a jelszót egy jól védett archívumban rögzíteni kell, hogy később megtalálható legyen. A jelszót tároló konfigurációs adatbázis biztonsági másolatát is el kell készíteni. Ezzel az RMS akkor is helyreállítható lesz, ha megsérül az SQL adatbázis. Ha bármilyen okból megváltoztatja a jelszót, készítsen új másolatot az új jelszóval védett kulcsot tartalmazó konfigurációs adatbázisról, és a jelszóval együtt archiválja biztonságos helyen. A konfigurációs adatbázis biztonsági mentéséről és visszaállításáról a további tudnivalókat lásd a dokumentumgyűjtemény „RMS bevezetésének tervezése” részében „Az RMS rendszer biztonsági mentése és visszaállítása” témakörben.
-   A kiszolgálói licencelői tanúsítványon belül használt név megadása. Ez alapértelmezés szerint a kiszolgáló neve.
-   Ha az internet proxykiszolgálón keresztül érhető el, ennek megadása, a címet és a port számát is beleértve.
-   Annak az e-mail címnek a megadása, amelyen a többi RMS rendszergazda kapcsolatba léphet az adott rendszergazdával olyan esetben, amikor problémák adódnak a licenckiszolgálók aligénylésével. Ez a cím a legfelső szintű telepítés létesítése után is módosítható.
-   A kiszolgálói licencelői tanúsítvány visszavonási módszerének kiválasztása. Ez határozza meg, hogy a Microsoft igénylési szolgáltatásán kívül kinek áll jogában visszavonni a legfelső szintű telepítés kiszolgálói licencelői tanúsítványát. Ha külső fél számára is engedélyezni szeretné a visszavonást, meg kell adnia a külső fél nyilvános kulcsát tartalmazó fájl elérési útvonalát és nevét.

Amikor az on-line igénylés választása és az összes beállítás megadása után a **Létesítés** lapon a **Küldés** gombra kattint, az RMS előállít egy kulcspárt, és a nyilvános kulcsot elküldi a Microsoft igénylési szolgáltatásának. (Ha hibaüzenetet kap, ne zárja be a hibaüzenetet megjelenítő oldalt. A hibák kijavítása után a parancssori ablakból az `IISReset` paranccsal állítsa le és indítsa újra az IIS szolgáltatást, térjen vissza az előző képernyőre, adja meg ismét a létesítési adatokat, majd kattintson újból a **Küldés** gombra.) A Microsoft igénylési szolgáltatása létrehoz egy kiszolgálói licencelői tanúsítványt, és néhány percen belül visszaküldi azt a konfigurációs adatbázisba. Mivel ez a tartomány első olyan kiszolgálja, amelyre az RMS telepítve van, a folyamatnak ez a lépése a legfelső szintű tanúsítási kiszolgáló igénylése.

Ha a kapcsolat nélküli (off-line) igénylést választotta, a kiszolgáló igénylését a Microsoft igénylési szolgáltatásánál kézzel hajthatja végre a létesítési folyamat befejezése után. A kiszolgáló csak az igénylési eljárás végrehajtása után használható. A további tudnivalókat lásd a dokumentumgyűjtemény „RMS kiszolgáló működtetése” részében a „Legfelső szintű tanúsítási kiszolgáló kézi igénylése” témakörben.

A kiszolgáló létesítésének és igénylésének befejezése után megváltoznak a **Globális felügyelet** lapon olvasható hivatkozások. Az **RMS létesítése a webhelyen** hivatkozás helyén ekkor **A webhelyen működő RMS felügyelete** hivatkozás jelenik meg, **A kiszolgáló hozzáadása egy fürthöz** hivatkozás helyén **Az RMS szolgáltatásfiókjának módosítása** hivatkozás lesz látható, és a lapon megjelenik **A webhelyen működő RMS eltávolítása** hivatkozás is.

Ez az első kiszolgáló alkotja az RMS legfelső szintű telepítését. A legfelső szintű telepítés állhat egyetlen kiszolgálóból, vagy lehet fürt is. Az első kiszolgáló telepítése és létesítése után további kiszolgálók telepítésével redundancia és terheléselosztás biztosítható a tanúsítási és a licenckiszolgálók számára.

A konfigurálás befejezése után regisztrálni kell a legfelső szintű tanúsítási fürt szolgáltatáskapcsolódási pontját az Active Directoryban, mert az RMS-kompatibilis ügyfelek csak így tudják észlelni a szolgáltatást. A további tudnivalókat lásd a dokumentumgyűjtemény „RMS kiszolgáló működtetése” részében „A szolgáltatás kapcsolódási pontjának regisztrálása” témakörben. Ha nincs regisztrálva a szolgáltatás kapcsolódási pontja, az ügyfél nem lesz használható az RMS szolgáltatással.

> [!IMPORTANT]  
> Csak akkor kezdjen hozzá az RMS további kiszolgálókra telepítéséhez, ha az első kiszolgálón teljesen befejezte az RMS telepítését és létesítését. Az RMS a tartalomvédelmet a több erdőre kiterjedő tagsággal rendelkező Active Directory-csoportoknál is lehetővé teszi. Ha a szervezetben nincs több erdő, illetve több erdőre kiterjedő csoport, az RMS konfigurációs adatbázisában a **MaxCrossForestCalls** fürtszabályzat módosításával optimalizálhatja a használati licencek kiadási eljárásának teljesítményét a kiszolgálón. Ez a szabályzat azt adja meg, hogy egy csoport tagja hányszor léphet át erdők közötti határon. Az alapértelmezett érték 10. A 0 érték beállításához a következő SQL utasítás használható:`update DRMS_ClusterPolicies set PolicyData=0 where PolicyName='MaxCrossForestCalls'` 

A következő témakörök részletesen ismertetik az RMS Globális felügyelet lapján végrehajtható műveletek lépéseit:

-   Az első kiszolgáló telepítésénél a telepítővarázsló használatáról a tudnivalókat lásd a dokumentumgyűjtemény „RMS kiszolgáló működtetése” részében „A Service Pack 1 csomaggal frissített RMS telepítése“ témakörben.
-   Az első kiszolgáló létesítéséről a tudnivalókat lásd a dokumentumgyűjtemény „RMS kiszolgáló működtetése” részében „Az első legfelső szintű tanúsítási kiszolgáló létesítése” témakörben.
-   A legfelső szintű telepítésbe kiszolgálók felvételével létrehozható fürtökről a tudnivalókat ebben a témakörben „[A tanúsítást és a licencelést biztosító kiszolgálók hozzáadása](https://technet.microsoft.com/089ceb62-2a96-444f-ab42-1d5deaabd0c3)” pontban találja.
