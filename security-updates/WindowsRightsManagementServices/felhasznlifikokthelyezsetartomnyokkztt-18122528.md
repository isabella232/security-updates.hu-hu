---
TOCTitle: Felhasználói fiókok áthelyezése tartományok között
Title: Felhasználói fiókok áthelyezése tartományok között
ms:assetid: '0010b0ea-07c0-41c9-81f7-5881343d1d55'
ms:contentKeyID: 18122528
ms:mtpsurl: 'https://technet.microsoft.com/hu-hu/library/Cc720179(v=WS.10)'
---

Felhasználói fiókok áthelyezése tartományok között
==================================================

Amikor a szervezetben legfelső szintű tanúsítási kiszolgálót telepít és létesít, az erdő szintű bejegyzéssel regisztrálódik RMS-szolgáltatóként az Active Directoryban. Active Directory-erdőnként csak egy legfelső szintű tanúsítási fürt létezhet.

Amikor egy felhasználói fiókot az egyik tartományból egy másik, ugyanabban az erdőben lévő tartományba helyez át, általában új SID jön létre az új tartományban lévő felhasználói fiók számára. Ha ezután a felhasználó új tartalomvédelmi fióktanúsítványt kísérel meg beszerezni a kiszolgálóról, a kiszolgáló az új SID miatt újnak tekinti a felhasználót. A kiszolgáló új kulcsokat állít elő a felhasználónak, és a felhasználó eredeti e-mail címének felhasználásával új tartalomvédelmi fióktanúsítványt állít ki. Amikor a felhasználó meglévő licenccel próbálja meg használni az új tartalomvédelmi fióktanúsítványt, az SID és a kulcsok nem fognak egyezni, és a felhasználónak új licencet kell beszereznie. Ugyanez vonatkozik a felhasználói fiók másik erdőben lévő tartományba való áthelyezésére is.
