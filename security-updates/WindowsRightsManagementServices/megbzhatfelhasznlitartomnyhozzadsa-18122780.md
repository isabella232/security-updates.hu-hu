---
TOCTitle: Megbízható felhasználói tartomány hozzáadása
Title: Megbízható felhasználói tartomány hozzáadása
ms:assetid: 'ed672e58-6272-4ac0-a434-d1d938037e93'
ms:contentKeyID: 18122780
ms:mtpsurl: 'https://technet.microsoft.com/hu-hu/library/Cc747793(v=WS.10)'
---

Megbízható felhasználói tartomány hozzáadása
============================================

A művelet végrehajtásához helyben kell bejelentkeznie a felügyeleti webhelyre olyan tartományi felhasználói fiókkal, amely a Rendszergazdák csoport tagja az elérni kívánt számítógépen. A Tartománygazdák csoport tagjai is végrehajthatják ezt a műveletet. Biztonsági szempontból ajánlott a műveletet a **Futtatás másként** parancs segítségével végrehajtani.

A **Globális felügyelet** lap megnyitásához kattintson a **Start** gombra, és válassza a **Minden program**, a **Windows RMS**, majd a **Windows RMS felügyeleti webhely** parancsot.

Megbízható felhasználói tartomány hozzáadása
--------------------------------------------

#### Megbízható felhasználói tartomány hozzáadása

1.  Nyissa meg a **Globális felügyelet** lapot, majd keresse meg azt a webhelyet, amelyhez megbízható felhasználói tartományt szeretne hozzáadni, és kattintson a mellette látható **A webhelyen működő RMS felügyelete** hivatkozásra.

2.  A **Felügyeleti hivatkozások** csoportban kattintson a **Bizalmi szabályzatok** hivatkozásra.

3.  A **Megbízható felhasználói tartományok** csoportban kattintson a **Tallózás** gombra, keresse meg annak felhasználói tartománynak a kiszolgálói licencelői tanúsítványát, amelynek importálásával létre szeretné hozni a bizalmi kapcsolatot, kattintson duplán a tanúsítványra, majd kattintson a **Hozzáadás** gombra.

    A tartomány neve megjelenik a **Megbízható felhasználói tartományok** listában.

4.  Ha meg szeretné határozni, hogy a megbízható felhasználói tartományokon belül mely e-mail tartományok megbízhatók, kattintson a tanúsítványokat felsoroló lista melletti **Megbízható tartományok** elemre. Ennek hatására megnyílik a **Megbízható e-mail tartományok** ablak.

5.  Válasszon az alábbi beállítások közül:

    -   Ha a tartomány minden felhasználói fiókját megbízhatónak szeretné minősíteni, jelölje be a **Minden e-mail tartomány megbízható** beállítást.
        vagy
    -   Válassza a **Csak a megadott e-mail tartományok megbízhatók** beállítást, majd írja be a megbízható tartomány nevét (például pelda.com), majd kattintson a **Hozzáadás** gombra. Ennek hatására a tartomány felkerül a Megbízható e-mail tartományok listájára. Ha el szeretne távolítani egy nevet a listáról, jelölje azt ki, és kattintson az **Eltávolítás** gombra. Ha egy tartományt felvesz a listára, az annak minden altartományára is érvényes.

6.  Ha olyan környezetben használja az RMS-szolgáltatást, ahol a csoporttagság behelyettesítése erdőhatárokon is átnyúlik, jelölje be **Az RM licencelés megbízható a felhasználói tartomány biztonsági azonosítói (SID) szempontjából** négyzetet.

7.  Ha befejezte a műveletet, kattintson **Az ablak bezárása és visszatérés a Bizalmi szabályzatok lapra** elemre.

Az eljárás végrehajtásáról a további tudnivalókat lásd: „[Megbízható felhasználói tartományok hozzáadása és eltávolítása](https://technet.microsoft.com/7c440b15-01c4-49f1-b43c-00f67f3388c1)”.
