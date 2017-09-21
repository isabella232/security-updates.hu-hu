---
TOCTitle: Az aligénylési szolgáltatás észlelése
Title: Az aligénylési szolgáltatás észlelése
ms:assetid: 'b159953a-af38-4a9e-8c87-1aff5fb4e366'
ms:contentKeyID: 18122641
ms:mtpsurl: 'https://technet.microsoft.com/hu-hu/library/Cc747641(v=WS.10)'
---

Az aligénylési szolgáltatás észlelése
=====================================

Az egyedi licenckiszolgálóknak, illetve a licencelési fürtök első kiszolgálójának aligénylési kérelmet kell benyújtaniuk az RMS legfelső szintű tanúsítási kiszolgálójához, és kiszolgálói licencelői tanúsítványt kell szerezniük. Ekkor a licenckiszolgáló a következőképpen jut hozzá az legfelső szintű tanúsítási kiszolgáló aligénylési szolgáltatásának URL-címéhez.

A licenckiszolgáló létesítése során az RMS telepítője lekérdezi az Active Directoryt, és megkeresi a legfelső szintű tanúsítási fürt szolgáltatáskapcsolódási pontját. Az RMS a szolgáltatás kapcsolódási pontjában tárolt URL-cím segítségével határozza meg a legfelső szintű tanúsítási fürt helyét, majd kiszolgálói licencelői tanúsítványt kérelmez a legfelső szintű tanúsítási kiszolgálón futó aligénylési szolgáltatástól.

Az aligénylési szolgáltatás iránti kérelem benyújtásakor a licenckiszolgáló először beolvassa az Active Directoryból a legfelső szintű tanúsítási kiszolgáló Certification virtuális könyvtárának URL-címét (itt található az aligénylési szolgáltatás). Ezután a címet kiegészíti az aligénylési szolgáltatás elérési útjával.

A legfelső szintű tanúsítási kiszolgáló Certification virtuális könyvtárának URL-címét a következő formában tárolja az Active Directory:

http://*kiszolgálónév*/\_wmcs/Certification

Amikor a licenckiszolgáló az aligénylési szolgáltatáshoz küld kérelmet, hozzáfűzi az URL-címhez a szolgáltatásfájl nevét:

http://kiszolgálónév/\_wmcs/Certification/SubEnrollService.asmx

| ![](images/Cc747641.note(WS.10).gif)Megjegyzés:                                                  |
|-------------------------------------------------------------------------------------------------------------------------------|
| Ha engedélyezte az SSL használatát az RMS kiszolgálón, akkor ezek az URL-címek a https:// kapcsolódási protokollt használják. |
