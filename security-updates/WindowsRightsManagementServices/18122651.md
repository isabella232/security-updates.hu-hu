---
TOCTitle: A topológiai célok megállapítása
Title: A topológiai célok megállapítása
ms:assetid: '8275a04d-3e5b-40b0-be9d-2f31b7aeca6b'
ms:contentKeyID: 18122651
ms:mtpsurl: 'https://technet.microsoft.com/hu-hu/library/Cc747652(v=WS.10)'
---

A topológiai célok megállapítása
================================

A topológia megtervezésének egyik legfontosabb lépése a célok helyes megállapítása. Az RMS topológiájának megtervezése során többek között az alábbi fontos területeket kell végiggondolni:

-   **Felügyeleti költségek**. A hely topológiájának lehetővé kell tennie a felügyeleti költségek minimalizálását. Vagyis lehetőleg központilag kell felügyelni a kiszolgálókat, valamint a lehető legkevesebb kiszolgálót kell használni.

-   **Hálózati késés**. Az ügyfél és a kiszolgáló közötti hálózati késés a felhasználó számára az e-mailek és a dokumentumok megnyitásakor jelentkező további várakozás formájában fog megnyilvánulni. Általános szabályként az üzemidő legalább 90 százaléka alatt mindkét irányban két másodpercnél rövidebbnek kell lennie a késésnek.

-   **Megbízhatóság**. Az ügyfél és a kiszolgáló közötti hálózatnak elegendően megbízhatónak kell lennie ahhoz, hogy a HTTP-kérelmek és -válaszok sikertelenségi aránya (vagyis az elveszett vagy sérült tranzakciók aránya) 5 százalék alatt legyen.

Ezek csak általános irányelvek, minden esetben egyedileg kialakítani a szervezet követelményein és erőforrásain alapuló célkitűzéseket. A célkitűzések meghatározásából kiindulva lehet megállapítani, hogy milyen topológia felel meg az igényeknek. Számos tényező befolyásolja a célok megvalósíthatóságát, például a felhasználók, a licenckérelmek, a lekérdezések és az üzenetek száma, valamint az RMS egyéb, a hálózati forgalomra hatással lévő tényezői. Emellett jelentős hatással van a topológiai célok elérésére a bevezetési stratégia is, például az, hogy mely tartományokban és erdőkben kívánja bevezetni az RMS szolgáltatást. A topológiatervezési folyamat minden lépése során szem előtt kell tartani a célokat, és meg kell vizsgálni, hogy az egyes döntések milyen hatással lesznek a célokra.
