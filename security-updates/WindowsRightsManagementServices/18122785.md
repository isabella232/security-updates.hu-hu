---
TOCTitle: A kulcskezelési követelmények meghatározása
Title: A kulcskezelési követelmények meghatározása
ms:assetid: 'f0e08fb8-bf5e-4278-a09f-daa57696e786'
ms:contentKeyID: 18122785
ms:mtpsurl: 'https://technet.microsoft.com/hu-hu/library/Cc747797(v=WS.10)'
---

A kulcskezelési követelmények meghatározása
===========================================

Az RMS kriptográfiai kulcsok segítségével védi a tartalmat és tartatja be a jogokat. A kriptográfiai kulcsok alapvető fontosságúak, ezek biztosítják a rendszer zavartalan és biztonságos működését. A rendszergazdáknak különös gondot kell fordítaniuk a kulcsok kezelésére, és meg kell őket védeni az adatvesztésben, rendszerhibákban és a lopásban rejlő kockázatokkal szemben.

Az alapértelmezett konfigurációban a kiszolgáló kulcspárját és a kapcsolódó GUID azonosítót a konfigurációs adatbázis egyik táblájában tárolja az RMS. A kiszolgáló kulcspárját a létesítési eljárás során megadott jelszóval titkosítja a rendszer.

A kiszolgáló kulcspárjának és a kapcsolódó GUID azonosító védelméhez készítse el a konfigurációs adatbázis biztonsági másolatát egy adathordozón (például CD-lemez), és tárolja ezt biztonságos helyen (például páncélszekrényben). A biztonsági mentés gyakorisága attól függ, hogy milyen gyakran hajt végre felügyeleti jellegű változtatásokat, és hogy milyen szinten fogadható el az a kockázat, amely az adathordozó állagának romlásából vagy egyéb tényezőkből fakad. Ügyeljen arra, hogy ismerje a konfigurációs adatbázis biztonsági mentésekor a személyes kulcshoz használt jelszót. A megfelelő jelszó nélkül nem fogja tudni visszaállítani az RMS kiszolgálót a biztonsági másolatból.

Ha adatbázis-kiszolgálóként az SQL Server rendszert használja, az SQL Server Enterprise Manager segédprogramjával közvetlenül másolhatja a személyes kulcs titkosított adatainak és a GUID azonosítónak az értékét egy biztonságos hajlékonylemezre vagy más adathordozóra. Mivel a személyes kulcs védelemmel van ellátva, az RMS telepítésének a biztonsági mentéssel azonos szolgáltatásfiókkal kell futnia, amikor helyreállítja azt egy védett adathordozóról egy RMS-telepítésbe.

Ha szoftveres vagy hardveres kriptográfiai szolgáltatót (CSP) használ a személyes kulcs védelméhez, kézzel kell biztonsági másolatot készítenie a kulcstárolóról és a kulcsról. A hardveres biztonsági modul használata azzal javítja a személyes kulcsok biztonságát, hogy a tárolás hardvereszközben történik, és szoftver számára a kulcsok sohasem elérhetők. A rendszer továbbítja a visszafejtendő vagy aláírandó adatokat a hardveres biztonsági modulba, amely végrehajtja a visszafejtést vagy az aláírást, majd visszaküldi ezeket.

Valamennyi kriptográfiai szolgáltató (CSP), legyen az hardveres vagy szoftveres, saját eljárással rendelkezik a kulcs biztonsági mentésének végrehajtásához. Az eljárás részletes ismertetése az adott CSP dokumentációjában olvasható.
