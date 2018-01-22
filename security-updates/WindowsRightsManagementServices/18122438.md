---
TOCTitle: RMS gépaktiválás
Title: RMS gépaktiválás
ms:assetid: '09a0d631-9860-477f-9d10-df61b3bfe125'
ms:contentKeyID: 18122438
ms:mtpsurl: 'https://technet.microsoft.com/hu-hu/library/Cc720182(v=WS.10)'
---

RMS gépaktiválás
================

A gépaktiválás előfeltétele annak, hogy adott ügyfélszámítógépen RMS-védelemmel ellátott tartalmat lehessen közzétenni vagy használni. A gépaktiválás az a folyamat, amelynek során az ügyfélszámítógép egyedi kulcstárolóhoz és az annak megfelelő géptanúsítványhoz jut hozzá. A kulcstároló a számítógép személyes kulcsát tárolja, a géptanúsítvány pedig a nyilvános kulcsát. Mivel a kulcstárolóban található a számítógép személyes kulcsa, ezért ez a titkosítás és a visszafejtés szempontjából alapvető biztonsági elem. A számítógép minden felhasználója egyedi, a gépaktiválási folyamat során létrehozott géptanúsítványt kap.

A Service Pack 1 csomaggal frissített RMS-ügyfélnél használt gépaktiválási folyamat lényegesen eltér az 1.0-s verziónál alkalmazott eljárástól. A Service Pack 1 csomaggal frissített RMS-ügyfél „önaktiváló”. Amikor az RMS-ügyfelet egy bejelentkezett felhasználó telepíti, illetve amikor egy RMS-szolgáltatást először használ egy bejelentkezett felhasználó, az ügyfél elindítja az aktiválási folyamatot, amely a Windows titkosítási alkalmazásprogramozási felületének (API) használatával több kulcskészletet állít elő. Ezeknek a kulcsoknak a segítségével számos titkosítási műveletre kerül sor, és az így létrehozott géptanúsítvány köti össze a felhasználót, a számítógépet és az RMS-ügyfelet az RMS bizalmi hierarchiájában.
