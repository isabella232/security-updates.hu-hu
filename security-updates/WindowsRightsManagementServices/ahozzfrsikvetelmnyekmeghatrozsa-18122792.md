---
TOCTitle: A hozzáférési követelmények meghatározása
Title: A hozzáférési követelmények meghatározása
ms:assetid: 'eb2ce9a5-0430-4811-bd40-4a94a84426a8'
ms:contentKeyID: 18122792
ms:mtpsurl: 'https://technet.microsoft.com/hu-hu/library/Cc747790(v=WS.10)'
---

A hozzáférési követelmények meghatározása
=========================================

A tervezési szakasz ezen részében az RMS megvalósításának hatókörét kell azonosítani. Az RMS rendszer biztonságának értékelésekor olyan módszereket kell megfontolni, amelyekkel adott résztvevőkre korlátozható a hatókör, és a hagyományos gyakorlati tanácsok alkalmazásával biztosítani kell az általuk az RMS szolgáltatással védett adatok biztonságát. Gondoskodni kell arról is, hogy az RMS kiszolgáló felügyeletét és konfigurálását csak a megbízható rendszergazdák hajthassák végre. Az RMS rendszerrel használható biztonsági módszerek közé a következők tartoznak:

-   **Hozzáférés-szabályozási listák (ACL)**. Az RMS webszolgáltatásainak mindegyike és a felügyeleti webhely is védhető hozzáférés-szabályozási listákkal (ACL). Annak biztosításához, hogy csak a jogosult felhasználók férhessenek hozzá az RMS szolgáltatáshoz, hozzáférés-szabályozási listákkal korlátozhatja az RMS tanúsítási és licencelési szolgáltatásainak elérését. Ez hasznos lehet akkor is, ha csak adott csoportoknak engedélyezi védett tartalom létrehozását, illetve csak adott csoportoknak teszi lehetővé licencek beszerzését a védett tartalomhoz.
-   **Ügyfél-hitelesítés**. Előírhatja intelligens kártyák vagy más ügyfél-hitelesítési módszer használatát, amikor a felhasználók használati licencet vagy tanúsítványt igényelnek. Ezzel csökkenthető az a lehetséges veszély, hogy jogosulatlan felhasználó jogosulatlan munkamenetben védett tartalmaz nyisson meg.
-   **Secure Sockets Layer**. A védelem további rétegének bevezetéséhez SSL-kapcsolatot írhat elő az RMS ügyfelek és az RMS kiszolgáló között. Azt ajánljuk, hogy az RMS webszolgáltatások minden fájlján engedélyezze és követelje meg a 128 bites titkosítású SSL protokollt. Ezeknek a fájloknak .asmx a kiterjesztése, és a Licensing, a Certification és az Admin virtuális könyvtárban találhatók. Ha távoli számítógépen lévő böngészőből szeretné megnyitni az **RMS felügyeleti weblapjait,** engedélyeznie kell az SSL szolgáltatást. A **Globális felügyelet** lapot azonban még az SSL engedélyezésekor sem nyithatja meg távoli számítógépről.
    Az SSL konfigurálásáról lásd az IIS súgóját.

Egyes szervezeteknél igény lehet részlegekhez tartozó licencelési rendszer kialakítására, amely el van különítve a többi részlegtől, és megfelelően védett. Az RMS kiszolgáló az ilyen esetek kezelésére is alkalmas, és lehetőséget nyújt tartalomvédelmi szabályzatok kialakítására. Ha a szervezeten belül olyan részleg vagy más egység működik, amely szigorúan titkos anyagokkal dolgozik, érdemes lehet külön licenckiszolgálót vagy licencelési fürtöt létrehozni a számára, hogy a szervezet többi részétől függetlenül kezelhessék a licencelést és a közzétételt. A licenckiszolgálók aligényléssel szereznek tanúsítványt a legfelső szintű tanúsítási kiszolgálótól (vagy fürttől), amely biztosítja a licencelési kiszolgálóknak a tanúsítási és az egyéb szolgáltatásokat. A licenckiszolgálók azonban maguk is nyújtanak saját licencelési és közzétételi szolgáltatást.

A bevezetés létfontosságú részét alkotják a felhasználói fiókok, a hozzáférés-szabályozási listák (ACL) és a fizikai védelem. Mielőtt éles környezetben bevezetné az RMS szolgáltatást, feltétlenül értékelje ki és alkalmazza a biztonsággal kapcsolatos gyakorlati tanácsokat, valamint szükség szerint a szervezet biztonsági modelljét.
