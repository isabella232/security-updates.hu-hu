---
TOCTitle: Szolgáltatás kapcsolódási pontjának regisztrálása
Title: Szolgáltatás kapcsolódási pontjának regisztrálása
ms:assetid: '630cc3c3-9ed9-4423-8874-cbaceb43b353'
ms:contentKeyID: 18122511
ms:mtpsurl: 'https://technet.microsoft.com/hu-hu/library/Cc720283(v=WS.10)'
---

Szolgáltatás kapcsolódási pontjának regisztrálása
=================================================

Szolgáltatás kapcsolódási pontjának regisztrálása
-------------------------------------------------

Ha altartománybeli RMS-kiszolgálóról regisztrál szolgáltatáskapcsolódási pontot, megjelenhet egy hibaüzenet, amely arról tájékoztatja, hogy sikertelen a szolgáltatáskapcsolódási pont (SCP) regisztrálása. A regisztrálás az esetek jó részében sikerült, ám a regisztráció előbb a legfelső szintű tartományban valósul meg, és időt vesz igénybe, amíg a rendszer átmásolja abba az altartományba, ahol az RMS-kiszolgáló az SCP-objektumot keresi. Mihelyt a kapcsolódási pont az erdő valamennyi globáliskatalógus-kiszolgálójára átmásolódott, az üzenet nem jelenik meg többé. Ha megjelenik ez az üzenet, ne indítsa el rögtön a hibaelhárítási műveletet, hanem egy ideig legyen türelemmel.

#### Szolgáltatás kapcsolódási pontjának regisztrálása

1.  Jelentkezzen be arra a kiszolgálóra, amelyen regisztrálni szeretné a szolgáltatás csatlakozási pontját. A bejelentkezéshez olyan tartományi fiókot használjon, amelynek engedélyei lehetővé teszik, hogy tároló objektumot hozzon létre az Active Directory-erdő Configuration tárolójában található Services tárolóban. A **Vállalati rendszergazdák** nevű előre megadott biztonsági csoport például olyan fiók, amely rendelkezik a szükséges jogosultságokkal.

2.  A **Globális felügyelet** weblapon kattintson **A webhelyen működő RMS felügyelete** hivatkozásra.

3.  A **Felügyeleti kezdőlapon** kattintson **Az RMS-szolgáltatás kapcsolódási pontja** hivatkozásra.

4.  Az **RMS-szolgáltatás kapcsolódási pontja** lapon kattintson az **URL-cím regisztrálása** gombra.
