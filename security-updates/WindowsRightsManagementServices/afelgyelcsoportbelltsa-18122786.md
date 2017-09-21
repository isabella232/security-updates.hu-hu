---
TOCTitle: A felügyelő csoport beállítása
Title: A felügyelő csoport beállítása
ms:assetid: 'f2ef847e-2824-471f-9079-5c343094aba8'
ms:contentKeyID: 18122786
ms:mtpsurl: 'https://technet.microsoft.com/hu-hu/library/Cc747798(v=WS.10)'
---

A felügyelő csoport beállítása
==============================

A művelet végrehajtásához helyben kell bejelentkeznie a felügyeleti webhelyre olyan tartományi felhasználói fiókkal, amely a Rendszergazdák csoport tagja az elérni kívánt számítógépen. A Tartománygazdák csoport tagjai is végrehajthatják ezt a műveletet. Biztonsági szempontból ajánlott a műveletet a **Futtatás másként** parancs segítségével végrehajtani.

A **Globális felügyelet** lap megnyitásához kattintson a **Start** gombra, és válassza a **Minden program**, a **Windows RMS**, majd a **Windows RMS felügyeleti webhely** parancsot.

A csoport csak akkor jelölhető ki az RMS felügyelői csoportjának, ha az már létezik az Active Directoryban, és a csoport tulajdonságaiban szerepel a fióknévvel azonos e-mail cím (teljesen minősített tartománynév formájában megadva).

A felügyelő csoport beállítása
------------------------------

#### A felügyelő csoport beállítása

1.  Nyissa meg a **Globális felügyelet** lapot, majd keresse meg azt a webhelyet, amelyen felügyelő csoportot szeretne beállítani, és kattintson a mellette látható **A webhelyen működő RMS felügyelete** hivatkozásra.

2.  A **Felügyeleti hivatkozások** csoportban kattintson a **Biztonsági beállítások** hivatkozásra.

3.  A **Felügyelők** csoportban a felügyelői felhasználócsoport felvételéhez kattintson az **Engedélyezés** gombra.

4.  A **felügyelő csoport neve** mezőbe írja be az adott Active Directory-erdőben található meglévő csoport teljesen megadott tartománynevét a *csoportnév*@*tartománynév.com* formában, amelynek tagjai tulajdonosi jogosultságokat kapnak az RMS által védett valamennyi dokumentumhoz, és kattintson a **Mentés** gombra.

    A felügyelői felhasználócsoport jogosultságainak tiltásához kattintson a **Letiltás** gombra.

Az eljárás végrehajtásáról a további tudnivalókat lásd: „[A felügyelő csoport használata](https://technet.microsoft.com/0febcb3e-7124-4e51-971a-1013b928d33b)”.
