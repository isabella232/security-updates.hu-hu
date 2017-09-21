---
TOCTitle: A fióktanúsítási szolgáltatás észlelése
Title: A fióktanúsítási szolgáltatás észlelése
ms:assetid: '293a2f91-4712-45ec-8b74-7533f4144cbd'
ms:contentKeyID: 18122455
ms:mtpsurl: 'https://technet.microsoft.com/hu-hu/library/Cc720224(v=WS.10)'
---

A fióktanúsítási szolgáltatás észlelése
=======================================

Az RMS fióktanúsítási szolgáltatása állítja ki a felhasználók számára a tartalomvédelmi fióktanúsítványokat. Minden tartalomvédelmi fióktanúsítvány (RAC) csak adott számítógépen vagy eszközön érvvényes, és a tanúsítványt igénylő felhasználónak érvényes géptanúsítvánnyal kell rendelkeznie.

A fióktanúsítási szolgáltatás csak a legfelső szintű tanúsítási kiszolgálón vagy fürtön fut. A fióktanúsítási iránti kérelem benyújtásakor az ügyfél először beolvassa az Active Directoryból a legfelső szintű tanúsítási kiszolgáló Certification virtuális könyvtárának URL-címét (itt található a fióktanúsítási szolgáltatás). Ezután a címet kiegészíti a fióktanúsítási szolgáltatás elérési útjával.

A legfelső szintű tanúsítási kiszolgáló Certification virtuális könyvtárának URL-címét a következő formában tárolja az Active Directory:

http://*kiszolgálónév*/\_wmcs/Certification

Amikor egy ügyfél tartalomvédelmi fióktanúsítványt kérelmez, hozzáfűzi az URL-címhez a fióktanúsítási szolgáltatás fájlnevét:

http://*kiszolgálónév*/\_wmcs/Certification/Certification.asmx

| ![](images/Cc720224.note(WS.10).gif)Megjegyzés:                                                  |
|-------------------------------------------------------------------------------------------------------------------------------|
| Ha engedélyezte az SSL használatát az RMS kiszolgálón, akkor ezek az URL-címek a https:// kapcsolódási protokollt használják. |
