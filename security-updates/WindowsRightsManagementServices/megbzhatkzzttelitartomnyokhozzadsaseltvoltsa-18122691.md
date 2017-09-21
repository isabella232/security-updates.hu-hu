---
TOCTitle: Megbízható közzétételi tartományok hozzáadása és eltávolítása
Title: Megbízható közzétételi tartományok hozzáadása és eltávolítása
ms:assetid: 'd87b502d-5497-4ccd-badf-f6807d587cee'
ms:contentKeyID: 18122691
ms:mtpsurl: 'https://technet.microsoft.com/hu-hu/library/Cc747687(v=WS.10)'
---

Megbízható közzétételi tartományok hozzáadása és eltávolítása
=============================================================

Az RMS kiszolgálók alapértelmezés szerint csak a saját maguk vagy a fürtjükben található más kiszolgálók által kiállított közzétételi licencek ellenében állítanak ki használati licenceket. Ha a tartalom közzététele más legfelső szintű tanúsítási kiszolgáló (akár a szervezeten belül egy másik erdő leányvállalatában, vagy másik szervezet leányvállalatában) használatával történt, az RMS kiszolgáló akkor adhat a tartalomra vonatkozó használati licenceket a felhasználóknak, ha az RMS kiszolgálón megbízható közzétételi tartományt állít be. Megbízható közzétételi tartomány megadásakor a másik legfelső szintű tanúsítási kiszolgáló licencelői tanúsítványának importálásával bizalmi kapcsolatot hoz létre az RMS kiszolgáló és a másik kiszolgáló között. Az RMS kiszolgálóhoz tetszőleges számú megbízható közzétételi tartományt állíthat be.

A listára felvett megbízható közzétételi tartományok bármikor eltávolíthatók, ehhez elegendő eltávolítani az adott tartomány tanúsítványát a megbízható közzétételi tartományok tanúsítványait tartalmazó listáról.

Megbízható közzétételi tartomány felvételéhez importálnia kell a felvenni kívánt RMS kiszolgáló vagy fürt kiszolgálói licencelői tanúsítványát, személyes kulcsát (ha a személyes kulcsot a szoftver tárolja, és nem egy hardveres biztonsági modul), valamint az összes jogmegadási sablonját. A rendszergazdának előbb jelszóval védett fájlba kell exportálnia ezeket az elemeket az adott kiszolgálóról vagy fürtből, és meg kell adnia a fájl visszafejtéséhez szükséges jelszót. A rendszergazdának ezután egy megosztott mappába kell másolnia a fájlt, és el kell juttatnia Önhöz a jelszót. A fájlt ezután a megfelelő hely és jelszó megadásával importálhatja. A fájl mentéséhez az **Admin** alkalmazáskészletet futtató fióknak a megfelelő engedélyekkel kell rendelkeznie a megosztott mappához.

A megbízható közzétételi tartományok létrehozásának lépéseit a „[Megbízható közzétételi tartomány hozzáadása](https://technet.microsoft.com/731416d8-ddf4-4d4a-9f1a-bbd1ea48fe3c)” című témakör ismerteti.

Ha a személyes kulcsot hardveres biztonsági modulban tárolja, továbbítania kell a személyes kulcsot a megbízhatónak nyilvánított kiszolgáló hardveres biztonsági moduljába az eszköz dokumentációjában ismertetett módon. A kiszolgálókon található hardveres biztonsági modul típusától és az ahhoz tartozó eszközök konfigurációjától függően előfordulhat, hogy a személyes kulcs nem vihető át az egyik hardveres biztonsági modulból a másikba. A hardveres biztonsági modul dokumentációjából tudhatja meg, hogy a személyes kulcs átvihető-e a célként választott hardveres biztonsági modulban tárolt adatok elvesztése nélkül. Ha nem sikerül átvinni a személyes kulcsot, nem alakítható ki megbízható közzétételi tartomány a két kiszolgáló között.

| ![](images/Cc747687.note(WS.10).gif)Megjegyzés:                                                                                                                                                                                                                                                                                             |
|--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| Ha az RMS személyes kulcsának védelméhez hardveres biztonsági modult használ, és olyan RMS-telepítésből importál kiszolgálói licencelői tanúsítványt, amely szoftveres megoldást alkalmaz a személyes kulcs védelméhez, a tanúsítvány importálása előtt a fürtbe tartozó összes RMS-kiszolgáló Biztonsági beállítások lapján meg kell adnia a személyes kulcs jelszavát. |
