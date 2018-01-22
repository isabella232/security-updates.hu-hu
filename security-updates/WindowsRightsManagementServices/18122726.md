---
TOCTitle: Az RMS szolgáltatásfiók megváltoztatása
Title: Az RMS szolgáltatásfiók megváltoztatása
ms:assetid: 'f257d66d-b823-41e4-bcb7-7c90eb295238'
ms:contentKeyID: 18122726
ms:mtpsurl: 'https://technet.microsoft.com/hu-hu/library/Cc747736(v=WS.10)'
---

Az RMS szolgáltatásfiók megváltoztatása
=======================================

A telepítés során az RMS létrehozza az RMS szolgáltatás nevű csoportot a helyi számítógépen, és ellátja a megfelelő engedélyekkel az összes olyan erőforráshoz, amelyek az RMS működéséhez szükségesek. Az RMS kiszolgálón történő létesítése során tartományi fiók használatával kell meghatározni az RMS szolgáltatásfiókját. Az RMS szolgáltatásfiókja nem egyezhet meg az RMS telepítéséhez használt tartományi fiókkal. Ez a fiók az RMS szolgáltatás csoport tagja lesz, és megkapja mindazokat az engedélyeket, amelyek be vannak állítva a csoporthoz. A rutinműveletek során az RMS az RMS-szolgáltatásfiókkal fut.

Az RMS-szolgáltatásfiókot bármikor megváltoztathatja. Ilyenkor az előzőleg megadott fiók automatikusan törlődik az RMS szolgáltatás csoportból, és az új fiók lesz a csoport tagja.

> [!IMPORTANT]
> Biztonsági megfontolásokból kifejezetten ajánljuk, hogy külön felhasználói fiókot hozzon létre az RMS szolgáltatásfiókjaként való használatra, és ezt a fiókot kizárólag az RMS szolgáltatásfiókjaként használja. Javasoljuk továbbá, hogy ennek a fióknak semmilyen egyéb engedélyt se adjon.

> [!NOTE]
> Az RMS szolgáltatásfiók nem egyezhet meg a Service Pack 1 javítócsomaggal kiegészített RMS telepítéséhez használt tartományi fiókkal.
