---
TOCTitle: Az első legfelső szintű tanúsítási kiszolgáló létesítése
Title: Az első legfelső szintű tanúsítási kiszolgáló létesítése
ms:assetid: 'debc42f3-74ff-4c99-b7a4-4921fccdabc2'
ms:contentKeyID: 18122764
ms:mtpsurl: 'https://technet.microsoft.com/hu-hu/library/Cc747768(v=WS.10)'
---

Az első legfelső szintű tanúsítási kiszolgáló létesítése
========================================================

A művelet végrehajtásához helyben kell bejelentkeznie a felügyeleti webhelyre olyan tartományi felhasználói fiókkal, amely a Rendszergazdák csoport tagja az elérni kívánt számítógépen. A Tartománygazdák csoport tagjai is végrehajthatják ezt a műveletet. Ha távoli SQL Server adatbázist használ, a fióknak adatbázis-létrehozói szereppel is rendelkeznie kell az SQL Server kiszolgálón. Biztonsági szempontból ajánlott a műveletet a **Futtatás másként** parancs segítségével végrehajtani.

A **Globális felügyelet** lap megnyitásához kattintson a **Start** gombra, és válassza a **Minden program**, a **Windows RMS**, majd a **Windows RMS felügyeleti webhely** parancsot.

Kiszolgálónként csak egy webhelyen létesíthető az RMS-szolgáltatás. Ha az RMS-szolgáltatást nem az alapértelmezés szerinti webhelyen szeretné létesíteni, a létesítési művelet elkezdése előtt az Internet Information Services kezelője segítségével hozza létre a webhelyet. Ha a létesíteni kívánt webhely nem szerepel a webhelyek listájában, zárja be a **Globális felügyelet** lapot, hozza létre a webhelyet, majd kezdje el újból a létesítési műveletet.

Ha olyan környezetben vezeti be az RMS-szolgáltatást, amelyben az Active Directory tartomány működési szintje natív Windows 2000 működési szinten áll, előfordulhat, hogy az RMS nem tudja beolvasni az Active Directory-objektumok **memberOf** attribútumának értékét, amikor megpróbálja behelyettesíteni a csoportok tagságát. Az RMS akkor tudja beolvasni a **memberOf** attribútumot, ha az RMS szolgáltatásfiókja olyan tartományi fiókot használ, amely tagja az adott erdőben működő, a Windows 2000 előtti rendszerekkel kompatibilis beépített hozzáférési csoportnak.

Ha egyéni URL-címet ad a fürtnek, ne felejtse el bejegyezni azt a tartománynévrendszerbe (DNS), és ellenőrizni a működését. Ha internetes bevezetésről van szó, ellenőrizze, hogy az URL-cím elérhető-e az internetről és a szervezeten belülről is. Ha engedélyezte az SSL-titkosítást a webszolgáltatások fájljaira vonatkozóan, a HTTPS protokollt kell megadnia a fürt URL-címében.

Az első legfelső szintű tanúsítási kiszolgáló létesítése
--------------------------------------------------------

#### Az első legfelső szintű tanúsítási kiszolgáló létesítése

1.  Miután telepítette az RMS-szolgáltatást arra a kiszolgálóra, amely az első legfelső szintű tanúsítási kiszolgáló lesz az Active Directory-erdőben, nyissa meg a **Globális felügyelet** lapot.

2.  Keresse meg azt a webhelyet, amelyen létesíteni szeretné az RMS-szolgáltatást, majd kattintson a mellette látható **RMS létesítése a webhelyen** hivatkozásra. Megadhatja az alapértelmezés szerinti webhelyet, vagy választhatja az Internet Information Services (IIS) szolgáltatásban erre a célra létrehozott webhelyet is.

    | ![](images/Cc747768.Warning(WS.10).gif)Figyelmeztetés:                                                                                                                                                                                                                                                                       |
    |-----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
    | Nem támogatott megoldás, ha az RMS-szolgáltatást futtató kiszolgálón más webhelyek vagy szolgáltatások is futnak. Ez esetben ugyanis több alkalmazás és szolgáltatás futhat az RMS-szolgáltatással azonos fiókkal (különösképpen a Helyi rendszerfiókkal), ami azt a veszélyt rejti, hogy jogosulatlan műveleteket hajtanak végre a személyes kulcsokkal. |

3.  A **Konfigurációs adatbázis** csoportban az alapértelmezés szerinti beállítás a konfigurációs adatbázis létrehozása a helyi kiszolgálón. A helyi adatbázisokhoz például az SQL Server™ 2000 SP3 csomaggal frissített verzióját vagy a Microsoft SQL Server 2000 Desktop Engine (MSDE) adatbázis-kezelőt veheti igénybe. Ha távoli adatbázist használ, illetve ha az adatbázis-kiszolgálót ugyan a helyi kiszolgálón futtatja, de az adatbázis-kiszolgáló példány neve különbözik az adott kiszolgáló nevétől, válassza a **Távoli adatbázis** beállítást, és írja be az adatbázis-kiszolgáló nevét.

    | ![](images/Cc747768.Important(WS.10).gif)Fontos:                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                       |
    |-------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
    | Azt ajánljuk, hogy csak tesztkörnyezetben használja a Microsoft SQL Server Desktop Engine adatbázis-kezelőt az RMS adatbázisaihoz, mert a Microsoft SQL Server Desktop Engine semmilyen hálózati csatlakozófelületet sem támogat. A Microsoft SQL Server Desktop Engine használati feltételei továbbá megtiltják az SQL Server ügyféleszközeinek használatát a Microsoft SQL Server Desktop Engine adatbázisok kezelésére. Ezt a korlátozást figyelembe véve nem áll majd módjában megtekinteni a naplózott adatokat, sem módosítani a konfigurációs adatbázisban tárolt adatokat.  |

4.  Az **RMS szolgáltatásfiókja** csoportban adja meg azt az RMS-szolgáltatásfiókot, amellyel az RMS futni fog a szokásos műveletek többségénél. Egykiszolgálós telepítésnél megadhatja a helyi rendszerfiókot, vagy tartományi fiókot is választhat. Minden más telepítés esetén tartományi fiókot kell megadni. Tartományi fióknál adja meg a *tartománynév*\\*felhasználónév* formátumú fióknevet és a jelszót.

    | ![](images/Cc747768.Warning(WS.10).gif)Figyelmeztetés:                                                                                                                                                                                                                                                                                                                                                                                          |
    |------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
    | A Helyi rendszerfiók szinte az operációs rendszer minden erőforrásához hozzáfér, használata tehát komoly biztonsági következményeket von maga után. Lehetőség szerint ne használja a helyi rendszerfiókot az RMS szolgáltatásfiókjaként. Célszerű különleges engedélyekkel nem rendelkező, külön felhasználói fiókot létrehozni az RMS szolgáltatásfiókjaként való használatra. Az RMS szolgáltatásfiókja nem egyezhet meg az RMS telepítéséhez használt tartományi fiókkal. |

    | ![](images/Cc747768.Important(WS.10).gif)Fontos:                                                                                                                                                                                                                               |
    |-------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
    | Biztonsági megfontolásokból célszerű különleges engedélyekkel nem rendelkező, külön felhasználói fiókot létrehozni a Windows RMS szolgáltatásfiókjaként való használatra. Az RMS-szolgáltatásfiók nem egyezhet meg a Windows RMS Service Pack 1 szervizcsomaggal telepítéséhez használt tartományi fiókkal. |

5.  A **Fürt URL-címe** területre írja be a kiszolgálónak vagy a fürtnek azt az URL-címét, amelyet a belső hálózaton lévő ügyfelek fognak használni. Az itt található alapértelmezés szerinti értékben a kiszolgáló neve szerepel, például Kiszolg1. Ezt az értéket igény szerint módosíthatja, például megadhatja a fürt vagy a fürtöt kiszolgáló terheléselosztó URL-címét. A HTTP és a HTTPS protokoll közül választhat. A fürt URL-címének megadásáról a művelet ismertetését követő **Megjegyzések** című részben talál további részleteket. A létesítést követően a felügyeleti weblapokon beállíthatja a fürt külső URL-címét is, amelyet a belső hálózaton kívül eső ügyfelek fognak használni.

6.  A **Személyeskulcs-védelem és igénylés** csoportban adja meg a kiszolgáló személyes kulcsának védelmére használandó eljárást:

    -   **Az alapértelmezés szerinti szoftveres személyeskulcs-védelem használata**. Ha ezt a beállítást választja, a személyes kulcs tárolása az RMS konfigurációs adatbázisában történik. A kulcs titkosításához erős jelszót kell megadnia.

    | ![](images/Cc747768.Important(WS.10).gif)Fontos:                                                                                                                                                                                                                                                                                                                                                       |
    |-------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
    | A választott jelszót tárolja biztonságos helyen. Készítsen másolatot a konfigurációs adatbázisról (amelyhez az adott jelszót használja), és azt is helyezze biztonságba. Ezzel az óvintézkedéssel visszaállíthatja az RMS-szolgáltatást, ha megsérül az SQL Server adatbázis. Ha bármilyen okból megváltoztatja a jelszót, készítsen új másolatot a konfigurációs adatbázisról és a jelszóval együtt archiválja biztonságos helyen. |

    -   **Kriptográfiai szolgáltató (CSP) használata**. Ha kriptográfiai szolgáltatót (CSP) vagy hardveres biztonsági modult szeretne használni, törölje a jelet **Az alapértelmezés szerinti szoftveres személyeskulcs-védelem használata** jelölőnégyzetből. A **Kriptográfiai szolgáltató kiválasztása** listában jelölje ki a telepített kriptográfiai szolgáltatót vagy hardveres biztonsági modult.

    | ![](images/Cc747768.note(WS.10).gif)Megjegyzés:                                                                          |
    |-------------------------------------------------------------------------------------------------------------------------------------------------------|
    | Az RMS teljes RSA (Rivest-Shamir-Adleman) szolgáltatót igényel, ezért csak az ilyen szolgáltatók szerepelnek a kriptográfiai szolgáltatók listájában. |

    | ![](images/Cc747768.note(WS.10).gif)Megjegyzés:                                                                                                                                                                                                                                                                                                                                                                          |
    |-------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
    | Célszerű az alapértelmezés szerinti szoftveres személyeskulcs-védelmet használni, vagy valamilyen hardveres biztonsági modult. Ha más szoftveres kriptográfiai szolgáltatót választ, ellenőrizze, hogy rendelkezik-e a megfelelő szervezeti kulcskezelési eljárásokkal (ilyen például a biztonsági mentés és a visszaállítás) az adott szolgáltatóhoz, és csak akkor vegye igénybe azt az RMS-szolgáltatáshoz, ha adva vannak az említett feltételek. |

7.  Ez a lépés csak akkor hajtandó végre, ha kriptográfiai szolgáltatót választott. Az alkalmazandó kiszolgálói kulcspár megadásához hajtsa végre a megfelelő műveletet:

    -   Új telepítés esetében válassza az **Új nyilvános/személyeskulcspár létrehozása** beállítást.
    -   Meglévő RMS-kiszolgáló visszaállításakor vagy frissítésekor válassza a **Meglévő nyilvános/személyeskulcspár használata** beállítást. A **Létező kulcstároló** csoportban kattintson a **Tallózás** gombra, és válassza ki a kiszolgálói kulcspár kulcstárolóját.

    | ![](images/Cc747768.note(WS.10).gif)Megjegyzés:                                                           |
    |----------------------------------------------------------------------------------------------------------------------------------------|
    | A Microsoft Base (alap), Enhanced (fokozott) és Strong (erős) kriptográfiai szolgáltatók (CSP-k) ugyanazt a kulcstárhelyet használják. |

    | ![](images/Cc747768.note(WS.10).gif)Megjegyzés:                                                                                                                                                                                                                                       |
    |--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
    | Ha meglévő RMS-kiszolgáló visszaállításakor vagy frissítésekor még nem létező kulcspárt használ, a tartalom használatához valamennyi RMS-ügyfél licenctárát üríteni kell (törölni kell a használati licenceket és a tartalomvédelmi fióktanúsítványokat), és számukra a kiszolgálótól új licencet kell beszerezni. |

8.  A **Kiszolgáló internetes csatlakoztathatósága** mezőben adja meg, hogy a kiszolgáló kiszolgálói licencelői tanúsítvány beszerzéséhez csatlakozzon-e az internethez.

    -   Ha az **On-line** beállítást választja, a kiszolgáló a létesítési folyamat közben kiszolgálói licencelői tanúsítvány igényléséhez automatikusan kapcsolódik a Microsoft igénylési szolgáltatásához.
    -   Ha az RMS-kiszolgáló nem rendelkezik internetkapcsolattal, illetve ha a kiszolgálói licencelői tanúsítványt a létesítési folyamatot követően kézzel kívánja beszerezni és az RMS-kiszolgálóra importálni, válassza a **Kapcsolat nélkül** beállítást.

9.  **A kiszolgáló licencelői tanúsítványának neve** mezőben adja meg a kiszolgáló licencelői tanúsítványában használandó nevet. Ez alapértelmezés szerint a kiszolgáló neve.

10. Ha a szervezet proxykiszolgálóval csatlakozik az internethez, jelölje be az **Ez a számítógép proxykiszolgálón keresztül kapcsolódik az internethez** négyzetet, majd írja be a proxykiszolgáló címét és portját.

    Ha a proxykiszolgáló megköveteli a hitelesítést, válassza ki a hitelesítés típusát, majd adjon meg egy felhasználónevet és egy jelszót, amelyet a proxykiszolgáló hitelesíteni tud. Ha a beépített Windows-hitelesítést használja, tartománynevet is meg kell adnia.

    | ![](images/Cc747768.note(WS.10).gif)Megjegyzés:                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                            |
    |-------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
    | Ez a beállítás létesítés után a felügyeleti webhely **Biztonsági beállítások** lapján módosítható. Ez a lap azonban csak akkor válik elérhetővé, ha a kiszolgálót a Microsoft igénylési szolgáltatással már igényelte. Ha a szervezetnél proxykiszolgálón keresztül kell kapcsolódni az internethez, és nem konfigurál proxykiszolgálót, mert a **Kiszolgáló internetes csatlakoztathatósága** beállításnál a **Kapcsolat nélkül** beállítást választotta, akkor az igénylési eljárás és a proxykiszolgáló beállításait csak a kézi igénylési folyamat befejezése, illetve az RMS újralétesítése után tudja módosítani. |

11. A **Kapcsolatfelvétel a rendszergazdával** mezőbe írja be a rendszergazda e-mail címét, akihez a többi kiszolgáló létesítése során felmerülő problémák esetén lehet fordulni. A létesítés befejezése után ez az e-mail cím módosítható.

12. A **Visszavonás** csoportban adja meg, hogy engedélyezi-e a külső entitások számára a kiszolgáló licencelői tanúsítványának visszavonását. Ha megadja ezt a beállítást, írja be a külső fél nyilvános kulcsát tartalmazó fájl elérési útvonalát és nevét.

13. Kattintson a **Küldés** gombra.

    A szolgáltatás létesítése akkor történik, amikor rákattint a **Küldés** gombra. Ha az on-line igénylést választotta, akkor a legfelső szintű tanúsítási kiszolgáló igénylési folyamatára is sor kerül. A folyamat során az RMS előállít egy nyilvános/személyes kulcspárt, és elküldi a nyilvános kulcsot a Microsoft igénylési szolgáltatásának. A Microsoft igénylési szolgáltatása létrehoz egy kiszolgálói licencelői tanúsítványt, és néhány percen belül visszaküldi azt a konfigurációs adatbázisba. Ha az igénylést kapcsolat nélküli hajtja végre, akkor az RMS kiszolgáló konfigurálása előtt végre kell hajtania a „[Legfelső szintű tanúsítási kiszolgáló kézi igénylése](https://technet.microsoft.com/aecdebb5-b28b-4b58-937a-392bb6ce9643)” pontban ismertetett feladatot.

    | ![](images/Cc747768.note(WS.10).gif)Megjegyzés:                                                                                                                                                                                                                                    |
    |-----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
    | Ez a kiszolgáló mindaddig nem használható, amíg nem regisztrálták a szolgáltatás kapcsolódási pontját (SCP) az Active Directoryban. Ezt a „[Szolgáltatás kapcsolódási pontjának regisztrálása](https://technet.microsoft.com/630cc3c3-9ed9-4423-8874-cbaceb43b353)” című témakör lépéseivel lehet végrehajtani. |

A további legfelső szintű tanúsítási kiszolgálók létesítéséről és fürtbe való felvételéről a „[Kiszolgáló felvétele fürtbe](https://technet.microsoft.com/db635238-5528-4bec-9cc6-8244e2b3d733)” című témakör nyújt tájékoztatást.
