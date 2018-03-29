---
TOCTitle: 'Fürt extranetes URL-címének felvétele'
Title: 'Fürt extranetes URL-címének felvétele'
ms:assetid: '12c83186-ce9e-4100-bbd1-d87a885331c7'
ms:contentKeyID: 18122442
ms:mtpsurl: 'https://technet.microsoft.com/hu-hu/library/Cc720193(v=WS.10)'
---

Fürt extranetes URL-címének felvétele
=====================================

A művelet végrehajtásához helyben kell bejelentkeznie a felügyeleti webhelyre olyan tartományi felhasználói fiókkal, amely a Rendszergazdák csoport tagja az elérni kívánt számítógépen. A Tartománygazdák csoport tagjai is végrehajthatják ezt a műveletet. Biztonsági szempontból ajánlott a műveletet a **Futtatás másként** parancs segítségével végrehajtani.

A **Globális felügyelet** lap megnyitásához kattintson a **Start** gombra, és válassza a **Minden program**, a **Windows RMS**, majd a **Windows RMS felügyeleti webhely** parancsot.

Ne felejtse el bejegyezni az URL-címet a tartománynévrendszerbe (DNS), majd ellenőrizni a működését és elérhetőségét az internetről. Ha engedélyezte az SSL-titkosítást a webszolgáltatások fájljaira vonatkozóan, a HTTPS protokollt kell megadnia a fürt URL-címében.

Ha már működő RMS-kiszolgálóhoz ad fürt extranetes URL-címet, a jelenlegi RMS-ügyfelek részére az extranetes fürthöz licencelési célból hozzáféréshez új ügyfél licencelői tanúsítványokat kell beszerezni.

Fürt extranetes URL-címének felvétele
-------------------------------------

#### Fürt extranetes URL-címének felvétele

1.  Nyissa meg a **Globális felügyelet** lapot, majd keresse meg azt a webhelyet, amelyen meg szeretné adni a fürt extranetes URL-címét, és kattintson a mellette látható **A webhelyen működő RMS felügyelete** hivatkozásra.

2.  A **Felügyeleti hivatkozások** csoportban kattintson **A fürt extranetes URL-címének beállítása** hivatkozásra.

3.  A **Fürt extranetes URL-címe** csoportban adja meg azt az URL-címet, amelyről a külső felhasználók licenceket kérhetnek. A HTTP és a HTTPS protokoll közül választhat.

4.  Kattintson a **Küldés** gombra.
