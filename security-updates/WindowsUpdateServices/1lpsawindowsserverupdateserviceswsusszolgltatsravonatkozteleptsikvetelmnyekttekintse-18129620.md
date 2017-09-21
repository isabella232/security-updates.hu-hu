---
TOCTitle: '1. lépés: A Windows Server Update Services (WSUS) szolgáltatásra vonatkozó telepítési követelmények áttekintése'
Title: '1. lépés: A Windows Server Update Services (WSUS) szolgáltatásra vonatkozó telepítési követelmények áttekintése'
ms:assetid: '57d7f8ec-1523-4485-9967-604be9ba2aac'
ms:contentKeyID: 18129620
ms:mtpsurl: 'https://technet.microsoft.com/hu-hu/library/Cc720547(v=WS.10)'
---

1. lépés: A Windows Server Update Services (WSUS) szolgáltatásra vonatkozó telepítési követelmények áttekintése
===============================================================================================================

Ez a rész a WSUS szolgáltatás Microsoft Windows Server 2003 operációs rendszerre történő telepítéséhez tartalmaz útmutatást (a Web Edition verzió és a 64 bites verziók kivételével). Ha kiszolgálóján a Microsoft Windows 2000 Server rendszer működik, és további információra van szüksége, tanulmányozza a „Deploying Microsoft Windows Server Update Services” (A Microsoft Windows Server Update Services szolgáltatás központi telepítése) című (angol nyelvű) szakmai dokumentációt.

A következőkben leírtak az alapértelmezett beállításokkal történő telepítés alapkövetelményeit jelentik. Az egyéb telepítési esetek hardverrel és szoftverrel szemben támasztott követelményeiről a „Deploying Microsoft Windows Server Update Services” című (angol nyelvű) szakmai dokumentációban talál bővebb felvilágosítást.

Hardverkövetelmények a legfeljebb ötszáz ügyfélszámítógéppel kapcsolatot létesítő kiszolgálókhoz:

-   1 gigahertzes (GHz) processzor
-   1 gigabájt (GB) RAM memória

Szoftverkövetelmények
---------------------

A WSUS szolgáltatás alapbeállításokkal történő telepítéséhez az alábbiakban felsorolt szoftverek megléte szükséges a számítógépen. A WSUS szoftverkövetelményeiről a „Deploying Microsoft Windows Server Update Services” című (angol nyelvű) szakmai dokumentációban olvashat részletesen. Amennyiben az itt említett frissítések bármelyike a számítógép újraindítását kéri a telepítés végeztével, akkor az újraindítást a WSUS alkalmazás telepítése előtt kell végrehajtani.

-   Microsoft Internet Information Services (IIS) 6.0 – az IIS szolgáltatás telepítésének mikéntjéről a „Deploying Microsoft Windows Server Update Services” című (angol nyelvű) szakmai dokumentáció és a Windows Server 2003 rendszer súgója nyújt bővebb információt.
-   Service Pack 1 szervizcsomag a Microsoft .NET-keretrendszer 1.1-es verziójához (Windows Server 2003) – a szoftver letölthető a Microsoft [letöltőközpontjából](http://go.microsoft.com/fwlink/?linkid=47358) (http://go.microsoft.com/fwlink/?LinkId=47358).
    Megteheti azt is, hogy ellátogat a http://www.windowsupdate.com webhelyre, és a keresőmezőbe beírja a „Critical Updates and Service Packs – Install Microsoft .NET Framework 1.1 Service Pack 1 for Windows Server 2003” kifejezést.
-   Háttérben futó intelligens átviteli szolgáltatás (BITS) 2.0 – a BITS szoftver Windows Server 2003 rendszerhez készült 2.0-s verziója jelenleg nem tölthető le a letöltőközpontból, ezért a [Microsoft Windows Update Services Open Evaluation webhelyről](http://go.microsoft.com/fwlink/?linkid=47357) (http://go.microsoft.com/fwlink/?LinkId=47357) kell letölteni.

| ![](images/Cc720547.note(WS.10).gif)Megjegyzés:                                                                                                                                                                                                             |
|------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| Habár a WSUS szolgáltatás telepítéséhez adatbázisszoftverre is szükség van, arról most nem teszünk említést, hiszen a Windows Server 2003 rendszerre telepített WSUS alkalmazás alapértelmezés szerint tartalmazza a Windows SQL Server™ 2000 Desktop Engine (WMSDE) adatbázisszoftvert. |

Merevlemezekkel kapcsolatos követelmények és ajánlások
------------------------------------------------------

A WSUS szolgáltatás telepítéséhez a kiszolgáló fájlrendszere meg kell, hogy feleljen az alábbi követelményeknek.

-   Mind a rendszerpartíciót, mind pedig a WSUS alkalmazást tároló partíciót NTFS fájlrendszerrel kell formázni.
-   A rendszerpartíciónak legalább 1 gigabájt (GB) szabad lemezterületet kell biztosítani.
-   A WSUS szolgáltatás tartalomtároláshoz használt kötetének lemezterülete legalább 6 gigabájt kell, hogy legyen (az ajánlott lemezterület 30 gigabájt).
-   A Windows SQL Server 2000 Desktop Engine (WMSDE) összetevő kötetéhez legalább 2 gigabájt szabad lemezterület szükséges.

Az Automatikus frissítések szolgáltatással kapcsolatos követelmények
--------------------------------------------------------------------

Az Automatikus frissítések segédprogram a WSUS szolgáltatás ügyfélszámítógépeken futó egyik összetevője, amelyhez mindössze annak a hardverkövetelménynek kell teljesülnie, hogy legyen működő hálózati kapcsolat. A WSUS szolgáltatás és az Automatikus frissítések összetevő a következő operációs rendszereken használható együtt:

-   Service Pack 3 (SP3) vagy Service Pack 4 (SP4) szervizcsomaggal bővített Microsoft Windows 2000 Professional rendszer, SP3 vagy SP4 csomaggal bővített Windows 2000 Server rendszer, valamint SP3 vagy SP4 csomaggal bővített Windows 2000 Advanced Server rendszer
-   Microsoft Windows XP Professional rendszer (Service Pack 1 vagy Service Pack 2 csomaggal, illetve anélkül)
-   Microsoft Windows Server 2003, Standard Edition, Windows Server 2003, Enterprise Edition, Windows Server 2003, Datacenter Edition vagy Windows Server 2003, Web Edition rendszer
