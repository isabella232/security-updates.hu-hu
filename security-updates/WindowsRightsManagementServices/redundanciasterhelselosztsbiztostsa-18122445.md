---
TOCTitle: Redundancia és terheléselosztás biztosítása
Title: Redundancia és terheléselosztás biztosítása
ms:assetid: '162d547c-78a7-4848-b43e-58e481832af2'
ms:contentKeyID: 18122445
ms:mtpsurl: 'https://technet.microsoft.com/hu-hu/library/Cc720199(v=WS.10)'
---

Redundancia és terheléselosztás biztosítása
===========================================

Annak biztosításához, hogy a felhasználók mindig licenchez juttassanak és közzétehessék a tartalmat, amikor ez szükséges, kifejezetten ajánljuk, hogy fürtök használatával redundáns RMS kiszolgálókat vezessen be. Ez legkevesebb azt jelenti, hogy egy legalább két kiszolgálóból álló legfelső szintű tanúsítási fürtöt célszerű üzembe helyezni. Ha külön licenckiszolgálót is üzembe helyez a szervezet valamely csoportjának sajátos licencszükségleteinek kielégítésére, a licenckiszolgálót is ajánlatos legalább két kiszolgálóból álló fürtként megvalósítani.

A legfelső szintű tanúsítási fürtbe vagy a valamelyik licencelési fürtbe tartozó több fizikai kiszolgáló közös URL-cím (vagy virtuális cím) mögött működő webfarmot alkot. Ha a szervezetnél kiszolgálófarmot használnak, az RMS beépíthető az eddig használt virtuális címzési architektúrába, legyen az ciklikus multiplexeléses DNS, terheléselosztási szolgáltatás vagy e célra rendelt hardveres megoldás.

A virtuális címzés a terheléselosztás mellett azért is előnyös az RMS szolgáltatásnál, mert megszünteti, hogy a rendszer a tanúsítás és a licencelés szempontjából egyetlen fizikai kiszolgálónak legyen kiszolgáltatva. A végfelhasználók számítógépének nem kell közvetlenül hozzáférnie a fürt egyetlen kiszolgálójához sem.
