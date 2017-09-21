---
TOCTitle: Az RMS belső és külső elérésével kapcsolatos kérdések
Title: Az RMS belső és külső elérésével kapcsolatos kérdések
ms:assetid: '59c2c51f-6c20-450c-a334-0e1486292074'
ms:contentKeyID: 18122587
ms:mtpsurl: 'https://technet.microsoft.com/hu-hu/library/Cc747577(v=WS.10)'
---

Az RMS belső és külső elérésével kapcsolatos kérdések
=====================================================

Az RMS belső és külső elérésével kapcsolatos kérdések
-----------------------------------------------------

-   [Milyen módosításokat kell végrehajtani a tűzfalon, hogy a külső ügyfelek elérhessék az RMS kiszolgálóit?](#bkmk_37)
-   [Hogyan működik az extranetes kialakítás?](#bkmk_38)
-   [Ha egy felhasználó a létrehozott, védelemmel ellátott tartalomhoz olyan valakinek ad jogot, aki nem fér hozzá az RMS telepítéséhez, használhatja-e a címzett a tartalmat?](#bkmk_39)
-   [Ha a védelemmel ellátott e-mail üzenetek elküldéséhez az Outlook 2003 vagy Outlook 2007 programot használom, mire van szükségük a címzetteknek, hogy elolvashassák azokat?](#bkmk_40)
-   [Ha a szervezetek saját RMS kiszolgálókkal rendelkeznek, hogyan cserélhetik ki a védelemmel ellátott tartalmat?](#bkmk_41)
-   [Ha az RMS-védelemmel ellátott e-mail üzenetet olyan külső szervezetnek küldik, amelyben nem használják az Outlook programot, válaszolhat-e a címzett az üzenetre, ha azt az Internet Explorer tartalomvédelmi bővítménye segítségével olvassa el?](#bkmk_42)

<span id="BKMK_37"></span>
#### Milyen módosításokat kell végrehajtani a tűzfalon, hogy a külső ügyfelek elérhessék az RMS kiszolgálóit?

A tűzfalnak engedélyeznie kell a külső számítógépek számára, hogy a SOAP (Simple Object Access Protocol) protokoll szerinti kérelmeket küldjenek az RMS kiszolgálójába a HTTP (80-as TCP port) vagy a HTTPS (443-as TCP port) protokollon keresztül.

<span id="BKMK_38"></span>
#### Hogyan működik az extranetes kialakítás?

A tartalomhoz kötött közzétételi licenc két URL-címet tartalmaz. Az egyik az intranetes URL-cím, amelynek beállítására az RMS fürtjének létesítéskor kerül sor. A másik egy extranetes URL-cím, amelyet az RMS rendszergazdája állíthat be. Ez az extranetes URL-cím a tűzfalon kívüli ügyfélnek is lehetővé teszi használati licencek beszerzését. Az extranetes URL-cím nem használható új, védelemmel ellátott tartalom létrehozásához. Ebben az esetben az RMS ügyfél rendszerleíró adatbázisának felülírására van szükség.

<span id="BKMK_39"></span>
#### Ha egy felhasználó a létrehozott, védelemmel ellátott tartalomhoz olyan valakinek ad jogot, aki nem fér hozzá az RMS telepítéséhez, használhatja-e a címzett a tartalmat?

Ha a felhasználó a védett tartalom első megnyitásakor nem tud kapcsolódni az RMS telepítéséhez, nem használhatja a tartalmat.

Az Office 2003 és újabb verziója viszont automatikusan beszerzi a használati licenceket a tartalomvédelemmel ellátott e-mail üzenetekhez a szinkronizáláskor, így azok hálózati kapcsolat nélkül is elolvashatók. Bár az Outlook 2003 és újabb verziója automatikusan megszerzi a használati licenceket az e-mail üzenetekhez, az üzenethez mellékelt Excel 2007, Excel 2003, Word 2007, Word 2003, PowerPoint 2007 és PowerPoint 2003 dokumentumokhoz a befogadó e-mail üzenettel megegyező jogok fognak tartozni. Ezek szinkronizálása nem történik meg automatikusan az e-mail üzenet letöltésekor, így ezeket használati licenc beszerzéséhez egyedileg kell megnyitni, amikor a számítógép kapcsolódik a hálózatra.

<span id="BKMK_40"></span>
#### Ha a védelemmel ellátott e-mail üzenetek elküldéséhez az Outlook 2003 vagy Outlook 2007 programot használom, mire van szükségük a címzetteknek, hogy elolvashassák azokat?

A címzetteknek ehhez az Outlook 2003 vagy Outlook 2007 programra, illetve az Internet Explorer tartalomvédelmi bővítményére van szükségük. Ha a címzett és a feladó szervezete bizalmi kapcsolatot létesített az RMS telepítései között, a címzett minden további nélkül elolvashatja az e-mail üzenetet. A bizalmi kapcsolat létesítése az RMS kiszolgálói licencelői tanúsítványok kicseréléséből áll, ezek tartalmazzák a megfelelő nyilvános kulcsokat.

Ha a címzett szervezete nem rendelkezik RMS infrastruktúrával, vagy nem létesítettek bizalmi kapcsolatot, megkérheti a felhasználót, hogy hozzon létre egy Windows Live ID azonosítót, és ennek a Windows Live ID hitelesítő adataihoz rendelt jogokkal küldje e-mail üzenetet a címzettnek. Ez a megoldás az interneten elérhető Microsoft IRM Service szolgáltatást alkalmazza használati licenc megszerzéséhez. Az IRM Service ingyenes a szolgáltatás kipróbálásához, és csak az RMS tesztelésére szolgál. Ha ezt a szolgáltatást választja a tartalom védelméhez, tisztában kell lennie azzal, hogy a szolgáltatás külön értesítés nélkül bármikor elérhetetlenné válhat.

<span id="BKMK_41"></span>
#### Ha a szervezetek saját RMS kiszolgálókkal rendelkeznek, hogyan cserélhetik ki a védelemmel ellátott tartalmat?

Az RMS megbízható felhasználói tartományokat használ, amelyeknél az egyik RMS rendszeren előállított felhasználói tanúsítványokat megbízhatónak fogadja el a másik.

<span id="BKMK_42"></span>
#### Ha az RMS-védelemmel ellátott e-mail üzenetet olyan külső szervezetnek küldik, amelyben nem használják az Outlook programot, válaszolhat-e a címzett az üzenetre, ha azt az Internet Explorer tartalomvédelmi bővítménye segítségével olvassa el?

Az e-mail címzettje a szokásos módon válaszolhat a tartalomvédelemmel ellátott üzenetre, de az eredeti üzenettörzs védett marad az eredeti címzettek számára. Az e-mail üzenetek csomagjának összeállítási módját az ügyfélalkalmazás határozza meg. Az eredeti e-mail üzenet szövege titkosított mellékletként szerepelhet a válaszban, vagy az véglegesen eltávolítható, ahogy ez például az Outlook 2003 vagy Outlook 2007 programnál történik.
