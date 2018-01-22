---
TOCTitle: Megbízható felhasználói tartományok hozzáadása és eltávolítása
Title: Megbízható felhasználói tartományok hozzáadása és eltávolítása
ms:assetid: '7c440b15-01c4-49f1-b43c-00f67f3388c1'
ms:contentKeyID: 18122557
ms:mtpsurl: 'https://technet.microsoft.com/hu-hu/library/Cc747571(v=WS.10)'
---

Megbízható felhasználói tartományok hozzáadása és eltávolítása
==============================================================

Az RMS alapértelmezés szerint nem szolgálja ki az olyan felhasználók kérelmeit, akiknek a tartalomvédelmi fióktanúsítványát másik RMS-telepítés állította ki. Ha azonban a megfelelő felhasználói tartományokat felveszi a megbízható felhasználói tartományok listájára, az RMS az ilyen kérelmeket is feldolgozza.

A megbízható tartományokba meghatározott felhasználókat vagy csoportokat is felvehet, és el is távolíthatja azokat. A megbízható felhasználói tartományok is eltávolíthatók, azonban az adott Active Directory-erdő legfelső szintű tanúsítási fürtje nem távolítható el a megbízható felhasználói tartományok közül. A telepítésben szereplő összes RMS kiszolgáló, beleértve a legfelső szintű tanúsítási kiszolgálót is, a saját erdőjében található legfelső szintű tanúsítási fürtöt tartja megbízhatónak.

A megbízható felhasználói tartományok a következőképpen kezelhetők:

-   A külső felhasználók általános kezeléséhez felveheti a Microsoft® .NET Passport szolgáltatást a megbízható tartományok listájába. Ez lehetővé teszi, hogy a vállalatban működő RMS kiszolgáló feldolgozza a Microsoft .NET Passport szolgáltatás által kiállított tartalomvédelmi fióktanúsítványt tartalmazó licenckérelmeket.

-   Más szervezetek RMS-telepítéséhez tartozó külső felhasználók megbízhatóvá nyilvánításához az adott szervezetet felveheti a megbízható felhasználói tartományok közé. Ez lehetővé teszi, hogy az RMS kiszolgáló feldolgozza a másik szervezet RMS kiszolgálója által kiállított tartalomvédelmi fióktanúsítványt tartalmazó licenckérelmeket.

-   A saját szervezet másik Active Directory-erdőjében található felhasználóktól érkező licenckérelmek feldolgozásához az adott erdőben lévő RMS-telepítést ugyanígy felveheti a megbízható felhasználói tartományok listájára. Ez lehetővé teszi, hogy az aktuális erdőben lévő RMS kiszolgáló feldolgozza a másik erdő RMS kiszolgálója által kiállított tartalomvédelmi fióktanúsítványt tartalmazó licenckérelmeket.

-   Mindegyik megbízható felhasználói tartománynál megadhatja a megbízható e-mail tartományokat. A megbízható Passport-tartományoknál megadhatja a nem megbízható e-mail felhasználókat, illetve tartományokat.

Ha RMS-telepítést szeretne felvenni a megbízható felhasználói tartományok listájára, importálja a felvenni kívánt RMS-telepítés kiszolgálói licencelői tanúsítványát. Ehhez a rendszergazdának előbb exportálnia kell a kiszolgálói licencelői tanúsítványt a kiszolgálóról vagy a fürtből, majd el kell küldenie Önnek a tanúsítványt tartalmazó fájlt. A kapott fájlt ezután a megfelelő hely megadásával importálhatja. A fájl mentéséhez a bejelentkezett felhasználónak megfelelő engedélyekkel kell rendelkeznie a megosztott mappához. Megbízható felhasználói tartományok beállításakor a program nem továbbítja a személyes kulcs adatait.

A megbízható felhasználói tartományok létrehozásának lépéseit a „[Megbízható felhasználói tartomány hozzáadása](https://technet.microsoft.com/ed672e58-6272-4ac0-a434-d1d938037e93)” című pont ismerteti.