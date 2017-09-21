---
TOCTitle: Megbízható felhasználói tartományok
Title: Megbízható felhasználói tartományok
ms:assetid: 'a09b883f-f455-4c46-a4fd-d37b689e1d24'
ms:contentKeyID: 18122616
ms:mtpsurl: 'https://technet.microsoft.com/hu-hu/library/Cc747618(v=WS.10)'
---

Megbízható felhasználói tartományok
===================================

Az RMS alapértelmezés szerint nem állít ki használati licencet olyan felhasználóknak, akik tartalomvédelmi fióktanúsítványát másik felhasználói tartomány állította ki. Felhasználói tartománynak az RMS olyan telepítését nevezzük, amely legfelső szintű tanúsítási fürtből, esetleg licenckiszolgálókból vagy fürtökből, illetve az ezekhez tartozó adatbázisokból áll.

Az RMS beállítható úgy, hogy az ilyen kéréseket is feldolgozza: ehhez importálni kell a másik felhasználói tartomány kiszolgálói licencelői tanúsítványát, és fel kell venni a tartományt a megbízható felhasználói tartományok listájára. Ezt követően azok a felhasználók, akiknek a megbízható felhasználói tartomány állította ki a fióktanúsítványát, ettől a telepítéstől is kérelmezhetnek használati licencet. A használati licencek feldolgozása ugyanúgy megy végbe, mint ha belső felhasználók nyújtották volna be őket.

| ![](images/Cc747618.note(WS.10).gif)Megjegyzés:                                                                                 |
|--------------------------------------------------------------------------------------------------------------------------------------------------------------|
| A legfelső szintű tanúsítási fürt automatikusan szerepel az ugyanabba a telepítésbe tartozó RMS kiszolgálók megbízható felhasználói tartományainak listáján. |

Más tartományokba tartozó felhasználók számára is engedélyezheti védett tartalom megosztását. Ezt az alábbi példával mutatjuk be:

-   A szervezet egy másik szervezettel szoros együttműködésben bizalmas dokumentumokon dolgozik, és ezeket védelemmel szeretné ellátni, és meg szeretné őket osztani egymással. A másik szervezetnél is működik az RMS szolgáltatás. Mindkét szervezet felveheti a másik RMS-telepítést a megbízható felhasználói tartományok közé, így mindkét szervezet felhasználói tudnak közösen dolgozni a védett tartalmon, és ki tudják cserélni a fájlokat az interneten vagy egy extraneten keresztül.
-   Minden Active Directory-erdőben csak egy RMS-telepítés létezhet. A szervezet több Active Directory-erdőt működtet, és mindegyikben fut az RMS. A felhasználók az otthonukul szolgáló erdőtől függetlenül szeretnék egymással megosztani a védett tartalmat. Ez úgy érhető el, hogy minden erdőben felveszi az összes többi erdő RMS-telepítését a megbízható felhasználói tartományok közé.
-   A szervezetbe tartozó felhasználók más szervezetbe tartozó felhasználókkal közösen dolgoznak bizalmas dokumentumokon, amelyeket meg szeretnének védeni. A másik szervezetnél nem működik az RMS szolgáltatás. A másik szervezet felhasználói .NET Passport-fiókokat hozhatnak létre, Ön pedig felveheti a .NET Passport tartományt az RMS-telepítés megbízható felhasználói tartományai közé. Ezt követően mindkét vállalat felhasználói dolgozhatnak védett tartalommal, és kicserélhetik azt egymással az interneten keresztül.

A megbízható felhasználói tartományokról és a lépésenkénti utasításokról a további tudnivalókat lásd a dokumentumgyűjtemény „RMS kiszolgáló működtetése” részében a „Megbízható felhasználói tartományok hozzáadása és eltávolítása” és a „Bizalmi szabályzatok kialakítása” témakörben.
