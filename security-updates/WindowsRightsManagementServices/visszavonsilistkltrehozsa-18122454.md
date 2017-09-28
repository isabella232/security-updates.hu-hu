---
TOCTitle: Visszavonási listák létrehozása
Title: Visszavonási listák létrehozása
ms:assetid: '1ef75199-3344-4225-84de-a863a777696a'
ms:contentKeyID: 18122454
ms:mtpsurl: 'https://technet.microsoft.com/hu-hu/library/Cc720208(v=WS.10)'
---

Visszavonási listák létrehozása
===============================

A visszavonás megvalósításához visszavonási lista alkalmazása szükséges. Ez az eXtensible Rights Markup Language (XrML) nyelvet használó XML dokumentum azokat a résztvevőket sorolja fel, amelyek ezután nem férhetnek hozzá a tartalomvédelemmel ellátott tartalomhoz. A visszavonási listákat időbélyeggel kell ellátni, és az RMS Visszavonási lista aláírása eszközével (RLsigner.exe) megfelelően alá kell írni.

| ![](images/Cc720208.Important(WS.10).gif)Fontos:                                                |
|------------------------------------------------------------------------------------------------------------------------------|
| A visszavonási lista RLsigner.exe programmal való aláírásához a visszavonási listát unicode kódolású fájlként kell mentenie. |

Visszavonási lista – példa
--------------------------

Ez a témakör egy olyan teljes visszavonási listát mutat be példaként, amelyben az összes visszavonási lehetőség szerepel. A példa alapján egyszerűen elkészíthetők a saját visszavonási listák.

A visszavonási lista az XrML nyelvet használó XML formátumú fájl.

A BODY elem négy gyermekelemet tartalmaz:

-   **ISSUEDTIME**. A visszavonási lista kiadási dátumát és időpontját tartalmazza. Ezt az elemet az RLsigner.exe program szúrja be a fájlba. A példában csak a visszavonási lista általános felépítésének bemutatása érdekében szerepel.
-   **DESCRIPTOR**. Azokat az adatokat tartalmazza, amelyek a fájlt visszavonási listaként azonosítják.
-   **ISSUER**. A visszavonási listát kiállító entitás azonosítására szolgáló adatokat tartalmazza.
-   **REVOCATIONLIST**. A gyermek REVOKE elemekből áll: ezek az adott listával visszavont entitásokat adják meg.

A példaként használható visszavonási lista az alábbiakban látható.

| ![](images/Cc720208.note(WS.10).gif)Megjegyzés:                                         |
|----------------------------------------------------------------------------------------------------------------------|
        ```
| ![](images/Cc720208.Caution(WS.10).gif)Figyelmeztetés:                                                                 |
|-----------------------------------------------------------------------------------------------------------------------------------------------------|
| Ha a visszavonási listában URL-címet ad meg, UNC-útvonal már nem használható az RMS SP1 és az RMS SP2 rendszerben. Ekkor URL-címet kell használnia. |

A REVOKE elemek megadása után a visszavonási lista készen áll az aláírásra.

A REVOKE elem használata
------------------------

A példafájl Visszavonási lista – példa szakaszában minden REVOKE elem olyan résztvevőt ad meg, amelyet vissza kell vonni. A nyitócímke kategória- és típusattribútuma adja meg, hogy mit kell visszavonni, és milyen azonosítási kritérium alapján. A különböző REVOKE elemek a kategória- és a típusattribútumban meghatározott művelettől függően különböző gyermekelemekből állnak.

A REVOKE elemek megadásáról további tudnivalókat talál a következő példákban:

-   [Résztvevők visszavonása nyilvános kulcs alapján](#bkmk_1)
-   [Tanúsítványok és licencek visszavonása GUID alapján](#bkmk_2)
-   [Tanúsítványok és licencek visszavonása kivonatérték alapján](#bkmk_3)
-   [Tanúsítványok és licencek visszavonása a kiállító nyilvános kulcsa alapján](#bkmk_4)
-   [Tanúsítványok és licencek visszavonása a kiállító azonosítója alapján](#bkmk_5)
-   [Tartalom visszavonása a tartalom azonosítója alapján](#bkmk_6)
-   [Tanúsítványok visszavonása a résztvevő azonosítója alapján](#bkmk_10)
-   [Résztvevők visszavonása Windows Live ID alapján](#bkmk_7)

<span id="BKMK_1"></span>
#### Résztvevők visszavonása nyilvános kulcs alapján

        ```

<span id="BKMK_2"></span>
#### Tanúsítványok és licencek visszavonása GUID alapján

        ```
#### Visszavonás alkalmazási jegyzékfájl megadásával

Az alkalmazási jegyzékfájl szerinti visszavonáshoz az alkalmazási jegyzékfájlból ki kell nyernie a kiállító azonosítóját, a kiállító nyilvános kulcsát, a licencazonosítót vagy a licenckivonatot. Az alkalmazási jegyzékfájlok azonban base 64 kódolásúak, így az adatok egyszerű szövegként nem érhetők el. A Tartalomvédelmi szolgáltatások SDK (Software Development Kit) készletének DRMConstructCertificateChain, DRMDeconstructCertificateChain és DRMDecode metódusával készíthető olyan program, amellyel dekódolható az alkalmazási jegyzékfájl, és így megszerezhetők a kívánt adatok.

Ha meg szeretné akadályozni, hogy adott alkalmazás képes legyen a védelemmel ellátott tartalom használatára, érdemes megfontolni az alkalmazás kizárását, hogy így az RMS fürt ne adjon használati licencet ennek az alkalmazásnak. A kizárás azzal a megszorítással érvényes, hogy nem tudja meggátolni, hogy egy érvényes használati licenccel rendelkező felhasználó visszafejtse a tartalomvédelemmel ellátott tartalmat. Alkalmazás kizárásáról lásd a témakör [Alkalmazások kizárása](https://technet.microsoft.com/b68ae4b2-b9ba-44ae-90cb-c88df600ec86) című pontját.

<span id="BKMK_3"></span>
#### Tanúsítványok és licencek visszavonása kivonatérték alapján

        ```
#### Visszavonás alkalmazási jegyzékfájl megadásával

Az alkalmazási jegyzékfájl szerinti visszavonáshoz az alkalmazási jegyzékfájlból ki kell nyernie a kiállító azonosítóját, a kiállító nyilvános kulcsát, a licencazonosítót vagy a licenckivonatot. Az alkalmazási jegyzékfájlok azonban base 64 kódolásúak, így az adatok egyszerű szövegként nem érhetők el. A Tartalomvédelmi szolgáltatások SDK készletének DRMConstructCertificateChain, DRMDeconstructCertificateChain és DRMDecode metódusával készíthető olyan program, amellyel dekódolható az alkalmazási jegyzékfájl, és így megszerezhetők a kívánt adatok.

Ha meg szeretné akadályozni, hogy adott alkalmazás képes legyen a védelemmel ellátott tartalom használatára, érdemes megfontolni az alkalmazás kizárását, hogy így az RMS fürt ne adjon használati licencet ennek az alkalmazásnak. A kizárás azzal a megszorítással érvényes, hogy nem tudja meggátolni, hogy egy érvényes használati licenccel rendelkező felhasználó visszafejtse az RMS-védelemmel ellátott tartalmat. Alkalmazás kizárásáról lásd a témakör [Alkalmazások kizárása](https://technet.microsoft.com/b68ae4b2-b9ba-44ae-90cb-c88df600ec86) című pontját.

<span id="BKMK_4"></span>
#### Tanúsítványok és licencek visszavonása a kiállító nyilvános kulcsa alapján

        ```

<span id="BKMK_5"></span>
#### Tanúsítványok és licencek visszavonása a kiállító azonosítója alapján

        ```
| ![](images/Cc720208.note(WS.10).gif)Megjegyzés:                                                                                                                                                                   |
|------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| Az azonosítótípus megadásakor ügyeljen arra, hogy ne legyen kocsivissza karakter a GUID azonosító és a záró címke között. Ha véletlenül kocsivissza karakter kerül az említett helyre, az RMS-ügyfél nem tudja elemezni a visszavonási listát. |

<span id="BKMK_6"></span>
#### Tartalom visszavonása a tartalom azonosítója alapján

        ```
| ![](images/Cc720208.note(WS.10).gif)Megjegyzés:                                                                                                                                                                   |
|------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| Az azonosítótípus megadásakor ügyeljen arra, hogy ne legyen kocsivissza karakter a GUID azonosító és a záró címke között. Ha véletlenül kocsivissza karakter kerül az említett helyre, az RMS-ügyfél nem tudja elemezni a visszavonási listát. |

<span id="BKMK_10"></span>
#### Résztvevők visszavonása Windows fiók alapján

        ```
| ![](images/Cc720208.note(WS.10).gif)Megjegyzés:                                                                                                                                                                                        |
|---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| Az azonosítótípus megadásakor ügyeljen arra, hogy ne legyen kocsivissza karakter a Windows fiók biztonsági azonosítója és a záró címke között. Ha véletlenül kocsivissza karakter kerül az említett helyre, az RMS-ügyfél nem tudja elemezni a visszavonási listát. |

<span id="BKMK_7"></span>
#### Résztvevők visszavonása Windows Live ID alapján

        ```
| ![](images/Cc720208.note(WS.10).gif)Megjegyzés:                                                                                                                                                                   |
|------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| Az azonosítótípus megadásakor ügyeljen arra, hogy ne legyen kocsivissza karakter a PUID azonosító és a záró címke között. Ha véletlenül kocsivissza karakter kerül az említett helyre, az RMS-ügyfél nem tudja elemezni a visszavonási listát. |

<span id="BKMK_8"></span>
Aláírás beszúrása a visszavonási listába
----------------------------------------

A visszavonási lista létrehozása után az itt bemutatott módon aláírást kell beszúrnia a visszavonási listába. Ezután a kapcsolódó jogmegadási sablonban meghatározott URL-címen közzéteheti a visszavonási listát a felhasználók számára.

Az aláírás beszúrásának első lépéseként elő kell állítania egy kulcspárt és egy kulcsfájlt a visszavonási listához az Nehezen feltörhető jelszó eszközzel (Sn.exe). Az Sn.exe program a Microsoft .NET-keretrendszer 1.1-es szoftverfejlesztői készletének része, amely letölthető a Microsoft webhelyéről: [http://go.microsoft.com/fwlink/?LinkId=104796](http://go.microsoft.com/fwlink/?linkid=104796).

A visszavonási listát unicode kódolású fájlként kell mentenie, hogy aláírható legyen az RLsigner.exe programmal.

**Az új kulcspár előállítása és annak fájlba írása**
1.  Hozza létre a személyes kulcsot. Írja be a parancssorba a következő parancsot, majd nyomja meg az ENTER billentyűt:

    **sn -k** *személyes\_kulcs\_fájl***.snk**

    ahol *személyes\_kulcs\_fájl* a kulcsfájl neve.

2.  Az Sn.exe segítségével az 1. lépésben létrehozott kulcspárfájlból kinyerheti a nyilvános kulcsot, és azt külön fájlba exportálhatja. Írja be a következő parancsot, majd nyomja meg az ENTER billentyűt:

    **sn -p** *személyes\_kulcs\_fájl nyilvános\_kulcs\_fájl*

    ahol *személyes\_kulcs\_fájl* az 1. lépésben létrehozott kulcsfájl neve, míg *nyilvános\_kulcs\_fájl* annak a fájlnak a neve, amelyben az exportált nyilvános kulcsot kívánja tárolni.

3.  Változtassa meg az 1. lépésben létrehozott kulcsfájl kiterjesztését: az .snk helyett ez legyen .dat az RLsigner.exe programmal való használathoz.

4.  Ezután RLsigner.exe programmal szúrja be az aláírást a visszavonási listát tartalmazó fájlba. Ez a program az RMS része. Alapértelmezés szerint a %systemdrive%\\Program Files\\Windows Rights Management Services\\Tools könyvtárban található.

| ![](images/Cc720208.note(WS.10).gif)Megjegyzés:           |
|----------------------------------------------------------------------------------------|
| Az RLsigner.exe program nem teszi lehetővé a szóközt tartalmazó fájlnevek használatát. |

<span id="BKMK_9"></span>
Az RLsigner.exe használata
--------------------------

Az RLsigner.exe program a futtatásakor elsőként a kulcsfájlban megadott személyes kulcs alapján egy aláírást hoz létre. Ezután a visszavonási listát tartalmazó megadott fájl alapján egy kimeneti fájlt állít elő.

| ![](images/Cc720208.Important(WS.10).gif)Fontos:                               |
|-------------------------------------------------------------------------------------------------------------|
| A visszavonási listát unicode kódolású fájlként kell mentenie az RLsigner.exe programmal való használathoz. |

Az RLsigner.exe programmal a visszavonási lista aláírásához írja be a parancssorba a következő parancsot:

**rlsigner.exe** *bemeneti\_fájl* **{-f** *kulcsfájl* **| -h** *tároló\_neve* **CSP}** *kimeneti\_fájl*

A parancs paramétereit az alábbiak alapján adja meg:

###  

 
<table style="border:1px solid black;">
<colgroup>
<col width="50%" />
<col width="50%" />
</colgroup>
<thead>
<tr class="header">
<th>Paraméter</th>
<th>Leírás</th>
</tr>
</thead>
<tbody>
<tr class="odd">
<td style="border:1px solid black;"><em>bemeneti_fájl</em></td>
<td style="border:1px solid black;">A korábban elkészített, a visszavonási listát tartalmazó XrML-kompatibilis fájl neve</td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><em>kulcsfájl</em></td>
<td style="border:1px solid black;">A korábban előállított, a nyilvános és a személyes kulcsot tartalmazó fájl neve</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><em>tároló_neve</em></td>
<td style="border:1px solid black;">A kulcstároló neve</td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><em>kimeneti_fájl</em></td>
<td style="border:1px solid black;">A programmal előállított, az aláírt visszavonási listát tartalmazó fájl neve</td>
</tr>
</tbody>
</table>
  
| ![](images/Cc720208.note(WS.10).gif)Megjegyzés:           |  
|----------------------------------------------------------------------------------------|  
| Az RLsigner.exe program nem teszi lehetővé a szóközt tartalmazó fájlnevek használatát. |
  
A következő példákból megismerheti, hogyan használhatja az RLsigner.exe programot a parancssorból különböző kriptográfiai szolgáltatókkal:
  
-   Kulcsfájlt használó parancssori szintaxis:  
    **rlsigner.exe rl.xml -f kulcs.dat kimenet.xml**  
-   Hardveres biztonsági modult használó parancssori szintaxis:  
    **rlsigner.exe rl.xml -h Tároló CSP kimenet.xml**
  
Az RLsigner.exe program visszatérési kódja a sikeres végrehajtást, illetve hibánál annak típusát jelzi. A következő táblázat a lehetséges visszatérési kódokat ismerteti.
  
###  

 
<table style="border:1px solid black;">
<colgroup>
<col width="50%" />
<col width="50%" />
</colgroup>
<thead>
<tr class="header">
<th>Visszatérési kód</th>
<th>Leírás</th>
</tr>
</thead>
<tbody>
<tr class="odd">
<td style="border:1px solid black;">0</td>
<td style="border:1px solid black;">Sikeres végrehajtás</td>
</tr>
<tr class="even">
<td style="border:1px solid black;">-1</td>
<td style="border:1px solid black;">Nem olvasható a forrásfájl</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;">-2</td>
<td style="border:1px solid black;">Nem olvasható a kulcsfájl</td>
</tr>
<tr class="even">
<td style="border:1px solid black;">-3</td>
<td style="border:1px solid black;">Érvénytelen kulcsfájl</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;">-4</td>
<td style="border:1px solid black;">Érvénytelen forrásfájl</td>
</tr>
<tr class="even">
<td style="border:1px solid black;">-5</td>
<td style="border:1px solid black;">Nem írható a kimeneti fájl</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;">-6</td>
<td style="border:1px solid black;">Ismeretlen hiba</td>
</tr>
</tbody>
</table>
  
Szükségessé válhat a visszavonási listák aláírásának ütemezése a kiszolgálóhoz megadott frissítési gyakoriság alapján.
  
A visszavonási lista aláírásának eljárását parancsfájl használatával automatizálhatja. A következő VBScript az RLsigner.exe parancsot hívja, és az eredményeket a rendszer eseménynaplójába írja.
  
<codesnippet asp="http://msdn2.microsoft.com/asp" language displaylanguage="Visual Basic">const EVT\_SUCCESS = 0 const EVT\_ERROR = 1 const EVT\_WARNING = 2 const EVT\_INFORMATION = 4 const EVT\_AUDIT\_SUCCESS = 8 const EVT\_AUDIT\_FAILURE = 16 Dim WshShell, oExec Set WshShell = CreateObject( "WScript.Shell" ) Set oExec = WshShell.Exec("rlsigner.exe input\_file key\_file output\_file") Do While oExec.Status = 0 WScript.Sleep 100 Loop if WshShell.ExitCode &lt;&gt; 0 Then WshShell.LogEvent EVT\_ERROR, "RLsigner failed with error """ + WshShell.ExitCode + """" else WshShell.LogEvent EVT\_SUCCESS, "RLsigner completed successfully" end if  
```
