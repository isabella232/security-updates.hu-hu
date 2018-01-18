---
TOCTitle: RMS támogatás engedélyezése kiszolgálói szolgáltatásokhoz
Title: RMS támogatás engedélyezése kiszolgálói szolgáltatásokhoz
ms:assetid: '6288323c-0638-41b6-bef8-67a7c9433424'
ms:contentKeyID: 18122596
ms:mtpsurl: 'https://technet.microsoft.com/hu-hu/library/Cc747593(v=WS.10)'
---

RMS támogatás engedélyezése kiszolgálói szolgáltatásokhoz
=========================================================

Az RMS szolgáltathatja a tartalomvédelmi fióktanúsítványokat és használati licenceket az RMS-kompatibilis kiszolgálói alkalmazások részére is. Van néhány dolog, amire figyelni kell a kiszolgálói szolgáltatások konfigurálásakor:

-   A tulajdonosi hozzáférés-szabályozási listák (DACL) az RMS csatornákon alapértelmezésben a legbiztonságosabb beállításokat használják. Az RMS kiszolgálói szolgáltatások használatakor szükség van a DACL módosítására.

-   Ha az RMS ügyfélszoftver Windows Server 2003 alapú kiszolgálóra lett telepítve, és az Internet Explorer fokozott biztonsági beállításai engedélyezettek, az RMS fürtöt fel kell venni az Internet Explorernek a megbízható helyek zónájában lévő URL-címek közé.

-   Sok kiszolgálói szolgáltatás az Active Directory továbbfejlesztett címtárszolgáltatási funkcióját használja, ami csak akkor lehetséges, ha minden Active Directory tartományvezérlő a Windows Server 2003 operációs rendszeren fut. Ha használ ilyen kiszolgálói szolgáltatást (például a Microsoft Office SharePoint Server 2007 vagy a Microsoft Exchange Server 2007), ajánlatos, hogy minden tartományvezérlő a Windows Server 2003 rendszeren fusson, és a tartomány és az erdő Active Directory címtárának a működési szintje a Windows Server 2003 szintje legyen.

Alapértelmezett tulajdonosi hozzáférés-szabályozási lista (DACL) a kiszolgálótanúsítási csatornán
-------------------------------------------------------------------------------------------------

Az olyan alkalmazások, mint a Microsoft Office SharePoint Server 2007 vagy a Microsoft Exchange Server 2007 RMS-kompatibilisek a felhasználók nevében érkező használati licencekre irányuló kérelmek vonatkozásában. Alapértelmezett RMS telepítésnél az RMS kiszolgáló tanúsítási csatornájához tartozó DACL korlátozott, ami azt jelenti, hogy az alkalmazás nem tud tanúsítványt és licenceket szerezni a felhasználóinak. Az RMS kiszolgáló tanúsítási csatornáján a tulajdonosi hozzáférés-szabályozási listák (DACL) konfigurálásával azonban ezen számítógépeknek is engedélyezheti az RMS-rendszerben való részvételt, ha azokon van RMS-kompatibilis alkalmazás.

Az RMS-kompatibilis kiszolgálói alkalmazások az RMS tanúsítási szolgáltatáshoz a ServerCertification.asmx nevű fájl használatával csatlakoznak.

Amikor az RMS létrehozza ezeket a fájlokat, a fájlok hozzáférés-szabályozási listája (DACL) úgy van beállítva, hogy csak rendszerfolyamatokkal teszi lehetővé a hozzáférést. Ajánlott egy Active Directory biztonsági csoport létrehozása a kiszolgálói szolgáltatások részére, és annak feltöltése azon számítógépek Active Directory objektumaival, amelyek felhasználóik nevében használati licenceket kérelmeznek.

A csoport létrehozása után a DACL úgy módosítható a ServerCertification.asmx fájl részére, hogy engedélyezze a csoport Olvasás & Végrehajtás engedéllyel való ellátását a szolgáltatáson. Az RMS szolgáltatáscsoportot is fel kell vennie a DACL-listára Olvasás & Végrehajtás engedéllyel.

> [!NOTE]  
> Ha a fürtben több RMS kiszolgáló van, az ServerCertification.asmx fájlhoz tartozó DACL módosítandó a fürtben lévő mindegyik kiszolgálón. 

A Microsoft Exchange Server 2007 esetén az Exchange mindegyik hídfőkiszolgálójára vonatkozó Active Directory számítógépobjektumot fel kell venni a kiszolgálói szolgáltatások csoportba. Ha ez nem történik meg, az Exchange hídfőkiszolgáló nem lesz képes licenceket kérelmezni azoknak a felhasználóknak a nevében, akik az e-mailt kapták.

Az Office SharePoint Server 2007 estén annak a kiszolgálónak az Active Directory számítógépobjektumát kell felvenni a kiszolgálói szolgáltatások csoportjába, amelyiken az Office SharePoint Server 2007 fut. Ha az Office SharePoint Server 2007 kiszolgálószoftver úgy lett beállítva, hogy az Active Directory címtárban alapértelmezett kiszolgálót használja, az RMS szolgáltatási csoportot és a kiszolgálói szolgáltatásokhoz létrehozott csoportot fel kell venni az Olvasás & Végrehajtás engedéllyel ellátott ServiceLocater.asmx fájlba.

> [!IMPORTANT]  
> A ServerCertification.asmx és a ServiceLocater.asmx fájlhoz tartozó DACL módosítása után szükséges az Internet Information Services (IIS) újraindítása. Az IIS parancssorból az **iisreset** paranccsal állítható vissza. 