---
TOCTitle: Az RMS felügyeletével kapcsolatos kérdések
Title: Az RMS felügyeletével kapcsolatos kérdések
ms:assetid: '43f77336-5e62-4405-9efb-55417a402d62'
ms:contentKeyID: 18122560
ms:mtpsurl: 'https://technet.microsoft.com/hu-hu/library/Cc747547(v=WS.10)'
---

Az RMS felügyeletével kapcsolatos kérdések
==========================================

Az RMS felügyeletével kapcsolatos kérdések
------------------------------------------

-   [Mi a leghelyesebb módja a megfelelő dokumentumokra vonatkozó engedélyek visszavonásának, amikor egy felhasználó kilép a szervezettől?](#bkmk_1)
-   [Az RMS-védelemmel ellátott tartalom közös használatához két szervezet közötti bizalmi kapcsolat kialakításakor igényel-e különös kezelést az átadott XrML licenctanúsítvány?](#bkmk_2)
-   [Hogyan működik együtt az RMS a központi felhasználói profilokkal?](#bkmk_3)
-   [Mikor válhat szükségessé az RMS leszerelése egy szervezetnél?](#bkmk_4)
-   [Miből áll a leszerelési eljárás?](#bkmk_5)
-   [Leszerelhető-e az RMS úgy, hogy csak néhány felhasználó állíthassa helyre a dokumentumokat?](#bkmk_6)
-   [Mit jelent az alkalmazás könyvtárának elérhetetlenségére vonatkozó hibaüzenet?](#bkmk_7)
-   [Használható-e nyomkövetés az RMS kiszolgálóval?](#bkmk_8)
-   [Mit jelent az órák közötti eltérés és hogyan kezelhető?](#bkmk_9)

#### Mi a leghelyesebb módja a megfelelő dokumentumokra vonatkozó engedélyek visszavonásának, amikor egy felhasználó kilép a szervezettől?

Általában az a leghelyesebb, ha a dokumentumok licencelése nem egyes felhasználói fiókokra, hanem az Active Directoryban megadott csoportokra történik. Ez azért javasolt, mert így egy felhasználó kilépésekor eltávolíthatja őt az Active Directory-csoportból, így nem olvashatja a csoportnak küldött dokumentumokat. A felhasználó azonban továbbra is olvashatja a meglévő használati licencekkel rendelkező dokumentumokat, ha a dokumentum jogai nem úgy vannak beállítva, hogy a felhasználónak a dokumentum minden megnyitásakor használati licencet kell szereznie. Ha ez a szabály nem lett megadva, a meglévő használati licencekkel rendelkező dokumentumok olvasása csak úgy akadályozható meg, hogy a felhasználó számítógépén törli a licenctárat.

#### Az RMS-védelemmel ellátott tartalom közös használatához két szervezet közötti bizalmi kapcsolat kialakításakor igényel-e különös kezelést az átadott XrML licenctanúsítvány?

Megbízható felhasználói tartomány vagy megbízható közzétételi tartomány létesítésekor azt választja, hogy megbízik a partnerszervezetben, így az részt vehet tartalomvédelmi rendszerében. Ily módon bizonyos kockázatot vállal, hiszen ez a bizalmi kapcsolat alapján veszélybe kerülhetnek adatai. Gyakorlati tanács: kérje meg a másik szervezetet, hogy hitelesített csatornán (például S/MIME e-mail üzenetben) küldje el saját kiszolgálói licencelői tanúsítványát, így csökkenthető annak kockázata, hogy a kiszolgálói licencelői tanúsítványt RMS kiszolgálójára importálás előtt meghamisítottak.

#### Hogyan működik együtt az RMS a központi felhasználói profilokkal?

A felhasználók azonosításához használt tartalomvédelmi fióktanúsítványok (RAC) számítógéphez kötöttek. Központi felhasználói profilok használatakor az RMS adott számítógépen való első indítása új tartalomvédelmi fióktanúsítványt hoz létre a számítógép felhasználója számára.

#### Mikor válhat szükségessé az RMS leszerelése egy szervezetnél?

Az RMS leszerelése eltávolítja az RMS kiszolgálót az infrastruktúrából, és lehetővé teszi a felhasználóknak hogy RMS-védelem ellátott tartalmat védelem nélkül mentsék. Erre három alapvető okból kerülhet sor a szervezeteknél:

-   Az architektúra egyszerűsítése, például kiszolgálók összevonása fürtbe.
-   Próbaüzemi RMS-bevezetés áttelepítése éles környezetbe.
-   RMS kiszolgálók egyesítése például vállalatok egyesítésekor.

#### Miből áll a leszerelési eljárás?

A leszerelési eljárás első lépése a szolgáltatás engedélyezése az RMS legfelső szintű fürtjéről. Amikor a leszerelési szolgáltatás engedélyezve van, az összes egyéb szolgáltatás (például licencelés és tanúsítás) tiltva lesz. Ezután valamennyi RMS-kompatibilis alkalmazást úgy kell beállítani, hogy a leszerelési szolgáltatáshoz kapcsolódjanak, amikor az RMS valamelyik funkcióját használják. A Microsoft Office 2003 például RMS-kompatibilis alkalmazás. Az Office 2003 alkalmazásaiban az RMS-ügyfél RMS szolgáltatásokra irányítása rendszerleíró kulcsokkal történik. Az egyik ilyen rendszerleíró kulcs a leszerelési szolgáltatást azonosítja. Amikor a kulcs beállítása olyan, hogy az ügyfelet a leszerelési szolgáltatásra irányítja, az RMS fürt az összes engedélyt (olvasás, írás, másolás, nyomtatás, szerkesztés stb.) tartalmazó használati licencet ad a felhasználóknak függetlenül attól, hogy eredetileg milyen engedélyekkel rendelkeztek. A felhasználóknak ekkor el kell távolítaniuk az összes tartalomvédelmet minden olyan dokumentumból, amelyet a leszerelés végrehajtása után meg kívánnak tartani. Miután ez megtörtént, az RMS fürt véglegesen üzemen kívül helyezhető.

Gyakorlati tanács: célszerű biztonsági másolatot készíteni az RMS fürt konfigurációs adatbázisáról arra az esetre, ha a fürt üzemen kívül helyezése után vissza kell állítani egy tartalomvédelemmel ellátott dokumentumot. Az RMS legfelső szintű fürtjének személyes kulcsa nélkül csak a dokumentum szerzője képes megnyitni a tartalomvédelemmel ellátott dokumentumot a kiszolgáló eltávolítása után.

#### Leszerelhető-e az RMS úgy, hogy csak néhány felhasználó állíthassa helyre a dokumentumokat?

Hozzáférés-szabályozási listát (ACL) alkalmazhat a leszerelési webszolgáltatásra (decommission.asmx), így csak adott felhasználók szerezhetik meg a visszafejtő kulcsot a védelemmel ellátott tartalomhoz.

#### Mit jelent az alkalmazás könyvtárának elérhetetlenségére vonatkozó hibaüzenet?

Ez a hiba az RMS telepítése után az RMS felügyeleti webhelyének első megnyitásakor fordulhat elő. Ekkor nem fogja tudni konfigurálni és felügyelni az RMS rendszert.

A hibaüzenet általában akkor jelenik meg, ha az Internet Information Services (IIS) az IIS 5.0-s verzió elkülönítési üzemmódjában fut. A probléma megoldásához a következő eljárással tiltsa ezt a beállítást a kiszolgálón, és indítsa újra az IIS szolgáltatást.

**Az IIS 5.0-s elkülönítési üzemmódjának tiltása**
1.  Jelentkezzen be az RMS kiszolgálóra a helyi Rendszergazdák csoport tagjaként.

2.  Mutasson a **Start** menü **Felügyeleti eszközök** pontjára, majd kattintson az **Internet Information Services (IIS) kezelője** parancsra.

3.  Az **IIS-kezelőben** bontsa ki a helyi számítógép csomópontja alatti ágakat, kattintson a jobb gombbal a **Webhelyek** csomópontra, és válassza a **Tulajdonságok** parancsot.

4.  A **Szolgáltatás** lapon törölje **A webszolgáltatás futtatása az IIS 5.0-s verziójának elkülönítési üzemmódjában** négyzet jelölését, majd kattintson az **OK** gombra.

5.  A változtatás érvénybe léptetéséhez újra kell indítani az IIS szolgáltatást. Az IIS szolgáltatás újraindítását kérő üzenetpanelen kattintson az **Igen** gombra.

#### Használható-e nyomkövetés az RMS kiszolgálóval?

Mivel az RMS a Microsoft® .NET-keretrendszer segítségével készült, így a nyomkövetés engedélyezésével egyszerűbbé tehető a rendszeresemények visszakeresése és a problémák elhárítása.

A nyomkövetés a Web.config vagy a Machine.config fájl módosításával valósítható meg. Ha a Machine.config fájlban kapcsolja be a nyomkövetést, az a számítógépen lévő összes szoftverösszetevőt érinti, ha viszont a Web.config fájlban hajtja ezt végre, akkor csak a webszolgáltatásokban bekövetkező eseményekre vonatkozik.

**A nyomkövetés engedélyezése**
1.  Nyissa meg a Machine.config vagy a Web.config fájlt, és vegye fel a következő sorokat a fájl &lt;system.diagnostics&gt; szakaszába:

    
        ```
2.  Indítsa újra az IIS szolgáltatást az IISRESET paranccsal a parancssorból.

3.  Miután hozzájutott a szükséges adatokhoz, törölje az 1. lépésben a .config fájlban elhelyezett sorokat.

4.  Indítsa újra az IIS szolgáltatást az IISRESET paranccsal a parancssorból.

> [!IMPORTANT]  
> Ha bekapcsolja a nyomkövetést egy RMS kiszolgálón, csökkenhet a kiszolgáló teljesítménye: tovább tarthat például a licencigénylés és a tartalomvédelmi fióktanúsítványok kiállítása. Csak kifejezetten indokolt esetben használja a nyomkövetést fennálló problémák diagnosztizálására és elhárítására. 

#### Mit jelent az órák közötti eltérés és hogyan kezelhető?

Előfordulhat, hogy az egyik számítógép órája más időt mutat, mint a másiké. Ez egyáltalán nem ritka eset: egy helyiségen belül aligha találni két olyan embert, akinek pontosan ugyanannyit mutatna az órája. Az ilyen időkülönbség azonban problémákat okozhat, ha a licencekben érvényességi idő van megadva.

A licencekben az érvényességi idő beállítása mindig a közzétevő órája szerint történik. Az órák közötti eltérés két esetben okozhat problémát a közzététel és a használat során:

-   Amikor egy alkalmazás olyan közzétételi licenccel próbál meg használati licencet szerezni, amelynek az érvényességi ideje az RMS kiszolgáló órája szerint a múltban ért véget, vagy csak a jövőben kezdődik el. Ebben az esetben sikertelen lesz a kérelem. Ez megtörténhet végfelhasználókkal, amikor licencet kérelmeznek, valamint alkalmazásokkal, amikor előlicencet próbálnak meg kérelmezni egy dokumentumhoz (vagyis egy felhasználó nevében próbálnak meg licencet szerezni).
-   Ha már lejárt (vagy még nem kezdődött el) a licenc érvényességi ideje, sikertelen lesz a használati licenc iránti kérelem. Más esetben csak a lejárt (vagy még nem érvényes) jogok nem lesznek használhatók.

Ha például a közzétevő számítógép órája 15 percet késik a tartalmat felhasználó számítógépéhez képest, és a közzétevő egy 15 percig érvényes licencet készít, a felhasználó értéktelen használati licencet kap a kiszolgálótól, hiszen a tartalom megtekintésére adott jogok már lejártak.

Az órák közötti eltérésekre nincs tökéletes megoldás. Jó megoldás, hogy a jogok érvényességének kezdetét korábbira állítja az aktuális időnél, hogy azok is használni tudják a licencet, akiknek késik az órája, illetve hosszabb érvényességi időt ad meg, hogy azok is használni tudják a licencet, akinek siet az órája. Célszerű figyelemmel lenni erre a lehetséges problémára, különösen a rövid érvényességi idejű licencek létrehozásakor.
