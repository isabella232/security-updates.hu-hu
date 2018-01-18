---
TOCTitle: A tanúsítást és a licencelést biztosító kiszolgálók hozzáadása
Title: A tanúsítást és a licencelést biztosító kiszolgálók hozzáadása
ms:assetid: '089ceb62-2a96-444f-ab42-1d5deaabd0c3'
ms:contentKeyID: 18122484
ms:mtpsurl: 'https://technet.microsoft.com/hu-hu/library/Cc720189(v=WS.10)'
---

A tanúsítást és a licencelést biztosító kiszolgálók hozzáadása
==============================================================

Miután az első kiszolgáló telepítésével és létesítésével létrehozta az RMS legfelső szintű telepítését, további kiszolgálókat is üzembe helyezhet, amelyek segítségével magasabb színvonalon biztosíthatók a tanúsítási és a licencelési szolgáltatások:

-   Újabb kiszolgáló hozzáadásával legfelső szintű tanúsítási fürtöt hozhat létre, amely fokozza a tanúsítási és licencelési szolgáltatás megbízhatóságát. A fürthöz hozzáadott kiszolgálók ugyanazt a konfigurációt és ugyanazokat az adatbázisokat használják, mint a legfelső szintű tanúsítási kiszolgáló.
-   Külön licenckiszolgáló is üzembe helyezhető önállóan vagy licenckiszolgálói fürt tagjaként. Ez aligénylést nyújt be a legfelső szintű tanúsítási kiszolgálóhoz, és kiszolgálói licencelői tanúsítványát (SLC) a legfelső szintű tanúsítási kiszolgáló tanúsítási szolgáltatásain keresztül kapja. A licenckiszolgáló a hozzá benyújtott tanúsítási kérelmeket továbbítja a tanúsítási kiszolgálónak. A licenckiszolgáló anélkül képes használati és közzétételi licenceket kiállítani, hogy a kérelmet be kellene nyújtania a legfelső szintű tanúsítási kiszolgálónak.

A bevezetett megoldás kiválasztásánál figyelemmel kell lenni a szervezet méretére, a szükséges redundanciára, a skálázási igényekre, a terheléselosztásra és a biztonságra. Ha a tanúsítás, licencelés és közzététel iránti igény fokozódásával további RMS kiszolgálók üzembe helyezése válik szükségessé, akkor azokat a legfelső szintű tanúsítási kiszolgáló részeként célszerű üzembe helyezni, mert így redundáns, terheléselosztásos megoldás alakítható ki. A tanúsítási kiszolgálók fürtbe szervezhetők, és a licencelési és közzétételi szolgáltatások feldolgozásából adódó terhelés licenckiszolgálók aligénylésével csökkenthető (ez a terheléselosztáshoz szintén fürtözhető), de aligénylési licencelési fürt és a legfelső szintű tanúsítási fürt között nem alakítható ki terheléselosztás.

A következő témakörök részletes útmutatást tartalmaznak erről:

-   [A telepítéshez és a létesítéshez szükséges szerepek, engedélyek és jogok](#bkmk_1)
-   [A további tanúsítási és licenckiszolgálók létesítési folyamata](#bkmk_2)
-   [A fürtök és a terheléselosztás beállítása](#bkmk_3)

<span id="BKMK_1"></span>
A telepítéshez és a létesítéshez szükséges szerepek, engedélyek és jogok
------------------------------------------------------------------------

A további kiszolgálók telepítéséhez és létesítéséhez ugyanazokra a szerepkörökre, engedélyekre és jogokra van szükség, mint az első kiszolgálóéhoz. Emellett engedélyt kell szerezni a legfelső szintű tanúsítási kiszolgálótól külön licenckiszolgáló létesítéséhez. Ezt nevezzük aligénylésnek. A legfelső szintű tanúsítási kiszolgálóhoz való hozzáférést a SubEnrollService.asmx fájl tulajdonosi hozzáférés-szabályozási listája (DACL) határozza meg. Az RMS szolgáltatás csoport, amelynek tagja a legfelső szintű tanúsítási kiszolgáló létesítésekor megadott RMS-szolgáltatásfiók, rendelkezik az aligénylés végrehajtásához szükséges engedéllyel. A további tudnivalókat lásd „[A tanúsítási és a licencelési szolgáltatás beállítása az első kiszolgálón](https://technet.microsoft.com/cce29a2f-984f-48ed-9187-0eb68286ec5b)” című pontban.

<span id="BKMK_2"></span>
A további tanúsítási és licenckiszolgálók létesítési folyamata
--------------------------------------------------------------

A kiszolgálók tanúsítási és licencelési fürtbe történő felvétele alkalmával a kiszolgálónak át kell esnie a létesítési folyamaton. A létesítési folyamat menete attól függ, hogy milyen típusú kiszolgáló létesítése történik.

-   Ha külön licenckiszolgálót létesít, a legfelső szintű tanúsítási kiszolgáló létesítéséhez hasonló módon meg kell adnia a konfigurációs adatbázist, az RMS szolgáltatásfiókját, a fürt URL-címét, valamint a személyes kulcs védelmével kapcsolatos információkat. Nem szükséges viszont megadni a kiszolgálói licencelői tanúsítvány visszavonási szabályzatát, ekkor ezt a szabályzatot a legfelső szintű tanúsítási kiszolgáló határozza meg.
-   Ha egy kiszolgálót fürt tagjaként létesít, a létesítés során csak az RMS szolgáltatásfiókját, a konfigurációs adatbázist és a személyes kulcsot védő jelszót (itt használható a meglévő fürtével megegyező CSP és személyes kulcs is) kell megadni. Az azonos fürtbe tartozó kiszolgálók ugyanazt a kiszolgálói licencelői tanúsítványt és kiszolgálói kulcspárt használják.

> [!IMPORTANT]  
> Addig ne kezdje el az RMS szolgáltatást más kiszolgálókra telepíteni, amíg az első kiszolgálón üzembe nem helyezte a szolgáltatást, a telepítést és a létesítést is beleértve. 

Az újabb kiszolgáló telepítése és létesítése után automatikusan tagjává válik a fürtnek. Ha viszont terheléselosztás is működik, akkor a terheléselosztó szoftvert be kell állítani, hogy az új kiszolgálóval is működjön.

<span id="BKMK_3"></span>
A fürtök és a terheléselosztás beállítása
-----------------------------------------

Az RMS kialakításánál fogva alkalmas a kiszolgálók fürtözésére. Az RMS kiszolgálók fürtözésével skálázhatóbb, megbízhatóbb, terheléselosztással működő RMS rendszer alakítható ki.

**Fürtök létrehozása**

A fürt létrehozásának első lépése egy legfelső szintű tanúsítási kiszolgáló vagy egy licenckiszolgáló üzembe helyezése. A fürtöt alkotó második kiszolgáló és a további kiszolgálók esetében telepíteni kell a kiszolgálóra az RMS szolgáltatást. Ezt követően a **Globális felügyelet** lap **A kiszolgáló hozzáadása egy fürthöz** hivatkozását használva létesíteni kell a szükséges erőforrásokat, és csatlakoztatni kell a fürtöt egy legfelső szintű tanúsítási kiszolgálóhoz vagy egy licencelési fürthöz.

Ehhez a kívánt fürt adatbázisának nevét kell megadni.

**A fürtök terhelésének elosztása**

Az RMS automatikusan nem alkalmaz terheléselosztást. Az RMS kiszolgálókra háruló terhelés azonban hardveres vagy szoftveres terheléselosztás (például hálózati terheléselosztás) segítségével megosztható.

Az alábbi témakörök részletesebben ismertetik ezt a területet:

-   A tanúsítási és a licencelési szolgáltatás közötti különbségről a további tudnivalókat lásd a dokumentumgyűjtemény „RMS műszaki források” részében „Az RMS rendszer áttekintése” témakörben.
-   A bevezetett kiszolgálók és a szervezet rendelkezésre állási és teljesítménykövetelményei közötti összhang eléréséről a további tudnivalókat lásd a dokumentumgyűjtemény „RMS bevezetésének tervezése” részében a „Redundancia és terheléselosztás biztosítása” témakörben.
-   A szervezeten belül az RMS működtetéséhez szükséges kiszolgálók számának meghatározásáról a további tudnivalókat lásd a dokumentumgyűjtemény „RMS bevezetésének tervezése” részében „A skálázási követelmények felmérése” témakörben.
-   Az RMS bevezetésének informatikai szempontú védelmének kialakításáról a további tudnivalókat lásd „[Az RMS bevezetésének védelme](https://technet.microsoft.com/6de8b636-a824-4844-aefc-f26347abfc14)” pontban.
-   Az RMS telepítéséről a további tudnivalókat lásd a dokumentumgyűjtemény „RMS kiszolgáló működtetése” részében „A Service Pack 1 csomaggal frissített RMS telepítése” témakörben.
    Az RMS telepítése a parancssorból is végrehajtható. A további tudnivalókat lásd a dokumentumgyűjtemény „RMS kiszolgáló működtetése” részében „Az RMS telepítése a parancssorból” témakörben.
-   Licenckiszolgáló létesítéséről a további tudnivalókat lásd a dokumentumgyűjtemény „RMS kiszolgáló működtetése” részében a „Licenckiszolgáló létesítése” témakörben.
-   Fürtbe tartozó további kiszolgálók létesítéséről a további tudnivalókat lásd a dokumentumgyűjtemény „RMS kiszolgáló működtetése” részében a „Kiszolgáló felvétele fürtbe” témakörben.
