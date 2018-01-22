---
TOCTitle: Az RMS felügyeletével kapcsolatos problémák
Title: Az RMS felügyeletével kapcsolatos problémák
ms:assetid: '97013c08-d3fa-4ea0-8914-995b6c97f900'
ms:contentKeyID: 18122595
ms:mtpsurl: 'https://technet.microsoft.com/hu-hu/library/Cc747605(v=WS.10)'
---

Az RMS felügyeletével kapcsolatos problémák
===========================================

Az RMS szolgáltatás sikeres létesítése után a napi felügyelet során problémák is előfordulhatnak. Az itt következő szakaszok ezek megoldásához nyújtanak segítséget.

Az „SQL Server does not exist or access denied” (SQL Server nem létezik, vagy a hozzáférés megtagadva) üzenet érkezett az RMS felügyeleti webhelyének megnyitási kísérletekor.
------------------------------------------------------------------------------------------------------------------------------------------------------------------------------

Ha az RMS telepítéséhez adatbázis-kiszolgálóként az SQL Server 2005 új telepítését használta, valószínűleg nem indult el az SQL Server szolgáltatás. Az SQL Server 2005 rendszerben az MSSQLSERVER szolgáltatás nincs automatikus indításra beállítva a kiszolgáló indításakor. Ha az RMS telepítése óta újraindította az SQL Server rendszert, és nem állította be a szolgáltatás automatikus újraindítását, az RMS működésképtelen lesz, és csak az RMS Globális felügyeleti lapja lesz elérhető.

Az MSSQLSERVER elindítása után az RMS működőképességének helyreállításához újra kell indítani az IIS szolgáltatást az RMS kiszolgálón.

Nem hajtható végre a kapcsolat nélküli igénylés eljárása
--------------------------------------------------------

Ha az igénylési kérelmet tartalmazó fájl hiányos, vagy az EnrollService webhelyre való elküldése előtt módosították, nem hajtható végre a kapcsolat nélküli igénylés. Vélhetőleg megsérült az igénylési kérelmet tartalmazó fájl, ennek oka rosszindulatú program, felhasználói vagy rendszerhiba lehet.

A hiányzó adatoktól függően az EnrollService webhely elfogadhatja a fájlt, és kiszolgálói licencelői tanúsítványt küldhet, illetve elutasíthatja a kérelem elfogadását, és hibaüzenetet jeleníthet meg.

Ha kiszolgálói licencelői tanúsítvány érkezett, az az igénylési kérelmet tartalmazó fájl hiányosságainak vagy sérülésének megfelelő lesz, és az RMS hibaüzenetet jelenít meg, amikor a tanúsítvány importálását kísérli meg.

Ha nem tudja végrehajtani az igénylési eljárást, ellenőrizze az internetkapcsolattal rendelkező számítógép vírusmentességét, exportálja újra az igénylési kérelmet tartalmazó fájlt az RMS kiszolgálóról, és más adathordozón vigye át az internetkapcsolattal rendelkező számítógépre. Ha a hiba újból jelentkezik, forduljon a Microsoft terméktámogató szolgáltatásához.

Nem jönnek létre a naplófájlok
------------------------------

Az RMS naplózási szolgáltatásának működéséhez a Message Queuing (más néven MSMQ) szolgáltatásra és a naplózási adatbázis elérésére van szükség. Ha nem jönnek létre a naplófájlok, akkor valószínűleg nem megfelelően lettek konfigurálva az összetevők, vagy megszakadt közöttük a kommunikáció.

Ellenőrizze az RMS kiszolgáló és az adatbázis-kiszolgáló hálózati kapcsolatát. Ha ez megfelelő, a következő lépésekkel tekintse át az RMS naplózási szolgáltatásának előfeltételeit, és ellenőrizze a szükséges szoftverek megfelelő konfigurálását.

Elsőként ellenőrizze a Message Queuing konfigurálásának helyességét. A Message Queuing telepítésénél engedélyezni kell az Active Directory-integrációt.

**A Message Queuing telepítésének és konfigurálásának ellenőrzése**
1.  A **Vezérlőpulton** kattintson a **Programok telepítése és törlése** ikonra, majd a **Windows-összetevők hozzáadása vagy eltávolítása** ikonra: ekkor a **Windows-összetevők varázsló** jelenik meg.

2.  A **Windows-összetevők varázslóban** jelölje be az **Alkalmazáskiszolgáló** négyzetet, majd kattintson a **Részletek** gombra.

3.  Jelölje be az **Üzenetsor-kezelés** négyzetet, majd kattintson a **Részletek** gombra.

4.  Ha az **Active Directory-integráció** négyzet be van jelölve, térjen át a következő vizsgálatra, amely a Message Queuing futását ellenőrzi. Ha a négyzet nincs bejelölve, folytassa az 5–9. lépés végrehajtásával.

5.  Kattintson a **Start** gombra, és válassza a **Minden program**, a **Windows RMS**, végül a **Windows RMS felügyeleti webhely** parancsot. Ekkor a Globális felügyelet lap jelenik meg.

6.  Keresse meg azt a webhelyet, amelyen létesítve van az RMS, és kattintson a mellette látható **A webhelyen működő RMS eltávolítása** hivatkozásra, majd az **OK** gombra.

7.  A **Programok telepítése és törlése** párbeszédpanelen (**Vezérlőpult**) kattintson a **Windows-összetevők hozzáadása vagy eltávolítása** gombra, az **Alkalmazáskiszolgáló**, majd az **Üzenetsor-kezelés** elemre.

8.  Az **Active Directory-integráció** engedélyezéséhez kattintson a **Részletek** gombra, jelölje be az **Active Directory-integráció** négyzetet, majd kattintson az **OK** gombra.

9.  Nyissa meg a **Globális felügyelet** oldalt. Keresse meg azt a webhelyet, amelyen létesíteni szeretné az RMS szolgáltatást, majd kattintson a mellette látható **RMS létesítése a webhelyen** hivatkozásra.

Második feladatként ellenőrizze, hogy fut-e a Message Queuing szolgáltatás a kiszolgálón.

**A Message Queuing futásának ellenőrzése a kiszolgálón**
1.  Kattintson a **Vezérlőpulton** a **Felügyeleti eszközök** ikonra, majd a **Szolgáltatások** elemre.

2.  A szolgáltatások listájának görgetésével keresse meg az **Üzenetsor-kezelés** elemet.

3.  Az **Állapot** oszlopban az **Elindítva** feliratnak kell szerepelnie, ha nem, kattintson a jobb oldali egérgombbal a szolgáltatásra, és válassza az **Indítás** parancsot.

Harmadik feladatként ellenőrizze, hogy a naplózási szolgáltatás rendelkezik-e engedéllyel események naplózási adatbázisba írásához. Az RMS naplózási szolgáltatás az RMS szolgáltatásfiókjának használatával fut. Ellenőrizze, hogy az RMS szolgáltatásfiókja rendelkezik-e érvényes bejelentkezéssel az adatbázis-kiszolgálóra, illetve megfelelő engedélyekkel adatbázis létrehozásához és adatok fájlba írásához.

Ha az összes előfeltétel teljesül, állítsa le, majd indítsa újra az RMS naplózási szolgáltatását a Szolgáltatások beépülő modul segítségével. Az újraindítás után a naplófájlok létrehozásának sikeresnek kell lennie az adatbázis-kiszolgálón. Ha adatbázis-kiszolgálóként SQL Server kiszolgálót használ, a következő eljárással ellenőrizheti a naplófájlok létrehozását.

**A naplófájlok létrehozásának ellenőrzése SQL Server kiszolgálón**
1.  Az SQL Server Enterprise Manager programjában keresse meg a naplózási adatbázist, bontsa ki a **Databases (Adatbázisok)** ágat, majd azt az adatbázist, amely az RMS naplózási adatbázisát tartalmazza.

2.  Kattintson a naplózási adatbázisra, kattintson a **Tables (Táblák)** elemre, majd kattintson a jobb gombbal a **DRMS\_log\_master** táblára, és válassza az **Open table – return all rows (Tábla megnyitása - összes sor megjelenítése)** parancsot. Ha már készít naplófájlokat a szolgáltatás, itt megjelenik legalább egy naplófájl.

A konfigurációs adatbázis visszaállítása
----------------------------------------

Az RMS működésének feltétele, hogy a konfigurációs adatbázis működőképes legyen. Ha problémák adódnak a konfigurációs adatbázissal, például az adatbázis sérülése vagy merevlemezhiba az adatbázis-kiszolgálón, a konfigurációs adatbázis biztonsági másolatának visszaállításával helyreállítható az RMS működőképessége. A biztonsági másolatból az RMS konfigurációs adatbázisának visszaállításához a következő adatokra van szükség:

-   Az adatbázisról legutóbb készült biztonsági másolat neve.
-   Annak a számítógépnek a neve, amelyre a biztonsági másolat visszaállítása történik.
-   Az RMS létesítésekor használt fiók neve és jelszava.
-   A személyes kulcs szoftveres védelmének beállításakor megadott jelszó (ha ezt a védelmi módszert választotta).

A biztonsági másolatból való visszaállításhoz nincs szükség sem új kiszolgálói licencelői tanúsítványra, sem új személyes kulcsra, mert az RMS az összes beállítást megtartja (ezeket a konfigurációs adatbázis biztonsági másolatából veszi).

A konfigurációs adatbázist a következő eljárással állíthatja vissza a biztonsági másolatból.

**Adatbázis visszaállítása biztonsági másolatból**
1.  Kattintson a **Start** gombra, és válassza a **Minden program**, a **Windows RMS**, végül a **Windows RMS felügyeleti webhely** parancsot. Ekkor a **Globális felügyelet** lap jelenik meg.

2.  Keresse meg azt a webhelyet, amelyen létesítve van az RMS, és kattintson a mellette látható **A webhelyen működő RMS eltávolítása** hivatkozásra, majd az **OK** gombra.

3.  Állítsa vissza a konfigurációs adatbázisról készült biztonsági másolatból a fájlokat. Ha a biztonsági másolat készítésekor a naplózási adatbázisról is készített másolatot, és fenn szeretné tartani az adatok folytonosságát, állítsa vissza a naplózási adatbázist is.

    -   Ha teljes rendszerösszeomlás után állítja vissza a rendszert, az adatbázisfájlok visszaállítása előtt állítsa vissza a rendszerleíró adatbázist a rendszer állapotáról készült biztonsági másolatból.

4.  Ha a visszaállított adatbázis egy különálló legfelső szintű tanúsítási kiszolgálóhoz tartozik, a szolgáltatás újralétesítése előtt módosítsa a következő rendszerleíró kulcsot:

    -   A Windows Server 2003 rendszer 32 bites verziójával működő számítógépeken:

        `HKEY_LOCAL_MACHINE\Software\Microsoft\DRMS\1.0\`
        
    -   A Windows Server 2003 rendszer 64 bites verziójával működő számítógépeken:

        `HKEY_LOCAL_MACHINE\Software\WOW6432Node\Microsoft\DRMS\1.0\`

    Hozza létre a következő, karaktersorozat típusú bejegyzést, és hagyja üresen értékét:

    `GicURL`

    Ezzel megakadályozza, hogy az Active Directory észlelje a legfelső szintű tanúsítási kiszolgálót, és így megjelennek a tanúsítási kiszolgáló létesítésére szolgáló oldalak.

5.  Ha hardveres biztonsági modullal védi az RMS szermélyes kulcsát, állítsa vissza a biztonsági világ biztonsági másolatát, hogy visszanyerhetők legyenek a kulcsok.

6.  Hajtsa végre a megfelelő lépést:

    -   Ha nem fürt, hanem különálló kiszolgáló adatbázisát állítja vissza, keresse meg azt a webhelyet, amelyen létesíteni szeretné az RMS szolgáltatást, majd kattintson a mellette látható RMS létesítése a webhelyen hivatkozásra.

        vagy
        
    -   Ha egy fürt adatbázisát állítja vissza, keresse meg azt a webhelyet, amelyen létesíteni szeretné az RMS szolgáltatást, majd kattintson a mellette látható Kiszolgáló hozzáadása fürthöz hivatkozásra.

7.  Adja meg a kiszolgáló első létesítésekor használt RMS-szolgáltatásfiókot.

8.  Adja meg konfigurációs adatbázisról készült biztonsági másolat nevét (az adatbázis nevét és az adatbázist tároló számítógép nevét).

9.  Adja meg a kiszolgáló első létesítésekor használt jelszót.

10. Kattintson a **Küldés** gombra.

Elindul a létesítési folyamat, és az RMS szolgáltatás újból használható lesz a kiszolgálón.

További tájékoztatás: rendszer-helyreállítás tervezése, RMS-rendszer biztonsági mentése és visszaállítása fejezetek a dokumentumgyűjteménynek az RMS bevezetésének tervezését bemutató részében.

Lejárt az RMS szolgáltatásfiókjának a jelszava
----------------------------------------------

Ha leáll az RMS szolgáltatás működése, ennek oka az is lehet, hogy lejárt az RMS szolgáltatásfiókjának jelszava. Nézze meg az IIS kezelőjében. Ha az RMS-alkalmazáskészletek állnak, és nem lehet őket újraindítani, valószínűleg lejárt az RMS szolgáltatásfiókjának a jelszava.

Ha lejárt az RMS szolgáltatásfiókjának a jelszava, akkor minden olyan RMS kiszolgálón módosítani kell a jelszót, amely a lejárt jelszavú fiókot használja, majd újra kell indítani az IIS szolgáltatást. A további tudnivalókat lásd a dokumentumgyűjtemény „RMS kiszolgáló működtetése” részében „Az RMS szolgáltatásfiók jelszavának módosítása” témakörben.

Korábbi RMS-telepítés visszaállítása
------------------------------------

Ha meghibásodik az RMS kiszolgáló hardvere vagy szoftvere, úgy állíthatja vissza az RMS kiszolgálót, hogy az előzőleg telepített konfigurációs adatbázis használatával új kiszolgálópéldányt létesít.

> [!NOTE]  
> Ez az eljárás csak arra az esetre érvényes, ha az RMS szolgáltatást futtató kiszolgáló hibásodik meg. Ha a konfigurációs adatbázist futtató kiszolgáló hibásodik meg, lásd a témakör „A konfigurációs adatbázis visszaállítása” című pontját. Ha az RMS kiszolgáló egyúttal adatbázis-kiszolgáló is, a teljes kiszolgálót vissza kell állítani a biztonsági másolatból. 

A következő eljárással a létesítési folyamatot az eredeti telepítés alkalmával használt konfigurációs adatbázisra irányíthatja.

**Az RMS korábbi telepítésének visszaállítása**
1.  Jelentkezzen be rendszergazdai jogokkal rendelkező fiókkal arra a számítógépre, amelyet RMS kiszolgálóként kíván konfigurálni. Ellenőrizze, hogy a számítógép megfelel-e az RMS minimális rendszerkövetelményeinek. A további tudnivalókat lásd a dokumentumgyűjtemény „RMS bevezetésének tervezése” részében a „Hardverkövetelmények” témakörben.

2.  Ha hardveres biztonsági modullal védi az RMS személyes kulcsait, ellenőrizze megfelelő konfigurálását ugyanazokkal a beállításokkal és biztonsági világgal, amelyet az RMS előző telepítésekor használt.

3.  Telepítse a számítógépre az RMS szolgáltatást.

4.  Az RMS telepítésének befejezése után kattintson a **Start** gombra, és válassza a **Minden program**, a **Windows RMS**, végül a **Windows RMS felügyeleti webhely** parancsot. Ekkor a **Globális felügyelet** lap jelenik meg.

5.  Keresse meg azt a webhelyet, amelyen létesíteni kívánja az RMS-szolgáltatást, majd kattintson a mellette látható **A kiszolgáló hozzáadása egy fürthöz** hivatkozásra.

6.  Írja be az **RMS szolgáltatásfiókja** csoportban az RMS azon szolgáltatásfiókjának nevét (tartománynév\\felhasználónév formátumban) és jelszavát, amellyel szokásos körülmények között az RMS futni fog. A fióknak tartományi fióknak kell lennie.

7.  A **Konfigurációs adatbázis** csoportban adja meg az adatbázis-kiszolgáló nevét, valamint a helyreállítani kívánt, eredeti RMS-telepítés konfigurációs adatbázisának nevét.

8.  Jelölje ki **A személyes kulcs védelme** csoportban a fürtben a személyes kulcs védelemére használt módszert. Ha a szoftveres személyeskulcs-védelmet választotta, meg kell adnia a fürt első létesítésekor a jelszó titkosításához megadott jelszót.

9.  Kattintson a **Küldés** gombra.

A lejárt engedélyek miatt az ügyfelek nem tudják megnyitni az RMS-védelemmel ellátott tartalmat
-----------------------------------------------------------------------------------------------

Ha egy felhasználó engedélye lejárt, nem tudja használni az RMS-védelemmel ellátott tartalmat. Ha az RMS kiszolgáló rendszerórája siet az RMS ügyfél rendszerórájához képest, a felhasználó esetleg akkor sem tudja használni az RMS-védelemmel ellátott tartalmat, ha engedélye még nem járt le. Mivel a két számítógép rendszerórája nincs szinkronizálva, a következő hibaüzenet jelenhet meg, amikor az ügyfélszámítógép megkísérli a tartalom megnyitását:

**Nincs engedélye az üzenet megnyitására, mert engedélye lejárt.??? Kívánja más hitelesítő adatokkal megnyitni? ???**  

Az ügyfél és a tartalom licence egyaránt érvényes, de az időeltérés miatt az ügyfél a tartalom licencét érvénytelennek értelmezi, és ezt a hibaüzenetet adja. Ez alapján a felhasználó azt gondolhatja, hogy probléma van a fióktanúsítvánnyal vagy a dokumentumhoz rendelt engedélyekkel. Amikor az ügyfélgép órája eléri a tartalom közzétételi licencének érvényességi időtartományát, a felhasználó meg tudja nyitni a tartalmat.

Gyakorlati tanácsként az RMS rendszeren érdemes valamennyi kiszolgálót és ügyfelet ugyanazzal az időszolgáltatással szinkronizálni.

„A hozzáférés megtagadva" hibaüzenet jelenik meg, amikor az RMS eseményeket kísérel meg bejegyezni az alkalmazások eseménynaplójába
-----------------------------------------------------------------------------------------------------------------------------------

Alapértelmezés szerint az ASP lapról futtatott összetevők, ilyen az RMS is, létrehozása az IUSR\_COMPUTERNAME fiókkal történik. Ez a fiók a Vendégek csoport tagja, és alkalmazások eseménynaplójába való íráshoz szükséges hozzáférési jogok hiányában a Vendégek csoport fiókjai nem írhatnak adatokat az eseménynaplóba.

A probléma megoldásához a rendszerleíró adatbázis szerkesztőjét használhatja a megfelelő kulcs módosításához.

> [!CAUTION]  
> A rendszerleíró adatbázis nem megfelelő módosítása súlyos károkat okozhat a rendszerben. A rendszerleíró adatbázis módosítása előtt készítsen biztonsági másolatot a számítógépen tárolt fontos adatokról. 

Állítsa a következő rendszerleíró kulcsot 0 helyett 1 értékűre, majd a változtatás érvénybe léptetéséhez indítsa újra a számítógépet.

`HKEY_LOCAL_MACHINE\System\CurrentControlSet\Services\EventLog\Application`

Név: `RestrictGuestAccess`

Típus: `REG_DWORD`

> [!NOTE]  
> Ez írási engedélyt ad a Vendégek csoport tagjainak az alkalmazások eseménynaplójához. 

A hiba okáról a további tudnivalókat az ASP lapokról engedélyezett naplózással foglalkozó cikk tartalmazza a [Microsoft Tudásbázisban](http://go.microsoft.com/fwlink/?linkid=44167).
