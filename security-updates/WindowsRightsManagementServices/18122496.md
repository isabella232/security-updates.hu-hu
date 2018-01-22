---
TOCTitle: Felhasználói kulcsok
Title: Felhasználói kulcsok
ms:assetid: '12dad6e2-64e7-4bab-bde7-b72f90f5cb05'
ms:contentKeyID: 18122496
ms:mtpsurl: 'https://technet.microsoft.com/hu-hu/library/Cc720202(v=WS.10)'
---

Felhasználói kulcsok
====================

Az RMS minden felhasználójanak van egy 1024 bites RSA-kulcspárja. A felhasználó kulcspárját az RMS konfigurációs adatbázisa tárolja, így adott felhasználóhoz mindig ugyanaz a kulcspár tartozik a teljes RMS rendszerben.

A felhasználó nyilvános kulcsát a tartalomvédelmi fióktanúsítvány tartalmazza. Ezzel a kulccsal van titkosítva a használati licencben lévő tartalomkulcs, így csak az adott felhasználó tudja az RMS-védelemmel ellátott tartalmat az adott licenccel használni.

Ugyanaz a tartalomvédelmi fióktanúsítvány a felhasználó személyes kulcsát is tartalmazza, amely az ügyfélgép nyilvános kulcsával van titkosítva. Ez biztosítja, hogy a tartalomvédelmi fióktanúsítványt csak azon a számítógépen lehessen használni, amelyhez kiállították, de azt is, hogy adott felhasználó mindegyik tartalomvédelmi fióktanúsítványa ugyanazt a kulcspárt tartalmazza. A felhasználó személyes kulcsa szükséges minden olyan tartalom használatához, amelyet az RMS segítségével védelemmel láttak el.
