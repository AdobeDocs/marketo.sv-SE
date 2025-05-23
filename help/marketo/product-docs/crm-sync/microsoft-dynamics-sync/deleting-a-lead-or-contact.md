---
unique-page-id: 45417322
description: Ta bort en lead eller kontakt - Marketo Docs - produktdokumentation
title: Ta bort en lead eller kontakt
exl-id: d561b424-6a2b-4abe-b9bd-81eb23f1a25b
feature: Microsoft Dynamics
source-git-commit: 2403ae0f1fdca3b8238f3f59e2a3b94129deb301
workflow-type: tm+mt
source-wordcount: '158'
ht-degree: 0%

---

# Ta bort en lead eller kontakt {#deleting-a-lead-or-contact}

Det finns en del att veta när det gäller att ta bort leads/kontakter i Microsoft Dynamics.

* Marketo Engage tar inte automatiskt bort personer bara för att leads har tagits bort i Dynamics. I stället är fältet&quot;Microsoft is Deleted&quot; satt till true. Du kan avaktivera det här fältet om du vill ta bort posten i Marketo.

* Flödesåtgärden &quot;Ta bort person&quot;: Detta tar endast bort en person i Marketo (ett alternativ för att även ta bort dem i Dynamics är inte tillgängligt).

* Om ett lead tas bort i Marketo (men inte i Dynamics) och sedan uppdateras i Dynamics, skapas en ny person i Marketo (samma e-postadress, nytt person-ID).

* Om ett lead tas bort i Dynamics (men inte i Marketo) och sedan körs genom flödesåtgärden Synkronisera person till Microsoft, skapas ett nytt lead i Dynamics.
