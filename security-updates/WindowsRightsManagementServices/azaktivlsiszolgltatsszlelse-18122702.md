---
TOCTitle: Az aktiválási szolgáltatás észlelése
Title: Az aktiválási szolgáltatás észlelése
ms:assetid: 'e178d81b-b35c-4958-87ef-e077e2204b32'
ms:contentKeyID: 18122702
ms:mtpsurl: 'https://technet.microsoft.com/hu-hu/library/Cc747697(v=WS.10)'
---

Az aktiválási szolgáltatás észlelése
====================================

Az aktiválási szolgáltatás kulcstárolókat és RMS géptanúsítványokat állít ki az RMS 1.0-s verziójú ügyfelek számára. Ez a szolgáltatás az RMS 1.0-s verziójú ügyfélszoftverével való kompatibilitás miatt szerepel. Az RMS legfelső szintű tanúsítási fürtje nyújtja az aktiválási proxy szolgáltatást, amely továbbítja a vállalati hálózatban működő ügyfélszámítógépek RMS-gépaktiválási kérelmeit az aktiválási szolgáltatásnak.

A gépaktiválási kérelem benyújtásakor az RMS 1.0-s verziójú ügyfél először beolvassa az Active Directoryból a legfelső szintű tanúsítási kiszolgáló Certification virtuális könyvtárának URL-címét (itt található aktiválási proxy szolgáltatás). Ezután a címet kiegészíti az aktiválási proxy szolgáltatás elérési útjával.

A legfelső szintű tanúsítási kiszolgáló Certification virtuális könyvtárának URL-címét a következő formában tárolja az Active Directory:

http://*kiszolgálónév*/\_wmcs/Certification

Amikor egy ügyfél RMS-gépaktiválást kérelmez, hozzáfűzi az URL-címhez az aktiválási proxy szolgáltatás fájlnevét:

http://*kiszolgálónév*/\_wmcs/Certification/Activation.asmx

A vállalati hálózaton kívül futó ügyfelek az UDDI segítségével keresik meg az aktiválási szolgáltatást. A további tudnivalókat lásd: „[A Microsoft által működtetett szolgáltatások közzététele](https://technet.microsoft.com/7ee8cb4d-1b46-48be-8a4c-5ff6a458231a)”.

> [!NOTE]  
> Ha engedélyezte az SSL használatát az RMS kiszolgálón, akkor ezek az URL-címek a https:// kapcsolódási protokollt használják. 
