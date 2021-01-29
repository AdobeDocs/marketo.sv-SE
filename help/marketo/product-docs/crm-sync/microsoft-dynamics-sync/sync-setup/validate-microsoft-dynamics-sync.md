---
unique-page-id: 8783322
description: Validera Microsoft Dynamics Sync - Marketo Docs - Produktdokumentation
title: Verifiera Microsoft Dynamics Sync
translation-type: tm+mt
source-git-commit: 20d4c8a079916f47267df3dab5a8e663f6eb019b
workflow-type: tm+mt
source-wordcount: '266'
ht-degree: 0%

---


# Verifiera Microsoft Dynamics Sync {#validate-microsoft-dynamics-sync}

>[!CAUTION]
>
>Om Multi-Factor Authentication (MFA) är aktiverat för Dynamics Sync måste du inaktivera det för att Dynamics ska kunna synkroniseras korrekt med Marketo. Kontakta [Marketo Support](https://nation.marketo.com/t5/Support/ct-p/Support) om du vill ha mer information.

## Kör Verifiera synkronisering i Marketo {#run-validate-sync-in-marketo}

Det är viktigt att du kör verktyget Validera synkronisering för att kontrollera att Microsoft Dynamics Sync with Marketo är korrekt konfigurerat innan du skapar den slutliga anslutningen mellan dem. Processen genererar en checklista med sju konfigurationssteg som identifierar var det finns problem. Om du kontrollerar att detta var korrekt kan du spara mycket tid senare.

1. Klicka på fliken **Admin** och sedan på länken **Microsoft Dynamics** i integrationsområdet.

   ![](assets/image2015-9-28-16-3a7-3a51.png)

1. Välj **Microsoft**.

   ![](assets/image2015-9-28-16-3a10-3a47.png)

1. Klicka på fliken **Validera synkroniseringsinställningar**.

   ![](assets/image2015-9-28-16-3a11-3a45.png)

1. Ange ditt användarnamn, lösenord och URL (klient-ID och klienthemlighet är valfria). Klicka på **Nästa** när du är klar.

   ![](assets/four-1.png)

   >[!NOTE]
   >
   >Om du har synkroniserat tidigare kommer **CRM** i det vänstra trädet att läsa **Microsoft Dynamics**, och data i ovanstående formulär kan vara förifyllda.

1. Om allt är bra genererar Validera synkronisering en checklista med alla gröna bockmarkeringar ![—](assets/check.png).

   ![](assets/image2015-9-22-15-3a58-3a12.png)

1. Om du ser ett ![—](assets/delete.png) har det steget ett problem. Se [Åtgärda problem med synkronisering av Dynamics-validering](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/validate-microsoft-dynamics-sync/fix-dynamics-validation-sync-issues.md) för att identifiera och åtgärda problemet. Kör sedan synkroniseringsvalideringsstegen igen tills resultatet ser ut som bilden ovan.

   >[!CAUTION]
   >
   >Vi stöder för närvarande inte uppdatering av sandlådan för Marketo Dynamics Sync. Om du behöver uppdatera din Dynamics CRM-sandlåda krävs en ny Marketo-sandlåda. Kontakta din Customer Success Manager om du vill ha mer information.

>[!MORELIKETHIS]
>
>[Åtgärda problem med synkronisering av Dynamics-validering](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/validate-microsoft-dynamics-sync/fix-dynamics-validation-sync-issues.md)
