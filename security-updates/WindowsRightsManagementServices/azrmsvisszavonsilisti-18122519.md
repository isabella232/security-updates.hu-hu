---
TOCTitle: Az RMS visszavonási listái
Title: Az RMS visszavonási listái
ms:assetid: '688d4dfa-c928-4b2f-8116-2f9e87d2b6f7'
ms:contentKeyID: 18122519
ms:mtpsurl: 'https://technet.microsoft.com/hu-hu/library/Cc720287(v=WS.10)'
---

Az RMS visszavonási listái
==========================

A visszavonási listák felsorolják a visszavont érvényességű tartalmat, alkalmazásokat, felhasználókat és más résztvevőket. Például az alábbi okoknál fogva vehetnek fel a szervezetek a visszavonási listára egy entitást:

-   Tudják vagy gyanítják, hogy sérült a személyes kulcs biztonsága.
-   Egy tulajdonos kéri egy kulcs érvényességének visszavonását, mert véleménye szerint sérült a kulcs biztonsága.
-   Egy résztvevő többé nem érvényes (például megszűnt egy dolgozó munkaviszonya).
-   Akadályba ütközik a védelmi rendszabályok betartatása (például sérült az egyik ügyfélszámítógép részére kiállított tanúsítvány biztonsága).
-   Az engedélyezésben beállt módosítások folytán új tanúsítványok kiosztása vált szükségessé.
-   Egy RMS-kompatibilis alkalmazásban biztonsági rések észlelhetők, amelyekből fakadóan nem alkalmas szigorúan titkos, vagy egyáltalán bármiféle védett tartalom használatára.
-   Egy korábban terjesztett tartalom érvényessége lejárt, vagy immár nem alkalmas használatra.

A következő táblázat bemutatja, hogy milyen entitások vehetők fel a visszavonási listákba, párhuzamosan az entitások azonosítására használt információkkal.

###  

 
<table style="border:1px solid black;">
<colgroup>
<col width="50%" />
<col width="50%" />
</colgroup>
<thead>
<tr class="header">
<th style="border:1px solid black;" >Entitás</th>
<th style="border:1px solid black;" >Azonosító</th>
</tr>
</thead>
<tbody>
<tr class="odd">
<td style="border:1px solid black;">Licencek vagy tanúsítványok egy csoportja</td>
<td style="border:1px solid black;">A kiállító azonosítója vagy nyilvános kulcsa</td>
</tr>
<tr class="even">
<td style="border:1px solid black;">Alkalmazási jegyzékfájlok egy csoportja</td>
<td style="border:1px solid black;">A kiállító azonosítója vagy nyilvános kulcsa</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;">Egy bizonyos licenc vagy tanúsítvány</td>
<td style="border:1px solid black;">A licenc azonosítója vagy kivonata</td>
</tr>
<tr class="even">
<td style="border:1px solid black;">Egy bizonyos alkalmazási jegyzékfájl</td>
<td style="border:1px solid black;">A licenc azonosítója vagy kivonata</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;">Egy bizonyos résztvevő</td>
<td style="border:1px solid black;">A résztvevő azonosítója vagy nyilvános kulcsa</td>
</tr>
<tr class="even">
<td style="border:1px solid black;">Egy bizonyos tartalom</td>
<td style="border:1px solid black;">A tartalom azonosítója</td>
</tr>
</tbody>
</table>
  
| ![](images/Cc720287.note(WS.10).gif)Megjegyzés:                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                     |  
|----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|  
| A visszavonásnál és a kizárásnál használt kivonatok mind az SHA-1 \[NIS94c\] algoritmussal készülnek, amely az SHS, FIPS 180 szabványban megadott SHA algoritmus átdolgozott változata. Az SHA-1 algoritmust az ANSI X9.30 szabvány 2. része írja le. Az alkalmazási jegyzékfájl szerinti visszavonáshoz az alkalmazási jegyzékfájlból ki kell nyernie a kiállító azonosítóját, a kiállító nyilvános kulcsát, a licencazonosítót vagy a licenckivonatot. Az alkalmazási jegyzékfájlok azonban base 64 kódolásúak, így az adatok közvetlenül nem érhetők el. A tartalomvédelmi szolgáltatások SDK készletének **DRMConstructCertificateChain**, **DRMDeconstructCertificateChain** és **DRMDecode** metódusával készíthető olyan program, amellyel dekódolható az alkalmazási jegyzékfájl, és így megszerezhetők a kívánt adatok. Ha meg szeretné akadályozni, hogy adott alkalmazás képes legyen az RMS-védelemmel ellátott tartalom használatára, érdemes megfontolni az alkalmazás kizárását, hogy így az RMS kiszolgáló ne adjon használati licencet ennek az alkalmazásnak. A kizárás azzal a megszorítással érvényes, hogy nem tudja meggátolni, hogy egy érvényes használati licenccel rendelkező felhasználó visszafejtse az RMS-védelemmel ellátott tartalmat. Az alkalmazások kizárásáról a további tudnivalókat lásd a dokumentumgyűjtemény „RMS kiszolgáló működtetése” részében az Alkalmazások kizárása témakörben. |
  
A visszavonási listák XrML fájlok, a következő paramétereket adják meg.
  
###  

 
<table style="border:1px solid black;">
<colgroup>
<col width="50%" />
<col width="50%" />
</colgroup>
<thead>
<tr class="header">
<th style="border:1px solid black;" >Paraméter</th>
<th style="border:1px solid black;" >Leírás</th>
</tr>
</thead>
<tbody>
<tr class="odd">
<td style="border:1px solid black;">ISSUEDTIME</td>
<td style="border:1px solid black;">Az XrML fájl létrehozásakor érvényes rendszeridő. Ezt a használati licencekben szereplő REFRESH feltétel használja visszavonási lista korának megállapítására.</td>
</tr>
<tr class="even">
<td style="border:1px solid black;">ISSUER</td>
<td style="border:1px solid black;">A visszavonási lista kiállítójának neve, azonosítója és címe.</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;">PUBLICKEY</td>
<td style="border:1px solid black;">A visszavonási lista kiállítójának nyilvános kulcsa.</td>
</tr>
<tr class="even">
<td style="border:1px solid black;">REVOCATIONLIST</td>
<td style="border:1px solid black;">A visszavont entitások nevének, típusának és azonosítójának felsorolása.</td>
</tr>
</tbody>
</table>
