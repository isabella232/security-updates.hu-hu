---
TOCTitle: Legfelső szintű tanúsítási kiszolgáló igénylése
Title: Legfelső szintű tanúsítási kiszolgáló igénylése
ms:assetid: '3f69d25e-ecae-447f-b741-a819c8cf6227'
ms:contentKeyID: 18122476
ms:mtpsurl: 'https://technet.microsoft.com/hu-hu/library/Cc720250(v=WS.10)'
---

Legfelső szintű tanúsítási kiszolgáló igénylése
===============================================

Minden RMS-telepítésnek tartalmaznia kell legalább egy legfelső szintű tanúsítási kiszolgálót, de szükség szerint további legfelső szintű tanúsítási kiszolgálókat is tartalmazhat a fürtökben. Az első telepített legfelső szintű tanúsítási kiszolgálót be kell jegyezni a Microsoft igénylési szolgáltatással, így kap legfelső szintű kiszolgálói licencelői tanúsítványt. Ez a tanúsítvány a bizalmi hierarchia alapja az RMS megvalósításaiban.

A legfelső szintű kiszolgálói licencelői tanúsítványok a következő módszerek valamelyikével szerezhetők be. A kívánt módszer az RMS kiszolgáló létesítési adatainak megadásakor választható ki:

-   **On-line igénylés**. Ha a legfelső szintű tanúsítási kiszolgáló rendelkezik internetkapcsolattal, a kiszolgálói licencelői tanúsítvány automatikusan szerezhető be a létesítés során. Ez az alapértelmezett módszer.

-   **Off-line igénylés**. Ha a legfelső szintű tanúsítási kiszolgáló nem csatlakozik az internethez, az igénylést kézzel küldheti el a létesítési folyamat befejezése után. Ehhez az adott kiszolgálón exportálja fájlba az igénylési kérelmet, másolja a fájlt internetkapcsolattal rendelkező számítógépre, majd a kiszolgálói licencelői tanúsítvány beszerzéséhez küldje el azt a Microsoft igénylési szolgáltatásának. Ha a létesítés során off-line igénylést választott, az RMS végrehajtja a létesítési folyamatot, azonban nem lesz használható mindaddig, amíg nem importálja a másik számítógéppel beszerzett kiszolgálói licencelői tanúsítványt. További tudnivalók: „[Legfelső szintű tanúsítási kiszolgáló kézi igénylése](https://technet.microsoft.com/aecdebb5-b28b-4b58-937a-392bb6ce9643)”.

Az igénylési kérelem a következő adatokat tartalmazza:

-   Visszavonási adatok. Megadja, hogy az RMS-telepítés szabványos vagy egyéni (harmadik fél általi) visszavonást fog-e használni. Ha harmadik fél általi visszavonást használ, szerepelni fog a visszavonási hatóság nyilvános kulcsa is.

-   Tanúsítvány nyilvános kulcsa. A kiszolgálói licencelői tanúsítvány nyilvános kulcsa. Ezt a nyilvános kulcsot a rendszer az RMS-kiszolgálón állítja elő, és a kiszolgálói licencelői tanúsítvány beszerzéséhez elküldi a Microsoft igénylési szolgáltatásának.

-   Termékváltozat. Az RMS hivatalos termékváltozata.

-   Verzió. Az RMS termék verziószáma.

-   URL-cím. Az RMS-kiszolgálófürt alapvető URL-címe.

Amikor a Microsoft igénylési szolgáltatása válaszol az igénylési kérelemre, a következő adatokat küldi vissza az RMS kiszolgálónak XML formátumban:

-   Kiszolgálói licencelői tanúsítvány.

-   Az aláíró hatóságok tanúsítványlánca.

A szolgáltatás ugyanezeket az adatokat használja a legfelső szintű RMS tanúsítási kiszolgáló on-line és off-line igénylésénél egyaránt. Más adatokat egyik módszer esetében sem gyűjt.

> [!NOTE]  
> Ha a kapcsolat nélküli igénylési lehetőséget választotta és az internethez kapcsolódáshoz és kiszolgálói licencelői tanúsítvány igényléséhez fokozott böngésző biztonságra konfigurált számítógépet használ – például Windows Server 2003 rendszert vagy a Windows XP Service Pack 2 szervizcsomagot futtató számítógépet –, a kiszolgálói licencelői tanúsítvány letöltésének engedélyezéséhez ne feledje felvenni az Igénylési szolgáltatás webhely URL-címét a Megbízható helyek zónájába. Ez az URL-cím a https://activation.drm.microsoft.com. Ha az off-line igénylési folyamatot használja, ellenőrizze, hogy az igénylési kérelem elküldéséhez használt számítógépen telepítve van-e az összes legújabb tanúsítványfrissítés. A Microsoft igénylési szolgáltatások SSL-tanúsítványa a GTE Cyber Trust Root CA, amely alapértelmezés szerint megbízhatónak számít a Windows Server 2003 rendszerrel működő összes számítógépen. Ha az off-line igénylési folyamatot használja, ügyeljen arra, hogy az RMS ügyfelek az igénylés befejeződéséig ne próbáljanak licencekért az RMS-kiszolgálóhoz kapcsolódni. Ha az ügyfelek még nem bejegyzett RMS kiszolgálóhoz próbálnak csatlakozni, a webszolgáltatások olyan hibaállapotba kerülnek, amely működésképtelenné teszi azokat. Ha nem tudja biztosítani, hogy az ügyfelek ne kapcsolódjanak az RMS-kiszolgálóhoz, a legjobb, ha az igénylést követően az IIS alaphelyzetbe állításával megszünteti az esetlegesen bekövetkező hibaállapotokat.