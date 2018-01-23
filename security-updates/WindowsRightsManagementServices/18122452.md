---
TOCTitle: Az RMS biztonsági csoportjai
Title: Az RMS biztonsági csoportjai
ms:assetid: '25749a83-8c12-48ec-96ad-296d31fd55d4'
ms:contentKeyID: 18122452
ms:mtpsurl: 'https://technet.microsoft.com/hu-hu/library/Cc720215(v=WS.10)'
---

Az RMS biztonsági csoportjai
============================

Az RMS telepítője két csoportot hoz létre: az RMS szolgáltatás és a Felügyelők csoportot.

Az RMS szolgáltatás helyi biztonsági csoport, amely minden olyan engedélyt megkap, amellyel az RMS működéséhez szükséges összes erőforrást elérhet. A telepítés során a rendszergazda megadja azt a felhasználói fiókot, amelyet az RMS szolgáltatásfiókként használ. Ez a felhasználói fiók automatikusan tagjává válik az RMS szolgáltatás csoportnak, ezáltal hozzájut az annak megadott engedélyekhez. Az RMS normál működése java részében ezzel a felhasználói fiókkal fut.

Az RMS másik fontos csoportja a Felügyelők csoport. Ez a csoport teljes jogosultsággal rendelkezik minden tartalomhoz. Ez azt jelenti, hogy a csoport tagja minden RMS-védelemmel ellátott tartalomfájlt vissza tud fejteni, és el tudja róluk távolítani az RMS összes védelmi funkcióját. A Felügyelők csoportnak alapértelmezés szerint nincsenek tagjai, az RMS rendszergazdái sem kerülnek be automatikusan. A csoport tagságának kezelése létfontosságú az RMS-védelemmel ellátott tartalom biztonsága szempontjából. A további tudnivalókat lásd a dokumentumgyűjtemény „RMS kiszolgáló működtetése” részében „A Felügyelők csoport használata” témakörben.
