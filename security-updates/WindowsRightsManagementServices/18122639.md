---
TOCTitle: A közzétételi szolgáltatás észlelése
Title: A közzétételi szolgáltatás észlelése
ms:assetid: '5d500841-a202-4865-b5d2-d0775d4e1bbc'
ms:contentKeyID: 18122639
ms:mtpsurl: 'https://technet.microsoft.com/hu-hu/library/Cc747580(v=WS.10)'
---

A közzétételi szolgáltatás észlelése
====================================

Az RMS közzétételi szolgáltatása állítja ki a közzétételi licenceket, amelyek a tartalom védelmére szolgálnak. Ez bocsátja ki az ügyfél licencelői tanúsítványokat is, amelyek módot adnak a felhasználóknak arra, hogy akkor is közzétegyenek tartalmat, amikor nem kapcsolódnak a vállalati hálózathoz.

A közzétételi szolgáltatás a legfelső szintű tanúsítási fürttől vagy a licenckiszolgálóktól érhető el. Ezt a szolgáltatást az RMS-kompatibilis alkalmazások kérelmezik akkor, amikor a szerző RMS-védelemmel ellátott tartalmat tesz közzé. A közzétételi szolgáltatás iránti kérelem benyújtásakor az alkalmazás először beolvassa az Active Directoryból a kiszolgáló Licensing virtuális könyvtárának URL-címét (itt található a közzétételi szolgáltatás). Ezt követően a címet kiegészíti a közzétételi szolgáltatás elérési útjával.

A kiszolgáló Licensing virtuális könyvtárának URL-címét a következő formában tárolja az Active Directory:

http://*kiszolgálónév*/\_wmcs/Licensing

Amikor egy kiszolgáló közzétételi licencet kérelmez, hozzáfűzi az URL-címhez a közzétételi szolgáltatás fájlnevét:

http://*kiszolgálónév*/\_wmcs/Licensing/Publish.asmx

Ha az RMS azt észleli, hogy a tartalomvédelmi fióktanúsítvány a Windows-hitelesítésen alapul, az Active Directory-erdő alapján állapítja meg a közzétételi szolgáltatás helyét. Ez mind a belső felhasználókra, mind a vállalati hálózathoz virtuális magánhálózaton (VPN) át kapcsolódó külső felhasználókra érvényes.

Ha az RMS azt észleli, hogy a tartalomvédelmi fióktanúsítvány a Microsoft® .NET Passport hitelesítő adatain alapul, a közzétételi szolgáltatás helye az RMS-védelemmel ellátott tartalomban megadott .NET Passport-fiók.

> [!NOTE]  
> Ha engedélyezte az SSL használatát az RMS kiszolgálón, akkor ezek az URL-címek a https:// kapcsolódási protokollt használják. 
