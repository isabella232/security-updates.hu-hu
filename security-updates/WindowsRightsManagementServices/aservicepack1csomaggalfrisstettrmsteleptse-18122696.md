---
TOCTitle: A Service Pack 1 csomaggal frissített RMS telepítése
Title: A Service Pack 1 csomaggal frissített RMS telepítése
ms:assetid: 'dab20175-a690-43f8-b943-768d289daa0d'
ms:contentKeyID: 18122696
ms:mtpsurl: 'https://technet.microsoft.com/hu-hu/library/Cc747689(v=WS.10)'
---

A Service Pack 1 csomaggal frissített RMS telepítése
====================================================

A művelet végrehajtásához helyben kell bejelentkeznie a felügyeleti webhelyre olyan tartományi felhasználói fiókkal, amely a Rendszergazdák csoport tagja az elérni kívánt számítógépen. A Tartománygazdák csoport tagjai is végrehajthatják ezt a műveletet. Biztonsági szempontból ajánlott a műveletet a **Futtatás másként** parancs segítségével végrehajtani.

Az RMS telepítéséhez választott kiszolgálónak egy tartomány tagkiszolgálójának vagy tartományvezérlőnek kell lennie. Az RMS nem vezethető be munkacsoportok különálló kiszolgálóin.

| ![](images/Cc747689.Important(WS.10).gif)Fontos:                                                                                                                                                                                                                                                                                                                                                                                                                                                                         |
|-------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| Az RMS-szolgáltatást csak akkor létesítse más kiszolgálón, ha már befejezte az első legfelső szintű tanúsítási kiszolgáló telepítését és létesítését. További tájékoztatás „[Az első legfelső szintű tanúsítási kiszolgáló létesítése](https://technet.microsoft.com/debc42f3-74ff-4c99-b7a4-4921fccdabc2)”, a „[Licenckiszolgáló létesítése](https://technet.microsoft.com/4d67b898-0ba9-4eef-ab7d-ee0ca55a688e)” és a „[Kiszolgáló felvétele fürtbe](https://technet.microsoft.com/db635238-5528-4bec-9cc6-8244e2b3d733)”című témakörben olvasható. |

| ![](images/Cc747689.Important(WS.10).gif)Fontos:                                                                                                                                                                                |
|--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| Az RMS SP1 olyan kiszolgálóra telepíthető, amelyen jelenleg az RMS korábbi verziója fut. Az RMS leszerelése után viszont az RMS SP1 csak akkor telepíthető, ha előbb a Programok telepítése és törlése segédprogrammal teljesen eltávolítja a szolgáltatást. |

A Service Pack 1 csomaggal frissített RMS telepítése
----------------------------------------------------

#### A Service Pack 1 csomaggal frissített RMS telepítése

1.  Jelentkezzen be az adott kiszolgáló helyi Rendszergazdák csoportjába tartozó tartományi fiókkal arra a kiszolgálóra, amelyre az RMS SP1 szolgáltatást telepíteni kívánja.

2.  A megjelenő **üdvözlő** párbeszédpanelen tekintse át a telepítendő szoftverek listáját, és kattintson a **Tovább** gombra.

3.  A **Licencszerződés** párbeszédpanelen olvassa el a szerződést, jelölje be az **Elfogadom** választógombot, és kattintson a **Tovább** gombra.

4.  Fogadja el a **Mappa** mezőben megjelenített alapértelmezés szerinti mappát, vagy adjon meg egy új mappát, és kattintson a **Tovább** gombra.

5.  A telepítés elkezdéséhez **A telepítés megerősítése** párbeszédpanelen kattintson a **Telepítés** gombra.

6.  Amikor megjelenik **A telepítés befejeződött** párbeszédpanel, kattintson a **Bezárás** gombra.

    | ![](images/Cc747689.note(WS.10).gif)Megjegyzés:                                                                              |
    |-----------------------------------------------------------------------------------------------------------------------------------------------------------|
    | Ha az alkalmazás újraindítására figyelmeztető hibaüzenet jelenik meg, a Microsoft Internet Explorer programban frissítse a **Globális felügyelet** lapot. |

Az RMS telepítése a parancssorból is végrehajtható. Ennek lépéseit „[Az RMS kiszolgálószoftver telepítése parancssorból](https://technet.microsoft.com/b55b1e2a-dd14-4168-a37f-9cdedbec660b)” pont ismerteti.
