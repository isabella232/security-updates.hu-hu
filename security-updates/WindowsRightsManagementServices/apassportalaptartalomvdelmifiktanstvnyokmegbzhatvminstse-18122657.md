---
TOCTitle: 'A Passport-alapú tartalomvédelmi fióktanúsítványok megbízhatóvá minősítése'
Title: 'A Passport-alapú tartalomvédelmi fióktanúsítványok megbízhatóvá minősítése'
ms:assetid: 'c096fa36-c40d-4b28-843c-e9cbbe8eef70'
ms:contentKeyID: 18122657
ms:mtpsurl: 'https://technet.microsoft.com/hu-hu/library/Cc747655(v=WS.10)'
---

A Passport-alapú tartalomvédelmi fióktanúsítványok megbízhatóvá minősítése
==========================================================================

A felhasználó tartalomvédelmi fióktanúsítványának létesítéséhez a Microsoft olyan fióktanúsítási szolgáltatást is biztosít, amelyik a Microsoft .NET Passport hitelesítő adatait használja. H azt szeretnék, hogy az abból a szolgáltatásból származó tartalomvédelmi fióktanúsítványoknak lehetőségük legyen használati licenceket szerezni az RMS fürtből, telepíteni kell egy olyan megbízható felhasználói tartományt, amelyik elfogadja a Microsoft fióktanúsítási szolgáltatásából származó hitelesítő adatokat.

Ennek a funkciónak a használatához szükség van az Internet Information Services olyan konfigurálására, hogy lehetővé tegye az RMS licencelési szolgáltatásának névtelen elérését. Ez a lépés a külső felhasználók számára lényeges, mert a licencelési szolgáltatás úgy van konfigurálva, hogy alapértelmezésben a Windows integrált hitelesítését használja. Ha a névtelen hozzáférés nincs beállítva, a Passport alapú tartalomvédelmi fióktanúsítvánnyal (RAC) rendelkező külső felhasználók nem kaphatnak licencet.

A Passport-alapú tartalomvédelmi fióktanúsítványok megbízhatóvá minősítése
--------------------------------------------------------------------------

#### Az RMS licencelési szolgáltatás névtelen elérésének lehetővé tétele

1.  Nyissa meg az **Internet Information Services (IIS) kezelője** beépülő modult, és tárja ki az RMS működtetését biztosító kiszolgálót jelképező csomópontot.

2.  A konzolfán nyissa ki a **Webhelyek**, majd annak a webhelynek a csomópontját, amelyiken az RMS konfigurálása történt. Alapértelmezésben ez az **Alapértelmezett webhely**.

3.  A konzolfán nyissa ki a **\_wmcs** webhelyet, és válassza a **licencelés** virtuális könyvtárat.

4.  Kattintson a jobb egérgombbal a **licencelés** virtuális könyvtárra, majd kattintson a **Tulajdonságok** parancsra.

5.  Kattintson a **Licencelési tulajdonságok** párbeszédpanel **Könyvtárbiztonság** fülére.

6.  A **Hitelesítés és hozzáférés-vezérlés** területen kattintson a **Szerkesztés** feliratra.

7.  Jelölje be a **Névtelen hozzáférés engedélyezése** jelölőnégyzetet.

#### A Passport-alapú tartalomvédelmi fióktanúsítványok megbízhatóvá minősítése

1.  Nyissa meg a **Globális felügyelet** lapot, majd keresse meg azt a webhelyet, amelyen tartalomvédelmi fióktanúsítványokat szeretne megbízhatóvá minősíteni és kattintson a mellette látható **A webhelyen működő RMS felügyelete** hivatkozásra.

2.  A **Felügyeleti hivatkozások** csoportban kattintson a **Bizalmi szabályzatok** hivatkozásra.

3.  A **Megbízható felhasználói tartományok** csoportban kattintson **A Passport RAC-k megbízhatók** elemre. A Microsoft RM tanúsítási szolgáltatás megjelenik a **Megbízható felhasználói tartományok** listában.

4.  Ha szükséges, kizárhat egyes felhasználókat az e-mail címük alapján. Ehhez kattintson a **Kizárt identitások** elemre, majd írja be a megbízhatók köréből kizárandó felhasználó e-mail címét.
