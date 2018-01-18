---
TOCTitle: '2. lépés: A Windows Server Update Services (WSUS) szolgáltatás telepítése a kiszolgálóra'
Title: '2. lépés: A Windows Server Update Services (WSUS) szolgáltatás telepítése a kiszolgálóra'
ms:assetid: 'f593532c-e92e-47f3-914a-38a6c2519e94'
ms:contentKeyID: 18129940
ms:mtpsurl: 'https://technet.microsoft.com/hu-hu/library/Cc708622(v=WS.10)'
---

2. lépés: A Windows Server Update Services (WSUS) szolgáltatás telepítése a kiszolgálóra
========================================================================================

A telepítési követelmények áttekintése után megkezdheti a WSUS szolgáltatás telepítését: ehhez a helyi Rendszergazdák csoportba tartozó felhasználói fiókkal kell bejelentkeznie arra a kiszolgálóra, amelyre telepíteni szeretné a szolgáltatást, ugyanis annak telepítésére kizárólag a helyi Rendszergazdák csoport tagjai jogosultak.

A következőkben ismertetett telepítési eljárás a Windows Server 2003 rendszeren alkalmazni kívánt WSUS szolgáltatás telepítésének alapértelmezett beállításai szerint történik, így magában foglalja a WSUS adatbázisszoftverhez használandó Windows SQL Server 2000 Desktop Engine (WMSDE) összetevő telepítését, a frissítések helyi számítógépre mentését, valamint az IIS szolgáltatás alapértelmezett webhelyének 80-as portra történő telepítését. Az egyéni telepítési beállításokra (például más operációs rendszer használatára, eltérő adatbázisszoftverre vagy egyéni portszámot használó webhelyre) vonatkozó tudnivalókat a „Deploying Microsoft Windows Server Update Services” (A Microsoft Windows Server Update Services szolgáltatás központi telepítése) című (angol nyelvű) szakmai dokumentációban találja meg.

**A WSUS szolgáltatás telepítése Windows Server 2003 operációs rendszerre**
1.  Kattintson duplán a **WSUSSetup.exe** nevű telepítőfájlra.

    > [!NOTE]  
    > A WSUSSetup.exe fájl legújabb verzióját a [Microsoft Windows Update Services](http://go.microsoft.com/fwlink/?linkid=47374) angol nyelvű webhelyéről (http://go.microsoft.com/fwlink/?LinkId=47374) töltheti le. 

2.  A varázsló **üdvözlőlapján** kattintson a **Tovább** gombra.

3.  Olvassa el figyelmesen a licencszerződést, jelölje be az **Elfogadom a licencszerződés feltételeit** választógombot, majd kattintson a **Tovább** gombra.

4.  A **Frissítés forrásának kijelölése** lapon megadhatja, hogy az ügyfélszámítógépek honnan töltsék le a frissítéseket. Ha a **Frissítések helyi tárolása** jelölőnégyzetet jelöli be, akkor a WSUS-kiszolgáló tárolja a frissítéseket, és a fájlrendszerbeli tárolási hely szabadon megválasztható. Amennyiben nem ezt a lehetőséget választja, az ügyfélszámítógépek a Microsoft Update webhelyről töltik le a jóváhagyott frissítéseket.

    Tartsa meg az alapértelmezett beállításokat, majd kattintson a **Tovább** gombra.

    ![](images/Cc708622.fa6ac6a6-6814-4b7e-96e8-e08af5e534b8(WS.10).gif)

5.  Az **Adatbázis-beállítások** lapon a WSUS szolgáltatás adatbázisának kezeléséhez használt szoftvert kell megadni. Ha a szóban forgó számítógép operációs rendszere a Windows Server 2003 rendszer, a WSUS telepítője alapértelmezés szerint a WMSDE összetevő telepítését ajánlja fel.

    Ha nincs lehetőség a WMSDE alkalmazás használatára, akkor az **Ezen a számítógépen lévő létező adatbázis-kiszolgáló használata** választógombot bejelölve meg kell adni a WSUS által használandó SQL Server kiszolgálópéldányt, és be kell írni annak nevét az **SQL-példány kijelölése** mezőbe. A WMSDE összetevőtől eltérő adatbázisszoftver alkalmazási lehetőségeiről a „Deploying Microsoft Windows Server Update Services” című (angol nyelvű) szakmai dokumentációban talál bővebb felvilágosítást.

    Tartsa meg az alapértelmezett beállításokat, majd kattintson a **Tovább** gombra.

    ![](images/Cc708622.bc0b73ad-b338-437c-a3c7-0299e819840d(WS.10).gif)

6.  A WSUS által használandó webhelyet a **Webhely kijelölése** lapon adhatja meg, és ugyanezen a lapon találja a beállításhoz kapcsolódó két fontos URL-címet is: az egyik cím a WSUS-kiszolgálóhoz kapcsolódó ügyfélszámítógépekre telepítendő frissítések letöltésére szolgáló cím, a másik pedig a WSUS szolgáltatás beállításához használandó WSUS-konzol címe.

    Ha a 80-as porton már működik webhely, a WSUS által használt webhelyet egy másik porton kell létrehozni. A WSUS szolgáltatás egyéni porton történő futtatásáról a „Deploying Microsoft Windows Server Update Services” című (angol nyelvű) szakmai dokumentációban talál részletes tájékoztatást.

    Tartsa meg az alapértelmezett beállítást, majd kattintson a **Tovább** gombra.

    ![](images/Cc708622.64ed7643-a050-4f54-bf9f-04cf7931adc0(WS.10).gif)

7.  A **Frissítési beállítások tükrözése** lapon a szóban forgó WSUS-kiszolgáló kezelési szerepköre határozható meg. Ha ez a hálózat első WSUS-kiszolgálója, illetve ha elosztott rendszerkezelési topológiát kíván alkalmazni, ugorja át ezt a lapot.

    Amennyiben központi rendszerkezelési topológiát szeretne használni, és már működik WSUS-kiszolgáló a hálózaton, jelölje be a jelölőnégyzetet, majd írja be egy másik WSUS-kiszolgáló nevét a **Kiszolgáló neve** mezőbe. A rendszerkezelési szerepkörökről a „Deploying Microsoft Windows Server Update Services” című (angol nyelvű) szakmai dokumentációban olvashat részletesen.

    Tartsa meg az alapértelmezett beállítást, majd kattintson a **Tovább** gombra.

    ![](images/Cc708622.f26e09d5-983c-418d-8511-8960850403ef(WS.10).gif)

8.  Tekintse át a megadott beállításokat a **Kezdődhet a Microsoft Windows Server Update Services telepítése** lapon, majd kattintson a **Tovább** gombra.

    ![](images/Cc708622.20de7d09-3d30-4867-9253-6f353dd1923d(WS.10).gif)

9.  Ha a varázsló utolsó lapján a rendszer közli, hogy a WSUS szolgáltatás telepítése sikeresen befejeződött, kattintson a **Befejezés** gombra.
