---
TOCTitle: 'A Microsoft SQL Server 2000 Desktop Engine (MSDE 2000) telepítése az RMS adatbázis-támogatásának biztosításához'
Title: 'A Microsoft SQL Server 2000 Desktop Engine (MSDE 2000) telepítése az RMS adatbázis-támogatásának biztosításához'
ms:assetid: 'c9b9cd08-98c4-424f-b3fc-d685f57c002e'
ms:contentKeyID: 18122667
ms:mtpsurl: 'https://technet.microsoft.com/hu-hu/library/Cc747667(v=WS.10)'
---

A Microsoft SQL Server 2000 Desktop Engine (MSDE 2000) telepítése az RMS adatbázis-támogatásának biztosításához
===============================================================================================================

A Microsoft SQL Server 2000 Desktop Engine (MSDE 2000) telepítése az RMS adatbázis-támogatásának biztosításához
---------------------------------------------------------------------------------------------------------------

#### A Microsoft SQL Server 2000 Desktop Engine (MSDE 2000) telepítése az RMS adatbázis-támogatásának biztosításához

1.  Jelentkezzen be az adott kiszolgáló helyi Rendszergazdák csoportjába tartozó tartományi fiókkal arra a kiszolgálóra, amelyre a Microsoft SQL Server 2000 Desktop Engine (MSDE 2000) adatbázis-kezelőt telepíteni kívánja.

2.  A [Microsoft webhelyéről](http://www.microsoft.com/) (http://www.microsoft.com/) töltse le a Microsoft MSDE 2000 adatbázis-kezelőt a helyi számítógép egyik mappájába.

3.  Az MSDE2000A.exe fájl futtatásával bontsa ki az MSDE 2000 telepítőcsomagot egy mappába. A mappa alapértelmezés szerint az MSDERelA nevet kapja, de más név is megadható.

4.  Nyisson meg egy parancssori ablakot, és lépjen abba a mappába, amelybe az MSDE 2000 telepítést mentette.

5.  A Microsoft SQL Server 2000 Desktop Engine alkalmazásnak az RMS szolgáltatással együttműködést lehetővé tevő beállításokkal való telepítéséhez írja be a következő parancsot, és a *jelszó* helyőrzőt cserélje le a kívánt erős jelszóra:

    **Setup.exe /i setup\\sqlrun10.msi INSTANCENAME=RMS DISABLEAGENTSTARTUP=1 SAPWD=** *jelszó*

    > [!IMPORTANT]  
    > Az MSDE szolgáltatást telepítése után kell elindítani. A szolgáltatás a **VezérlőpultSzolgáltatások** elemével indítható. A szolgáltatást érdemes automatikus indulásra konfigurálni, így az MSDE-adatbázis az RMS futtatásakor mindig elérhető lesz. 

Az RMS-szolgáltatást csak az RMS konfigurációs adatbázisát kezelő adatbázis telepítése után létesítse a kiszolgálón.

A Microsoft SQL Server Desktop Engine adatbázis-kezelőt csak tesztkörnyezetben ajánlott használni az RMS adatbázisaihoz, mivel a Microsoft SQL Server Desktop Engine nem tartalmazza a teljes vállalati rendszert átfogó adatbázisok működtetéséhez szükséges eszközöket. Emellett az MSDE nem támogatja a távoli hálózatkezelést sem, ezért az RMS szolgáltatással azonos kiszolgálóra kell telepíteni, és nem lehet további RMS kiszolgálókat felvenni az RMS fürtbe. A Microsoft SQL Server Desktop Engine használati feltételei megtiltják az SQL Server ügyféleszközeinek használatát a Microsoft SQL Server Desktop Engine adatbázisok kezeléséhez. E korlátozás miatt nem tudja elkészíteni az RMS konfigurációs adatbázisának biztonsági másolatát, illetve nem tudja azt visszaállítani, nem tudja megtekinteni a naplózott adatokat és közvetlenül módosítani a konfigurációs adatbázisban tárolt adatokat.
