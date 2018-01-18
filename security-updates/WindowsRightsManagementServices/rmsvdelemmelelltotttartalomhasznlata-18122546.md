---
TOCTitle: 'RMS-védelemmel ellátott tartalom használata'
Title: 'RMS-védelemmel ellátott tartalom használata'
ms:assetid: '3cf6d64b-1187-433c-bbb2-c68069bc3c30'
ms:contentKeyID: 18122546
ms:mtpsurl: 'https://technet.microsoft.com/hu-hu/library/Cc720251(v=WS.10)'
---

RMS-védelemmel ellátott tartalom használata
===========================================

Amikor a felhasználók védett tartalmat használnak, két folyamat megy végbe a felhasználó számára észrevétlenül. Az első az, hogy az RMS-kompatibilis alkalmazás használati licencet kérelmez, amikor a felhasználó megnyitja a dokumentumot. A második az, hogy az RMS-kompatibilis alkalmazás megvizsgálja a használati licencet annak megállapítására, hogy az megköveteli-e a visszavonási listát, és ellenőrzi, hogy nincs-e visszavonva a licenc és a tartalomvédelmi fióktanúsítvány tanúsítványláncába tartozó valamelyik tanúsítvány. Miután mindkét folyamat befejeződött, az RMS-kompatibilis alkalmazás megjeleníti a tartalmat, ha ezt a jogok és a visszavonások összessége megengedi.

Ha a licenc megköveteli a visszavonási listát, az alkalmazás megnézi, hogy elérhető-e helyben a visszavonási lista egy még le nem járt érvényességű példánya. Ha nem, letölti a visszavonási lista aktuális példányát. Az alkalmazás ezt követően alkalmazza az adott összefüggésben értelmezhető esetleges visszavonási feltételeket.

Ha nincs olyan visszavonási feltétel, amely megakadályozná a tartalom megnyitását, az alkalmazás megjeleníti a tartalmat, a felhasználó pedig élhet a neki megadott jogokkal.

Az RMS beállítható úgy is, hogy feldolgozza a jogosult külső felhasználóktól érkező kérelmeket is. Ez lehetővé teszi, hogy a felhasználók az interneten át megosszák egymással a védett tartalmat.

A szakasz tartalma:

-   [Használati licenc megszerzése](https://technet.microsoft.com/0b6cde34-418a-4dee-9d27-b65b93b535ac)

-   [A használati licencek és a külső felhasználók](https://technet.microsoft.com/02db9bda-180e-438f-863d-26252083a471)