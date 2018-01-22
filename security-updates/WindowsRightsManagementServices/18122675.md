---
TOCTitle: 'A címtár-szolgáltatási adatbázis karbantartása'
Title: 'A címtár-szolgáltatási adatbázis karbantartása'
ms:assetid: '911a62f2-c1d6-4091-99b0-b53211be27a7'
ms:contentKeyID: 18122675
ms:mtpsurl: 'https://technet.microsoft.com/hu-hu/library/Cc747680(v=WS.10)'
---

A címtár-szolgáltatási adatbázis karbantartása
==============================================

Az RMS része az adatbázis-kiszolgálón futó címtár-szolgáltatási adatbázis, amely a felhasználókra, az azonosítókra (például e-mail címek), biztonsági azonosítókra (SID), a csoporttagságra és a másodlagos azonosítókra vonatkozó adatokat tárolja. Ezeket az adatokat az RMS licencelési szolgáltatása szerzi be az Active Directory globális katalógusának küldött LDAP-lekérdezésekkel, majd helyileg tárolja ebben az adatbázisban, így rövidebb lesz a kiszolgáló válaszideje, amikor a felhasználók a használati licencet kérelmeznek.

Mivel az adatbázisban tárolt adatoknál gyakran előfordul a beszúrás és a törlés, az adatok töredezetté válhatnak. Rendszeres időközönként (naponta vagy hetente) végre kell hajtani az adatbázis újraszervezését a DRMS\_DirectoryServices valamennyi tábláján. Ez a művelet újból felépíti az indexeket, így megszűnik az adatok töredezettsége. A töredezett adatok ronthatják a teljesítményt, sőt akár a kiszolgáló leállását is okozhatják.

Ha adatbázis-kiszolgálóként az SQL Server rendszert használja, az adatbázis újraszervezése a Maintenance Wizard (Karbantartó varázsló) vagy az SQL Server Agent (SQL Server ügynök) használatával saját parancsfájl segítségével hajtható végre.

Ha a tranzakciónapló elfogadhatatlan méretűre növekszik az adatbázis újraindexelésénél, a növekedés csökkentése érdekében az újraindexelés előtt a teljes helyreállíthatóság üzemmódról térjen át a tömeges naplózás üzemmódra.
