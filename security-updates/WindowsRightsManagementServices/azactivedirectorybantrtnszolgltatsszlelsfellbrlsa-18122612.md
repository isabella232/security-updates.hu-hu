---
TOCTitle: Az Active Directoryban történő szolgáltatásészlelés felülbírálása
Title: Az Active Directoryban történő szolgáltatásészlelés felülbírálása
ms:assetid: '9d97e7fb-5b05-4853-ad7b-6cc82b9729f0'
ms:contentKeyID: 18122612
ms:mtpsurl: 'https://technet.microsoft.com/hu-hu/library/Cc747614(v=WS.10)'
---

Az Active Directoryban történő szolgáltatásészlelés felülbírálása
=================================================================

Az RMS szolgáltatásai és ügyfelei először a helyi rendszerleíró adatbázisban keresik a szolgáltatások helyét. Ha a rendszerleíró adatbázis bizonyos kulcsai nem tartalmaznak értéket, az RMS szolgáltatásai és ügyfelei az Active Directoryban keresik a szolgáltatás kapcsolódási pontját (SCP). Ez azt jelenti, hogy ha beír meghatározott kulcsokat a kiszolgáló vagy az ügyfél rendszerleíró adatbázisába, felülbírálhatja az alapértelmezett, az Active Directoryban való észlelést eredményező beállítást.

| ![](images/Cc747614.note(WS.10).gif)Megjegyzés:                                                                                                                 |
|----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| Ha az RMS legfelső szintű fürtje úgy van beállítva, hogy az SCP nincs közzétéve az Active Directoryban,ezeket a kulcsokat használhatja a megfelelő hely megadásához az RMS-ügyfelek számára. |

Ez a rész ezeket a rendszerleíró bejegyzéseket és létrehozásuk módját ismerteti.

Szolgáltatásészlelés felülbírálása licencelésre szolgáló fürt aligényléséhez
----------------------------------------------------------------------------

Ha olyan csak licencelésre szolgáló fürtöt létesít, amelyet aligénylés keretében a licencelői fürt Active Directory erdőjében működő legfelső szintű tanúsítási fürttől eltérő legfelső szintű tanúsítási fürtbe kíván bejegyezni, akkor mind az aligénylési, mind a fióktanúsítási szolgáltatások észlelését felül kell bírálni.

#### A bejegyzések ismertetése

Az aligénylési és a fióktanúsítási szolgáltatások felülbírálásához a következő bejegyzések használhatók.

-   **SubEnrollmentURL**. Ez a bejegyzés annak a legfelső szintű fürtnek az elérési útvonalát adja meg, amelyet a licencelői kiszolgáló használ kiszolgálói licencelői tanúsítványának igénylésekor.
-   **GicURL**. Ez a bejegyzés a fióktanúsítási szolgáltatás elérési útvonalát adja meg az adott licencelői fürt számára.

#### A bejegyzések részletei

A Windows Server 2003 32 bites verzióját futtató számítógépeken a licencelésre szolgáló fürt aligényléséhez a szolgáltatásészlelési bejegyzések alkulcsának teljes elérési útvonala a következő:

**HKEY\_LOCAL\_MACHINE\\Software\\Microsoft\\DRMS\\1.0**

A Windows Server 2003 64 bites verzióját futtató számítógépeken a licencelésre szolgáló fürt aligényléséhez a szolgáltatásészlelési bejegyzések alkulcsának teljes elérési útvonala a következő:

**HKEY\_LOCAL\_MACHINE\\SoftwareWOW6432Node\\Microsoft\\DRMS\\1.0**

A következő táblázat azokat a bejegyzéseket tartalmazza, amelyek létrehozásával felülbírálható a szolgáltatásészlelés.

###  

 
<table style="border:1px solid black;">
<colgroup>
<col width="33%" />
<col width="33%" />
<col width="33%" />
</colgroup>
<thead>
<tr class="header">
<th style="border:1px solid black;" >Név</th>
<th style="border:1px solid black;" >Típus</th>
<th style="border:1px solid black;" >Érték</th>
</tr>
</thead>
<tbody>
<tr class="odd">
<td style="border:1px solid black;">SubEnrollmentURL</td>
<td style="border:1px solid black;">Karakterlánc</td>
<td style="border:1px solid black;">http(vagy https)://<em>kiszolgálónév</em>/_wmcs/certification/subenrollservice.asmx</td>
</tr>
<tr class="even">
<td style="border:1px solid black;">GicURL</td>
<td style="border:1px solid black;">Karakterlánc</td>
<td style="border:1px solid black;">http(vagy https)://<em>kiszolgálónév</em>/_wmcs/certification/certification.asmx</td>
</tr>
</tbody>
</table>
  
Az ügyféloldali szolgáltatásészlelés felülbírálása közzétételhez  
----------------------------------------------------------------
  
Ha a felhasználók a számítógépükről fogják közzétenni a tartalmat, a vállalatnál alkalmazott topológiának megfelelően felülbírálhatja a közzétételhez használt kiszolgálók helyét. A közzétételhez használt kiszolgálók helyét szokásos esetben az ügyfél az Active Directory segítségével keresi meg. Az ügyfélszámítógépeken megfelelő rendszerleíró kulcsok felvételével elérheti, hogy az ügyfelek a fenti módszer helyett az ezekben megadott URL-címeket fogják használni.
  
| ![](images/Cc747614.note(WS.10).gif)Megjegyzés:                                                                                                                   |  
|------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|  
| Az itt bemutatott felülbírálásokat önálló bejegyzés helyett kulcsként kell létrehozni. Ezeknek a kulcsoknak az értékét az egyes kulcsok alapértelmezés szerinti bejegyzésében kell létrehozni. |
  
#### A beállításkulcsok ismertetése
  
Az RMS fürt automatikus észlelésének felülbírálásához a következő beállításkulcsok használhatók.
  
-   **Activation**. Ez a beállításkulcs a gépaktiválási szolgáltatás URL-címét adja meg. Ha a Service Pack 1 vagy újabb javítócsomaggal bővített RMS ügyfélszoftvert használ, ez a bejegyzés már nem szerepel.  
-   **EnterprisePublishing**. Ez a beállításkulcs az ügyfél licenckérelmeinél használni kívánt RMS-telepítés URL-címét adja meg.  
-   **CloudPublishing**. Ez a beállításkulcs a Microsoft által működtetett licencelési szolgáltatás URL-címét adja meg, amely akkor használható, ha az ügyfél nem fér hozzá egy RMS-telepítéshez, de az internetet eléri.
  
#### A kulcsok részletei
  
A közzétételnél az ügyféloldali szolgáltatásészlelés felülbírálásához tartozó alkulcs teljes elérési útvonala a következő:
  
**HKEY\_LOCAL\_MACHINE\\Software\\Microsoft\\MSDRM\\ServiceLocation\\**
  
A következő táblázat az RMS ügyfélszámítógépeken a szolgáltatásészlelés felülbírálásához használható beállításkulcsokat ismerteti.
  
###  

 
<table style="border:1px solid black;">
<colgroup>
<col width="33%" />
<col width="33%" />
<col width="33%" />
</colgroup>
<thead>
<tr class="header">
<th style="border:1px solid black;" >Név</th>
<th style="border:1px solid black;" >Típus</th>
<th style="border:1px solid black;" >Érték</th>
</tr>
</thead>
<tbody>
<tr class="odd">
<td style="border:1px solid black;">Activation</td>
<td style="border:1px solid black;">Karakterlánc</td>
<td style="border:1px solid black;">http(vagy https)://<em>RMS_fürt_neve</em>/_wmcs/Certification ahol <em>RMS_fürt_neve</em> az adott RMS fürt neve.</td>
</tr>
<tr class="even">
<td style="border:1px solid black;">EnterprisePublishing</td>
<td style="border:1px solid black;">Karakterlánc</td>
<td style="border:1px solid black;">http(vagy https)://<em>RMS_fürt_neve</em>/_wmcs/Licensing ahol <em>RMS_fürt_neve</em> az adott RMS fürt neve.</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;">CloudPublishing</td>
<td style="border:1px solid black;">Karakterlánc</td>
<td style="border:1px solid black;">http(vagy https)://<em>FQDN_fürt_neve</em>/_wmcs/Licensing ahol <em>FQDN_fürt_neve</em> az RMS fürt teljesen megadott tartományneve.</td>
</tr>
</tbody>
</table>
  
Azt javasoljuk, hogy a beállításkulcsok megadását a Systems Management Server vagy a Csoportházirend segítségével hajtsa végre annak biztosításához, hogy a vállalatnál az összes ügyfél a megfelelő közzétételi kiszolgálókat használja.
  
| ![](images/Cc747614.Caution(WS.10).gif)Figyelmeztetés:                                                                                                     |  
|-----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|  
| A rendszerleíró adatbázis nem megfelelő módosítása súlyosan károsíthatja a rendszert. Mielőtt módosítaná a rendszerleíró adatbázist, készítsen biztonsági másolatot a fontos adatokról. |
  
A megfelelő beállításkulcsok importálásához az RMS fürt egyes kiszolgálóira egy mintaként szolgáló beállításfájl (.reg) használható.
  
**A megfelelő beállításkulcsok importálása az RMS fürt egyes kiszolgálóira**  
1.  Másolja a következő, mintaként szolgáló beállításfájlt a segédprogrammal megnyitott fájlba.
  
    `Windows Registry Editor Version 5.00`
  
    `[HKEY_LOCAL_MACHINE\SOFTWARE\Microsoft\MSDRM\ServiceLocation]`
  
    `[HKEY_LOCAL_MACHINE\SOFTWARE\Microsoft\MSDRM\ServiceLocation\Activation]`
  
    `@="http://<RMS_cluster_name>/_wmcs/certification"`
  
    `[HKEY_LOCAL_MACHINE\SOFTWARE\Microsoft\MSDRM\ServiceLocation\EnterprisePublishing]`
  
    `@="http://<RMS_cluster_name>/_wmcs/licensing"`
  
2.  Az &lt;RMS\_fürt\_neve&gt; helyére írja be az adott RMS fürt nevét.
  
3.  Mentse a fájlt .reg kiterjesztéssel.
  
4.  Kattintson duplán a fájl nevére az Intézőben.
  
5.  Ha megjelenik **A felhasználói fiókok beállítása** párbeszédablak, hagyja jóvá az abban megjelenő műveletet, és kattintson a **Tovább** gombra.. Az adatok felvételére vonatkozó üzenetpanelen kattintson az **Igen** gombra.
