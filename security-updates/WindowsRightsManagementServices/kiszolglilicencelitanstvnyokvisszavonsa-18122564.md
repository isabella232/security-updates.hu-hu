---
TOCTitle: Kiszolgálói licencelői tanúsítványok visszavonása
Title: Kiszolgálói licencelői tanúsítványok visszavonása
ms:assetid: '8020861d-d196-4431-8282-044675ef5616'
ms:contentKeyID: 18122564
ms:mtpsurl: 'https://technet.microsoft.com/hu-hu/library/Cc747578(v=WS.10)'
---

Kiszolgálói licencelői tanúsítványok visszavonása
=================================================

Az RMS kiszolgáló biztonságának sérülésével fenyegető, előre nem látható körülmények bekövetkezésekor szükségessé válhat a kiszolgálói licencelői tanúsítványok visszavonása. A nem hardveres biztonsági modulban tárolt személyes kulcs illetéktelen hozzáférésnek van kitéve. A kiszolgálói licencelői tanúsítvány és kulcs megsérülhet egy szervezetnél úgy, hogy egy támadó hozzáfér a kiszolgálóhoz, vagy egy elégedetlen dolgozó lemásolja vagy eltávolítja a tanúsítványt vagy a kulcsot. A visszavonás a kárelhárítás és a tisztességtelen felhasználás korlátozásának egyik módja.

Alapértelmezés szerint minden licencet vagy tanúsítványt a kiállító résztvevő vonhat vissza. Mivel a védett tartalommal kapcsolatos licenceket és tanúsítványokat az RMS kiszolgálók állítják ki, szükség szerint bármikor visszavonhatja azokat. Ha a licenckiszolgáló biztonsága megsérül, visszavonhatja annak kiszolgálói licencelői tanúsítványát. Ha visszavonja egy kiszolgáló licencelői tanúsítványát, az ezzel a kiszolgálóval kiállított összes tanúsítvány és licenc érvénytelenné válik. A licencek és a tanúsítványok visszavonását „[A visszavonás megvalósítása](https://technet.microsoft.com/4735f060-7197-4ae2-830a-f91bcc4de30a)” című pont ismerteti.

A legfelső szintű tanúsítási fürt azonban különleges eset. A legfelső szintű tanúsítási fürt számára a kiszolgálói licencelői tanúsítványt a Microsoft igénylési szolgáltatása állítja ki, és alapértelmezés szerint csak a Microsoft igénylési szolgáltatása vonhatja vissza ezt a kiszolgálói licencelői tanúsítványt.

A Microsoft csak akkor tudja visszavonni egy legfelső szintű tanúsítási kiszolgáló kiszolgálói licencelői tanúsítványát, ha ehhez bírósági végzést mutatnak be, és benyújtják a bíróság kiszolgálójának nyilvános kulcsát. Amikor a Microsoft értesíti a visszavonási végzés kiadásáról, a Microsoft megadja a kiszolgáló nyilvános kulcsát a visszavonási listájában, majd nyilvánosan hozzáférhetővé teszi a listát. Abban az esetben kérhet a bíróságtól visszavonási végzést, ha az alábbiak valamelyike igaz arra a kiszolgálóra, amelynek vissza kell vonni a licencét:

-   Ön a kiszolgáló tulajdonosa, és sérült a kiszolgáló személyes kulcsának biztonsága.
-   Ön a kiszolgáló által közétett tartalom tulajdonosa, és a kiszolgáló az Ön szerzői jogainak megsértésével teszi közzé a tartalmat.

Legfelső szintű tanúsítási kiszolgáló visszavont kiszolgálói licencelői tanúsítványát tartalmazó Microsoft visszavonási lista beszerzésének és közzétételének lépéseit „[A visszavonási listák alkalmazása](https://technet.microsoft.com/e331338b-66d4-45e4-8d3f-acccf2302ac4)” című pont mutatja be.

Legfelső szintű tanúsítási kiszolgáló létesítésekor megadhat olyan nyilvános kulcsot, amely jogosult a legfelső szintű fürt kiszolgálói licencelői tanúsítványának visszavonására. Ez a kulcs a szervezethez vagy külső félhez is tartozhat. A kiszolgálói licencelői tanúsítványt a megfelelő személyes kulccsal aláírt visszavonási lista vonhatja vissza.

A legfelső szintű tanúsítási kiszolgáló licencelői tanúsítványának visszavonásához létrehozhat egy olyan visszavonási listát, amely megnevezi ezt a kiszolgálói licencelői tanúsítványt, a szervezet vagy külső fél személyes kulcsával aláírhatja ezt, majd az összes felhasználónak kioszthatja a visszavonási listát. Az utasításokat lásd „[A visszavonási listák alkalmazása](https://technet.microsoft.com/e331338b-66d4-45e4-8d3f-acccf2302ac4)” rész „Szervezeti visszavonási listák alkalmazása” pontjában.

A visszavonási listán szereplő kiszolgálói licencelői tanúsítvány visszavonásához a következő paraméterek használhatók:

-   **GUID**. A kiszolgálói licencelői tanúsítvány visszavonható globális egyedi azonosítója (GUID) alapján. A paraméter visszavonási listában való használatát lásd a „[Visszavonási listák létrehozása](https://technet.microsoft.com/1ef75199-3344-4225-84de-a863a777696a)” rész „Tanúsítványok és licencek visszavonása GUID alapján” pontjában.

-   **Kivonatérték**. A kiszolgálói licencelői tanúsítvány visszavonható a tanúsítvány törzsrészében lévő Unicode karakterek SHA-1 algoritmussal készített kivonata alapján. A paraméter visszavonási listában való használatát lásd a „[Visszavonási listák létrehozása](https://technet.microsoft.com/1ef75199-3344-4225-84de-a863a777696a)” rész „Tanúsítványok és licencek visszavonása kivonatérték alapján” pontjában.

Egy RMS-telepítés kiszolgálói licencelői tanúsítványát az RMS konfigurációs adatbázisának lekérdezésével kaphatja meg. A következő lépésekkel SQL konfigurációs adatbázisból kérdezheti le ezt az adatot, és böngészővel egyszerűen olvasható fájlba mentheti:

1.  Nyissa meg az SQL Query Analyzer alkalmazást, és kapcsolódjon a legfelső szintű tanúsítási kiszolgáló konfigurációs adatbázisához.

2.  Válassza a **Query** (Lekérdezés) menü **Results in Text** (Szöveges eredmény) parancsát.

3.  A **Tools** (Beállítások) párbeszédpanel megnyitásához válassza az **Options** (Eszközök) menü **Options** (Beállítások) parancsát. A **Results** (Eredmények) lapon, a **Maximum characters per column** (Karakterek maximális száma oszloponként) beállításnál adja meg a **8192** értéket.

4. A Query (Lekérdezés) párbeszédpanelen írja be a következő lekérdezést:

```
select DRMS_XrML_Certificate.s_certificate from DRMS_XrML_Certificate, DRMS_LicensorCertificate, DRMS_ClusterConfiguration where DRMS_ClusterConfiguration.CurrentLicensorCertID = DRMS_LicensorCertificate.i_CertID and DRMS_LicensorCertificate.i_CertificateID = DRMS_XrML_Certificate.i_CertificateID
```

1.  Másolja a **Results** (Eredmények) ablakban lévő eredményt, majd illessze be egy szövegszerkesztő (például a Jegyzettömb) üres dokumentumába. Mentse a dokumentumot egy .xml kiterjesztésű fájlba.

Az adatok visszavonási listában való használatáról a további tudnivalókat lásd a „[Visszavonási listák létrehozása](https://technet.microsoft.com/1ef75199-3344-4225-84de-a863a777696a)” című pontban.

Miután XML-fájlként mentette a kiszolgálói licencelői tanúsítvány adatait, az alábbi lépésekkel nyerheti ki a nyilvános kulcsot:

1.  Nyissa meg a kiszolgálói licencelői tanúsítványt tartalmazó fájlt XML- vagy szövegfájl-szerkesztőben.

2.  Másolja az &lt;ISSUEDPRINCIPALS&gt; szakasz &lt;PUBLICKEY&gt; elemét.

3.  Mentse ezt az információt egy olyan fájlba, amelyet benyújthat a bíróság részére, vagy helyezze el egy szervezeti visszavonási listában.

Miután megtörtént a legfelső szintű tanúsítási fürt kiszolgálói tanúsítványának visszavonása, az RMS-telepítés által kiállított minden tanúsítvány és licenc érvényét veszti olyan tartalom esetében, amely megköveteli a visszavonási lista használatát. Az ilyen tartalom tehát használhatatlanná válik. Ez az eljárás független attól, hogy a felhasználó milyen típusú licenccel rendelkezik. Ha meg szeretné őrizni a visszavont licencű kiszolgáló segítségével közzétett tartalmat, még a visszavonási lista alkalmazása előtt végre kell hajtania a megfelelő műveletet:

-   Mentse a tartalmat RMS-védelem nélkül.

-   Tegye közzé újra a tartalmat úgy, hogy nem követeli meg a visszavonási listát.

Mindkét esetben – a Microsoft és a külső fél által végrehajtott visszavonásnál – a visszavonási lista minden kötési kérelemnél érvényre jut, mivel a használati licenc bizalmi láncába tartozó résztvevő személyes kulcsával írták alá. Ezért sikertelen lesz minden olyan kötési kérelem, amely az RMS-telepítéssel a visszavont kiszolgálói licencelői tanúsítvány alapján kiállított licencet használ.

> [!NOTE]  
> A Microsoft csak akkor vonja vissza a kiszolgálói licencelői tanúsítványt, ha erre bírósági végzés kötelezi. 