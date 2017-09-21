---
TOCTitle: Az RMS szoftverkövetelményei
Title: Az RMS szoftverkövetelményei
ms:assetid: '17faf2ad-2366-4a92-98a5-766e20a0f741'
ms:contentKeyID: 18122444
ms:mtpsurl: 'https://technet.microsoft.com/hu-hu/library/Cc720201(v=WS.10)'
---

Az RMS szoftverkövetelményei
============================

Az RMS kiszolgálók működéséhez szükséges szoftverfeltételeket a következő táblázat ismerteti.

###  

<p> </p>
<table style="border:1px solid black;">
<colgroup>
<col width="50%" />
<col width="50%" />
</colgroup>
<thead>
<tr class="header">
<th>Szoftver</th>
<th>Követelmény</th>
</tr>
</thead>
<tbody>
<tr class="odd">
<td style="border:1px solid black;"><p>Operációs rendszer</p></td>
<td style="border:1px solid black;"><p>Microsoft Windows Server® 2003 bármely kiadása a Web Edition kivételével.</p></td>
</tr>  
<tr class="even">
<td style="border:1px solid black;"><p>Fájlrendszer</p></td>
<td style="border:1px solid black;"><p>Az NTFS fájlrendszer javasolt.</p></td>
</tr>  
<tr class="odd">
<td style="border:1px solid black;"><p>Operációsrendszer-összetevők</p></td>
<td style="border:1px solid black;"><ul>
<li>Message Queuing (MSMQ) az Active Directory® címtárszolgáltatás-integráció támogatásával.<br />  
<br />  
</li>  
<li>Internet Information Services (IIS) engedélyezett ASP.NET összetevővel.<br />  
<br />  
</li>  
<li>Microsoft .NET Framework 1.1<br />  
<br />  
</li>
</ul></td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><p>Active Directory® címtárszolgáltatás</p></td>
<td style="border:1px solid black;"><p>Az RMS rendszert olyan Active Directory-tartományba kell telepíteni, amelyben a tartományvezérlőkön a Windows Server 2000 Service Pack 3 (SP3) vagy újabb csomaggal frissített verziója fut. Minden, az RMS-szolgáltatást tartalom elérésére és közzétételére használó felhasználónak e-mail címmel kell rendelkeznie, amelyet be kell állítani az Active Directoryban.</p></td>
</tr>  
<tr class="odd">
<td style="border:1px solid black;"><p>Adatbázis-kiszolgáló</p></td>
<td style="border:1px solid black;"><p>Az RMS adatbázist és tárolt eljárásokat igényel a működéshez. Használható a Microsoft SQL Server 2000 SP3a vagy újabb csomaggal, vagy a Microsoft SQL Server 2005. Tesztelés vagy egyéb, egyszámítógépes telepítés céljaira a Microsoft SQL Server Desktop Engine (MSDE 2000) SP3, illetve a Microsoft SQL Server 2005 Express Edition használható.</p></td>
</tr>  
</tbody>  
</table>
  
Ha az RMS üzembe állítása olyan környezetben történik, ahol több Active Directory erdő létezik, az Active Directory univerzális csoportjait kell használni, hogy a csoporttagság minden globális katalógusba replikálva legyen. Az univerzális csoportok létrehozása érdekében a tartomány működési szintjét legalább a natív Windows 2000 működési szintre kell beállítani, és az erdő működési szintjét a Windows Server 2003 szintre kell emelni.
  
Azt ajánljuk, hogy csak tesztkörnyezetben használja az MSDE 2000 vagy a Microsoft SQL Server Edition adatbázis-kezelőt az RMS adatbázisaihoz, mert az MSDE 2000 vagy a Microsoft SQL Server Edition semmilyen hálózati csatlakozófelületet sem támogat. Az MSDE 2000 vagy a Microsoft SQL Server Edition használati feltételei továbbá megtiltják az SQL Server ügyféleszközeinek használatát az MSDE 2000 vagy a Microsoft SQL Server Edition adatbázisok kezelésére. Ezt a korlátozást figyelembe véve nem áll majd módjában megtekinteni a naplózott adatokat, sem módosítani a konfigurációs adatbázisban tárolt adatokat. 
  
Ha az ASP.NET 1.1 verzió nincs telepítve a kiszolgálón, a telepítési folyamat különböző a 32 bites Windows Server 2003, illetve a 64 bites Windows Server 2003 rendszer esetében.
  
Ha a 32 bites Windows Server 2003 rendszert használja, az ASP.NET 1.1 verzió telepítéséhez és engedélyezéséhez hajtsa végre a következő lépéseket:
  
1.  Nyissa meg a **VezérlőpultProgramok telepítése és törlése** segédprogramját, és kattintson a **Windows-összetevők hozzáadása vagy eltávolítása** gombra.  
2.  Kattintson az **Alkalmazáskiszolgáló**, majd a **Részletek** elemre.  
3.  A Windows-összetevők varázslóban válassza az **ASP.NET** elemet.  
4.  Ha ASP.NET 1.1 telepítve van, de nincs engedélyezve az IIS webszolgáltatás bővítményeként:  
    -   Nyissa meg az Internet Information Services kezelőjét.  
    -   Kattintson az **IIS webszolgáltatás bővítménye** elemre, válassza az ASP.NET v1.1.4322 elemet, majd kattintson az **Engedélyezés** elemre.
  
Ha a 64 bites Windows Server 2003 rendszert használja, az ASP.NET 1.1 verzió telepítéséhez és engedélyezéséhez hajtsa végre a következő lépéseket:
  
1.  Telepítse a .NET keretrendszer 1.1-es verzióját, amely telepíti az ASP.NET 1.1 verziót. A Microsoft .NET keretrendszer 1.1-es verziójának terjeszthető csomagja letölthető a Microsoft letöltőközpontjából ([http://go.microsoft.com](http://go.microsoft.com/fwlink/?linkid=69985)).(http://go.microsoft.com/fwlink/?LinkId=69985)  
2.  Nyissa meg az Internet Information Services kezelőjét.  
3.  Kattintson az IIS webszolgáltatás bővítménye elemre, válassza az ASP.NET v1.1.4322 elemet, majd kattintson az Engedélyezés elemre.
  
Ha az RMS 64 bites Windows Server 2003 rendszeren fut, a következő lépésekkel engedélyezheti az IIS és az RMS együttműködését:
  
1.  Kattintson a **Start** gombra, és válassza a **Futtatás** parancsot.  
2.  A **Megnyitás** mezőbe írja be a következő parancsot, majd nyomja meg az ENTER billentyűt:
  
**"cscript %Rendszerlemezegység%\\inetpub\\AdminScripts\\adsutil.vbs set w3svc/AppPools/Enable32bitAppOnWin64 1"**
  
Az RMS nem a .NET Framework 2.0 verzióhoz lett kialakítva. A megengedett mellételepítéskor azonban garantálni kell, hogy az ASP.NET az ASP.NET v1.1.4322 használatára legyen konfigurálva. Két lehetőség van annak garantálására, hogy a mellételepítés sikeres legyen:
  
-   Biztosítsa, hogy a .NET Framework 2.0 telepítése az RMS kiszolgálószoftver telepítése előtt történjék.  
-   Állítsa vissza az ASP.NET verzióját a 1.1.4322 verzióra az IIS alapértelmezett webhelyén a következő paranccsal:
  
**"%SystemRoot%\\Microsoft.NET\\Framework\\v1.1.4322\\aspnet\_regiis -s w3svc/1/root"**
  
Az Active Directory, a Message Queuing és az IIS szolgáltatás részletes ismertetését lásd a Windows Server 2003 súgójában.
  
| ![](images/Cc720201.Caution(WS.10).gif)Figyelmeztetés:                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                             |  
|---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|  
| Az RMS kiszolgáló létesíthető az alapértelmezett webhelyen, illetve bármely olyan helyen, amelyet korábban definiált az IIS szolgáltatásban. Biztonsági szempontok miatt ezen a kiszolgálón nem tanácsos más webhelyet és szolgáltatást futtatni. Ellenkező esetben több alkalmazás és szolgáltatás futhat az RMS-szolgáltatással azonos fiókkal (különösképpen a Helyi rendszerfiókkal), ami azt a veszélyt rejti magában, hogy jogosulatlan műveleteket hajtanak végre személyes kulcsokkal. Ne létesítse az RMS kiszolgálót ugyanazon a webhelyen, amelyiken a Microsoft Office SharePoint Server 2007 fut. Az RMS nem használható Kerberos-hitelesítéssel. Amikor létesítik az RMS kiszolgálót egy webhelyen, a rendszer a letiltja Kerberos-hitelesítést azon a kiszolgálón. Ha az RMS nem lett az ASP.NET v1.1.4322 verzióra konfigurálva, nem történik naplózás a naplózási adatbázisban, ez adatveszteséget eredményez. |
  
Lásd még  
--------
  
####  
  
[Az adatbázis-kiszolgáló infrastruktúrájának tervezése](https://technet.microsoft.com/b12354bd-3143-4d1f-b5aa-450c4550653c)
