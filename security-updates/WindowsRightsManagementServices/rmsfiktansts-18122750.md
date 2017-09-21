---
TOCTitle: RMS fióktanúsítás
Title: RMS fióktanúsítás
ms:assetid: 'c9a385c5-6dbb-47f5-a80f-69718e6f9deb'
ms:contentKeyID: 18122750
ms:mtpsurl: 'https://technet.microsoft.com/hu-hu/library/Cc747750(v=WS.10)'
---

RMS fióktanúsítás
=================

A fióktanúsítási folyamat során létrejön egy tartalomvédelmi fióktanúsítvány, amely egy felhasználói fiókot és egy számítógépet társít egymáshoz, és lehetővé teszi a felhasználónak, hogy azon a számítógépen RMS-védelemmel ellátott tartalmat használjon. Amikor egy ügyfélszámítógépen először tesznek közzé RMS-védelemmel ellátott tartalmat, vagy először kísérelnek meg RMS-védelemmel ellátott tartalmat használni, az RMS-kompatibilis alkalmazás tartalomvédelmi fióktanúsítványt kérelmez az RMS fióktanúsítási szolgáltatásától.

A tanúsítási szolgáltatás a Windows-hitelesítés vagy egy hardveres titkosítási eszközben (például intelligens kártya) tárolt x.509 tanúsítvány segítségével hitelesíti a felhasználót. Ezután a kiszolgáló a hitelesítő adatokon alapján létrehozza a felhasználó tartalomvédelmi fióktanúsítványát. Titkosítja a felhasználó személyes kulcsát az ügyfélszámítógép RMS-géptanúsítványának nyilvános kulcsával, majd a titkosított kulcsot elhelyezi a tartalomvédelmi fióktanúsítványban. Ezután kiállítja a tartalomvédelmi fióktanúsítványt a kérelmező alkalmazásnak, amely azt a számítógépen vagy az eszközön tárolja, hogy az ezt követő közzétételi vagy használati licenckérelmeknél rendelkezésre álljon. A tartalomvédelmi fióktanúsítvány bekerül a konfigurációs adatbázisba is.

A fióktanúsításra csak a gépaktiválási folyamat után kerülhet sor, mivel a tartalomvédelmi fióktanúsítvány kérelmezéséhez szükség van az ügyfélszámítógép RMS-géptanúsítványára.

A felhasználóknak minden általuk használt számítógéphez külön tartalomvédelmi fióktanúsítványt kell igényelniük. Ha egy felhasználó egynél több számítógépen dolgozik, mindegyik számítógéphez egyedi tartalomvédelmi fióktanúsítvány jön létre, de a felhasználó mindegyik számítógépen ugyanazt a kulcspárt kapja.

Amikor egy RMS-kompatibilis alkalmazás használati licencet igényel, a kérelembe belefoglalja a tartalomvédelmi fióktanúsítványt. A licencelési szolgáltatás a tartalomvédelmi fióktanúsítvány nyilvános kulcsával titkosítja a tartalomkulcsot, ami biztosítja, hogy csak a hitelesített felhasználó tudja a licencet használni.

A fióktanúsítási folyamat a következő lépésekből áll:

1.  Amikor egy felhasználó adott számítógépen először tesz közzé RMS-védelemmel ellátott tartalmat, vagy először próbál meg RMS-védelemmel ellátott tartalmat használni, az RMS-kompatibilis alkalmazás tartalomvédelmi fióktanúsítványt kérelmez a legfelső szintű tanúsítási kiszolgálón futó fióktanúsítási szolgáltatásától.
2.  A fióktanúsítási szolgáltatás a Windows-hitelesítés segítségével hitelesíti a felhasználót.
3.  A fióktanúsítási szolgáltatás a hitelesítő adatok alapján létrehoz a felhasználónak egy tartalomvédelmi fióktanúsítványt. Titkosítja a felhasználó személyes kulcsát az RMS-géptanúsítvány nyilvános kulcsával, majd a titkosított kulcsot elhelyezi a tanúsítványban. Ezután kiadja a tartalomvédelmi fióktanúsítványt a kérelmező alkalmazásnak.
4.  Az alkalmazás a számítógépen vagy az eszközön tárolja a tartalomvédelmi fióktanúsítványt, így az rendelkezésre áll az ezt követő közzétételi vagy használati licenckérelmekhez.

A tartalomvédelmi fióktanúsítvány kérelmezéséhez használt fióktanúsítási szolgáltatás az RMS ügyfélszoftverét futtató számítógép típusától függ. A szokásos asztali számítógépek a fióktanúsítási szolgáltatáshoz (certification.asmx) kapcsolódnak. Az RMS SP1 verzióban engedélyezett kiszolgálószolgáltatások a kiszolgálótanúsítási szolgáltatástól (ServeCertfication.asmx) kapják a tartalomvédelmi fióktanúsítványt. Az RMS SP1 verzióban engedélyezett mobil eszközök a mobil eszközök tanúsítási szolgáltatásától (MobileDeviceCertfication.asmx) kapják a tartalomvédelmi fióktanúsítványt. Az RMS SP 1 alapértelmezés szerinti telepítésénél csak a fióktanúsítási szolgáltatás van engedélyezve.

Az RMS SP1 mobil eszközökkel és kiszolgálószolgáltatásokkal való használatáról további tudnivalókat lásd a dokumentumgyűjtemény „RMS kiszolgáló működtetése” részében „Az RMS kiszolgáló támogatásának engedélyezése mobil eszközök és kiszolgálószolgáltatások számára” témakörben.
