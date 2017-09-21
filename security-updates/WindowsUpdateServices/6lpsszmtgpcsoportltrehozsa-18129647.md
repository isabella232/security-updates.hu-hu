---
TOCTitle: '6. lépés: Számítógépcsoport létrehozása'
Title: '6. lépés: Számítógépcsoport létrehozása'
ms:assetid: '6039e5dc-d2ce-4d4b-b737-17ebcadbd4a7'
ms:contentKeyID: 18129647
ms:mtpsurl: 'https://technet.microsoft.com/hu-hu/library/Cc720536(v=WS.10)'
---

6. lépés: Számítógépcsoport létrehozása
=======================================

A számítógépcsoportok még az egyszerű felépítésű környezetekben is fontos részét képezik a Windows Server Update Services (WSUS) programpéldányok működésének, hiszen segítségükkel megadott számítógépekre telepíthetők a frissítések. Két alapértelmezett számítógépcsoport különböztethető meg: Az összes számítógép csoport és a Hozzá nem rendelt számítógépek csoport. A WSUS-kiszolgálóval létesített első kapcsolat során a kiszolgáló alapértelmezés szerint minden egyes ügyfélszámítógépet mindkét csoportba felveszi.

Szükség esetén egyéni számítógépcsoportok is létrehozhatók: ennek egyik előnye, hogy a frissítések több számítógépre történő telepítését megelőzően lehetőség nyílik a frissítések tesztelésére. Ha a tesztelés eredménye kielégítő, a frissítések kiterjeszthetők Az összes számítógép csoportra. A létrehozható egyéni csoportok száma nem korlátozott.

A számítógépcsoportok létrehozása három részből álló folyamat: első lépésként azt kell megadni, hogy miként történik a számítógépek számítógépcsoportokba rendezése. Két lehetőség választható: *kiszolgálóoldali célcsoport-meghatározás* és *ügyféloldali célcsoport-meghatározás*. Az első módszerrel saját kezűleg kell hozzáadni az egyes számítógépeket a választott csoporthoz a WSUS szolgáltatással, míg a második módszer alkalmazásával automatikusan, csoportházirenddel vagy rendszerleíró kulccsal történik a hozzáadás. Második lépésként létre kell hozni a számítógépcsoportot a WSUS alkalmazásban. A harmadik lépésben az első lépésben választott módszerrel csoportokba kell helyezni a számítógépeket.

Ez az útmutató a kiszolgálóoldali célcsoport-meghatározást, valamint a számítógépek WSUS szolgáltatásbeli, saját kezűleg történő csoportokba helyezését mutatja be. Ha nagyszámú ügyfélszámítógépet szeretne számítógépcsoportokba szervezni, célszerű az ügyféloldali célcsoport-meghatározást alkalmazni, hiszen annak segítségével automatizálható a csoportba helyezés.

A 6. lépés végrehajtásával legalább egy számítógépet tartalmazó tesztcsoportot hozhat létre.

Ebben a lépésben a következő műveleteket kell végrehajtani:

-   Kiszolgálóoldali célcsoport-meghatározás megadása
-   Csoport létrehozása
-   Számítógépek csoportba helyezése

**A számítógépek csoportba helyezéséhez alkalmazott módszer megadása**
1.  Kattintson a WSUS-konzol eszköztárának **Beállítások** elemére, majd a **Számítógép beállításai** elemre.

2.  A **Számítógép beállításai** párbeszédpanelen válassza **A Microsoft Windows Server Update Services szolgáltatás Számítógépek áthelyezése feladatának használata** lehetőséget.

3.  Kattintson a **Feladatok** csoport **Beállítások mentése** gombjára, majd a megerősítést kérő párbeszédpanel **OK** gombjára.

**Csoport létrehozása**
1.  Kattintson a WSUS-konzol eszköztárán lévő **Számítógépek** elemre.

2.  Kattintson a **Feladatok** csoport **Számítógépcsoport létrehozása** elemére.

3.  A **Csoportnév** mezőbe írja be a **Teszt** szót, majd kattintson az **OK** gombra.

A következő műveletsort végrehajtva rendeljen hozzá egy, a tesztelésre alkalmas ügyfélszámítógépet a tesztcsoporthoz. A tesztelésre bármely olyan ügyfélszámítógép alkalmas, amelyen a hálózati környezetre jellemző hardver- és szoftverállomány működik, de arra ügyelni kell, hogy a számítógép ne rendelkezzen fontos szerepkörrel. Ezzel a megoldással megállapítható, hogy a tesztszámítógéppel összehasonlítandó számítógépek hogyan működnek együtt a jóváhagyott frissítésekkel.

**Számítógép saját kezű hozzáadása a tesztcsoporthoz**
1.  Kattintson a WSUS-konzol eszköztárán lévő **Számítógépek** elemre.

2.  A **Csoportok** mezőben jelölje ki az áthelyezendő számítógép csoportját.

3.  A számítógépeket felsoroló listában jelölje ki az áthelyezendő számítógépet.

4.  Kattintson a **Feladatok** csoport **Kijelölt számítógép áthelyezése** elemére.

5.  Jelölje ki a **Számítógépcsoport** lista azon csoportját, amelybe át kívánja helyezni a számítógépet, majd kattintson az **OK** gombra.
