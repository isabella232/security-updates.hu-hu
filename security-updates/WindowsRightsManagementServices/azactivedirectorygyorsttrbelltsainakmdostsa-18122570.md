---
TOCTitle: 'Az Active Directory-gyorsítótár beállításainak módosítása'
Title: 'Az Active Directory-gyorsítótár beállításainak módosítása'
ms:assetid: '8789a7a5-2065-4fae-9104-e0a70f1f2fb6'
ms:contentKeyID: 18122570
ms:mtpsurl: 'https://technet.microsoft.com/hu-hu/library/Cc747586(v=WS.10)'
---

Az Active Directory-gyorsítótár beállításainak módosítása
=========================================================

A rendszerleíró adatbázisban tárolt beállítások határozzák meg, hogy hány bejegyzést tárol az Active Directory gyorsítótára. A beállítások módosításával lerövidíthető az ügyfélkérelmekre adott válaszhoz szükséges idő. A további tudnivalókat lásd „A címtárszolgáltatás teljesítményének optimalizálása” című pontban. A gyorsítótárban tárolt információk érvényességi időtartama is megadható.

A Windows Server 2003 rendszer 32 bites verziójával működő számítógépeken a gyorsítótár-bejegyzéseket szabályozó beállítások a következő rendszerleíró kulcs alatt találhatók:

**HKEY\_LOCAL\_MACHINE\\Software\\Microsoft\\DRMS\\1.0\\DirectoryServices**

A Windows Server 2003 rendszer 64 bites verziójával működő számítógépeken a gyorsítótár-bejegyzéseket szabályozó beállítások a következő rendszerleíró kulcs alatt találhatók:

**HKEY\_LOCAL\_MACHINE\\SoftwareWOW6432Node\\Microsoft\\DRMS\\1.0\\DirectoryServices**

Az alábbi táblázat a memóriabeli gyorsítótár működését szabályozó bejegyzéseket tartalmazza.

###  

<p> </p>
<table style="border:1px solid black;">
<colgroup>
<col width="25%" />
<col width="25%" />
<col width="25%" />
<col width="25%" />
</colgroup>
<thead>
<tr class="header">
<th>Név</th>
<th>Típus</th>
<th>Alapértelmezett érték</th>
<th>Leírás</th>
</tr>
</thead>
<tbody>
<tr class="odd">
<td style="border:1px solid black;"><p>PrincipalCacheMax</p></td>
<td style="border:1px solid black;"><p>DWORD</p></td>
<td style="border:1px solid black;"><p>1,000</p></td>
<td style="border:1px solid black;"><p>A gyorsítótárban tárolható résztvevők (hozzájuk tartozó e-mail címek és SID azonosítók) száma.</p></td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><p>PrincipalCacheExpireMinutes</p></td>
<td style="border:1px solid black;"><p>DWORD</p></td>
<td style="border:1px solid black;"><p>12</p></td>
<td style="border:1px solid black;"><p>A résztvevőkről a gyorsítótárban tárolt adatok érvényességének időtartama.</p></td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><p>GroupIDCacheMax</p></td>
<td style="border:1px solid black;"><p>DWORD</p></td>
<td style="border:1px solid black;"><p>1,000</p></td>
<td style="border:1px solid black;"><p>A gyorsítótárban tárolható csoportok (hozzájuk tartozó e-mail címek és SID azonosítók) száma.</p></td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><p>GroupIDCacheExpireMinutes</p></td>
<td style="border:1px solid black;"><p>DWORD</p></td>
<td style="border:1px solid black;"><p>12</p></td>
<td style="border:1px solid black;"><p>A csoporttagságról a gyorsítótárban tárolt adatok érvényességének időtartama.</p></td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><p>GroupMembershipCacheMax</p></td>
<td style="border:1px solid black;"><p>DWORD</p></td>
<td style="border:1px solid black;"><p>1,000</p></td>
<td style="border:1px solid black;"><p>A gyorsítótárban maximálisan tárolható olyan kapcsolatok száma, amelyek csoport tagjai.</p></td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><p>GroupMembershipCacheExpireMinutes</p></td>
<td style="border:1px solid black;"><p>DWORD</p></td>
<td style="border:1px solid black;"><p>12</p></td>
<td style="border:1px solid black;"><p>A csoporttagkapcsolatok gyorsítótárban tárolt adatainak érvényességi időtartama.</p></td>
</tr>
</tbody>
</table>
  
| ![](images/Cc747586.Caution(WS.10).gif)Figyelmeztetés:                                                                                                                        |  
|------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|  
| A rendszerleíró adatbázis nem megfelelő módosítása súlyos károkat okozhat a rendszerben. A rendszerleíró adatbázis módosítása előtt készítsen biztonsági másolatot a számítógépen tárolt fontos adatokról. |
  
| ![](images/Cc747586.note(WS.10).gif)Megjegyzés:                                                                                                                                                                                                                                   |  
|----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|  
| A **PrincipalCacheExpireMinutes**, **GroupIDCacheExpireMinutes**, **GroupMembershipCacheExpireMinutes** és a **ContactMembersofGroupCacheExpireMinutes** rendszerleíró bejegyzés az adatbázis-kiszolgálón lévő címtár-szolgáltatási adatbázisban tárolt Active Directory-gyorsítótár lejáratát is szabályozza. |
