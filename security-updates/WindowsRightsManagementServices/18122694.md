---
TOCTitle: 'Az RMS Management Pack (kezelési csomag) importálása és használata'
Title: 'Az RMS Management Pack (kezelési csomag) importálása és használata'
ms:assetid: 'd9a73ef0-2f81-48c2-97cc-deb7bf477389'
ms:contentKeyID: 18122694
ms:mtpsurl: 'https://technet.microsoft.com/hu-hu/library/Cc747688(v=WS.10)'
---

Az RMS Management Pack (kezelési csomag) importálása és használata
==================================================================

Az RMS Management Pack (kezelési csomag) importálása és használata
------------------------------------------------------------------

#### Az RMS Management Pack (kezelési csomag) importálása és használata

1.  Másolja az RMS kezelési csomagot (RMS\_MOMPack.akm) a %ProgramFiles%\\Windows Rights Management Services\\Tools mappából a Microsoft Operations Manager (MOM) kiszolgálóra.

2.  Nyissa meg a MOM felügyeleti konzolját, és a következő műveletek végrehajtásával importálja az RMS kezelési csomagot:

    1.  A MOM felügyeleti konzoljának konzolfáján bontsa ki a **Rules** (Szabályok) elemet, majd az egér jobb gombjával kattintson a **Processing Rule Groups** (Feldolgozási szabályok csoportjai) elemre.
    2.  Válassza a helyi menü **Import Management Pack** (Kezelési csomag importálása) parancsát. Megjelenik az **Import Management Pack** (Kezelési csomag importálása) párbeszédpanel.
    3.  Kattintson a **Browse** (Tallózás) gombra, és keresse meg az RMS\_MOMPack.akm fájlt.

3.  Adja meg az egyesítésre, illetve a cserére vonatkozó beállításokat. Ha további tájékoztatást szeretne kapni az egyesítés és a csere beállításairól, a Microsoft webhelyén (http://www.microsoft.com/) olvassa el az „Exporting and Importing Management Packs” (Kezelési csomagok exportálása és importálása) című cikket.

    Kattintson a **Replace** (Csere) elemre. A cserét megadó beállítás hatására az importált kezelési csomag felülírja a meglévő feldolgozásiszabály-csoportokat, és a felhasználói megjegyzések sem őrződnek meg. Ha az adott kezelési csomagot egy meglévő kezelési csomaggal szeretné egyesíteni, először tesztkörnyezetben hajtsa végre a műveletet, és csak akkor használja a **Replace** (Csere) műveletet, amikor a tényleges munkakörnyezetben vezeti be a kezelési csomagot.

4.  A kezelési csomag importálásához kattintson az **Import** (Importálás) elemre.

5.  A **MOM felügyeleti konzolján** jelölje ki a **Configuration** (Konfigurálás) elemet, majd kattintson az **Agent Managers** (Ügynökkezelők) mappára.

6.  Az egér jobb gombjával kattintson arra a kiszolgálóra, amelyre az RMS kezelési csomagot importálta, majd válassza a helyi menü **Scan Managed Computers Now** (Kezelt számítógépek vizsgálata) parancsát.
