---
TOCTitle: A felügyelő csoport használata
Title: A felügyelő csoport használata
ms:assetid: '0febcb3e-7124-4e51-971a-1013b928d33b'
ms:contentKeyID: 18122491
ms:mtpsurl: 'https://technet.microsoft.com/hu-hu/library/Cc720198(v=WS.10)'
---

A felügyelő csoport használata
==============================

A létesítés során a RMS egy speciális felügyelő csoportot hoz létre, amely teljes hozzáféréssel rendelkezik a tartalomvédelemmel ellátott tartalmakhoz. A felügyelő csoport tagjai teljes körű tulajdonosi jogosultságot kapnak minden olyan használati licencben, amelyet az az RMS kiszolgáló vagy fürt adott ki, amelyhez a felügyelői csoport tartozik. Ez azt jelenti, hogy a csoport tagjai visszafejthetik a védett tartalmi fájlok bármelyikét, és megszüntethetik azok védelmét. A felügyelő csoport tagjai például megszüntethetik az olyan fájlok védelmét, amelyeket egy elbocsátott alkalmazott tett közzé, hogy a fájlok új tulajdonosa közzétehesse és kezelhesse a fájlokat.

A felügyelő csoportnak alapértelmezés szerint nincsenek tagjai, a rendszergazdák sem kerülnek bele automatikusan. A felügyeleti webhely használatakor megadhatja azt az Active Directory biztonsági csoportot, amelyet az RMS felügyelői csoportjaként kíván használni. Erre a célra választhat egy meglévő Active Directory-csoportot, vagy létrehozhat új csoportot is. A csoportnak ugyanabban az Active Directory-erdőben kell lennie, mint az RMS-telepítésnek. Az RMS felügyelő csoportjaként meghatározott csoportba tartozó összes felhasználói fiók rendelkezni fog a felügyelő csoport engedélyeivel.

Az RMS felügyelő csoportjának megadásáról a témakör „[A felügyelő csoport beállítása](https://technet.microsoft.com/f2ef847e-2824-471f-9079-5c343094aba8)” című pontjában olvashat.

> [!NOTE]  
> Az RMS felügyelői csoportjaként megadni kívánt csoportnak már léteznie kell ugyanabban az Active Directory-erdőben, amelyben az RMS-telepítés található. A csoport tulajdonságai között szerepelnie kell egy e-mail címnek, amely a fiók nevével megegyező teljesen minősített tartománynévvel rendelkezik. Az e-mail cím kötelező formátuma a következő: *csoportnév*@*tartománynév*. 
