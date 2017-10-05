---
TOCTitle: Az RMS aligénylési szolgáltatása
Title: Az RMS aligénylési szolgáltatása
ms:assetid: '6b05e71c-5e7d-467c-9e13-35ac14d3718a'
ms:contentKeyID: 18122521
ms:mtpsurl: 'https://technet.microsoft.com/hu-hu/library/Cc720289(v=WS.10)'
---

Az RMS aligénylési szolgáltatása
================================

Az aligénylési szolgáltatás csak az RMS legfelső szintű fürtjén fut. Ez válaszol a licencelő fürtök kiszolgálóinak létesítése alkalmával a kiszolgálói licencelői tanúsítványok iránt benyújtott kérelmekre.

Az aligénylési szolgáltatás alkalmazásfájlja, a SubEnrollService.asmx, az *RMS\_webhely*\\\_wmcs\\Certification\\ virtuális könyvtárban található, ahol az *RMS\_webhely* annak a webhelynek a neve, amelyen az RMS létesítése történt.

A szolgáltatás alapértelmezés szerint csak a helyi rendszergazdák számára férhető hozzá. A csak licencelő fürt alárendelt kiszolgálójának létesítéséhez és aligényléséhez a licenckiszolgáló rendszergazdájának felhasználói fiókját fel kell venni a SubEnrollService.asmx tulajdonosi hozzáférés-szabályozási listára (DACL) teljes hozzáférési jogosultsággal.

A szolgáltatás alapértelmezett hozzáférési szabálygyűjteményét a következő táblázat szemlélteti:

###  

 
<table style="border:1px solid black;">
<colgroup>
<col width="50%" />
<col width="50%" />
</colgroup>
<thead>
<tr class="header">
<th style="border:1px solid black;" >Felhasználó vagy Csoport</th>
<th style="border:1px solid black;" >Alapértelmezett engedély</th>
</tr>
</thead>
<tbody>
<tr class="odd">
<td style="border:1px solid black;">RENDSZER</td>
<td style="border:1px solid black;">Teljes hozzáférés</td>
</tr>
</tbody>
</table>
