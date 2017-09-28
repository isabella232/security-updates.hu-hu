---
TOCTitle: 'WSUS SP1 – Fontos tudnivalók'
Title: 'WSUS SP1 – Fontos tudnivalók'
ms:assetid: '937ecfe9-e8e0-41ac-85f7-4b65956f3d1e'
ms:contentKeyID: 18129694
ms:mtpsurl: 'https://technet.microsoft.com/hu-hu/library/Cc708486(v=WS.10)'
---

WSUS SP1 – Fontos tudnivalók
============================

Ez a dokumentum ismerteti azokat az ismert problémákat, amelyek hatással vannak az 1. szervizcsomaggal frissített Windows Server Update Services (WSUS SP1) szolgáltatásra. Közvetlenül a WSUS SP1 változatára vonatkozó tudnivalók után megtalálhatók a WSUS szolgáltatásról korábban kiadott Fontos tudnivalók is. Ez a tájékoztatás tartalmazza a WSUS telepítéséhez szükséges ajánlásokat és követelményeket is. A WSUS SP1 letölthető a [Microsoft letöltési központjából](http://go.microsoft.com/fwlink/?linkid=67516).

A WSUS SP1 újdonságai
---------------------

A WSUS SP1 olyan szervizcsomag jellegű továbbfejlesztés, ami a WSUS biztonságát, alkalmazhatóságát, méretezhetőségét, kompatibilitását és teljesítményét javítja. A továbbfejlesztett és az új szolgáltatások a következők:

-   Támogatás a Windows Vista ügyfeleként: A Windows Vista rendszerrel működő számítógépek frissíthetők a WSUS SP1 kiszolgálójával.
-   Szélesebb körű nyelvi támogatás: Az Office és a Windows Vista összes nyelvének támogatása.
-   A WMSDE új verziója: A WSUS SP1 a WMSDE példányt a WMSDE SP4 verzióra frissíti (A WSUS RTM a WMSDE SP3 változatát használja).
-   Teljesítménynövelések: A WSUS SP1 több teljesítményjavítást tartalmaz, hogy lerövidítse a felhasználói felület válaszidejét.
-   Minden gyorsjavítás: A WSUS SP1 tartalmaz minden a WSUS RTM óta megjelent változtatást és gyorsjavítást.
-   Az SQL Server 2005 támogatása.

A WSUS SP1-re frissítése előtt
------------------------------

A következő problémák jellemzően a WSUS SP1-re frissítésénél jelentkezhetnek. Tudjon róla, hogy a jelen témakör eredeti változatának „A telepítés előkészítése” című részében foglalt problémákkal és követelményekkel most nem foglalkozunk, azok továbbra is érvényben vannak. Érvényesek például továbbra is a telepítési feltételek, ahogy azt „A telepítés előkészítése” című rész eredetileg taglalta.

**Megjegyzés**   Ha az SP1 már alkalmazva lett a WSUS 2.0 verzióra, a szervizcsomag telepítése nem távolítható el. Az SP1 eltávolítása az egész termék eltávolítását eredményezi.

**Fontos**   Ez a dokumentum tartalmaz a rendszerleíró adatbázis módosításával kapcsolatos tudnivalókat. A rendszerleíró adatbázis módosítása előtt feltétlenül készítsen biztonsági másolatot arról, és csak akkor fogjon hozzá, ha tisztában van a rendszerleíró adatbázis visszaállításának módjával probléma esetén. A rendszerleíró adatbázis biztonsági mentéséről, visszaállításáról és módosításáról lásd a Microsoft Tudásbázis következő cikkét:

[A Microsoft Windows rendszerleíró adatbázis ismertetése](http://support.microsoft.com/kb/256986) (http://support.microsoft.com/kb/256986/)

#### 1. probléma: Biztosítson elegendő helyet az adatbázis biztonsági mentéséhez

A WSUS RTM frissítésekor a WSUS SP1 telepítője automatikusan biztonsági mentést készít a WSUS adatbázisáról. Meg kell győződnie, hogy a WSUS kiszolgáló fájlrendszerében van-e elegendő hely a WSUS adatbázisának biztonsági mentéséhez, mert különben a WSUS SP1 telepítése sikertelen lesz.

**Az elegendő szabad hely megállapítása**
1.  Nyissa meg a Windows Intézőt, és lépjen arra a mappára, amelyikben a WSUS adatbázis van tárolva. Alapértelmezésben a WSUS az adatbázist a következő helyre telepíti:

    
        ```
2.  Tartsa lenyomva a **CTRL** billentyűt, és jelölje ki a **SUSDB.MDF** és a **SUSDB\_log.LDF** fájlt, majd kattintson az egér jobb oldali gombjával és válassza a **Tulajdonságok** parancsot.

3.  A **Fájlok** párbeszédpanelen olvassa le a **Lemezterület** értékét. A lemezen legalább ennyi szabad helynek kell lenni a WSUS SP1 telepítéséhez.

4.  A **Start** menüben válassza a **Sajátgép** lehetőséget Ellenőrizze, hogy azon a lemezen, ahol a WSUS van telepítve rendelkezik-e a szükséges szabad lemezterülettel.

Ha valamilyen okból sikertelen a WSUS SP1 telepítése, az adatbázist manuálisan kell helyreállítani. A WSUS adatbázis helyreállításáról tájékozódjék a [WSUS kezelési útmutatójában](http://technet2.microsoft.com/windowsserver/en/library/05f2e884-ae62-4c90-9681-6c9f2f3c9fd91033.mspx).

#### 2. probléma: A WSUS SP1 csak a WSUS RTM frissítésére képes

Ezért a WSUS SP1 csak a WSUS RTM frissítésére használható. Jelenleg nincs támogatva a WSUS belső használatú, "kiadásra jelölt" változatának a frissítése. Ha a WSUS "jelölt" vagy más belső változata telepítve van, azt előbb el kell távolítani, és csak azután lehet elindítani a WSUS SP1 telepítését.

#### 3. probléma: A kiszolgálón az IIS szolgáltatás le lesz állítva a WSUS SP1 frissítésekor

A WSUS SP1 frissítés telepítője leállítja az Internet Information Services (IIS) szolgáltatást a frissítési folyamat idején. Ez azt jelenti, hogy a kiszolgálón üzembe helyezett IIS a frissítés idejére nem lesz elérhető. A frissítés végén az IIS automatikusan újraindul.

#### 4. probléma: A frissítés időtartama alatt nem futtatható WSUS API-hívásokat használó alkalmazás

A WSUS API (alkalmazásfejlesztői felület) meghívása ütközést okoz a WSUS SP1 telepítőjével, aminek következtében a frissítés megszakad (a frissítés folytatásához a telepítő a kiszolgáló újraindítását kérő üzenetet jelenít meg).

#### 5. probléma: A WSUS SP1 frissítésekor lehet, hogy le kell tiltani a vírusvédelmet

A WSUS SP1 használatával történő frissítéskor lehet, hogy szükség van a vírusvédelmi programok kikapcsolására, hogy a frissítés sikeresen legyen végrehajtható. A vírusvédelmi szoftverek letiltása után és a frissítés, illetve a szervizcsomag telepítése előtt újra kell indítani a Windows kiszolgáló számítógépét. Ez az eljárás teszi lehetővé, hogy a frissítési folyamat által elérni szükséges fájlok ne legyenek zárolva. A telepítés befejezése után ne feledje ismét bekapcsolni a vírusvédelmi programot. A vírusvédelmi program letiltásához és ismételt engedélyezéséhez szükséges lépésekről a vírusvédelmi program gyártójának webhelyén tájékozódhat.

| ![](images/Cc708486.Caution(WS.10).gif)Figyelmeztetés:                                                                                                                                                                                                                                                                               |
|-------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| Ez a kerülő megoldás a számítógépét vagy a hálózatát sebezhetőbbé teszi a rosszindulatú felhasználókkal vagy a kártékony szoftverekkel, vírusokkal szemben. Mi nem ajánljuk ezt a kerülőutat, csak tájékoztatjuk ennek lehetőségéről, de ennek igénybe vétele a felhasználó felelőssége. Ezt a kerülőutat a felhasználók csak saját felelősségükre használhatják. |

| ![](images/Cc708486.note(WS.10).gif)Megjegyzés:                                                                                                                                                                                                                                                         |
|--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| A vírusvédelmi programok úgy lettek kialakítva, hogy segítsék a számítógépet megvédeni a számítógépes vírusoktól. Amikor le van tiltva a vírusvédelem nem szabad letölteni vagy megnyitni olyan fájlokat, amelyek nem megbízható eredetűek, nem szabad látogatni nem megbízható webhelyeket, illetve megnyitni e-mail mellékleteket. |

#### 6. probléma: Ha proxykiszolgálót használ, lehet, hogy az SP1 frissítés törli a proxy konfigurált felhasználónevét és jelszavát

Ha proxykiszolgálót használ, néhány esetben az SP1 frissítés törli a proxy konfigurált felhasználónevét és jelszavát. Ez azt eredményezheti, hogy a Microsoft kiszolgálókról történő frissítések „Érvénytelen paraméter” üzenetű hibát generálnak. A probléma feloldása érdekében állítsa vissza a proxy konfiguráció felhasználónevét és jelszavát, majd szinkronizálja újra a kiszolgálót.

#### 7. probléma: Hogyan állítható helyre a WSUS kiszolgáló sikertelen telepítésből stabil állapotba a frissítés újbóli megkísérlése érdekében.

Ha a WSUS SP1 frissítés nem sikerül, a telepített WSUS bizonytalan vagy használhatatlan állapotban marad. Hogy újra megpróbálhassa a WSUS SP1 telepítését vissza kell térni a WSUS stabil állapotához. Ehhez használható az adatbázisnak frissítés elején előállított biztonsági mentése, amivel a WSUS kiszolgáló visszaállítható a frissítés előtti állapotba.

Sikertelen frissítés esetén hajtsa végre a következő lépéseket, hogy ismét megpróbálhassa a WSUS SP1 frissítését:

**A WSUS SP1 frissítésének ismételt megkísérlése**
1.  A WSUSSetup\_%időbélyeg%.log fájl megtekintésével állapítsa meg a tartaléknak mentett adatbázis helyét. A fájl a következő mappában található:

    -   %programfájlok%\\Update Services\\LogFiles

2.  Állítsa helyre az adatbázist a WSUS számítógépen a következőképpen:

    -   osql.exe -S &lt;AdatbázisPéldány&gt; -E -Q "USE master ALTER DATABASE SUSDB SET SINGLE\_USER WITH ROLLBACK IMMEDIATE RESTORE DATABASE SUSDB FROM DISK=N'&lt;MentettAdatbázisElérésiÚtja&gt;' WITH REPLACE ALTER DATABASE SUSDB SET MULTI\_USER"
    -   Ne feledje az &lt;AdatbázisPéldány&gt; és a &lt;MentettAdatbázisElérésiÚtja&gt; helyére a telepítésének megfelelő értéket írni.
    -   Az &lt;AdatbázisPéldány&gt; helyére a rendszerleíró adatbázis következő kulcsának az értékét kell beírni:
    -   HKLM\\Software\\Microsoft\\Update Services\\Server\\Setup\\SqlServerName
    -   A &lt;MentettAdatbázisElérésiÚtja&gt; helyére pedig azt, amit az 1. lépésben megállapított.

3.  Távolítsa el a WSUS programot, de tartsa meg a WSUS adatbázist, a naplófájlokat és a frissítési fájlokat, amikor a képernyőn erre felszólítást kap. (Gondoskodjon róla, hogy a **Microsoft Windows Server Update Services eltávolítása** egyik beállítása se legyen bejelölve.)

4.  Telepítse újra a WSUS RTM verziót (az eredeti verziót, ne a WSUS SP1 verziót). Amikor erre felszólítást kap, használja a létező adatbázist. Ez visszaállítja a WSUS rendszert a konzisztens állapotba.

5.  A WSUS SP1 telepítése

**Megjegyzés**    A fenti 1. lépés szerint biztonsági mentéssel mentett adatbázis a WSUS SP1 tiszta telepítésénél nem használható közvetlenül. Az adatbázis-séma megváltozott, ezért ez az adatbázis nem kompatibilis, amíg nem lett frissítve a WSUS SP1 telepítőjével.

#### 8. probléma: Néhány esetben sikertelen lehet a WSUS SP1 frissítés, ha a WMSDE adatbázis át lett telepítve

A megoldás eltérő attól függően, hogy helyi vagy távoli SQL kiszolgálóra történt az áttelepítés.

#### Helyi SQL 2000 kiszolgálóra áttelepített WMSDE adatbázis

Meg kell változtatni a rendszerleíró adatbázis kulcsát, hogy a WSUS SP1 telepítője tudomásul vegye, hogy a korábbi helyén nincs frissítendő WMSDE adatbázis.

Ha a WMSDE adatbázis helyi SQL 2000 kiszolgálóra lett áttelepítve, a következő változtatást kell végrehajtani a rendszerleíró adatbázisban a WSUS SP1 frissítésének megkísérlése előtt:

-   A következő rendszerleíró kulcsban "1" helyett "0" legyen az érték:
    -   HKLM\\Software\\Microsoft\\Update Services\\Server\\Setup\\WmsdeInstalled  

#### Távoli SQL 2000 kiszolgálóra áttelepített WMSDE adatbázis

Meg kell változtatni a rendszerleíró adatbázis két kulcsának az értékét, hogy a WSUS SP1 telepítője tudomásul vegye, hogy a korábbi helyén nincs frissítendő WMSDE adatbázis. A frissítést először a háttérkiszolgálón kell kezdeményezni, majd az előtérbeli kiszolgálón folytatni.  

Ha a WMSDE adatbázis távoli SQL kiszolgálóra lett áttelepítve, a következő változtatásokat kell végrehajtani a rendszerleíró adatbázisban a WSUS SP1 frissítésének megkísérlése előtt:

1.  A következő rendszerleíró kulcsban "1" helyett "0" legyen az érték:
    -   HKLM\\Software\\Microsoft\\Update Services\\Server\\Setup\\WmsdeInstalled 
2.  A következő rendszerleíró kulcsban "0x80" helyett "0x20" legyen az érték:
    -   HKLM\\Software\\Microsoft\\Update Services\\Server\\Setup\\InstallType 

A rendszerleíró kulcsok értékének módosítása után a frissítést először a háttérkiszolgálókon, majd az előtérbeli kiszolgálókon kell kezdeményezni.

#### 9. probléma: A WSUS SP1 nem frissíti az olyan WSUS kiszolgálókat, amelyek a távoli SQL rendszerbeállítással lettek telepítve

A WSUS SP1 telepítő csomagot el kell indítani az előtérbeli és a háttérbeli kiszolgálókon is.

**A WSUS SP1 frissítése távoli SQL használata esetén**
1.  Indítsa el a telepítőcsomagot kapcsolók nélkül az előtérben, és válassza a frissítést.

2.  Indítsa el a telepítőcsomagot kapcsolók nélkül a háttérben, és válassza a frissítést.

#### 10. probléma: Ha a számítógép nevét a WSUS SP1 frissítés előtt megváltoztatták, ez a frissítés sikertelenségét eredményezheti

Ha a számítógép nevét a WSUS RTM telepítése után és a WSUS SP1 verzióra való frissítés előtt megváltoztatták, ez a WSUS SP1 frissítés sikertelenségét eredményezheti.

Az ASPNET és a WSUS Rendszergazdák csoportjának eltávolításához, majd ismételt felvételéhez a következő parancsfájlt kell használni. Majd a frissítést újra elindítani.

        ```
| ![](images/Cc708486.note(WS.10).gif)Megjegyzés:                 |
|----------------------------------------------------------------------------------------------|
| A &lt;Tartalommappa&gt; helyére az utolsó sorban a tartalomtároló elérési útját kell beírni. |

A WSUS – Fontos tudnivalók eredeti tartalma
-------------------------------------------

A következő rész a WSUS eredetileg kiadott fontos tudnivalóit ismerteti. A WSUS SP1 *nem* befolyásolja a következőkben tisztázandó problémákat. Ezt a tartalmat azért idézzük, hogy ne kelljen keresgélnie.

A telepítés előkészítése
------------------------

#### 1. probléma: Az IIS terméknek telepítve kell lennie

A Microsoft® Windows Server™ Update Services (WSUS) igényli, hogy az Internet Information Services (IIS) telepítve legyen. Bár a Microsoft Windows Server 2003 és a Microsoft Windows® 2000 Server rendszerben az IIS nincs alapértelmezés szerint telepítve, a Windows Server Update Services (WSUS) telepítője nem tud továbblépni, hanem olyan üzenetet jelenít meg, hogy az IIS nincs telepítve.

Az IIS telepítése:

1.  Nyissa meg a Vezérlőpult ablakot.
2.  Kattintson duplán a **Programok telepítése/törlése** ikonra.
3.  Kattintson a **Windows-összetevők hozzáadása vagy eltávolítása** gombra.
4.  Az **Összetevő** listában kattintson az **Alkalmazáskiszolgáló** elemre.
5.  Kattintson a **Részletek** gombra.
6.  Jelölje be az **ASP.NET** jelölőnégyzetet. Válassza a **COM+ alapú hálózati hozzáférés engedélyezését**, és az Internet Information Services (IIS) automatikusan kijelölődik.
7.  Az **Internet Information Services (IIS)** kijelölése után kattintson a **Részletek** gombra, hogy megnézze az IIS választható összetevőit.
8.  Jelöljön be minden telepíteni kívánt összetevőt. A World Wide Web szolgáltatás olyan fontos alösszetevőket tartalmaz, mint az Active Server Pages összetevő és a Távfelügyelet (HTML). Ezen alösszetevők megtekintéséhez kattintson a World Wide Web szolgáltatás elemre, majd a Részletek gombra. Kattintson az OK gombra, hogy visszajusson a Windows-összetevők varázsló párbeszédpanelre.
9.  Kattintson a **Tovább** gombra, és a befejezéséig folytassa a Windows-összetevők varázsló használatát.
10. Az IIS telepítése után indítsa el a Windows Server Update Services telepítését.

#### 2. probléma: Windows 2000 Server rendszerű kiszolgálók esetében a WSUS telepítéséhez legalább egy webhelynek léteznie kell az IIS szolgáltatásban

Előfordulhat, hogy a Windows Server Update Services telepítő nem képes webhelyet létrehozni, ha a futtatásakor az IIS még egyetlen webhelyet sem tartalmaz. Ez megtörténhet például akkor, ha az IIS csak egy Software Update Services (SUS) 1.0 alapú webhelyet tartalmazott, azt azonban a WSUS telepítése előtt törölték.

Ilyen esetben egy új webhelyet kell létrehozni az Internet Information Services (IIS) kezelője beépülő modullal. Ezt követően a WSUS telepítése folyamán kijelölhető ez a webhely, illetve megadható egy új webhely.

Ha a WSUS telepítésére már kísérletet tett, és a telepítő létező webhely hiányában leállt, nyissa meg az IIS kezelője beépülő modult, és törölje a „Webhely 1” webhelyet. Ezután a telepítő ismételt futtatásához kövesse a korábban ismertetett eljárást.

#### 3. probléma: Az előfeltételként szolgáló összetevők telepítése

#### Szoftverkövetelmények

A következő táblázat ismerteti, hogy az egyes támogatott operációs rendszereken milyen szoftverre van szükség a WSUS telepítéséhez A WSUS telepítése előtt ellenőrizze, hogy a WSUS kiszolgáló megfelel-e ezen követelményeknek. Ha az itt említett frissítések bármelyike a számítógép újraindítását kéri a telepítés végeztével, akkor az újraindítást a WSUS telepítése előtt kell végrehajtani.

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
<th>Operációs rendszer</th>
<th>Követelmények</th>
<th>Letöltések</th>
</tr>
</thead>
<tbody>
<tr class="odd">
<td style="border:1px solid black;"><p>Mindegyik operációs rendszer</p></td>
<td style="border:1px solid black;"><p>Microsoft Internet Information Services (IIS) 5.0</p></td>
<td style="border:1px solid black;"><p>Az operációs rendszerből telepíthető.</p>
<p>Lásd 1. probléma: Az IIS terméknek telepítve kell lennie.</p></td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><p>Mindegyik operációs rendszer</p></td>
<td style="border:1px solid black;"><p>Háttérben futó intelligens átviteli szolgáltatás (BITS) 2.0</p></td>
<td style="border:1px solid black;"><p>A Windows Server 2003 operációs rendszer változatait illetően lásd Frissítés a Háttérben futó intelligens átviteli szolgáltatás (BITS) 2.0-s verziójára és a WinHTTP 5.1-es verziójára – Windows Server 2003 (KB842773) (<a href="http://go.microsoft.com/fwlink/?linkid=47251">http://go.microsoft.com/fwlink/?LinkId=47251</a>).</p>
<p>A Windows Server 2000 operációs rendszer változatait illetően lásd Frissítés a Háttérben futó intelligens átviteli szolgáltatás (BITS) 2.0-s verziójára és a WinHTTP 5.1-es verziójára – Windows 2000 (KB842773) (<a href="http://go.microsoft.com/fwlink/?linkid=46794">http://go.microsoft.com/fwlink/?LinkId=46794</a>).</p></td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><p>Windows Server 2003</p></td>
<td style="border:1px solid black;"><p>Microsoft .NET-keretrendszer 1.1 Service Pack 1 szervizcsomag a Windows Server 2003 operációs rendszerhez</p></td>
<td style="border:1px solid black;"><p><a href="http://go.microsoft.com/fwlink/?linkid=47358">Microsoft .NET-keretrendszer 1.1 Service Pack 1 szervizcsomag a Windows Server 2003 operációs rendszerhez</a></p>
<p>Megteheti azt is, hogy ellátogat a <a href="http://go.microsoft.com/fwlink/?linkid=47370">Windows Update</a> webhelyre, és a Keresés mezőbe beírja a „Microsoft .NET-keretrendszer 1.1 Service Pack 1 Windows Server 2003” kifejezést.</p></td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><p>Windows Server 2003</p></td>
<td style="border:1px solid black;"><p>A Microsoft SQL kiterjesztésével teljesen kompatibilis adatbázisszoftver</p></td>
<td style="border:1px solid black;"><p>N/A</p></td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><p>Windows 2000 Server</p></td>
<td style="border:1px solid black;"><p>A Microsoft SQL kiterjesztésével teljesen kompatibilis adatbázisszoftver</p></td>
<td style="border:1px solid black;"><p>Ha a Microsoft SQL Server 2000 nincs telepítve, telepítheti a Microsoft SQL Server 2000 Desktop Engine (MSDE 2000) verziót. Ez több lépésből áll. A további tudnivalókat lásd alább Az MSDE telepítése Windows 2000 rendszerre című részt.</p></td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><p>Windows 2000 Server</p></td>
<td style="border:1px solid black;"><p>Microsoft Internet Explorer 6.0 Service Pack 1 szervizcsomaggal</p></td>
<td style="border:1px solid black;"><p><a href="http://go.microsoft.com/fwlink/?linkid=47359">Internet Explorer 6 Service Pack 1</a></p></td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><p>Windows 2000 Server</p></td>
<td style="border:1px solid black;"><p>Újraterjeszthető csomag a Microsoft .NET-keretrendszer 1.1-es verziójához</p></td>
<td style="border:1px solid black;"><p><a href="http://go.microsoft.com/fwlink/?linkid=47369">Újraterjeszthető csomag a Microsoft .NET-keretrendszer 1.1-es verziójához</a></p></td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><p>Windows 2000 Server</p></td>
<td style="border:1px solid black;"><p>Microsoft .NET-keretrendszer 1.1 1. szervizcsomag</p></td>
<td style="border:1px solid black;"><p><a href="http://go.microsoft.com/fwlink/?linkid=47368">Microsoft .NET-keretrendszer 1.1 1. szervizcsomag</a></p>
<p>Megteheti azt is, hogy ellátogat a <a href="http://go.microsoft.com/fwlink/?linkid=47370">Windows Update</a> webhelyre, és a Keresés mezőbe beírja a „Microsoft .NET-keretrendszer 1.1 Service Pack 1 Windows Server 2000” kifejezést.</p></td>
</tr>
</tbody>
</table>
<p> </p>

A fenti követelmények mellett előfordulhat, hogy szükség esetén a WSUS telepíti és konfigurálja az ASP.NET 1.1-es verzióját a kiszolgálón. (A WSUS telepítő konfigurálja az ASP.NET összetevőt.)

#### Az MSDE 2000 telepítése Windows 2000 rendszerre

Ha a WSUS szolgáltatást Windows 2000 rendszerrel használja, és nincs Microsoft SQL Server 2000 hozzáférése, a WSUS telepítés előtt szükség van a Microsoft SQL Server 2000 Desktop Engine (MSDE) telepítésére. Ha az MSDE már telepítve lett a WSUS kiszolgálóra, nincs szükség a WSUS részére szóló külön példány telepítésére. Egyszerűen csak meg kell adni a meglévő példány nevét a WSUS telepítése során.

Az MSDE összetevő Windows 2000 Server rendszerre történő telepítése négy lépésből áll. Először le kell tölteni és ki kell csomagolni az MSDE tömörített archívumát a WSUS kiszolgáló egyik mappájába. Ezután a parancssorban a megfelelő parancssori kapcsolókkal el kell indítani az MSDE telepítését, meg kell adni a rendszergazdai jelszót, majd példánynévként definiálni kell a WSUS szolgáltatást. Miután az MSDE telepítése befejeződött, ellenőrizni kell, hogy a WSUS példány NT-szolgáltatásként működik-e. Végezetül szükség van az MSDE biztonsági javítócsomaggal történő frissítésére, hogy a WSUS kiszolgáló védett legyen.

#### 1. lépés: Az MSDE archivált példányának letöltése és kicsomagolása

Le kell tölteni és ki kell csomagolni az MSDE tömörített archívumát a WSUS kiszolgáló egyik mappájába. Lásd [Microsoft SQL Server 2000 Desktop Engine (MSDE 2000) Release A](http://go.microsoft.com/fwlink/?linkid=47366).

#### 2. lépés: Az MSDE telepítése

A parancssorban a megfelelő parancssori kapcsolókkal el kell indítani az MSDE telepítését, meg kell adni a rendszergazdai jelszót, majd példánynévként definiálni kell a WSUS szolgáltatást. Amikor az MSDE telepítése befejeződött, ellenőrizni kell, hogy a WSUS példány NT-szolgáltatásként működik-e.

Az MSDE telepítése, a rendszergazdai jelszó és példánynév megadása:

1.  A parancssorban lépjen az MSDE „1. lépés: Az MSDE archivált példányának letöltése és kicsomagolása” című részben megadott telepítési mappájába.
2.  Írja be a következőt: **setup sapwd="***jelszó***" instancename=WSUS**
    A *jelszó* az MSDE jelen példányához tartozó rendszergazdai fiók erősen védett jelszava, az **instancename** paraméter értéke pedig az adatbázispéldány neve. A WSUS adatbázis alapértelmezett példányneve is használható (a „WSUS” helyett). Ebben az esetben a parancssorból elhagyható az **instancename=WSUS** paraméter. A parancs elindítja az MSDE telepítőprogramját, beállítja a rendszergazdai jelszót, és az MSDE-példányhoz hozzárendeli a megadott nevet.

#### 3. lépés: Annak ellenőrzése, hogy az MSDE WSUS példánya telepítve van-e.

1.  Kattintson a **Start** menü **Futtatás** parancsára.
2.  A **Megnyitás** mezőbe írja be a **services.msc** parancsot, majd kattintson az **OK** gombra.

Görgesse lefelé a szolgáltatások listáját, és ellenőrizze, hogy az MSSQL$WSUS szolgáltatásnév (a „WSUS” példánynév használata esetén) vagy az MSSQLSERVER szolgáltatásnév (az alapértelmezett példánynév esetén) létezik-e.

#### 4. lépés: Az MSDE példány elindítása.

Az MSDE telepítésének a végén el kell indítani a telepített példányt. Ha az instancename paraméter értékeként a „WSUS” nevet használta, akkor az „MSSQL$WSUS” szolgáltatáspéldányt indítsa el. Ha az alapértelmezett példánynevet használta, akkor az MSSQLSERVER szolgáltatáspéldányt indítsa el. A szolgáltatás elindítása nélkül a WSUS nem képes az adatbázispéldány használatára.

#### 5. lépés: Az MSDE frissítése

Töltse le és telepítse az [MS03-031: Összesített biztonsági javítás az SQL Server programhoz](http://go.microsoft.com/fwlink/?linkid=47364) című közleményben ismertetett biztonsági javítást.

A biztonsági javítás letölthető az [SQL Server 2000 (32-bit) Security Patch MS03-031](http://go.microsoft.com/fwlink/?linkid=47363) hivatkozással.

#### 4. probléma: A lemezterület minimumának követelménye

A Windows Server Update Services telepítéséhez szükséges lemezterületre az alábbi követelmények vonatkoznak:

-   1 gigabájt (GB) a rendszerpartíción
-   2 GB az adatbázisfájlok majdani tárolására szolgáló köteten
-   6 GB a tervezett tartalomtól függően

#### 5. probléma: A WSUS legújabb verziójának telepítése előtt a korábbi verziót el kell távolítani a Programok telepítése és törlése segédprogrammal

Ha olyan kiszolgálón szeretné végrehajtani a Windows Server Update Services telepítését, amelyiken a Windows Update Services 1. vagy 2. bétaverziója fut, akkor ezt a korábbi verziót el kell távolítania a Vezérlőpult Programok telepítése és törlése segédprogramjával.

#### 6. probléma: A WSUS futtatásához az SQL Server alkalmazásban engedélyezni kell a beágyazott eseményindítók használatát

Ez a beállítás alapértelmezés szerint be van ugyan kapcsolva, de az SQL Server rendszergazdája kikapcsolhatja.

Ha a Windows Server Update Services adattárolójaként egy SQL Server alapú adatbázist szeretne használni, az SQL Server rendszergazdájának ellenőriznie kell, hogy a beágyazott eseményindítók engedélyezettek-e a kiszolgálón, a WSUS rendszergazdája csak ezután telepítheti a WSUS szolgáltatást, és adhatja meg a telepítés folyamán a használni kívánt adatbázist.

A WSUS telepítő bekapcsolja a RECURSIVE\_TRIGGERS adatbázis-specifikus beállítást, az egész kiszolgálóra érvényes, beágyazott eseményindítókra vonatkozó beállítást azonban nem kapcsolja be.

Az alábbi paranccsal ellenőrizhető, hogy a beágyazott eseményindítók engedélyezettek-e:

**sp\_configure 'nested triggers'**

A beágyazott eseményindítókra vonatkozó beállítás bekapcsolásához kötegfájlból futtassa az alábbi parancsokat az SQL Server alkalmazást működtető számítógépen:

**sp\_configure 'nested triggers', 1**

**GO**

**RECONFIGURE**

**GO**

#### 7. probléma: A WSUS telepítő parancssori paraméterei

A WSUS felügyelet nélkül is telepíthető. A további tudnivaló és a parancssori paraméterek felsorolása a [Deploying Microsoft Windows Server Update Services](http://go.microsoft.com/fwlink/?linkid=41777) (A Microsoft WSUS szolgáltatás létesítése) dokumentum "Appendix A: Unattended Installation" („A” függelék: Felügyelet nélküli telepítés) című részében.

Ismert problémák
----------------

#### 1. probléma: IIS Lockdown varázsló

Ha Windows 2000 Server rendszerű számítógépen működteti az Internet Information Services (IIS) szolgáltatást, akkor a Microsoft TechNet IIS Lockdown Tool lapjáról telepíteni kell az IIS Lockdown varázsló legújabb verzióját (amely tartalmazza az URLScan eszközt). Az IIS alapú kiszolgálók biztonsága érdekében a Microsoft feltétlenül ajánlja ezen eszköz telepítését. Az IIS Lockdown varázsló úgy működik, hogy kikapcsolja az IIS szükségtelen szolgáltatásait csökkentve ezzel a biztonsági kockázatot.

| ![](images/Cc708486.note(WS.10).gif)Megjegyzés:                                                                                                                                                                                      |
|-------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| A WSUS telepítő nem telepíti ezeket az összetevőket. Ezek telepítését külön kell végrehajtani. Az IIS Lockdown telepítése nem szükséges a Windows Server 2003 verzióval működő számítógépeken, mert ez a funkció már be lett építve ebbe az operációs rendszerbe. |

#### 2. probléma: A WSUS konfigurációjának közvetlen módosítása az adatbázisban nem támogatott

A Windows Server Update Services szolgáltatás konfigurációs adatait egy (MSDE vagy SQL Server alapú) adatbázis tárolja. A konfigurációs adatoknak közvetlenül az adatbázisban való módosítása azonban nem támogatott. A rendszergazdák ily módon ne kíséreljék meg a WSUS konfigurációjának módosítását. A WSUS konfigurációjának módosítása csak a WSUS-konzol és a WSUS API (alkalmazásprogramozási felület) hívásainak használatával támogatott.

#### 3. probléma: A WSUS felügyeleti webhelyének eléréséhez engedélyezni kell az Active scripting szolgáltatást

A rendszergazda munkaállomásán úgy kell beállítani az Internet Explorer böngészőt, hogy lehetővé tegye az Active scripting szolgáltatás használatát, az Internet Explorerrel ugyanis csak így érhető el a WSUS felügyeleti helye.

#### 4. probléma: Az IIS újraindul a WSUS telepítésekor

A Windows Server Update Services telepítő a felhasználó értesítése nélkül újraindítja az IIS szolgáltatást. Ez hatással lehet a szervezetben működő webhelyekre.

#### 5. probléma: A WSUS vagy az SMS kezelési pontjai virtuális könyvtárakhoz való hozzáférésének módosítása

Alapértelmezés szerint a Windows Server Update Services tartalmat tároló virtuális könyvtárhoz név nélküli hozzáférés van beállítva. Ha ezt a beállítást úgy módosítja, hogy a hozzáféréshez hitelesítésre legyen szükség, az ügyfelek hitelesítési hibáról szóló üzeneteket kapnak, és a rendszer megtagadja tőlük a hozzáférést, amikor frissítéseket szeretnének letölteni. Ezt az ismert hibát az okozza, hogy a Winhttp.dll hibás hitelesítési környezetet használ, amikor implicit hitelesítésre van szükség, ezért a hitelesítés nem sikerül. A hiba megakadályozása érdekében gondoskodjék arról, hogy a WSUS-kiszolgáló és az SMS kezelési pontjai név nélküli hozzáféréssel rendelkezzenek az IIS virtuális könyvtáraihoz.

#### 6. probléma: A WSUS szolgáltatás Windows Small Business Server 2003 rendszerre való telepítése esetén a WSUS által az alapértelmezett webhelyre telepített virtuális gyökerek hozzáférési beállításait módosítani kell ahhoz, hogy a WSUS ügyfelei frissíthessék magukat a kiszolgálóról

A WSUS-kiszolgáló két virtuális gyökeret, a SelfUpdate és a ClientWebService, és néhány fájlt telepít a 80-as porton lévő alapértelmezett webhely kezdőkönyvtárába. Ez lehetővé teszi, hogy az ügyfelek az alapértelmezett webhelyen keresztül frissítsék önmagukat. Alapértelmezés szerint a Windows Small Business Server 2003 rendszerben az alapértelmezett webhely úgy van beállítva, hogy a kiszolgálóén kívül minden IP-címhez vagy localhost címhez megtagadja a hozzáférést. Ez azt jelenti, hogy a SelfUpdate és a ClientWebService virtuális gyökerek sem kapnak hozzáférési jogosultságot, ezért az ügyfelek nem frissíthetik önmagukat. Ha az ügyfeleknek hozzáférést szeretne biztosítani, hajtsa végre az alábbi lépéseket az alapértelmezett webhely SelfUpdate és ClientWebService virtuális gyökerén.

1.  Jelenítse meg a virtuális gyökér **Tulajdonságok**, párbeszédpanelét, kattintson a **Könyvtárbiztonság** fülre, és az **IP-cím és tartománynév korlátozása** csoportban kattintson a **Szerkesztés** gombra.
2.  Jelölje be a **hozzáférése engedélyezve** választógombot, és kattintson az **OK** gombra. Zárja be az összes tulajdonságlapot.

#### 7. probléma: A WSUS telepítése Small Business Server operációs rendszerre – együttműködési problémák

-   Ha a Windows Small Business Server 2003 rendszer ISA-proxykiszolgálót használ az internet-hozzáféréshez, a következő adatokat kézzel meg kell adni a **Beállítások** párbeszédpanelen: a proxykiszolgáló beállításait, a proxykiszolgáló nevét és a proxykiszolgáló portszámát.
-   Ha az ISA Windows-hitelesítést igényel, a proxykiszolgáló hitelesítő adatait a következő formátumban kell megadni: „TARTOMÁNY\\felhasználó” (a felhasználónak az „Internetfelhasználók” csoportba kell tartoznia).

#### 8. probléma: Ha egy számítógépet egyik számítógépcsoportból a másikba helyez át, akár egy óráig is tarthat, amíg a számítógép megjelenik az új csoportban a felügyeleti konzolon

Amikor egy számítógépet első alkalommal rendel célcsoporthoz, a számítógépen lévő adatok a csoport adataival módosulnak. Az adatokat a rendszer szabályos időközönként, például óránként, frissíti. Ezért ha egy számítógépet egyik számítógépcsoportból a másikba helyez át, akár egy óra is eltelhet addig, amíg a szóban forgó információk frissülnek az ügyfélszámítógépen, és a WSUS felügyeleti konzolján megjelennek a módosítások.

#### 9. probléma: Ha a WSUS szolgáltatást tagkiszolgálóra telepíti, majd a tagkiszolgálót tartományvezérlővé elő szeretné léptetni, először el kell távolítania a WSUS szolgáltatást

Ha a WSUS szolgáltatást tagkiszolgálóra telepíti, majd a tagkiszolgálót tartományvezérlővé elő szeretné léptetni, végezze el az alábbi lépéseket:

1.  Távolítsa el a WSUS szolgáltatást.
2.  Léptesse elő a tagkiszolgálót tartományvezérlővé.
3.  Telepítse újra a WSUS szolgáltatást.

#### 10. probléma: Ha egy WSUS-kiszolgálót tartományvezérlőből tagkiszolgálóvá szeretne lefokozni, először el kell távolítania a WSUS szolgáltatást

Ha a WSUS-kiszolgálót tartományvezérlőn futtatja, és a tartományvezérlőt tagkiszolgálóvá szeretné lefokozni, végezze el az alábbi lépéseket:

1.  Távolítsa el a WSUS szolgáltatást, és őrizze meg az adatbázisát.
2.  ASPNET néven hozzon létre egy felhasználói fiókot
3.  A parancssorba írja be: **aspnet\_regiis -i**.
4.  Telepítse újra a WSUS szolgáltatást, és használja a megőrzött adatbázist.

#### 11. probléma: Ha a .NET-keretrendszer 1.0-s vagy 2.0-s verzióját a WSUS szolgáltatás után telepíti, nem jelenik meg a WSUS felügyeleti konzolja

A problémát az okozza, hogy ilyenkor az IIS szolgáltatáshoz a rendszer a .NET-keretrendszer 1.0-s verzióját regisztrálja, a WSUS-kiszolgáló működéséhez azonban a .NET-keretrendszer 1.1-es verziójára van szükség. A hiba elhárításához indítsa el az aspnet\_regiis.exe programot, és futtassa az alábbi parancsokat úgy, hogy a *webhely-azonosító* helyére a következő rendszerleíró kulcsban található értéket írja be:

HKLM\\Software\\Microsoft\\WindowsUpdateServices\\Server\\Setup\\IISTargetWebsiteIndex

-   %windir%\\Microsoft.NET\\Framework\\v1.1.4322\\\\aspnet\_regiis.exe -s W3SVC\\&lt;*webhely-azonosító*&gt;\\ROOT\\ReportingWebService
-   %windir%\\Microsoft.NET\\Framework\\v1.1.4322\\\\aspnet\_regiis.exe -s W3SVC\\&lt;*webhely-azonosító*&gt;\\ROOT\\ClientWebService
-   %windir%\\Microsoft.NET\\Framework\\v1.1.4322\\\\aspnet\_regiis.exe -s W3SVC\\&lt;*webhely-azonosító*&gt;\\ROOT\\SimpleAuthWebService
-   %windir%\\Microsoft.NET\\Framework\\v1.1.4322\\\\aspnet\_regiis.exe -s W3SVC\\&lt;*webhely-azonosító*&gt;\\ROOT\\WSUSAdmin
-   %windir%\\Microsoft.NET\\Framework\\v1.1.4322\\\\aspnet\_regiis.exe -s W3SVC\\&lt;*webhely-azonosító*&gt;\\ROOT\\AdministrationWebService
-   %windir%\\Microsoft.NET\\Framework\\v1.1.4322\\\\aspnet\_regiis.exe -s W3SVC\\&lt;*webhely-azonosító*&gt;\\ROOT\\ServrSyncWebService
-   %windir%\\Microsoft.NET\\Framework\\v1.1.4322\\\\aspnet\_regiis.exe -s W3SVC\\&lt;*webhely-azonosító*&gt;\\ROOT\\DssAuthWebService
-   %windir%\\Microsoft.NET\\Framework\\v1.1.4322\\\\aspnet\_regiis.exe -s W3SVC\\&lt;*webhely-azonosító*&gt;\\ROOT\\Content

#### 12. probléma: A távoli SQL használatával kapcsolatos korlátok

A WSUS az alábbi megszorításokkal támogatja olyan adatbázisszoftverek használatát, amelyek nem a WSUS szolgáltatást futtató számítógépen működnek.

-   Távoli SQL használata esetén előtér-számítógépként nem alkalmazható Windows 2000 Server operációs rendszerrel működő számítógép.
-   Távoli SQL használata esetén sem előtér-, sem háttérszámítógépként nem alkalmazható tartományvezérlőnek beállított kiszolgáló.
-   Sem WMSDE, sem MSDE nem használható adatbázisszoftverként a háttérszámítógépen.
-   A (WSUS adatbázisaként használandó) távoli SQL kiszolgáló telepítése sikertelen, ha a távoli kiszolgálóra terminálszolgáltatások lettek telepítve, és alkalmazási módban működnek. Amikor a terminálszolgáltatások kiszolgálójára telepít SQL kiszolgálót, a következőt kell tenni:
    1.  A telepítés indítása előtt nyissa meg a parancssort, és írja be: "change user /install"
    2.  Indítsa el az SQL Server telepítését
    3.  A telepítés után írja be a parancssorba: "change user /execute"
-   A WSUS adatbázist távoli SQL kiszolgálóra csak olyan felhasználó telepítheti, aki az előtérbeli és a háttérbeli számítógépen is tagja a helyi Rendszergazdák csoportjának.
-   A távoli SQL használatával kapcsolatban felmerülő problémákról további tájékoztatás található a [Deploying Microsoft Windows Server Update Services](http://go.microsoft.com/fwlink/?linkid=41777) (A Microsoft WSUS szolgáltatás létesítése) dokumentum "Appendix C: Remote SQL" („C” függelék: Távoli SQL) című részében.

#### 13. probléma: Előfordulhat, hogy az alsóbb rétegbeli replikakiszolgálón kevesebb jóváhagyott elem található, mint a felsőbb rétegbeli szülőkiszolgálón

Előfordulhat, hogy az alsóbb rétegbeli replikakiszolgálón kevesebb jóváhagyott elem található, mint a felsőbb rétegbeli szülőkiszolgálón. Ennek az az oka, hogy a telepítési jóváhagyások nem jutnak el az alsóbb rétegbeli kiszolgálóhoz mindaddig, amíg a tartalom teljes egészében le nem töltődik a felsőbb rétegbeli kiszolgálóra.

#### 14. probléma: Szinkronizálási hiba esetén meg kell ismételni a szinkronizálást

Ha a szinkronizálás folyamán hiba lép fel, hibaüzenet jelenik meg. Ha több egymást követő szinkronizálás sikertelen, meg kell nézni a WSUS üzemeltetési kézikönyvében a hibaelhárítási eljárásokat.

#### 15. probléma: A WSUS felügyeleti konzolja megnyitására tett kísérlet esetén a következő hibaüzenet jelenik meg: System.IO.FileNotFoundException

Ha az alábbi hibaüzenet jelenik meg, módosítani kell a Hálózatszolgáltatás vagy az ASP.NET fiók engedélyeit:

System.IO.FileNotFoundException: Nem található a(z) *xxxxxx*.dll vagy olyan fájl, illetve szerelvény, ami tőle függ

Az *xxxx* helyén bármilyen név lehet.

A probléma Windows Server 2003 operációs rendszereken való megoldásához a Hálózatszolgáltatás számára adjon írási és olvasási jogosultságot a %systemroot%\\Temp könyvtárhoz. A Windows 2000 Server operációs rendszerben az ASP.NET fióknak adjon írási és olvasási jogosultságot a %systemroot%\\Temp könyvtárhoz.

#### 16. probléma: MS03-031. jelű biztonsági frissítés az SQL programhoz (KB815495)

A WSUS-kiszolgálón ez a frissítés telepítettként jelenhet meg annak ellenére, hogy a telepítés valójában meghiúsult az ügyfélen. A hiba következtében a rendszer ismét felajánlja a csomagot az ügyfélnek. Kerülő megoldásként törölje a frissítés jóváhagyását a kiszolgálón.

#### 17. probléma: Az RTM verzióra való frissítés folyamán elvesznek az IIS beállításai

Ha a WSUS RTM (gyártásra kész) verzióját olyan kiszolgálóra telepíti, amelyen a WSUS egyik előző verziója (például az RC, azaz kiadásra jelölt verzió) fut, az RTM verzió először eltávolítja a korábbi verziót, majd telepíti az újat. Ez azt jelenti, hogy az IIS programban a WSUS-specifikus virtuális gyökerek és fájlok törlődnek.

Ha a WSUS szolgáltatást az alapértelmezett webhelyre telepítette, a WSUS virtuális gyökerekben megadott összes WSUS-specifikus beállítás elvész. Ha például a WSUS biztonsága érdekében a WSUS virtuális gyökereket az SSL használatára beállította, a WSUS RTM verziójának telepítése után ismét meg kell adnia ezeket a beállításokat. Megjegyzés: a WSUS-konzolban értesítés jelenik meg arról, hogy az SSL nincs engedélyezve.

Ha a WSUS szolgáltatást nem az alapértelmezett webhelyre telepítette, hanem valamelyik másikra, akkor a WSUS webhely szintjén megadott összes többi beállítás is elvész.

#### 18. probléma: Állomásfejlécek használata

Ha az IIS programban állomásfejléc-értékeket szeretne rendelni az alapértelmezett webhelyhez (WSUS webhelyhez), akkor az alapértelmezett webhely IP-címlistájába fel kell vennie „Az összes ki nem osztott” elemet, vagy egy állomásfejléc-érték nélküli kiosztott IP-címet. Ezt a nem alapértelmezett webhelyhez is hozzá kell adni

**Figyelem**: A művelet következtében a Microsoft SharePoint és az Exchange működése leállhat.

#### 19. probléma: A WSUS-konzol URL-címét hozzá kell adni a Megbízható helyek és a Helyi intranet webes zónához mindazokon a számítógépeken, amelyeken az Internet Explorer megerősítése engedélyezett

Ha a számítógépen engedélyezett az Internet Explorer megerősítése (azaz a Microsoft Windows Server 2003 Internet Explorer fokozott biztonsági beállításai összetevő), és a WSUS-konzol nem szerepel a Megbízható helyek és a Helyi intranet webes zónában, a rendszer hitelesítő adatokat kér, valahányszor egy lapot megnyit a WSUS-konzolban.

A WSUS-konzol felvétele a **Helyi intranet** és a **Megbízható webhelyek** webes zónák közé:

1.  Nyissa meg az **Internetbeállítások** párbeszédpanelt (például kattintson a **Start** gombra, válassza a **Vezérlőpult** menüpontot, majd kattintson az **Internetbeállítások** parancsra).
2.  A **Biztonság** lapon kattintson a **Helyi intranet** ikonra, kattintson a **Helyek**, majd pedig a **Speciális** gombra, adjon URL-címet a zónához (http://*WSUSServername*/WSUSAdmin), és kattintson az **OK** gombra.
3.  Kattintson a **Megbízható helyek** ikonra, majd a **Helyek** gombra, adja meg a WSUS-konzol URL-címét, kattintson az **OK**, majd újra az **OK** gombra, hogy bezárja az **Internetbeállítások** párbeszédpanelt.

#### Szerzői jog

Az ebben a dokumentumban szereplő információ a Microsoft Corporation a kiadás napján érvényes véleményét tükrözi a tárgyalt kérdésekről. Mivel a Microsoftnak reagálnia kell a változó piaci feltételekre, a dokumentum nem értelmezhető a Microsoft részéről tett elkötelezettségként, és a Microsoft nem garantálhatja a kiadás dátuma után megjelenő információ pontosságát.

Ez a dokumentum kizárólag tájékoztató jellegű. A MICROSOFT A JELEN DOKUMENTUM TARTALMÁVAL KAPCSOLATBAN NEM VÁLLAL SEMMILYEN KIFEJEZETT, BELEÉRTETT VAGY TÖRVÉNYES GARANCIÁT.

Az összes vonatkozó szerzői jogi törvény betartása a felhasználó felelőssége. A szerzői jogi törvények által biztosított jogokat nem korlátozva, a Microsoft Corporation külön írásos engedélye nélkül a jelen dokumentum egyetlen része sem reprodukálható, tárolható vagy helyezhető el dokumentum-visszakereső rendszerben, illetve nem adható tovább semmilyen célból, semmilyen formában, illetve semmilyen elektronikus, mechanikus, fénymásolási, rögzítési vagy más úton.

A jelen dokumentumban foglaltakra a Microsoft szabadalmai, bejegyzés előtt álló szabadalmai, védjegyei, szerzői jogai vagy más szellemi tulajdont érintő jogai vonatkozhatnak. Jelen dokumentum átadása semmilyen licencet nem biztosít a felhasználó számára e szabadalmakra, védjegyekre, szerzői jogokra, illetve más szellemi alkotásra, kivéve a Microsoft által kiadott bármely írásos licencszerződésben kifejezetten engedélyezett eseteket.

Az itt leírt, példaként említett társaságok, szervezetek, termékek, tartománynevek, e-mail címek, emblémák, személyek, helyek és események kitaláltak. Valamely létező társasággal, szervezettel, termékkel, tartománynévvel, e-mail címmel, emblémával, személlyel, hellyel vagy eseménnyel fennálló mindennemű kapcsolat a véletlen műve, hacsak másképpen nincs jelezve.

© 2006. Microsoft Corporation. Minden jog fenntartva.

A Microsoft, az SQL Server, a Windows és a Windows Server a Microsoft Corporation védjegye vagy bejegyzett védjegye az Egyesült Államokban és/vagy más országokban.

Az itt említett tényleges vállalat- és terméknevek azok tulajdonosainak védjegyei lehetnek.
