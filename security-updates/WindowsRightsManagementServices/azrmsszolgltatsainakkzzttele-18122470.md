---
TOCTitle: Az RMS szolgáltatásainak közzététele
Title: Az RMS szolgáltatásainak közzététele
ms:assetid: '3cca9325-6bd3-49ad-aa3f-e0693205d3f4'
ms:contentKeyID: 18122470
ms:mtpsurl: 'https://technet.microsoft.com/hu-hu/library/Cc720247(v=WS.10)'
---

Az RMS szolgáltatásainak közzététele
====================================

Az RMS szolgáltatásinak URL-címét a kiszolgáló létesítési eljárása teszi közzé az Active Directoryban. A létesítés során az RMS telepítője az Active Directory lekérdezésével állapítja meg, hogy van-e már másik RMS kiszolgáló telepítve az adott erdőben. Ha nincs másik RMS kiszolgáló telepítve, az RMS telepítője legfelső szintű tanúsítási kiszolgálóként konfigurálja a kiszolgálót. Az RMS használhatóságának feltétele, hogy az Active Directoryba be legyen jegyezve a szolgáltatás kapcsolódási pontja (SCP), amely lehetővé teszi az ügyfeleknek a legfelső szintű tanúsítási kiszolgáló URL-címének észlelését. A legfelső szintű tanúsítási kiszolgálón futó szolgáltatásokhoz való kapcsolódást kérelmező ügyfelek első dolga az, hogy lekérdezik az Active Directorytól a legfelső szintű tanúsítási kiszolgáló URL-címét. A további tudnivalókat lásd a dokumentumgyűjtemény „RMS kiszolgáló működtetése” részében „A szolgáltatás kapcsolódási pontjának regisztrálása” témakörben.

> [!NOTE]
> Ha a topológia több, legfelső szintű tanúsítási fürtöt alkotó kiszolgálót foglal magában, az URL a fürt terheléselosztó kiszolgálójára mutat, amelyet a rendszergazda ad meg a létesítés során.
