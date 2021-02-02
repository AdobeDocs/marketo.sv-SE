---
unique-page-id: 45417322
description: Ta bort en lead eller kontakt - Marketo Docs - produktdokumentation
title: Ta bort en lead eller kontakt
translation-type: tm+mt
source-git-commit: 2b5ccd7220557a5e966d33436d0f0d2a65e4589d
workflow-type: tm+mt
source-wordcount: '157'
ht-degree: 0%

---


# Ta bort en lead eller kontakt {#deleting-a-lead-or-contact}

Det finns en del att veta när det gäller att ta bort leads/kontakter i Microsoft Dynamics.

* Marketo tar inte automatiskt bort personer bara för att leads har tagits bort i Dynamics. I stället är fältet&quot;Microsoft is Deleted&quot; satt till true. Om du vill kan du avaktivera det här fältet och ta bort posten i Marketo.

* Flödesåtgärden &quot;Ta bort person&quot;: Detta tar bara bort en person i Marketo (ett alternativ för att även ta bort dem i Dynamics är inte tillgängligt).

* Om ett lead tas bort i Marketo (men inte i Dynamics) och uppdateras i Dynamics efter det, skapas en ny person i Marketo (samma e-postadress, nytt person-ID).

* Om ett lead tas bort i Dynamics (men inte i Marketo) och sedan körs genom flödesåtgärden Synkronisera person till Microsoft, skapas ett nytt lead i Dynamics.
