---
TOCTitle: 'RMS-kompatibilis alkalmazások.'
Title: 'RMS-kompatibilis alkalmazások.'
ms:assetid: '30bb5565-81d3-43d9-a64d-cf0c5b990712'
ms:contentKeyID: 18122459
ms:mtpsurl: 'https://technet.microsoft.com/hu-hu/library/Cc720231(v=WS.10)'
---

RMS-kompatibilis alkalmazások.
==============================

A felhasználók akkor tudnak RMS-védelemmel ellátott tartalmat létrehozni és használni, ha telepítve van a számítógépükre egy RMS-kompatibilis alkalmazás (a témakörben leírtak szerint). Emellett az RMS ügyfélszoftverét is telepíteni kell, és a számítógépeket aktiválni kell. A további tudnivalókat lásd: „[Az RMS ügyfélszoftvere](https://technet.microsoft.com/03294fa2-8350-430d-b4b0-03d5169937c2)” és „[RMS gépaktiválás](https://technet.microsoft.com/09a0d631-9860-477f-9d10-df61b3bfe125)”.

Az RMS-kompatibilis alkalmazások lehetővé teszik a tartalom szerzőinek, hogy közzétételi licencek formájában jogokat rendeljenek az általuk létrehozott fájlokhoz, ezzel szabályozva, hogy miként lehet a tartalmat használni. Az RMS-kompatibilis alkalmazások dolgozzák fel a titkosított fájlok adatait, lehetővé téve ezzel a felhasználóknak, hogy a közzétételi licencben foglalt engedélyek szerint használják a tartalmat.

A fejlesztők a tartalomvédelmi szolgáltatások SDK készlete segítségével készíthetnek RMS-kompatibilis alkalmazásokat, amelyekkel RMS-védelemmel ellátott tartalom licencelhető, tehető közzé és használható. A Microsoft® Windows® 98 Second Edition vagy újabb operációs rendszerű számítógépekre lehet RMS-kompatibilis alkalmazásokat fejleszteni..

A fejlesztők RMS-kompatibilis kiszolgálói alkalmazásokat is készíthetnek a tartalomvédelmi szolgáltatások SDK készlete segítségével. Az ilyen alkalmazások képesek RMS-védelemmel ellátott tartalmat közzétenni, de használni nem.

Azok a felhasználók, akiknek nincs más RMS-kompatibilis alkalmazásuk az RMS-védelemmel ellátott e-mailek és weblapok használatához, beszerezhetik és használhatják a Microsoft® Internet Explorer tartalomvédelmi bővítményét. Az Outlook Web Access (OWA) felhasználói például az Internet Explorer tartalomvédelmi bővítménye segítségével használhatják az RMS-védelemmel ellátott e-maileket.

Az Internet Explorer tartalomvédelmi bővítménye letölthető a [Microsoft webhelyéről](http://go.microsoft.com/fwlink/?linkid=14450) (http://go.microsoft.com/fwlink/?LinkId=14450).

| ![](images/Cc720231.note(WS.10).gif)Megjegyzés:                                                                                                            |
|-----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| Ha az Internet Explorer tartalomvédelmi bővítményét Windows XP Service Pack 2 rendszeren használja, a fokozott biztonsági beállítások alkalmazáskompatibilitási problémákat okozhatnak. |

Ha a szervezetben lévő tartományok extranetelérési URL-címét nem veszi fel az Internet Explorer Helyi intranet listájára, az Internet Explorer tartalomvédelmi bővítményét használók ismétlődően a helyek elérésére vonatkozó üzeneteket kapnak. Az üzenetekre adott helytelen válasznál előfordulhat, hogy az RMS ügyfél új tartalomvédelmi fióktanúsítványt kap a felhasználói fiókhoz.

A helyek teljes szervezetre vonatkozó helyes beállításához egy parancsfájl segítségével írja be a szükséges URL-címeket a rendszerleíró adatbázisba a Helyi intranet zóna részeként. A Helyi intranet zóna elegendően magas biztonsági szintje alapértelmezés szerint kiküszöböli ezeket az üzeneteket.
