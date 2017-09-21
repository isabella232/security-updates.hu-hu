---
TOCTitle: A Globális felügyelet lap használata
Title: A Globális felügyelet lap használata
ms:assetid: '57bbf402-2351-4dee-823c-27f4dd32447c'
ms:contentKeyID: 18122584
ms:mtpsurl: 'https://technet.microsoft.com/hu-hu/library/Cc747575(v=WS.10)'
---

A Globális felügyelet lap használata
====================================

A felügyeleti webhely **Globális felügyelet** lapján hajthatja végre az RMS kiszolgálók létesítését és megszüntetését, és itt változtathatja meg az RMS szolgáltatásfiókját is.

A felügyelni kívánt kiszolgálóról a következő lépések végrehajtásával érheti el ezt a weblapot:

1.  Jelentkezzen be helyi rendszergazdaként.
2.  Válassza a **Start** menü **Minden program**, **Windows RMS**, majd **Windows RMS felügyeleti webhely** parancsát.

Távoli számítógépen található böngészőből nem érhető el a **Globális felügyelet** lap.

Ha még nem létesítette azt a kiszolgálót, amelyről a **Globális felügyelet** lapot el szeretné érni, a következő beállítások jelennek meg a kiszolgálón futó weblapokhoz:

-   **RMS létesítése a webhelyen**. Kattintson erre a hivatkozásra, ha ez az első kiszolgáló, amelyet az adott fürtben létesíteni kíván. Ezzel elindítja a létesítési műveletet, amely telepíti az RMS-erőforrásokat, például a virtuális könyvtárakat. A program ezenkívül az adatbázisokat is telepíti az adatbázis-kiszolgálóra. További tudnivalók: „[Az első legfelső szintű tanúsítási kiszolgáló létesítése](https://technet.microsoft.com/debc42f3-74ff-4c99-b7a4-4921fccdabc2)”.
-   **RMS hozzáadása egy fürthöz**. Kattintson erre a hivatkozásra, ha létesíteni szeretné a kiszolgálót, majd fel szeretné venni azt egy meglévő fürtbe. A kiszolgálókat felveheti a legfelső szintű tanúsítási fürtbe vagy egy licencelési fürtbe. A program telepíti az RMS-erőforrásokat, például a virtuális könyvtárakat. Az adatbázisok azonban nem jönnek létre, mivel ez a kiszolgáló a fürt adatbázisait fogja használni. További tudnivalók: „[Kiszolgáló felvétele fürtbe](https://technet.microsoft.com/db635238-5528-4bec-9cc6-8244e2b3d733)”.

Ha a **Globális felügyelet** lapot olyan kiszolgálóról éri el, amelynek létesítése már megtörtént, a következő beállítások jelennek meg:

-   **A webhelyen működő RMS felügyelete.** Erre a hivatkozásra kattintva jelenítheti meg a Fürtfelügyelet lapot. A további tudnivalókat lásd: „[A felügyeleti kezdőlap használata](https://technet.microsoft.com/6c155977-bd0e-47d6-ac65-1746cddb505e)”.
-   **Az RMS szolgáltatásfiókjának módosítása.** Erre a hivatkozásra kattintva adhat meg másik szolgáltatásfiókot az RMS futtatásához. A további tudnivalókat lásd: „[Az RMS szolgáltatásfiók megváltoztatása](https://technet.microsoft.com/f257d66d-b823-41e4-bcb7-7c90eb295238)”.
-   **A webhelyen működő RMS eltávolítása.** Erre a hivatkozásra kattintva szüntetheti meg az RMS-szolgáltatást. Az RMS megszüntetése csak az RMS virtuális könyvtárainak és alkalmazásainak eltávolítását jelenti a kiszolgálóról, az RMS eltávolítását nem. A további tudnivalókat lásd: „[Az RMS eltávolítása](https://technet.microsoft.com/885e3b4f-ea32-466f-9f7f-d8440b0f7c28)”.

| ![](images/Cc747575.note(WS.10).gif)Megjegyzés:                                                                                                                                                                                                     |
|----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| Az RMS felügyeleti webhelyén egyes szolgáltatások felbukkanó ablakokban konfigurálhatók. Ha a webböngészőben felbukkanó ablak blokkolót használ, úgy konfigurálja a böngésző beállításait, hogy az RMS felügyeleti webhelyén található felbukkanó ablakok engedélyezve legyenek. |
