---
TOCTitle: RMS ügyféligénylés
Title: RMS ügyféligénylés
ms:assetid: '9c1d07bf-7235-4694-8291-ac2e5b221f4a'
ms:contentKeyID: 18122606
ms:mtpsurl: 'https://technet.microsoft.com/hu-hu/library/Cc747613(v=WS.10)'
---

RMS ügyféligénylés
==================

Az ügyfélszámítógépek az RMS közzétételi szolgáltatásától ügyfél-licencelői tanúsítványt igényelhetnek, amelynek birtokában a szerzők olyankor is közzétehetnek RMS-védelemmel ellátott tartalmat, amikor nem kapcsolódnak a vállalati hálózathoz. Ebben az esetben nem a közzétételi szolgáltatás, hanem az ügyfélszámítógép írja alá és állítja ki az adott számítógépről közzétett, RMS-védelemmel ellátott tartalom használati jogait tartalmazó közzétételi licenceket.

Az ügyfél-licencelői tanúsítványokat az RMS közzétételi szolgáltatása állítja ki.

Az ügyfelek igénylési folyamata a következő lépésekből áll:

1.  Az ügyfélszámítógép egy igénylési kérelemben elküldi a felhasználó tartalomvédelmi fióktanúsítványát a legfelső szintű tanúsítási kiszolgálón vagy fürtön, illetve licenckiszolgálón vagy licencelési fürtön futó közzétételi szolgáltatásnak.

2.  A kiszolgáló ellenőrzi, hogy a hálózati rendszergazda beállításai szerint engedélyezve van-e az ügyféligénylés, és hogy a tartalomvédelmi fióktanúsítvány nem szerepel-e a konfigurációs adatbázis kizárási listáján. A kizárási listák létrehozásáról a további tudnivalókat lásd a dokumentumgyűjtemény „RMS kiszolgáló működtetése” részében „A kizárási szabályzat kezelése” témakörben.

3.  A közzétételi szolgáltatás létrehoz egy kulcspárt az ügyfélszámítógép számára. Létrehoz egy ügyfél licencelői tanúsítványt, és elhelyezi a nyilvános kulcsot a tanúsítványban. Titkosítja a személyes kulcsot a tartalomvédelmi fióktanúsítvány nyilvános kulcsával, majd elhelyezi azt a tanúsítványban.

4.  A közzétételi szolgáltatás kibocsátja az ügyfélszámítógép részére az ügyfél-licencelői tanúsítványt.