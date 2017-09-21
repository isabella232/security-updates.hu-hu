---
TOCTitle: A kapcsolatkészlet rendszerleíró beállításainak módosítása
Title: A kapcsolatkészlet rendszerleíró beállításainak módosítása
ms:assetid: 'c61d91db-a1ad-4ca5-a492-015da629afbc'
ms:contentKeyID: 18122663
ms:mtpsurl: 'https://technet.microsoft.com/hu-hu/library/Cc747660(v=WS.10)'
---

A kapcsolatkészlet rendszerleíró beállításainak módosítása
==========================================================

A rendszer teljesítménye javítható egyes rendszerleíró kulcsok értékének módosításával. Ezekben a kulcsokban beállíthatók az RMS által használt Active Directory LDAP-kapcsolatkészlet tulajdonságai.

A Windows Server 2003 rendszer 32 bites verziójával működő számítógépeken a kapcsolatkészlet rendszerleíró bejegyzései a következő rendszerleíró kulcs alatt találhatók:

**HKEY\_LOCAL\_MACHINE\\Software\\Microsoft\\DRMS\\1.0**

A Windows Server 2003 rendszer 64 bites verziójával működő számítógépeken a kapcsolatkészlet rendszerleíró bejegyzései a következő rendszerleíró kulcs alatt találhatók:

**HKEY\_LOCAL\_MACHINE\\SoftwareWOW6432Node\\Microsoft\\DRMS\\1.0**

Az alábbi táblázat azokat a bejegyzéseket tartalmazza, amelyeknek létrehozásával felülbírálhatók az Active Directory kapcsolatkészlet alapértelmezett beállításai. A táblázatban az alapértelmezett értékek vannak feltüntetve. Ha továbbiakat szeretne megtudni arról, hogy az RMS hogyan állítja össze a lekérdezéslistát, és hogyan használja ezeket a beállításokat, olvassa el „Az Active Directory-kapcsolatkészlet beállításainak optimalizálása” című témakört.

###  

<p> </p>
<table style="border:1px solid black;">
<colgroup>
<col width="20%" />
<col width="20%" />
<col width="20%" />
<col width="20%" />
<col width="20%" />
</colgroup>
<thead>
<tr class="header">
<th>Név</th>
<th>Típus</th>
<th>Alapértelmezett érték</th>
<th>Leírás</th>
<th>Megjegyzések</th>
</tr>
</thead>
<tbody>
<tr class="odd">
<td style="border:1px solid black;"><p>GC</p></td>
<td style="border:1px solid black;"><p>Karaktersorozat</p></td>
<td style="border:1px solid black;"><p>1. név, ..., n. név</p></td>
<td style="border:1px solid black;"><p>A globális katalógusokat (DNS-nevükön) felsoroló, vesszővel tagolt lista. Az RMS csak azokat a globális katalógusokat használja, amelyek szerepelnek ebben a rendszerleíró kulcsban.</p></td>
<td style="border:1px solid black;"><p>Ha azt szeretné, hogy az RMS ne hozzon létre lekérdezéslistát, ezzel a beállítással adja meg, hogy mely globális katalógusokat használja.</p></td>
</tr>  
<tr class="even">
<td style="border:1px solid black;"><p>MinGC</p></td>
<td style="border:1px solid black;"><p>DWORD</p></td>
<td style="border:1px solid black;"><p>1</p></td>
<td style="border:1px solid black;"><p>Legalább ennyi globális katalógusnak elérhetőnek kell lennie ahhoz, hogy az RMS elindulhasson.</p></td>
<td style="border:1px solid black;"></td>
</tr>  
<tr class="odd">
<td style="border:1px solid black;"><p>MaxGC</p></td>
<td style="border:1px solid black;"><p>DWORD</p></td>
<td style="border:1px solid black;"><p>15</p></td>
<td style="border:1px solid black;"><p>A topológiaészlelési algoritmus legfeljebb ennyi globális katalógust vesz fel a lekérdezéslistába.</p></td>
<td style="border:1px solid black;"></td>
</tr>  
<tr class="even">
<td style="border:1px solid black;"><p>ThreshHoldAlive</p></td>
<td style="border:1px solid black;"><p>DWORD</p></td>
<td style="border:1px solid black;"><p>1</p></td>
<td style="border:1px solid black;"><p>Legalább ennyi kapcsolatnak válaszképesnek kell lennie ahhoz, hogy a DiscoveryServices elkezdje keresni a lekérdezéslistába felvehető globális katalógusokat azért, hogy az RMS fogadhassa a kérelmeket.</p></td>
<td style="border:1px solid black;"></td>
</tr>  
<tr class="odd">
<td style="border:1px solid black;"><p>RetryDown</p></td>
<td style="border:1px solid black;"><p>DWORD</p></td>
<td style="border:1px solid black;"><p>5</p></td>
<td style="border:1px solid black;"><p>Ennyiszer próbálja meg újra elérni a szolgáltatás a nem működő kapcsolatot, mielőtt válaszképtelennek minősítené.</p></td>
<td style="border:1px solid black;"></td>
</tr>  
<tr class="even">
<td style="border:1px solid black;"><p>TimeRetryDown</p></td>
<td style="border:1px solid black;"><p>DWORD</p></td>
<td style="border:1px solid black;"><p>300</p></td>
<td style="border:1px solid black;"><p>Ennyi másodperc várakozás után próbálkozik meg ismét a szolgáltatás a nem működő kapcsolatok elérésével.</p></td>
<td style="border:1px solid black;"><p>Ennek a beállításnak a módosítására csak kivételes körülmények között lehet szükség.</p></td>
</tr>  
<tr class="odd">
<td style="border:1px solid black;"><p>TimeRetrySlow</p></td>
<td style="border:1px solid black;"><p>DWORD</p></td>
<td style="border:1px solid black;"><p>30</p></td>
<td style="border:1px solid black;"><p>Ennyi másodperc várakozás után próbálkozik meg ismét a szolgáltatás a lassú kapcsolatok elérésével.</p></td>
<td style="border:1px solid black;"><p>Ennek a beállításnak a módosítására csak kivételes körülmények között lehet szükség.</p></td>
</tr>  
<tr class="even">
<td style="border:1px solid black;"><p>WtRoundRobin</p></td>
<td style="border:1px solid black;"><p>DWORD</p></td>
<td style="border:1px solid black;"><p>1</p></td>
<td style="border:1px solid black;"><p>A ciklikus multiplexelés súlya a terheléselosztás szempontjából.</p></td>
<td style="border:1px solid black;"><p>A ciklikus multiplexelés viszonylagos fontossága a terheléselosztáson belül. Az 1 a legkisebb érték.</p></td>
</tr>  
<tr class="odd">
<td style="border:1px solid black;"><p>WtThreadCount</p></td>
<td style="border:1px solid black;"><p>DWORD</p></td>
<td style="border:1px solid black;"><p>100</p></td>
<td style="border:1px solid black;"><p>A kapcsolatonkénti szálak számának súlya a terheléselosztás szempontjából.</p></td>
<td style="border:1px solid black;"><p>A szálak kis számának viszonylagos fontossága.</p></td>
</tr>  
<tr class="even">
<td style="border:1px solid black;"><p>WtSlow</p></td>
<td style="border:1px solid black;"><p>DWORD</p></td>
<td style="border:1px solid black;"><p>1,000</p></td>
<td style="border:1px solid black;"><p>A lassú kapcsolat súlya a terheléselosztás szempontjából.</p></td>
<td style="border:1px solid black;"><p>Annak a viszonylagos súlya, hogy a kapcsolat nem lassú.</p></td>
</tr>  
<tr class="odd">
<td style="border:1px solid black;"><p>TimeOutForGC</p></td>
<td style="border:1px solid black;"><p>DWORD</p></td>
<td style="border:1px solid black;"><p>5</p></td>
<td style="border:1px solid black;"><p>Ennyi másodpercig vár a szolgáltatás, mielőtt sikertelennek minősítené az egy globális katalógusnak a lekérdezéslistába való felvételére irányuló kérelmet.</p></td>
<td style="border:1px solid black;"></td>
</tr>  
<tr class="even">
<td style="border:1px solid black;"><p>LdapTimeOut</p></td>
<td style="border:1px solid black;"><p>DWORD</p></td>
<td style="border:1px solid black;"><p>5</p></td>
<td style="border:1px solid black;"><p>Ennyi másodpercig vár a rendszer az LDAP API-hívások időtúllépése előtt.</p></td>
<td style="border:1px solid black;"></td>
</tr>  
<tr class="odd">
<td style="border:1px solid black;"><p>TopDownExpansionLDAPTimeOut</p></td>
<td style="border:1px solid black;"><p>DWORD</p></td>
<td style="border:1px solid black;"><p>40</p></td>
<td style="border:1px solid black;"><p>Ennyi másodpercig vár a rendszer a felülről lefelé irányuló LDAP-behelyettesítési lekérdezések időtúllépése előtt.</p></td>
<td style="border:1px solid black;"></td>
</tr>  
</tbody>  
</table>
  
| ![](images/Cc747660.Caution(WS.10).gif)Figyelmeztetés:                                                                                                                        |  
|------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|  
| A rendszerleíró adatbázis nem megfelelő módosítása súlyos károkat okozhat a rendszerben. A rendszerleíró adatbázis módosítása előtt készítsen biztonsági másolatot a számítógépen tárolt fontos adatokról. |
