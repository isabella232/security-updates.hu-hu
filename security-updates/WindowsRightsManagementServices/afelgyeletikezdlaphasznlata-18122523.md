---
TOCTitle: A felügyeleti kezdőlap használata
Title: A felügyeleti kezdőlap használata
ms:assetid: '6c155977-bd0e-47d6-ac65-1746cddb505e'
ms:contentKeyID: 18122523
ms:mtpsurl: 'https://technet.microsoft.com/hu-hu/library/Cc720290(v=WS.10)'
---

A felügyeleti kezdőlap használata
=================================

A **Felügyeleti kezdőlap** jeleníti meg a kiszolgálóval vagy a fürttel kapcsolatos adatokat, és itt találhatók a felügyeleti beállítások. Ez a lap csak a kiszolgáló létesítésének végrehajtása után érhető el.

A felügyelni kívánt kiszolgálóról a következő lépések végrehajtásával érheti el ezt a weblapot:

1.  Jelentkezzen be helyi rendszergazdaként.
2.  Válassza a **Start** menü **Minden program**, **Windows RMS**, majd **Windows RMS felügyeleti webhely** parancsát.
3.  A **Globális felügyelet** lapon kattintson **A webhelyen működő RMS felügyelete** elemre.

Ha engedélyezte a Secure Sockets Layer (SSL) használatával történő távoli felügyeletet, a **Felügyeleti kezdőlap** más számítógépről is elérhető. Ehhez hajtsa végre a következő lépéseket:

1.  A webböngésző címsorába írja be a következő URL-címet:
    https://*fürt\_neve:port\_száma*/\_wmcs/admin
    Ahol a *fürt\_neve:port\_száma* az az URL-cím, amelyet a fürthöz adott meg a létesítés során. A portszámot csak akkor kell megadnia, ha az alapértelmezés szerinti port (80) számától különböző portszámot határozott meg.
2.  A program kérésére adja meg az elérni kívánt kiszolgáló helyi rendszergazdájának bejelentkezési adatait.

A **Felügyeleti kezdőlap** lapon megjelennek a fürt adatai, például a fürt URL-címe, a konfigurációs adatbázis neve és helye, a kiszolgálói licencelői tanúsítvány lejárati ideje stb. Az itt található hivatkozásokat követve a fürt következő felügyeleti beállításait adhatja meg:

-   **Bizalmi szabályzatok.** Megbízható tartományok felvétele és eltávolítása. A további tudnivalókat lásd: „[A bizalom és a bizalmi szabályzat kezelése](https://technet.microsoft.com/1c96ee74-fd28-4511-be21-087e2b04c3ee)”.
-   **Jogmegadási sablonok**. Jogmegadási sablonok létrehozása és módosítása. A további tudnivalókat lásd: „[A jogmegadási sablonok kezelése](https://technet.microsoft.com/718286dc-3399-4556-96c9-ec3a33d31877)”.
-   **Naplózási beállítások**. A naplózás be- és kikapcsolása, valamint a naplózást végző kiszolgáló és az adatbázis nevének megtekintése. A további tudnivalókat lásd: „[A naplózás kezelése](https://technet.microsoft.com/8fccfc57-2135-494e-8e44-f6191bf5e4a0)”.
-   **A fürt extranetes URL-címének beállítása.** Kívülről elérhető URL-cím megadása a licencelési és fióktanúsítási kérelmekhez. A további tudnivalókat lásd: „[Extranetes URL-cím beállítása](https://technet.microsoft.com/88fec9ff-c96c-4d20-8856-0485e7507572)”.
-   **Az RMS proxybeállításai.** A proxykiszolgáló címének, a hitelesítés típusának, valamint a felhasználónévnek a megadása. Ezeket használja az RMS kiszolgáló, amikor proxykiszolgálón keresztül kell kapcsolódnia az internethez. A további tudnivalókat lásd: „[Az RMS proxybeállításainak konfigurálása](https://technet.microsoft.com/179d2970-62e9-4487-aa5b-f4334234991e)”.
-   **Biztonsági beállítások.** A kiszolgáló személyes kulcsához tartozó jelszó átállítása, a licenccel védett tartalom visszafejtésére jogosult felhasználókból álló felügyelői felhasználócsoport meghatározása és az RMS leszerelése. A további tudnivalókat lásd: „[A biztonság kezelése az RMS működtetésekor](https://technet.microsoft.com/62050812-de4f-4392-8d63-f2f89aa01ed4)”.
-   **Tanúsítási beállítások.** A tartalomvédelmi fióktanúsítványok érvényességi idejének és a rendszergazda elérhetőségének megadása. (Ez a beállítás csak a legfelső szintű tanúsítási fürtben érhető el, a licenckiszolgálókon nem.) A további tudnivalókat lásd: „[A tartalomvédelmi fióktanúsítványok kezelése](https://technet.microsoft.com/49c5c2ba-e197-4e4b-b3b3-b3248f068bcc)”.
-   **Kizárási szabályzatok.** A kulcstároló verziószáma, a tartalomvédelmi fióktanúsítvány, a Windows verziószáma vagy az RMS-kompatibilis alkalmazás szerinti kizárás megadása. A további tudnivalókat lásd: „[A kizárási szabályzat kezelése](https://technet.microsoft.com/ee31e099-e095-4648-95da-0009fbeb48cb)”.
-   **RM-fióktanúsítási jelentés.** A kiadott tartalomvédelmi fióktanúsítványok számának megtekintése. (Ez a beállítás csak a legfelső szintű tanúsítási fürtben érhető el, a licenckiszolgálókon nem.) A további tudnivalókat lásd: „[A tartalomvédelmi fióktanúsítványok nyilvántartása](https://technet.microsoft.com/5bb0f3cf-fc44-4e60-a93f-c789d6f8a902)”.

A további témakörök az említett szolgáltatások használatát mutatják be. A lépésenkénti utasítások az „[RMS – Útmutató](https://technet.microsoft.com/82032075-f361-438f-a2c4-93ab29ae6cff)” című pontban olvashatók.

| ![](images/Cc720290.note(WS.10).gif)Megjegyzés:                                                                                                                                                                                                     |
|----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| Az RMS felügyeleti webhelyén egyes szolgáltatások felbukkanó ablakokban konfigurálhatók. Ha a webböngészőben felbukkanó ablak blokkolót használ, úgy konfigurálja a böngésző beállításait, hogy az RMS felügyeleti webhelyén található felbukkanó ablakok engedélyezve legyenek. |
