---
TOCTitle: 'Az RMS-ügyfél bevezetése'
Title: 'Az RMS-ügyfél bevezetése'
ms:assetid: 'c84f1724-cf71-4385-9003-ff68bc23c927'
ms:contentKeyID: 18122749
ms:mtpsurl: 'https://technet.microsoft.com/hu-hu/library/Cc747749(v=WS.10)'
---

Az RMS-ügyfél bevezetése
========================

A Microsoft Windows XP vagy a Microsoft Windows 2000 használata esetén telepíteni kell a tartalomvédelmi szolgáltatások (RMS) ügyfélszoftverét, mielőtt bármilyen RMS szolgáltatást használhatna, így például a Microsoft® Office 2003 Tartalomvédelmi szolgáltatását vagy az Internet Explorer Tartalomvédelmi bővítményét. Az RMS ügyfélszoftver a Windows Vista® operációs rendszerbe be lett építve.

Számos szervezet szabályozott körülmények között hajtja végre az ügyfélszoftver bevezetését. A 2. szervizcsomaggal bővített tartalomvédelmi szolgáltatás (RMS SP2) ügyfélszoftvere rendszerbe állítható akár a Systems Management Server (SMS), akár a Csoportházirend használatával.

Az RMS ügyfélszoftver rendszerbe állítása előtt letölthető innen: [http://go.microsoft.com](http://go.microsoft.com/fwlink/?linkid=67736).(http://go.microsoft.com/fwlink/?linkid=67736).

> [!IMPORTANT]  
> Az RMS ügyfélszoftver a Windows Vista operációs rendszerbe be lett építve. Ezért nincs szükség külön telepítésre. 

A telepítési fájlok kibontása
-----------------------------

A WindowsRightsManagementServicesSP2-KB917275-Client-ENU.exe fájl letöltése után a végrehajtható csomagból ki kell bontani a Microsoft® Windows® Installer működéséhez szükséges fájlokat.

Ez a parancssorba beírt következő paranccsal történhet:

`WindowsRightsManagementServicesSP2-KB917275-Client-ENU.exe /x <path>`

ahol az „&lt;útvonal&gt;” az a hely ahova a fájlokat kibontani kívánja.

A parancs végrehajtása után a következő fájlok kerülnek a megadott könyvtárba:

-   Bootstrap.exe
    A végrehajtható fájl ezt a fájlt használja a többi fájl telepítéséhez. A fájlra nincs szükség, ha az RMS SP2 ügyfélszoftver telepítése az SMS vagy a Csoportházirend segítségével történik.
-   MSDrmClient.msi
    Ez az RMS SP2 ügyfélszoftverhez tartozó telepítési fájl. Ez a telepítés törölni fogja a számítógépről az RMS-ügyfélszoftver bármely korábbi verzióját. A program először az ügyfélszámítógépekre kell telepíteni.
-   RMClientBackCompat.msi
    Ez a telepítési fájl azonosítja az új RMS SP2 ügyfélszoftvert az RMS-ügyfélszoftver előző verziójától függő RMS-kompatibilis alkalmazások számára (ilyen például a Microsoft Office Professional 2003 vagy a Microsoft Office System 2007), így a korábbi helyett az RMS SP2 ügyfél használható. Ezt a programot az MSDrmClient.msi sikeres telepítése után kell telepíteni az ügyfélszámítógépekre.

> [!NOTE]  
> Bármelyik telepítési módszer választásakor biztosítani kell a Windows Installer mindkét telepítési fájljának sikeres telepítését. Ha olyan hiba fordul elő, amely megakadályozza az MSDrmClient.msi telepítését, az RMClientBackCompat.msi fájlt nem szabad telepíteni. 

Az RMS ügyfélszoftvert rendszerbe állítása felügyelet nélküli telepítéssel
--------------------------------------------------------------------------

A Windows Installer használatával működő fájlok kicsomagolása nem kötelező. Az RMS ügyfélszoftver rendszerbe állítása felügyelet nélküli telepítéssel is elvégezhető. Ez a parancssorba beírt következő paranccsal történhet:

`WindowsRightsManagementServicesSP2-KB917275-Client-ENU.exe -override 1 /I MsDrmClient.msi REBOOT=ReallySuppress /q -override 2 /I RmClientBackCompat.msi REBOOT=ReallySuppress /q`

Ez a parancs elindítja az RMS ügyfélszoftver felügyelet nélküli telepítését.

> [!NOTE]  
> Mivel ez felügyelet nélküli telepítés, a telepítő nem ad tájékoztatást a telepítés befejezéséről. A felügyelet nélküli telepítést általában parancsfájl (kötegelt vagy szkript) végzi. 

Az RMS-ügyfél bevezetése az SMS használatával
---------------------------------------------

**Az RMS-ügyfél bevezetésének lépései az SMS segítségével**
1.  Nyissa meg az SMS felügyeleti konzolját.

2.  Bontsa ki a használni kívánt hely adatbázisát.

3.  A bal oldali ablaktáblán kattintson a jobb oldali egérgombbal a **Packages** elemre, és válassza a **New**, majd a **Package From Definition** parancsot.

4.  Hozzon létre csomagokat az MSDRMClient.msi és az RMClientBackCompat.msi fájlból. A csomagoknak a következő tulajdonságokkal kell rendelkezniük:

    **General**:

    -   A **Command line** elemnél írja a következőt:
        `msiexec.exe /q ALLUSERS=2 /m MSIDGHOG /i "<file_name>.msi"`
        | ![](images/Cc747749.note(WS.10).gif)Megjegyzés:                                                              |
        |-------------------------------------------------------------------------------------------------------------------------------------------|
        | Az MSIDGHOG véletlen érték. A &lt;fájlnév&gt; helyére írja annak a Windows Installer fájlnak a nevét, amelyet ez a csomag telepíteni fog. |

    -   A **Run** tulajdonságnál válassza a **Hidden** beállítást.
    -   Az **After running** beállítása legyen **No action required**.
    -   A **Category** tulajdonságnál válassza az **Administrative Software** beállítást.

    **Requirements:**

    -   Az **Estimated disk space** mezőbe írja a **445 KB** értéket.
    -   A **Maximum allowed run time** tulajdonságnál válassza az **Unknown** beállítást.
    -   Jelölje be a **This program can run on any platform** négyzetet.

    **Environment:**

    -   A **Program can run** tulajdonságnál válassza a **Whether or not a user is logged on** beállítást.
    -   A **Run mode** beállítása legyen **Run with administrative rights**.
    -   A **Drive mode** tulajdonságnál válassza a **Runs with UNC name** beállítást.

    **Advanced:**

    -   Törölje a **Run another program first** négyzet jelölését.
    -   Törölje a **Suppress program notification** négyzet jelölését a **When the program is assigned to a computer** csoportban.
    -   Törölje a **Disable this program on computers where it is advertised** négyzet jelölését.

5.  Az **Access Accounts and Distribution Points** tulajdonságnál válassza a szervezetnek megfelelő beállítást.

6.  Hozzon létre hirdetést a megfelelő gyűjteményhez. Javasolt, hogy az SMS segítségével végrehajtott bevezetésnél a **Per-system unattended** beállítást használja.

7.  Ütemezze a hirdetést a szervezet igényeinek megfelelően.

Az RMS-ügyfél bevezetése a Csoportházirend használatával
--------------------------------------------------------

A Csoportházirend szoftvertelepítés és -karbantartás szolgáltatásával rendszerbe állíthatja az RMS ügyfelet a kívánt számítógépeken.

A Csoportházirend használata a javasolt módszer az RMS ügyfelek rendszerbe állításához az olyan kis- és középméretű szervezeteknél, amelyek még nem használnak vállalati frissítéskezelő megoldást, ilyen például a Systems Management Server (SMS) 2003 vagy a Windows Update Services (SUS).

Amikor csoportházirendet használ programok terjesztéséhez, a programot számítógépekhez rendelheti. A program telepítésére a számítógép elindításakor kerül sor, és az elérhető lesz minden felhasználó számára, aki bejelentkezik a számítógépen. A további tudnivalókat lásd: Group Policy Infrastructure (A Csoportházirend infrastruktúrája) (<http://go.microsoft.com/fwlink/?linkid=24328>). Ez az eljárás a Group Policy Management Console (GPMC) használatát feltételezi. A GPMC letöltéséről lásd: Group Policy Management Console with Service Pack 1 (<http://go.microsoft.com/fwlink/?linkid=21813>).

Az itt következő eljárás gyors útmutató azoknak a rendszergazdáknak, akik nem ismerik a csoportházirenden alapuló szoftverterjesztést. Ezek a lépések a szervezet igényeinek megfelelően megváltoztathatók.

**Az RMS-ügyfél bevezetésének lépései a Csoportházirend segítségével**
1.  A tartományvezérlőn nyissa meg a Microsoft kezelőkonzol (MMC) **Active Directory – felhasználók és számítógépek** beépülő modulját.

2.  Hozzon létre egy új szervezeti egységet, vagy jelöljön ki egy meglévőt.

    Ha új szervezeti egységet hozott létre, vegye fel azokat a számítógépeket, amelyen telepíteni kívánja az RMS-ügyfelet.

3.  Kattintson a jobb oldali egérgombbal a szervezeti egységre, és a válassza a **Tulajdonságok** parancsot.

4.  Jelenítse meg a **Csoportházirend** panellapot.

5.  Új csoportházirend-objektum létrehozásához kattintson az **Új** gombra.

6.  Az új objektum szerkesztéséhez kattintson a **Szerkesztés** gombra.

7.  A konzolfán bontsa ki a **Számítógép konfigurációja,Szoftverbeállítások** csomópontot, és jelölje ki a Szoftvertelepítés elemet.

8.  A jobb oldali ablaktáblán kattintson jobb gombbal a **New** elemre, majd kattintson a **Package** parancsra.

9.  Adja meg az MSDRMclient.msi fájl hálózati megosztott mappáját, amelyet az ügyfélszámítógépek elérhetnek.

10. A csomag hozzárendeléséhez kattintson az **OK** gombra.

11. Ismételje meg az 5–10. lépéseket, és hozza létre az RMClientBackCompat.msi fájlt telepítő csoportházirend-objektumot.

> [!NOTE]  
> Ezek a lépések csak útmutatásul szolgálnak azoknak a rendszergazdáknak, akik nem használták még a csoportházirendet. A témában jártas rendszergazdák saját eljárásaikat alkalmazhatják az MSDrmClient.msi csomag terjesztésénél. Emellett ezek a lépések a Windows Server 2003 rendszerrel működő tartományvezérlőre vonatkoznak, a Windows 2000 rendszerű tartományon az eljárás és a fogalmak némileg eltérőek lehetnek. 

Frissítés előző verzióról
-------------------------

        ```
> [!NOTE]  
> Ez a parancsfájl nem működik a Windows Vista esetén, mert az RMS ügyfélszoftver már be van építve az operációs rendszerbe. 
