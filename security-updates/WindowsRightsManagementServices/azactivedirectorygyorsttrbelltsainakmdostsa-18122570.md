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
<th style="border:1px solid black;" >Név</th>
<th style="border:1px solid black;" >Típus</th>
<th style="border:1px solid black;" >Alapértelmezett érték</th>
<th style="border:1px solid black;" >Leírás</th>
</tr>
</thead>
<tbody>
<tr class="odd">
<td style="border:1px solid black;">PrincipalCacheMax</td>
<td style="border:1px solid black;">DWORD</td>
<td style="border:1px solid black;">1,000</td>
<td style="border:1px solid black;">A gyorsítótárban tárolható résztvevők (hozzájuk tartozó e-mail címek és SID azonosítók) száma.</td>
</tr>
<tr class="even">
<td style="border:1px solid black;">PrincipalCacheExpireMinutes</td>
<td style="border:1px solid black;">DWORD</td>
<td style="border:1px solid black;">12</td>
<td style="border:1px solid black;">A résztvevőkről a gyorsítótárban tárolt adatok érvényességének időtartama.</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;">GroupIDCacheMax</td>
<td style="border:1px solid black;">DWORD</td>
<td style="border:1px solid black;">1,000</td>
<td style="border:1px solid black;">A gyorsítótárban tárolható csoportok (hozzájuk tartozó e-mail címek és SID azonosítók) száma.</td>
</tr>
<tr class="even">
<td style="border:1px solid black;">GroupIDCacheExpireMinutes</td>
<td style="border:1px solid black;">DWORD</td>
<td style="border:1px solid black;">12</td>
<td style="border:1px solid black;">A csoporttagságról a gyorsítótárban tárolt adatok érvényességének időtartama.</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;">GroupMembershipCacheMax</td>
<td style="border:1px solid black;">DWORD</td>
<td style="border:1px solid black;">1,000</td>
<td style="border:1px solid black;">A gyorsítótárban maximálisan tárolható olyan kapcsolatok száma, amelyek csoport tagjai.</td>
</tr>
<tr class="even">
<td style="border:1px solid black;">GroupMembershipCacheExpireMinutes</td>
<td style="border:1px solid black;">DWORD</td>
<td style="border:1px solid black;">12</td>
<td style="border:1px solid black;">A csoporttagkapcsolatok gyorsítótárban tárolt adatainak érvényességi időtartama.</td>
</tr>
</tbody>
</table>
  
> [!CAUTION]  
> A rendszerleíró adatbázis nem megfelelő módosítása súlyos károkat okozhat a rendszerben. A rendszerleíró adatbázis módosítása előtt készítsen biztonsági másolatot a számítógépen tárolt fontos adatokról. 
  
> [!NOTE]  
> A **PrincipalCacheExpireMinutes**, **GroupIDCacheExpireMinutes**, **GroupMembershipCacheExpireMinutes** és a **ContactMembersofGroupCacheExpireMinutes** rendszerleíró bejegyzés az adatbázis-kiszolgálón lévő címtár-szolgáltatási adatbázisban tárolt Active Directory-gyorsítótár lejáratát is szabályozza. 
