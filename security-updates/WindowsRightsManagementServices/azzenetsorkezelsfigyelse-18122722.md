---
TOCTitle: 'Az üzenetsor-kezelés figyelése'
Title: 'Az üzenetsor-kezelés figyelése'
ms:assetid: 'a7109399-3a84-4681-874b-f6ea1646b0a0'
ms:contentKeyID: 18122722
ms:mtpsurl: 'https://technet.microsoft.com/hu-hu/library/Cc747716(v=WS.10)'
---

Az üzenetsor-kezelés figyelése
==============================

Az RMS naplózási szolgáltatása a Message Queuing (más néven MSMQ) segítségével küldi el az eseményeket a naplózási adatbázisba. Az RMS előtét-kiszolgálói elküldik az üzeneteket a Message Queuing szolgáltatásnak, a kiszolgálókon futó naplózási figyelőszolgáltatás pedig lekéri az üzeneteket a Message Queuing várólistából, majd beírja őket a naplózási adatbázisba. Ha a naplózási adatbázis vagy az adatbázis-kiszolgáló nem érhető el, vagy ha nem működik a naplózási figyelőszolgáltatás, a Message Queuing a várólistában tárolja az üzeneteket. Ha a naplózási adatbázis vagy az adatbázis-kiszolgáló leállítását tervezi, először a naplózási figyelőszolgáltatást állítsa le az összes előtét-kiszolgálón, majd az adatbázis vagy az adatbázis-kiszolgáló újraindítását követően indítsa újra a naplózási figyelőszolgáltatást is a kiszolgálókon.

Ha az adatbázis nem működik, és a naplózási figyelőszolgáltatás továbbra is fut, a szolgáltatás nem tudja beírni a naplózási üzeneteket az adatbázisba. A szolgáltatás a „kézbesíthetetlen leveleket” tároló Message Queuing várólistába helyezi át az üzeneteket az adatbázis elérhetővé válásáig, majd ezután új naplózási bejegyzéseket ír az adatbázisba. A kézbesíthetetlen levelek várólistájába helyezett üzeneteket a szolgáltatás nem írja be automatikusan a naplózási adatbázisba. A várólistába helyezett üzeneteket a következő művelet segítségével tekintheti meg és törölheti:

1.  Nyissa meg a Microsoft Management Console (MMC) Számítógép-kezelés beépülő modulját. Ehhez válassza a **Start** menü **Minden program**, **Felügyeleti eszközök**, majd **Számítógép-kezelés** parancsát.
2.  A konzolfa Szolgáltatások és kiszolgálói alkalmazások bejegyzésénél kattintson az Üzenetsor-kezelés, majd a Privát várólisták elemre.
3.  Két várólista jelenik meg. Mindkét várólista neve a „**drms\_logging**” kifejezéssel kezdődik, amelyet az adott fürt neve követ. Az egyik várólista neve „**drms\_logging\_***&lt;a fürt neve&gt;***\_deadletter**”. Ez a kézbesíthetetlen üzenetek várólistája. Kattintson a várólista nevére, majd a Várólista üzenetei várólistára.
4.  A tulajdonságok megtekintéséhez kattintson duplán az egyes üzenetekre.
5.  A várólista törléséhez az egér jobb gombjával kattintson a **Várólista üzenetei** várólistára, és válassza **Az összes feladat**, majd az **Eltávolítás** parancsot.

Az alapértelmezés szerinti konfigurációban a Message Queuing az összes üzenetet tárolja. Ezt csak a kiszolgálón rendelkezésre álló szabad tárolóhely mérete korlátozza. Ha a Message Queuing felhasználja a teljes szabad lemezterületet, az RMS kiszolgáló nem tudja kiszolgálni az ügyfélkérelmeket. Ennek megakadályozása érdekében a következő lépések végrehajtásával korlátozhatja a Message Queuing által a várólistákhoz felhasználható lemezterületet:

1.  Nyissa meg a Microsoft Management Console (MMC) Számítógép-kezelés beépülő modulját. Ehhez válassza a Start menü Minden program, Felügyeleti eszközök, majd Számítógép-kezelés parancsát.
2.  A konzolfa Szolgáltatások és kiszolgálói alkalmazások bejegyzésénél kattintson az Üzenetsor-kezelés, majd a Privát várólisták elemre.
3.  Két várólista jelenik meg. Mindkét várólista neve a „drms\_logging” kifejezéssel kezdődik. Mindkét várólistán hajtsa végre a következő lépéseket:
    -   Kattintson a Tulajdonságok elemre.
    -   Jelölje be az Üzenettároló méretkorlátozása (KB) négyzetet, majd adja meg a várólista maximális méretét (kilobájtban).

Ha megtelik a várólista, a szolgáltatás elveti az RMS által küldött üzeneteket, és a következő, 48-as eseményazonosítójú üzenetet küldi a rendszer eseménynaplójába:

„Nem sikerült elküldeni a tulajdonságcsoportot a Message Queuing szolgáltatásnak.”

A rendszerfigyelő eszközöket célszerű úgy beállítani, hogy a fenti esemény előfordulásakor értesítést küldjenek, mert ez problémát jelezhet a naplózási adatbázisban.
