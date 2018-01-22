---
TOCTitle: Az aligénylési szolgáltatás fájljára vonatkozó engedélyek megadása
Title: Az aligénylési szolgáltatás fájljára vonatkozó engedélyek megadása
ms:assetid: '737bb69b-fe26-4057-9569-e632f7bbf295'
ms:contentKeyID: 18122630
ms:mtpsurl: 'https://technet.microsoft.com/hu-hu/library/Cc747627(v=WS.10)'
---

Az aligénylési szolgáltatás fájljára vonatkozó engedélyek megadása
==================================================================

Az aligénylési szolgáltatás a legfelső szintű tanúsítási kiszolgálón fut, és a licenckiszolgálók igényeit teljesíti a létesítés során. Az aligénylési szolgáltatás alapértelmezés szerint csak a legfelső szintű tanúsítási kiszolgálón található helyi rendszerfiók számára engedélyezi a hozzáférést. Licenckiszolgáló létesítéséhez ilyen fiókkal kell bejelentkeznie a licenckiszolgálóra. Másik megoldásként a legfelső szintű tanúsítási kiszolgáló egyik helyi rendszergazdájának kell megváltoztatnia úgy az aligénylési szolgáltatás fájljának (SubEnrollService.asmx) tulajdonosi hozzáférés-szabályozási listáját, hogy azzal engedélyezze a hozzáférést a licenckiszolgáló létesítését végrehajtó felhasználói fiók számára. A SubEnrollService.asmx fájl a legfelső szintű tanúsítási kiszolgáló Certification virtuális könyvtárában található.
