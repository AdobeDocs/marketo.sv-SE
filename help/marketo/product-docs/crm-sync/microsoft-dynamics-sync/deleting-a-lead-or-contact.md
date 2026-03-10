---
unique-page-id: 45417322
description: Förstå hur lead- och kontaktborttagning fungerar mellan Microsoft Dynamics och Marketo. Använd flaggan Borttagen i Microsoft och åtgärden Ta bort personflöde efter behov.
title: Ta bort en lead eller kontakt
exl-id: d561b424-6a2b-4abe-b9bd-81eb23f1a25b
feature: Microsoft Dynamics
source-git-commit: 2b29f05a27f847184e0968442012d443e9e0597d
workflow-type: tm+mt
source-wordcount: '166'
ht-degree: 0%

---

# Ta bort en lead eller kontakt {#deleting-a-lead-or-contact}

Det finns några saker att veta när det gäller att ta bort leads/kontakter i [!DNL Microsoft Dynamics].

* Marketo tar inte automatiskt bort personer bara för att leads har tagits bort i [!DNL Dynamics]. I stället är fältet&quot;Microsoft is Deleted&quot; satt till true. Du kan avaktivera det här fältet om du vill ta bort posten i Marketo.

* Flödesåtgärden &quot;Ta bort person&quot;: Detta tar endast bort en person i Marketo (ett alternativ för att även ta bort dem i Dynamics är inte tillgängligt).

* Om ett lead tas bort i Marketo (men inte i [!DNL Dynamics]) och uppdateras i [!DNL Dynamics] därefter, skapas en ny person i Marketo (samma e-postadress, nytt person-ID).

* Om ett lead tas bort i [!DNL Dynamics] (men inte i Marketo) och sedan körs genom flödesåtgärden Synkronisera person till Microsoft, skapas ett nytt lead i [!DNL Dynamics].
