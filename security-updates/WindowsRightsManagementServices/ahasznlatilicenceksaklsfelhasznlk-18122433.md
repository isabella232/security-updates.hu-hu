---
TOCTitle: A használati licencek és a külső felhasználók
Title: A használati licencek és a külső felhasználók
ms:assetid: '02db9bda-180e-438f-863d-26252083a471'
ms:contentKeyID: 18122433
ms:mtpsurl: 'https://technet.microsoft.com/hu-hu/library/Cc720176(v=WS.10)'
---

A használati licencek és a külső felhasználók
=============================================

Az RMS lehetővé teszi a szerzők számára, hogy az interneten keresztül az arra jogosult külső felhasználókkal is megosszák a védett tartalmat. Az RMS egyforma védelmet nyújt a külső és a belső felhasználók részére közzétett tartalomhoz, mivel a tartalomhoz csatolt jogok csak RMS kiszolgáló által kiállított licenc birtokában gyakorolhatók. Ez lehetővé teszi a szervezetek számára, hogy az interneten át megoszthassák egymással a szerződésekhez hasonló bizalmas dokumentumokat, és együtt dolgozzanak azokon.

A külső felhasználók általában az interneten keresztül érik el az RMS szolgáltatást. (Ha a külső felhasználó közvetlenül is el tudja érni a belső hálózatot, például VPN-kapcsolat segítségével, funkcionális szempontból egyenértékű a belső felhasználókkal.) Akár része a felhasználó a közzétevő szervezetnek, akár azon kívülről érkezik, a használati licenc megszerzésének folyamata lényegében megegyezik a témakör „[Használati licenc megszerzése](https://technet.microsoft.com/0b6cde34-418a-4dee-9d27-b65b93b535ac)” című pontjában leírtakkal. A felhasználónak nem kell a szerző hálózatán belül lennie vagy ott felhasználói fiókkal rendelkeznie ahhoz, hogy használati licencet kérelmezhessen.

Ehhez mindössze a következő feltételeket kell teljesíteni:

-   A felhasználónak érvényes tartalomvédelmi fióktanúsítvánnyal kell rendelkeznie.
-   A felhasználónak hozzá kell férnie ahhoz az RMS licenckiszolgálóhoz, amely a közzétételi licencet kiállította (a kiszolgáló lehet az intraneten és az extraneten is).
-   A felhasználó fióktanúsítványát kiállító RMS-telepítésnek szerepelnie kell a használati licencet kiállító RMS-telepítés megbízható felhasználói tartományainak listáján.

A következő típusú külső felhasználók szerezhetnek használati licencet:

-   Olyan felhasználók, akiknek a fiókja más Active Directory-erdőbe tartozik, amelyben szintén létezik RMS-telepítés. A másik erdőben létező RMS-telepítést megbízható felhasználói tartományként kell megadni ebben a telepítésben.
-   Más olyan szervezet felhasználói, ahol RMS-telepítés fut, amely szerepel ennek a telepítésnek a megbízható felhasználói tartományai között.
-   A .NET Passport alapú tartalomvédelmi fióktanúsítvánnyal rendelkező felhasználók, ha a Microsoft RMS tanúsítási szolgáltatás szerepel az adott telepítés megbízható felhasználói tartományai között.

A megbízható felhasználói tartományok listájába más szervezetek vagy a szervezeten belüli más RMS-telepítések is felvehetők. A tartomány felvételét követően meghatározható, hogy a tartományon belül mely e-mail tartományok minősülnek megbízhatónak, valamint kiválasztható, hogy megbízhatónak tekintendők-e az adott tartományba tartozó biztonsági azonosítók (SID).

Más szervezet vagy a szervezetén belül az RMS más telepítése is felveheti RMS telepítését saját megbízható felhasználói tartományai listájára, így ezek RMS kiszolgálója is fel tudja dolgozni az Ön felhasználóitól érkező, használati licenc iránti kérelmeket.

Az RMS különböző telepítései és más szervezetek közötti megbízható felhasználói tartományok létrehozásáról a további tudnivalókat lásd a témakör „[Megbízható felhasználói tartományok](https://technet.microsoft.com/a09b883f-f455-4c46-a4fd-d37b689e1d24)” című pontjában, illetve a dokumentumgyűjtemény „RMS kiszolgáló működtetése” részében a „Megbízható közzétételi tartományok hozzáadása és eltávolítása” témakörben.
