---
TOCTitle: Az alapvető összetevők azonosítása
Title: Az alapvető összetevők azonosítása
ms:assetid: 'c9ec225b-0e51-42f5-aff6-0aecb62e3b27'
ms:contentKeyID: 18122753
ms:mtpsurl: 'https://technet.microsoft.com/hu-hu/library/Cc747751(v=WS.10)'
---

Az alapvető összetevők azonosítása
==================================

A megfelelő topológia kialakításának fontos feltétele, hogy ismerje az RMS bevezetésének alapvető összetevőit és ezek szerepét. A következő lista az RMS bevezetésében szereplő kiszolgálókat sorolja fel:

-   Legfelső szintű tanúsítási kiszolgálók. A legfelső szintű tanúsítási kiszolgáló az RMS-telepítés első összetevője, minden más összetevő ettől függően működik. A legfelső szintű tanúsítási kiszolgálón fut az RMS összes szolgáltatása, így a fióktanúsítási szolgáltatás is, amely a tartalomvédelmi fióktanúsítványokat biztosítja a szervezetben működő RMS-ügyfeleknek. Minden Active Directory-erdőben csak egy legfelső szintű tanúsítási kiszolgáló létezhet. Több kiszolgálót is felvehet azonban a telepítésbe legfelső szintű tanúsítási fürt kialakításához, amellyel redundancia és terheléselosztás valósítható meg. A legfelső szintű tanúsítási fürtöt alkotó valamennyi kiszolgáló a telepítés első tanúsítási kiszolgálójának létesítésekor megadott konfigurációs adatbázist használja.
-   Licenckiszolgálók. Licenckiszolgálót nem kötelező létrehozni, ez nem része a legfelső szintű tanúsítási fürtnek. A licenckiszolgáló a legfelső szintű tanúsítási kiszolgálótól aligényléssel szerzi a tanúsítványát. A licenckiszolgáló a tanúsítás és más szolgáltatások szempontjából a legfelső szintű tanúsítási kiszolgálóra hagyatkozik (fióktanúsítási szolgáltatásokat nem képes nyújtani), de ezen futnak a licencelési szolgáltatások, amelyek közzétételi licencet és használati licencet egyaránt képesek kibocsátani. Redundancia és terheléselosztás érhető el, ha a telepítésbe több kiszolgálót felvéve licencelési fürtöt hoznak létre. A licencelési fürtöt alkotó kiszolgálók mind a fürt első licenckiszolgálójának létesítésekor meghatározott konfigurációs adatbázist használják.
-   Az infrastrukturális összetevőket futtató kiszolgálók. A rendszernek részei lehetnek további kiszolgálók is, amelyek a szükséges infrastruktúrát biztosítják, például az SQL Server 2000 adatbázis-kezelőt és az Active Directory címtárszolgáltatást. Az igényektől függ, hogy hol és hány kiszolgálón érdemes ezeket az összetevőket bevezetni.

A szervezet számára tervezett RMS-topológiának valamennyi összetevőre megoldást kell nyújtania.
