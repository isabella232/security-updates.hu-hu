---
TOCTitle: '6. lépés: Számítógépcsoportok konfigurálása'
Title: '6. lépés: Számítógépcsoportok konfigurálása'
ms:assetid: '70518732-2179-4e41-9609-7f9999867f41'
ms:contentKeyID: 21741743
ms:mtpsurl: 'https://technet.microsoft.com/hu-hu/library/Dd939860(v=WS.10)'
---

6. lépés: Számítógépcsoportok konfigurálása
===========================================

A számítógépcsoportok a Windows Server Update Services 3.0 Service Pack 2 (WSUS 3.0 SP2) központilag telepített példányainak fontos részét képezik. A számítógépcsoportok lehetővé teszik a frissítések tesztelését és adott számítógépekre való telepítését. Két alapértelmezett számítógépcsoport létezik: Az összes számítógép és a Hozzá nem rendelt számítógépek csoport. A WSUS-kiszolgálóval létesített első kapcsolat során a kiszolgáló alapértelmezés szerint minden egyes ügyfélszámítógépet mindkét csoportba felveszi.

Tetszés szerinti számú egyéni számítógépcsoport hozható létre a frissítések szervezetben történő kezeléséhez. Érdemes legalább egy számítógépcsoportot létrehozni a frissítések teszteléséhez, mielőtt központilag telepíteni azt a szervezet többi számítógépére.

Az 6. lépés műveletei
---------------------

1.  Számítógépcsoport létrehozása
2.  Legalább egy számítógép áthelyezése a tesztcsoportba

**Tesztcsoport létrehozása**
1.  A WSUS felügyeleti konzolon bontsa ki a **Számítógépek** csomópontot, és jelölje ki **Az összes számítógép** elemet.

2.  Kattintson a jobb gombbal **Az összes számítógép** elemre, és válassza a **Számítógépcsoport hozzáadása** parancsot.

3.  A **Számítógépcsoport hozzáadása** párbeszédpanelen írja be a **Név** mezőbe az új tesztcsoport nevét, majd kattintson a **Hozzáadás** gombra.

A következő műveletsorral egy ügyfélszámítógépet rendelhet hozzá a tesztcsoporthoz. A tesztszámítógép bármely olyan számítógép lehet, amelynek szoftverei és hardvereszközei hasonlóak a hálózaton található ügyfélszámítógépekének többségéhez, ugyanakkor nincs kritikus szerepkörhöz rendelve. Ha a tesztek sikeresek, jóváhagyhatja a frissítéseket a tetszés szerinti csoportok számítógépeihez.

**Számítógép hozzárendelése a tesztcsoporthoz**
1.  A WSUS felügyeleti konzolon kattintson a **Számítógépek** elemre.

2.  Kattintson annak a számítógépnek a csoportjára, amelyet a tesztcsoporthoz szeretne rendelni.

3.  A számítógépek listájában jelölje ki a tesztcsoporthoz hozzárendelni kívánt számítógépet vagy számítógépeket.

4.  Kattintson a jobb gombbal a **Tagság módosítása** parancsra.

5.  A **Számítógépcsoport-tagság beállítása** párbeszédpanelen jelölje ki a korábban létrehozott tesztcsoportot, majd kattintson az **OK** gombra.

Ismételje meg e két eljárást, azaz hozzon létre egy csoportot, majd rendeljen hozzá egy vagy több számítógépet a csoporthoz, és hozzon létre annyi további számítógépcsoportot, amennyi a webhely frissítéseinek kezeléséhez szükséges.

Következő lépés
---------------

[7. lépés: A WSUS frissítéseinek jóváhagyása és központi telepítése](https://technet.microsoft.com/c4e58e17-d5e3-4194-8f26-b459e0c03b86)

További források
----------------

[Részletes útmutató a Windows Server Update Services 3.0 SP2 telepítéséhez](https://technet.microsoft.com/4b504edc-93b3-45b0-a7e8-d0107f1a4442)
