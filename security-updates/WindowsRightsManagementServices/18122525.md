---
TOCTitle: Bizalmi hierarchia
Title: Bizalmi hierarchia
ms:assetid: '2d44182f-a653-4383-aba1-dade53f7cf9a'
ms:contentKeyID: 18122525
ms:mtpsurl: 'https://technet.microsoft.com/hu-hu/library/Cc720232(v=WS.10)'
---

Bizalmi hierarchia
==================

Az RMS rendszert több összetevő alkotja: a Microsoft igénylési szolgáltatása, a szervezet RMS kiszolgálói, ügyfélszámítógépek, valamint a rendszer felhasználói. Mindegyik összetevő egy tanúsítványt kap, amely igazolja a rendszeren belül az összetevő identitását. A tanúsítványok, egyúttal az őket birtokló entitások közötti bizalmi viszonyokat egy bizalmi hierarchia határozza meg. Ez határozza meg a megbízható entitások és az általuk más megbízható entitások részére kibocsátott licencek közötti bizalmi kapcsolatokat is.

A bizalmi hierarchia bizalmi láncba köti a tanúsítványokat és a licenceket. Ezt az RMS mindig végig tudja követni egy adott tanúsítványtól vagy licenctől kezdve föl egészen egy megbízható kulcspárig. A bizalmi lánc a következőkből áll: az adott tanúsítvány, az ezt kiállító entitás tanúsítványa, az ennek az entitásnak a tanúsítványát kibocsátó entitás tanúsítványa, és így tovább, végig a láncon, föl egészen a bizalomforrásig.

Az RMS esetében a Microsoft egy kulcspárja szolgál bizalomforrásul, más szóval a bizalom gyökeréül. Ez a közös bizalomforrás lehetővé teszi a szervezetek számára egy olyan bizalmi ökoszisztéma kiépítését, amely minden, a szervezeten belüli és kívüli megbízható entitást (felhasználókat, partnereket) magában foglal.

Az alábbi ábra az egy szervezeten belüli bizalmi hierarchiát mutatja be. A bizalmi lánc visszanyúlik egészen az alaptanúsítványokat kiállító Microsoft-szolgáltatásokig.

![](images/Cc720232.6c169175-94fb-4ec0-93bc-12748aae3ac4(WS.10).gif)
1.  Minden ügyfélszámítógép kap egy egyedi kulcstárolót, amely tartalmazza a Microsoft legfelső szintű nyilvános kulcsát.
2.  Amikor az RMS licenckérelmet kap, úgy ellenőrzi a résztvevők érvényességét, hogy végigköveti a bizalmi hierarchiát egészen a bizalomforrásig.
3.  Az RMS ellenőrzi a licencben megnevezett megbízható entitás hitelességét.
4.  Az RMS ellenőrzi, hogy a megbízható entitás tanúsítványát a bizalmi hierarchiába tartozó kiszolgáló állította-e ki.

Az RMS a tanúsítványlánc mindegyik szintjén ellenőrzi a licenc vagy a tanúsítvány érvényességét, majd a bizalmi láncon végighaladva ellenőrzi, hogy a tanúsítvány ismert bizalomforrásból származik-e. Az RMS a láncba tartozó valamennyi licencnél vagy tanúsítványnál meggyőződik az alábbi feltételek fennállásáról:

-   Érvényes XrML-szöveget tartalmaz.
-   Érvényes a kiállító aláírása.
-   A licenc szemantikai szempontból jól tükrözi a szándékolt felhasználási célt.
-   Teljesülnek a feltételek (például az érvényességi dátumok).
-   A licencet még nem vonták vissza.
-   A licencet aláíró kulcs és a kiállító tanúsítvány kulcsa azonos.
