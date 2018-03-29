---
TOCTitle: A létesítési folyamat biztonsági vonatkozásai
Title: A létesítési folyamat biztonsági vonatkozásai
ms:assetid: '9f1282c5-5642-4870-a9a4-c3a485f8ff76'
ms:contentKeyID: 18122613
ms:mtpsurl: 'https://technet.microsoft.com/hu-hu/library/Cc747616(v=WS.10)'
---

A létesítési folyamat biztonsági vonatkozásai
=============================================

Az RMS felügyeleti webhelye segítségével az RMS erőforrásai meglévő webhelyen létesíthetők. A létesítés során virtuális könyvtárak és alkalmazáskészletek jönnek létre ezen a webhelyen, valamint sor kerül az RMS adatbázisainak létrehozására és konfigurálására az adatbázis-kiszolgálón. Ha a kiszolgáló csatlakozik az internethez, a létesítési eljárás alatt végrehajtható a kiszolgáló igénylése is a Microsoft igénylési szolgáltatásával.

A létesítés során az RMS a következő táblázatban bemutatott felhasználói fiókokat használja.


 
<p></p>
<table style="border:1px solid black;">
<colgroup>
<col width="33%" />
<col width="33%" />
<col width="33%" />
</colgroup>
<thead>
<tr class="header">
<th style="border:1px solid black;" >Fiók</th>
<th style="border:1px solid black;" >Rendeltetése</th>
<th style="border:1px solid black;" >Engedélyek</th>
</tr>
</thead>
<tbody>
<tr class="odd">
<td style="border:1px solid black;">A bejelentkezett felhasználó fiókja</td>
<td style="border:1px solid black;">Létrehozza a virtuális könyvtárakat és az alkalmazáskészleteket. Az IIS megköveteli a Windows-hitelesítést, az RMS pedig megszemélyesíti a bejelentkezett felhasználót, akinek helyben kell bejelentkezve lennie.</td>
<td style="border:1px solid black;">Teljes hozzáférés (a bejelentkezett felhasználónak helyi rendszergazdának kell lennie).</td>
</tr>
<tr class="even">
<td style="border:1px solid black;">Rendszerfiók</td>
<td style="border:1px solid black;">Összeállítja a sorba rendezéshez szükséges ideiglenes programkódot.</td>
<td style="border:1px solid black;">Olvasási és írási engedély a Windows ideiglenes mappájához (C:\Windows\Temp).</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;">ASPNET fiók</td>
<td style="border:1px solid black;">Összeállítja a *.aspx fájlok ideiglenes programkódját.</td>
<td style="border:1px solid black;">Hozzáférési jogosultság az átmeneti programkód gyorsítótáraként használt könyvtárhoz (ez alapértelmezés szerint a C:\Windows\Microsoft.NET\Framework\v1.1.4322\Temporary ASP.NET Files könyvtár).</td>
</tr>
<tr class="even">
<td style="border:1px solid black;">Hálózati szolgáltatásfiók</td>
<td style="border:1px solid black;">Regisztrálja az Active Directoryban a szolgáltatás kapcsolódási pontját.</td>
<td style="border:1px solid black;"><ul>
<li>Csak olvasási engedély a létesítő helyhez (általában a C:\Inetpub\Wwwroot\Provisioning mappához).<br />
<br />
</li>
<li>Olvasási és írási engedély a <strong>DRMS</strong> rendszerleíró kulcshoz. Az engedélyeket az RMS telepítője adja, és ez hozza létre a következő rendszerleíró kulcsot is.<br />
<br />
A Windows Server 2003 rendszer 32 bites verziójával működő számítógépeken:<br />
<br />
<code>HKEY_LOCAL_MACHINE\Software\Microsoft\DRMS\1.0</code><br />
<br />
A Windows Server 2003 rendszer 64 bites verziójával működő számítógépeken:<br />
<br />
<code>HKEY_LOCAL_MACHINE\Software\WOW6432Node\Microsoft\DRMS\1.0</code><br />
<br />
</li>
</ul></td>
</tr>
</tbody>
</table>
 

A létesítés során az RMS a következő műveleteket hajtja végre:

-   Az adatbázis-kiszolgálón:
    -   Létrehozza a konfigurációs, a címtár-szolgáltatási és a naplózási adatbázist.
    -   Bejelentkezési engedélyt ad az RMS szolgáltatás csoportnak.
    -   Telepíti az adatbázisokba a tárolt eljárásokat, és Execute (Végrehajtás) jogosultságot ad hozzájuk az RMS szolgáltatás csoportnak.
    -   Lekérdezéseket hajt végre az adatbázis mesterpéldányán.
-   Hozzáadja az RMS szolgáltatás csoportot az IIS\_WPG csoporthoz.
-   A C:\\Inetpub\\Wwwroot\\\_wmcs mappában létrehozza a webszolgáltatások és az RMS felügyeleti webhelye számára a virtuális könyvtárak, a fájlok és az alkalmazáskészletek hierarchiáját.
-   Beállítja a virtuális könyvtárak, fájlok és alkalmazáskészletek tulajdonosi hozzáférés-szabályozási listáját (DACL).
-   Hozzáférési jogosultságot ad az RMS szolgáltatás csoportnak az ideiglenes mappához.
-   Ha szoftveres kulcsvédelmet választanak, titkosítja a kiszolgáló licencelői személyes kulcsát, majd tárolja az adatbázisban. Az RMS egy jelszót kér a létesítés során, és eléri a gépi szintű DPAPI felületet.
-   Telepíti a naplózási figyelőszolgáltatást.
-   Létrehozza a naplózási üzenet-várólistát.
-   Ha a legfelső szintű tanúsítási kiszolgáló létesítése történik, beállítja az Active Directoryban a szolgáltatás kapcsolódási pontját.
