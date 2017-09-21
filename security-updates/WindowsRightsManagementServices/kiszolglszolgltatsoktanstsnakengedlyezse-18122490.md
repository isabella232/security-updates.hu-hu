---
TOCTitle: Kiszolgálószolgáltatások tanúsításának engedélyezése
Title: Kiszolgálószolgáltatások tanúsításának engedélyezése
ms:assetid: '0ed78c85-7acb-4e3b-a594-613f8ccb5b14'
ms:contentKeyID: 18122490
ms:mtpsurl: 'https://technet.microsoft.com/hu-hu/library/Cc720196(v=WS.10)'
---

Kiszolgálószolgáltatások tanúsításának engedélyezése
====================================================

A művelet végrehajtásához helyben kell bejelentkeznie a felügyeleti webhelyre olyan tartományi felhasználói fiókkal, amelyik a Rendszergazdák csoport tagja. Biztonsági szempontból ajánlott a műveletet a **Futtatás másként** parancs segítségével végrehajtani.

Ez a művelet csak a legfelső szintű fürtre vonatkozóan hajtható végre.

A művelet előfeltétele egy olyan felhasználócsoport létrehozása, amely azokat a felhasználói fiókokat tartalmazza, amelyek a kiszolgálói szoláltatások megszemélyesítenek a tartalomvédelemmel ellátott tartalom elérésekor.

Kiszolgálószolgáltatások tanúsításának engedélyezése
----------------------------------------------------

#### Kiszolgálószolgáltatások tanúsításának engedélyezése

1.  Jelentkezzen be a helyi rendszergazdák csoportjának tagjaként.

2.  Indítsa el a fájlkezelő programot, és lépjen a &lt;rendszerlemezegység&gt;:\\Inetpub\\wwwroot\\\_wmcs\\Certification mappába.

3.  Ha engedélyezni szeretné, hogy a kiszolgálószolgáltatások tartalomvédelmi fióktanúsítványt (RAC) kapjanak, a jobb oldali egérgombbal kattintson a ServerCertification.asmx fájlra, és válassza a **Tulajdonságok** parancsot.

4.  A **Biztonság** lapon kattintson a **Hozzáadás** gombra, és vegye fel az adott felhasználókategóriához létrehozott csoportot és az **RMS-szolgáltatáscsoportot**.

5.  A csoportok **Engedélyek** listáiban jelölje be az **Engedélyezés** négyzetet az **Olvasás & Végrehajtás** engedélynél, majd kattintson az **OK** gombra.

6.  Az 1 - 4. lépést a fürtben lévő összes kiszolgálóra meg kell ismételni.

| ![](images/Cc720196.note(WS.10).gif)Megjegyzés:                                                                                                                                                                                                                                                                                                                                                                                                                                    |
|-----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| A Microsoft Exchange Server 2007 esetén minden hídfőkiszolgáló Active Directory számítógép-objektumát fel kell venni a ServerCertification.asmx tulajdonosi hozzáférés-szabályozási listára (DACL). A Microsoft Office SharePoint Server 2007 esetén ugyancsak erre a DACL listára kell felvenni az Office SharePoint Server 2007 kiszolgáló Active Directory számítógép-objektumát. Ajánlott még egy biztonsági csoport felvétele is erre a DACL listára, és a megfelelő számítógép-objektumok hozzárendelése. |
