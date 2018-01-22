---
TOCTitle: Az RMS rendszer biztonsági mentése és visszaállítása
Title: Az RMS rendszer biztonsági mentése és visszaállítása
ms:assetid: 'c11f3ac1-e512-402b-bf13-9ff21f5fe745'
ms:contentKeyID: 18122744
ms:mtpsurl: 'https://technet.microsoft.com/hu-hu/library/Cc747745(v=WS.10)'
---

Az RMS rendszer biztonsági mentése és visszaállítása
====================================================

A rendszer helyreállításának tervezésekor figyelemmel kell lenni az adatbázis-kiszolgáló és az RMS kiszolgálók hibájára. Az adatbázis-kiszolgáló hibájánál a konfigurációs adatbázisról készült biztonsági másolatból helyreállítható az RMS kiszolgáló vagy fürt működőképessége. Ehhez nem kell új kiszolgálói licencelői tanúsítványt vagy személyes kulcsot beszereznie az RMS kiszolgálóhoz, mivel ezek megtalálhatók a konfigurációs adatbázisban.

Az RMS rendszer biztonsági mentésének tervezése
-----------------------------------------------

A kiszolgálói kulcson kívül a konfigurációs adatbázis a felhasználói adatokat is tárolja, beleértve a nyilvános kulcsra vonatkozó adatokat. A fontos kulcsadatok védelme érdekében készítsen biztonsági másolatot a konfigurációs adatbázisról a megfelelő adathordozóra, és tárolja biztonságos helyen azt. A legfelső szintű tanúsítási fürt konfigurációs adatbázisa gyakran változik, ezért a biztonsági mentéseket is a megfelelő gyakorisággal ajánlott végrehajtani. Minél gyakrabban kerülnek új felhasználók a szervezetbe, annál gyakrabban célszerű biztonsági mentést végrehajtani. A legfelső szintű tanúsítási kiszolgáló biztonsági mentésében a központi adatbázis **sysmessages** táblájának is szerepelnie kell. Ha ebben a táblában nem találhatók meg az RMS rendszerre vonatkozó üzenetek, a legfelső szintű tanúsítási kiszolgáló működésképtelen lesz, és hibaüzenetet fog adni. Ha a tábláról nem készült biztonsági másolat, újbóli létrehozásához meglévő adatbázissal meg kell ismételni a létesítési eljárást.

Az RMS naplózási adatbázisa értékes hibaelhárítási és statisztikai adatokat tartalmaz, de általában nem létfontosságú az RMS rendszer számára. A címtár-szolgáltatási adatbázis az Active Directory adatbázisának helyi gyorsítótára, így ez az RMS rendszer helyreállítása után automatikusan újból létrejön. Az RMS adatbázisainak biztonsági mentési tervének kidolgozásához kérjen segítséget az SQL Server rendszergazdájától.

Ha hardveres biztonsági modullal védi az RMS személyes kulcsait, akkor a hardveres biztonsági modul konfigurációjáról is kell biztonsági másolatot készítenie. A hardveres biztonsági modul konfigurációjának biztonsági mentéséről és helyreállításáról a hardveres biztonsági modul dokumentációjából tájékozódhat.

> [!NOTE]
> Ha az RMS személyes kulcsainak titkosítására az alapértelmezettől különböző szoftveres kriptográfiai szolgáltatót választ, ügyeljen rá, hogy a szervezetnél megfelelő kulcskezelési eljárások legyenek foganatosítva (biztonsági mentés, visszaállítás), és csak akkor vegye igénybe a CSP-t az RMS szolgáltatáshoz, ha adva vannak az említett feltételek.

Az RMS rendszer visszaállításának tervezése
-------------------------------------------

Az adatbázis-kiszolgáló biztonsági másolatból való visszaállításakor ügyeljen arra, hogy a biztonsági mentés végrehajtásakor meglévő RMS verzió fusson. Értesítse az RMS rendszer felhasználóit, hogy akik a biztonsági mentés dátumát követően léptek a rendszerbe, azoknak új tartalomvédelmi fióktanúsítványt kell beszerezniük. Védett tartalom nem fog elveszni.

Egy fürt valamelyik RMS kiszolgálójának visszaállításához telepítse újra az RMS rendszert, majd a meglévő adatbázis használatával csatlakoztassa a kiszolgálót a fürthöz. Ez a művelet nem érinti az RMS rendszer felhasználóit, mivel a fürtözött kiszolgálók egy egységként működnek.
