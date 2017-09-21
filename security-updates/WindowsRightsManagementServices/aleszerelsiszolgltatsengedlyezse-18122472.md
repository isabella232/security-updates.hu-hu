---
TOCTitle: A leszerelési szolgáltatás engedélyezése
Title: A leszerelési szolgáltatás engedélyezése
ms:assetid: '45226e85-b50d-41cc-aca7-0f603f8509d5'
ms:contentKeyID: 18122472
ms:mtpsurl: 'https://technet.microsoft.com/hu-hu/library/Cc720261(v=WS.10)'
---

A leszerelési szolgáltatás engedélyezése
========================================

Az RMS rendszer leszereléséhez szükség van a közzétett adatok védelméhez használt személyes kulcsra. Ezt a személyes kulcsot a konfigurációs adatbázis tárolja a DPAPI (Data Protection API) segítségével titkosítva, és a kulcs a létesítés során megadott jelszón alapul. Ha az RMS titkos kulcsot hardveres biztonsági modulon (HSM) tárolják, a titkos kulcsot a konfigurációs adatbázis helyett a HSM tárolja.

| ![](images/Cc720261.Caution(WS.10).gif)Figyelmeztetés:                                                                                                                            |
|----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| Az RMS rendszer leszerelése előtt győződjön meg arról, hogy ismeri a titkos kulcsa jelszavát. Ha nem ismeri ezt a jelszót, az RMS kiszolgáló leszerelése előtt vissza kell állítani a titkos kulcsa jelszavát. |

Az RMS rendszer eltávolításának első lépése a fürtben lévő kiszolgálók leszerelése. Mivel a leszerelés licencelési funkció, az aligényléssel létesített RMS csak licencelő fürtjében lévő kiszolgáló leszerelhető anélkül, hogy hatással lenne az RMS legfelső szintű fürtjére, vagy az RMS többi, aligényléssel létesített, csak licencelő fürtjére. Éppen ezért külön kell leszerelni az RMS legfelső szintű, csak licencelő fürtjét, mivel mindegyik csak licencelő fürt saját titkos kulccsal rendelkezik a közzétételi licencek létrehozásához.

A leszerelési szolgáltatás engedélyezéséhez hajtsa végre a következő eljárást:

1.  Nyissa meg az RMS felügyeleti webhelyét.
2.  Kattintson az **RMS felügyelete**, majd a **Biztonsági beállítások** elemre.
3.  Jelölje be **Az RMS-telepítés leszerelésének engedélyezése** négyzetet.
4.  A művelet jóváhagyását kérő üzenetpanelen kattintson az **OK** gombra.

A leszerelt kiszolgálókon nem állítható vissza az RMS szabványos konfigurációja. Ez az eljárás nem vonható vissza.

Az RMS leszerelése után újabb RMS példány csak akkor telepíthető, ha előbb a **Programok telepítése és törlése** segédprogrammal teljesen eltávolítja a szolgáltatást.
