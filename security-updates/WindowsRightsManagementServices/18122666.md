---
TOCTitle: 'Adatbázis-kiszolgáló'
Title: 'Adatbázis-kiszolgáló'
ms:assetid: 'c9844783-e6c4-49b4-8e7f-0f0377143b44'
ms:contentKeyID: 18122666
ms:mtpsurl: 'https://technet.microsoft.com/hu-hu/library/Cc747664(v=WS.10)'
---

Adatbázis-kiszolgáló
====================

Az RMS adatbázis-kiszolgálót, például SQL Server vagy Microsoft SQL Server 2000 Desktop Engine (MSDE 2000) Release A, használ az RMS konfigurációs, naplózási és címtár-szolgáltatási adatbázis kezeléséhez. Az MSDE 2000 csak egykiszolgálós telepítésekben használható. Feladatátvételes védelem megvalósításához adatbázis-kiszolgáló fürt alakítható ki.

A naplózási igények kielégítéséhez az adatbázis-kiszolgáló külön példányán futhat a konfigurációs és a naplózási adatbázis, illetve az adatbázis-kiszolgáló külön példánya vagy fürtje helyezhető üzembe a legfelső szintű tanúsítási kiszolgáló vagy fürt, illetve a licencelési fürtök számára. A további tudnivalókat lásd a dokumentumgyűjtemény „RMS rendszer bevezetése” részében.

Az RMS szolgáltatás csoportnak alapértelmezés szerint Execute (Végrehajtás) engedélye van ezen adatbázisok tárolt eljárásaihoz. A létesítés alkalmával bejelentkezve lévő felhasználói fióknak Database Owner (Adatbázis-tulajdonos) engedélyei vannak az adatbázisokhoz.

> [!NOTE]  
> A Microsoft SQL Server Desktop Engine adatbázis-kezelőt csak tesztkörnyezetben ajánlott használni az RMS adatbázisaihoz, mivel a Microsoft SQL Server Desktop Engine nem tartalmazza a teljes vállalati rendszert átfogó adatbázisok működtetéséhez szükséges eszközöket. Emellett az MSDE nem támogatja a távoli hálózatkezelést sem, ezért az RMS szolgáltatással azonos kiszolgálóra kell telepíteni, és nem lehet további RMS kiszolgálókat felvenni az RMS fürtbe. A Microsoft SQL Server Desktop Engine használati feltételei megtiltják az SQL Server ügyféleszközeinek használatát a Microsoft SQL Server Desktop Engine adatbázisok kezeléséhez. E korlátozás miatt nem tudja elkészíteni az RMS konfigurációs adatbázisának biztonsági másolatát, illetve nem tudja azt visszaállítani, nem tudja megtekinteni a naplózott adatokat és közvetlenül módosítani a konfigurációs adatbázisban tárolt adatokat. 
