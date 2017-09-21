---
TOCTitle: Az RMS bevezetésének előfeltételei és feladatlistái
Title: Az RMS bevezetésének előfeltételei és feladatlistái
ms:assetid: '836d96ef-d0fd-4935-b595-e8dec19cbb2b'
ms:contentKeyID: 18122568
ms:mtpsurl: 'https://technet.microsoft.com/hu-hu/library/Cc747582(v=WS.10)'
---

Az RMS bevezetésének előfeltételei és feladatlistái
===================================================

Az RMS telepítésének megkezdése előtt nézze át az RMS használatának technológiai előfeltételeit. A felsorolt technológiák mind az RMS szerves részét képezik, és ezek alapvető ismerete nélkülözhetetlen az RMS sikeres bevezetéséhez. Az itt következő feladatlisták segítséget nyújtanak az RMS bevezetésének és felügyeletének megtervezésében:

-   [Technológiai előfeltételek](#bkmk_9)
-   [Az RMS bevezetési feladatlistái](#bkmk_10)
-   [Az RMS felügyeleti feladatlistái](#bkmk_14)

<span id="BKMK_9"></span>
Technológiai előfeltételek
--------------------------

Ez a dokumentumgyűjtemény segítséget nyújt a Windows RMS működésének megértéséhez, a szolgáltatás szervezeten belüli bevezetésének megtervezéséhez és kivitelezéséhez, valamint a rendszer napi felügyeletéhez. A dokumentáció megértésének feltétele, hogy az olvasó tájékozott legyen a következő területeken:

-   A Windows Server 2003 bevezetése és felügyelete
-   Az Active Directory bevezetése és felügyelete
-   A Microsoft® Internet Information Services 6.0 (IIS) bevezetése és felügyelete
-   A Microsoft® SQL Server™ 2000 felügyelete
-   A nyilvános kulcsok infrastruktúrájának (PKI) alapfogalmai
-   A kiszolgáló alapú hálózatok és azok védelme

Ezekről a kérdésekről a további tudnivalókat lásd a dokumentumgyűjtemény [RMS kiszolgáló működtetése](http://go.microsoft.com/fwlink/?linkid=42495) részében a „További források” témakörben.

<span id="BKMK_10"></span>
Az RMS bevezetési feladatlistái
-------------------------------

Ez a szakasz a következő bevezetési műveletekhez kínál feladatlistát:

-   [Egykiszolgálós telepítés bevezetése](#bkmk_11)
-   [Legfelső szintű tanúsítási fürt és licencelési fürt bevezetése](#bkmk_12)
-   [Az RMS bevezetése több erdőben](#bkmk_13)

Az RMS bevezetéséről a további tudnivalókat lásd a dokumentumgyűjtemény következő témakörében: [RMS rendszer bevezetése](http://go.microsoft.com/fwlink/?linkid=42494).

<span id="BKMK_11"></span>
Egykiszolgálós telepítés bevezetése
-----------------------------------

Egyetlen RMS kiszolgáló bevezetéséhez a következő feladatlista használható.

###  

<p> </p>
<table style="border:1px solid black;">
<colgroup>
<col width="50%" />
<col width="50%" />
</colgroup>
<thead>
<tr class="header">
<th>Lépés</th>
<th>Források</th>
</tr>
</thead>
<tbody>
<tr class="odd">
<td style="border:1px solid black;"><p>Ismerkedjen meg az alapfogalmakkal és a tervezéssel kapcsolatos tudnivalókkal.</p></td>
<td style="border:1px solid black;"><p>„Felkészülés az RMS bevezetésére” témakör, <a href="http://go.microsoft.com/fwlink/?linkid=42494">RMS rendszer bevezetése</a> rész.</p></td>
</tr>  
<tr class="even">
<td style="border:1px solid black;"><p>Nézze át a rendszerkövetelményeket, és ellenőrizze, hogy az összes szükséges hardver és szoftver rendelkezésre áll.</p></td>
<td style="border:1px solid black;"><p>„Az RMS infrastrukturális előfeltételei” témakör, <a href="http://go.microsoft.com/fwlink/?linkid=37537">RMS bevezetésének tervezése</a> rész.</p>
<p>„Az adatbázis-kiszolgáló infrastruktúrájának megtervezése” témakör, <a href="http://go.microsoft.com/fwlink/?linkid=37537">RMS bevezetésének tervezése</a> rész.</p></td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><p>Alakítsa ki az infrastruktúrát, teremtse meg a hardveres és szoftveres előfeltételeket, hozza létre a felügyeleti fiókokat, illetve igény szerint az SMS- vagy a Csoportházirend-támogatást.</p></td>
<td style="border:1px solid black;"><p>„Felkészülés az RMS bevezetésére” témakör, <a href="http://go.microsoft.com/fwlink/?linkid=42494">RMS rendszer bevezetése</a> rész.</p></td>
</tr>  
<tr class="even">
<td style="border:1px solid black;"><p>Telepítse a kiszolgálóra az RMS szolgáltatást, és hajtsa végre konfigurálását.</p></td>
<td style="border:1px solid black;"><p>„A tanúsítási és a licencelési szolgáltatás beállítása az első kiszolgálón” témakör, <a href="http://go.microsoft.com/fwlink/?linkid=42494">RMS rendszer bevezetése</a> rész.</p></td>
</tr>  
<tr class="odd">
<td style="border:1px solid black;"><p>Tesztelje a bevezetett rendszert.</p></td>
<td style="border:1px solid black;"><p>„Tesztkörnyezet kialakítása” témakör, <a href="http://go.microsoft.com/fwlink/?linkid=42494">RMS rendszer bevezetése</a> rész.</p></td>
</tr>  
<tr class="even">
<td style="border:1px solid black;"><p>Helyezze üzembe az RMS szolgáltatást az éles környezetben.</p></td>
<td style="border:1px solid black;"><p>„Az RMS rendszer hatókörének meghatározása” témakör, <a href="http://go.microsoft.com/fwlink/?linkid=42494">RMS rendszer bevezetése</a> rész.</p></td>
</tr>  
</tbody>  
</table>
  
<span id="BKMK_12"></span>  
Legfelső szintű tanúsítási fürt és licencelési fürt bevezetése  
--------------------------------------------------------------
  
A legfelső szintű tanúsítási és licencelési fürt bevezetéséhez a következő feladatlista használható.
  
###  

<p> </p>
<table style="border:1px solid black;">  
<colgroup>  
<col width="50%" />  
<col width="50%" />  
</colgroup>  
<thead>  
<tr class="header">  
<th>Lépés</th>  
<th>Források</th>  
</tr>  
</thead>  
<tbody>  
<tr class="odd">
<td style="border:1px solid black;"><p>Ismerkedjen meg az alapfogalmakkal és a tervezéssel kapcsolatos tudnivalókkal.</p></td>
<td style="border:1px solid black;"><p>„Felkészülés az RMS bevezetésére” témakör, <a href="http://go.microsoft.com/fwlink/?linkid=42494">RMS rendszer bevezetése</a> rész.</p></td>
</tr>  
<tr class="even">
<td style="border:1px solid black;"><p>Nézze át a rendszerkövetelményeket, és ellenőrizze, hogy az összes szükséges hardver és szoftver rendelkezésre áll.</p></td>
<td style="border:1px solid black;"><p>„Az RMS infrastrukturális előfeltételei” témakör, <a href="http://go.microsoft.com/fwlink/?linkid=37537">RMS bevezetésének tervezése</a> rész.</p>
<p>„Az adatbázis-kiszolgáló infrastruktúrájának megtervezése” témakör, <a href="http://go.microsoft.com/fwlink/?linkid=37537">RMS bevezetésének tervezése</a> rész.</p></td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><p>A bevezetési terv végiggondolásával döntsön a topológiáról és a telepítendő összetevőkről.</p></td>
<td style="border:1px solid black;"><p>„Az RMS topológiájának meghatározása” témakör, <a href="http://go.microsoft.com/fwlink/?linkid=37537">RMS bevezetésének tervezése</a> rész.</p></td>
</tr>  
<tr class="even">
<td style="border:1px solid black;"><p>Alakítsa ki az infrastruktúrát, teremtse meg a hardveres és szoftveres előfeltételeket, hozza létre a felügyeleti fiókokat, illetve igény szerint az SMS- vagy a Csoportházirend-támogatást.</p></td>
<td style="border:1px solid black;"><p>„Felkészülés az RMS bevezetésére” témakör, <a href="http://go.microsoft.com/fwlink/?linkid=42494">RMS rendszer bevezetése</a> rész.</p></td>
</tr>  
<tr class="odd">
<td style="border:1px solid black;"><p>Telepítse és konfigurálja az RMS szolgáltatást a legfelső szintű tanúsítási fürtbe tartozó kiszolgálókon.</p></td>
<td style="border:1px solid black;"><p>„A tanúsítási és a licencelési szolgáltatás beállítása az első kiszolgálón” témakör, <a href="http://go.microsoft.com/fwlink/?linkid=42494">RMS rendszer bevezetése</a> rész.</p>
<p>„A tanúsítást és a licencelést biztosító kiszolgálók hozzáadása” témakör, <a href="http://go.microsoft.com/fwlink/?linkid=42494">RMS rendszer bevezetése</a> rész.</p></td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><p>Telepítse és konfigurálja az RMS szolgáltatást a licencelési fürtbe tartozó kiszolgálókon.</p></td>
<td style="border:1px solid black;"><p>„A tanúsítási és a licencelési szolgáltatás beállítása az első kiszolgálón” témakör, <a href="http://go.microsoft.com/fwlink/?linkid=42494">RMS rendszer bevezetése</a> rész.</p>
<p>„A tanúsítást és a licencelést biztosító kiszolgálók hozzáadása” témakör, <a href="http://go.microsoft.com/fwlink/?linkid=42494">RMS rendszer bevezetése</a> rész.</p></td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><p>Állítsa be a terheléselosztást.</p></td>
<td style="border:1px solid black;"><p>„Az alapvető infrastruktúra kiterjesztése a fürtözés támogatására” témakör, <a href="http://go.microsoft.com/fwlink/?linkid=42494">RMS rendszer bevezetése</a> rész.</p></td>
</tr>  
<tr class="even">
<td style="border:1px solid black;"><p>Tesztelje a bevezetett rendszert.</p></td>
<td style="border:1px solid black;"><p>„Tesztkörnyezet kialakítása” témakör, <a href="http://go.microsoft.com/fwlink/?linkid=42494">RMS rendszer bevezetése</a> rész.</p></td>
</tr>  
<tr class="odd">
<td style="border:1px solid black;"><p>Helyezze üzembe az RMS szolgáltatást az éles környezetben.</p></td>
<td style="border:1px solid black;"><p>„Az RMS rendszer hatókörének meghatározása” témakör, <a href="http://go.microsoft.com/fwlink/?linkid=42494">RMS rendszer bevezetése</a> rész.</p></td>
</tr>  
</tbody>  
</table>
  
<span id="BKMK_13"></span>  
Az RMS bevezetése több erdőben  
------------------------------
  
Az RMS több erdőben való bevezetéséhez a következő feladatlista használható.
  
###  

<p> </p>
<table style="border:1px solid black;">  
<colgroup>  
<col width="50%" />  
<col width="50%" />  
</colgroup>  
<thead>  
<tr class="header">  
<th>Lépés</th>  
<th>Források</th>  
</tr>  
</thead>  
<tbody>  
<tr class="odd">
<td style="border:1px solid black;"><p>Ismerkedjen meg az alapfogalmakkal és a tervezéssel kapcsolatos tudnivalókkal.</p></td>
<td style="border:1px solid black;"><p>„Felkészülés az RMS bevezetésére” témakör, <a href="http://go.microsoft.com/fwlink/?linkid=42494">RMS rendszer bevezetése</a> rész.</p></td>
</tr>  
<tr class="even">
<td style="border:1px solid black;"><p>A bizalmi modell alapján állítsa be a szükséges engedélyeket.</p></td>
<td style="border:1px solid black;"><p>„Az RMS bevezetése több erdőben” témakör, <a href="http://go.microsoft.com/fwlink/?linkid=42494">RMS rendszer bevezetése</a> rész.</p></td>
</tr>  
<tr class="odd">
<td style="border:1px solid black;"><p>Állítsa be az erdők megfelelő Active Directory-attribútumait.</p></td>
<td style="border:1px solid black;"><p>„Az RMS bevezetése több erdőben” témakör, <a href="http://go.microsoft.com/fwlink/?linkid=42494">RMS rendszer bevezetése</a> rész.</p></td>
</tr>  
</tbody>  
</table>
  
<span id="BKMK_14"></span>  
Az RMS felügyeleti feladatlistái  
--------------------------------
  
Ez a szakasz a következő felügyeleti műveletekhez kínál feladatlistát:
  
-   [Jogmegadási sablon alkalmazása](#bkmk_15)  
-   [Új RMS ügyfél bevezetése](#bkmk_16)  
-   [Megbízható felhasználói tartomány felvétele](#bkmk_17)  
-   [Megbízható közzétételi tartomány felvétele](#bkmk_18)
  
Az RMS kezeléséről a további tudnivalókat lásd a dokumentumgyűjtemény [RMS kiszolgáló működtetése](http://go.microsoft.com/fwlink/?linkid=42495) című részében.
  
<span id="BKMK_15"></span>  
Jogmegadási sablon alkalmazása  
------------------------------
  
Jogmegadási sablon megvalósításához a következő feladatlista használható.
  
###  

<p> </p>
<table style="border:1px solid black;">  
<colgroup>  
<col width="50%" />  
<col width="50%" />  
</colgroup>  
<thead>  
<tr class="header">  
<th>Lépés</th>  
<th>Források</th>  
</tr>  
</thead>  
<tbody>  
<tr class="odd">
<td style="border:1px solid black;"><p>Ismerkedjen meg az idevágó fogalmakkal.</p></td>
<td style="border:1px solid black;"><p>„Jogmegadási sablonok” témakör, <a href="http://go.microsoft.com/fwlink/?linkid=42496">RMS műszaki források</a> rész.</p></td>
</tr>  
<tr class="even">
<td style="border:1px solid black;"><p>Adja meg a jogmegadási sablon helyét.</p></td>
<td style="border:1px solid black;"><p>„A jogmegadási sablonok helyének megadása” témakör, <a href="http://go.microsoft.com/fwlink/?linkid=42495">RMS kiszolgáló működtetése</a> rész.</p></td>
</tr>  
<tr class="odd">
<td style="border:1px solid black;"><p>Hozza létre a jogmegadási sablont.</p></td>
<td style="border:1px solid black;"><p>„A jogmegadási sablonok létrehozása és módosítása” témakör, <a href="http://go.microsoft.com/fwlink/?linkid=42495">RMS kiszolgáló működtetése</a> rész.</p>
<p>„Jogmegadási sablon hozzáadása” témakör, <a href="http://go.microsoft.com/fwlink/?linkid=42495">RMS kiszolgáló működtetése</a> rész.</p></td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><p>Juttassa el a felhasználókhoz a jogmegadási sablont.</p></td>
<td style="border:1px solid black;"><p>„Jogmegadási sablonok terjesztése” témakör, <a href="http://go.microsoft.com/fwlink/?linkid=42495">RMS kiszolgáló működtetése</a> rész.</p></td>
</tr>  
</tbody>  
</table>
  
<span id="BKMK_16"></span>  
Új RMS ügyfél bevezetése  
------------------------
  
Az RMS ügyfél új verziójának bevezetéséhez a következő feladatlista használható.
  
###  

<p> </p>
<table style="border:1px solid black;">  
<colgroup>  
<col width="50%" />  
<col width="50%" />  
</colgroup>  
<thead>  
<tr class="header">  
<th>Lépés</th>  
<th>Források</th>  
</tr>  
</thead>  
<tbody>  
<tr class="odd">
<td style="border:1px solid black;"><p>Ismerkedjen meg az idevágó fogalmakkal.</p></td>
<td style="border:1px solid black;"><p>„Az ügyfél terjesztésének megtervezése” témakör, <a href="http://go.microsoft.com/fwlink/?linkid=42494">RMS rendszer bevezetése</a> rész.</p>
<p>„Kulcstároló-verziók kizárása” témakör, <a href="http://go.microsoft.com/fwlink/?linkid=42495">RMS kiszolgáló működtetése</a> rész.</p></td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><p>A régi kulcstároló-verzió kizárásával tegye kötelezővé minden ügyfélnek, hogy a legújabb ügyfélverzióra frissítsen.</p></td>
<td style="border:1px solid black;"><p>„Kulcstároló-verziók kizárása” témakör, <a href="http://go.microsoft.com/fwlink/?linkid=42495">RMS kiszolgáló működtetése</a> rész.</p></td>
</tr>  
</tbody>  
</table>
  
<span id="BKMK_17"></span>  
Megbízható felhasználói tartomány felvétele  
-------------------------------------------
  
Megbízható felhasználói tartomány felvételéhez a következő feladatlista használható.
  
###  

<p> </p>
<table style="border:1px solid black;">  
<colgroup>  
<col width="50%" />  
<col width="50%" />  
</colgroup>  
<thead>  
<tr class="header">  
<th>Lépés</th>  
<th>Források</th>  
</tr>  
</thead>  
<tbody>  
<tr class="odd">
<td style="border:1px solid black;"><p>Ismerkedjen meg az idevágó fogalmakkal.</p></td>
<td style="border:1px solid black;"><p>„Megbízható felhasználói tartományok” témakör, <a href="http://go.microsoft.com/fwlink/?linkid=42496">RMS műszaki források</a> rész.</p>
<p>„Megbízható felhasználói tartományok hozzáadása és eltávolítása” témakör, <a href="http://go.microsoft.com/fwlink/?linkid=42495">RMS kiszolgáló működtetése</a> rész.</p></td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><p>Szerezze be a hozzáadni kívánt felhasználói tartomány kiszolgálói licencelői tanúsítványát. (A megbízhatónak minősítendő telepítés rendszergazdájától kérheti a fájlt.) Vegye fel a felhasználói tartományt a telepítésbe.</p></td>
<td style="border:1px solid black;"><p>„Megbízható felhasználói tartomány hozzáadása” témakör, <a href="http://go.microsoft.com/fwlink/?linkid=42495">RMS kiszolgáló működtetése</a> rész.</p></td>
</tr>  
</tbody>  
</table>
  
<span id="BKMK_18"></span>  
Megbízható közzétételi tartomány felvétele  
------------------------------------------
  
Megbízható közzétételi tartomány felvételéhez a következő feladatlista használható.
  
###  

<p> </p>
<table style="border:1px solid black;">  
<colgroup>  
<col width="50%" />  
<col width="50%" />  
</colgroup>  
<thead>  
<tr class="header">  
<th>Lépés</th>  
<th>Források</th>  
</tr>  
</thead>  
<tbody>  
<tr class="odd">
<td style="border:1px solid black;"><p>Ismerkedjen meg az idevágó fogalmakkal.</p></td>
<td style="border:1px solid black;"><p>„Megbízható közzétételi tartományok” témakör, <a href="http://go.microsoft.com/fwlink/?linkid=42496">RMS műszaki források</a> rész.</p>
<p>„Megbízható közzétételi tartományok hozzáadása és eltávolítása” témakör, <a href="http://go.microsoft.com/fwlink/?linkid=42495">RMS kiszolgáló működtetése</a> rész.</p></td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><p>Szerezze meg a hozzáadni kívánt közzétételi tartomány titkosított licencelői tanúsítványát és személyes kulcsát, majd vegye fel a telepítésbe a közzétételi tartományt.</p></td>
<td style="border:1px solid black;"><p>„Megbízható közzétételi tartomány hozzáadása” témakör, <a href="http://go.microsoft.com/fwlink/?linkid=42495">RMS kiszolgáló működtetése</a> rész.</p></td>
</tr>  
</tbody>  
</table>
