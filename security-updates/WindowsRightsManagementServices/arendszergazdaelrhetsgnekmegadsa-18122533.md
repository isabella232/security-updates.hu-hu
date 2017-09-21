---
TOCTitle: A rendszergazda elérhetőségének megadása
Title: A rendszergazda elérhetőségének megadása
ms:assetid: '31777458-5530-4ae0-ac1f-131b3d98dd35'
ms:contentKeyID: 18122533
ms:mtpsurl: 'https://technet.microsoft.com/hu-hu/library/Cc720237(v=WS.10)'
---

A rendszergazda elérhetőségének megadása
========================================

A művelet végrehajtásához helyben kell bejelentkeznie a felügyeleti webhelyre olyan tartományi felhasználói fiókkal, amely a Rendszergazdák csoport tagja az elérni kívánt számítógépen. A Tartománygazdák csoport tagjai is végrehajthatják ezt a műveletet. Biztonsági szempontból ajánlott a műveletet a **Futtatás másként** parancs segítségével végrehajtani.

Az itt megadott rendszergazdának helyi rendszergazdának kell lennie a legfelső szintű tanúsítási kiszolgálón.Erre azért van szükség, mert a licenckiszolgálók létesítéséhez a bejelentkezett felhasználónak engedéllyel kell rendelkeznie a legfelső szintű tanúsítási kiszolgálón található SubEnrollService.asmx fájlhoz. Ha a licenckiszolgáló létesítésével próbálkozó felhasználónak nincs engedélye ehhez a fájlhoz, a felhasználó az itt megadott rendszergazdához fordulhat a szükséges engedélyek beszerzése céljából. A további tudnivalókat lásd: „[Az aligénylési szolgáltatás fájljára vonatkozó engedélyek megadása](https://technet.microsoft.com/737bb69b-fe26-4057-9569-e632f7bbf295)”.

A **Globális felügyelet** lap megnyitásához kattintson a **Start** gombra, és válassza a **Minden program**, a **Windows RMS**, majd a **Windows RMS felügyeleti webhely** parancsot.

A rendszergazda elérhetőségének megadása
----------------------------------------

#### A rendszergazda elérhetőségének megadása

1.  Nyissa meg a **Globális felügyelet** lapot, majd keresse meg azt a webhelyet, amelyen meg szeretné adni a rendszergazda elérhetőségét, és kattintson a mellette látható **A webhelyen működő RMS felügyelete** hivatkozásra.

2.  A **Felügyeleti hivatkozások** csoportban kattintson a **Tanúsítási beállítások** hivatkozásra.

3.  A **Kapcsolatfelvétel a rendszergazdával** csoportban adja meg annak a rendszergazdának az e-mail címét a *felhasználónév*@*tartománynév*.com formában, akihez a felhasználók a licenckiszolgáló létesítése során felmerülő aligénylési problémákkal fordulhatnak.

4.  Kattintson a lap alján található **Küldés** gombra.
