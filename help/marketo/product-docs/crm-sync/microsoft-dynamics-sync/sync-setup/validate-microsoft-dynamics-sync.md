---
unique-page-id: 8783322
description: Validera Microsoft Dynamics Sync - Marketo Docs - Produktdokumentation
title: Verifiera Microsoft Dynamics Sync
translation-type: tm+mt
source-git-commit: 47b2fee7d146c3dc558d4bbb10070683f4cdfd3d
workflow-type: tm+mt
source-wordcount: '267'
ht-degree: 0%

---


# Verifiera Microsoft Dynamics Sync {#validate-microsoft-dynamics-sync}

>[!CAUTION]
>
>Om Multi-Factor Authentication (MFA) är aktiverat för Dynamics Sync måste du inaktivera det för att Dynamics ska kunna synkroniseras korrekt med Marketo. Kontakta [Marketo Support](http://nation.marketo.com/community/support_solutions)om du vill ha mer information.

## Kör validera synkronisering i Marketo {#run-validate-sync-in-marketo}

Det är viktigt att du kör verktyget Validera synkronisering för att kontrollera att Microsoft Dynamics Sync with Marketo är korrekt konfigurerat innan du skapar den slutliga anslutningen mellan dem. Processen genererar en checklista med sju konfigurationssteg som identifierar var det finns problem. Om du kontrollerar att detta var korrekt kan du spara mycket tid senare.

1. Klicka på fliken **Admin** och sedan på länken **Microsoft Dynamics** i integreringsområdet.

   ![](assets/image2015-9-28-16-3a7-3a51.png)

1. Välj **Microsoft**.

   ![](assets/image2015-9-28-16-3a10-3a47.png)

1. Klicka på fliken **Validera synkroniseringsinställningar** .

   ![](assets/image2015-9-28-16-3a11-3a45.png)

1. Ange ditt användarnamn, lösenord och URL (klient-ID och klienthemlighet är valfria). Klicka på **Nästa** när du är klar.

   ![](assets/four-1.png)

   >[!NOTE]
   >
   >Om du har synkroniserat tidigare kommer **CRM** i det vänstra trädet att läsa **Microsoft Dynamics** och data i ovanstående formulär kan vara förifyllda.

1. Om allt är bra genererar Validera synkronisering en checklista full av gröna bockar ![—](assets/check.png).

   ![](assets/image2015-9-22-15-3a58-3a12.png)

1. Om du ser ett ![-](assets/delete.png)så har det ett problem. Information om hur du identifierar och åtgärdar problemet finns i [Åtgärda problem med synkronisering av Dynamics-validering](validate-microsoft-dynamics-sync/fix-dynamics-validation-sync-issues.md) . Kör sedan synkroniseringsvalideringsstegen igen tills resultatet ser ut som bilden ovan.

   >[!CAUTION]
   >
   >Vi stöder för närvarande inte uppdatering av sandlådan för Marketo Dynamics Sync. Om du behöver uppdatera din Dynamics CRM-sandlåda krävs en ny Marketo-sandlåda. Kontakta din Customer Success Manager om du vill ha mer information.

>[!NOTE]
>
>**Relaterade artiklar**
>
>[Åtgärda problem med synkronisering av Dynamics-validering](validate-microsoft-dynamics-sync/fix-dynamics-validation-sync-issues.md)

