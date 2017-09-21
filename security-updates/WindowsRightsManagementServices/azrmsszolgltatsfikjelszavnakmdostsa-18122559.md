---
TOCTitle: Az RMS szolgáltatásfiók jelszavának módosítása
Title: Az RMS szolgáltatásfiók jelszavának módosítása
ms:assetid: '435c9cef-b622-48b3-9d4d-4bf5cac7d52d'
ms:contentKeyID: 18122559
ms:mtpsurl: 'https://technet.microsoft.com/hu-hu/library/Cc720273(v=WS.10)'
---

Az RMS szolgáltatásfiók jelszavának módosítása
==============================================

Az RMS kiszolgálókhoz megadott jelszókezelési szabályzattól függően az RMS szolgáltatásfiókjának jelszava meghatározott időszakonként lejárhat. Ha a jelszó lejár, az RMS működése leáll. Éppen ezért még lejárat előtt meg kell változtatni a jelszót.

**Egy RMS szolgáltatásfiók használata**

Ha egy RMS-szolgáltatásfiókot használ, a következő művelet végrehajtásával változtathatja meg a jelszót az RMS kiszolgálókon:

1.  Ha a kiszolgáló fürthöz tartozik, vonja ki a kiszolgálót a fürt működéséből.
2.  Jelentkezzen be a kiszolgálóra az RMS-szolgáltatásfiók bejelentkezési adataival.
3.  Változtassa meg az RMS-szolgáltatásfiók jelszavát.
    Az azonos RMS-szolgáltatásfiókot használó kiszolgálókon leáll a szolgáltatás, mert a kiszolgálókon tárolt bejelentkezési adatok érvénytelenné válnak a jelszó megváltoztatása után.
4.  Jelentkezzen ki a kiszolgálóról.
5.  Az RMS rendszergazdai bejelentkezési adatait használva jelentkezzen be újra a kiszolgálóra.
6.  A felhasználói identitás újbóli megadásához a **Globális felügyelet** lapon kattintson **Az RMS szolgáltatásfiókjának módosítása** hivatkozásra, majd **Az RMS szolgáltatásfiókjának módosítása** lapon adja meg a tartományt, a felhasználónevet és a jelszót.
7.  Indítsa újra az IIS szolgáltatást.
8.  Ha szükséges, helyezze vissza a kiszolgálót a fürtbe.
9.  Ismételje meg a 6–8. lépést a fürtben található összes kiszolgálón.

Ez az RMS-szolgáltatásfiók jelszava megváltoztatásának egyszerűbb módja, azonban az RMS működésének időleges leállását eredményezheti, mivel a kiszolgálón az RMS-szolgáltatásfiók jelszavának megváltoztatásakor az Active Directoryt is frissíteni kell az új jelszóval. Az IIS meghatározott időközönként újraindítja az alkalmazáskészleteket, és a korábbi bejelentkezési adatokkal működő alkalmazáskészletek mindaddig nem indulhatnak újra, amíg meg nem változtatja az RMS szolgáltatásfiókjának jelszavát, és újra nem indítja az IIS szolgáltatást az adott kiszolgálón. Az RMS működése csak akkor áll helyre, ha az alkalmazáskészletek újraindultak.

**Két RMS szolgáltatásfiók használata**

Ennél a módszernél először hozzon létre két olyan RMS szolgáltatásfiókot, amelyek lejárati szabályzata vagy dátuma eltérő. A szokásos működés során az RMS az első fiókkal fut. Amikor meg kell változtatni az első fiók jelszavát, mindegyik RMS-kiszolgálón hajtsa végre a következő műveleteket:

1.  Ha a kiszolgáló fürthöz tartozik, vonja ki a kiszolgálót a fürt működéséből.
2.  Adja meg a második RMS-szolgáltatásfiókot az RMS futtatásához. A fiók megváltoztatásának ismertetését lásd: „[Az RMS szolgáltatásfiók megváltoztatása](https://technet.microsoft.com/f257d66d-b823-41e4-bcb7-7c90eb295238)”.
3.  Indítsa újra az IIS szolgáltatást.
4.  Ha szükséges, helyezze vissza a kiszolgálót a fürtbe.

Amikor valamennyi RMS kiszolgáló a második szolgáltatásfiókot használja, az RMS rendszer működésének fenntartása mellett megváltoztathatja az RMS első szolgáltatásfiókjának a jelszavát. Ezzel a módszerrel a két fiók felváltott használatával elkerülheti az RMS leállását.
