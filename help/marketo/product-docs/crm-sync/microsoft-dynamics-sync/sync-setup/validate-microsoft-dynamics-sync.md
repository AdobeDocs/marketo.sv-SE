---
unique-page-id: 8783322
description: Validera Microsoft Dynamics Sync - Marketo Docs - produktdokumentation
title: Validera Microsoft Dynamics Sync
exl-id: 00297a8d-36c3-42f6-a9b8-4a8dd7c1f30d
feature: Microsoft Dynamics
source-git-commit: 4045f262889d06304111288d30da893529396e81
workflow-type: tm+mt
source-wordcount: '253'
ht-degree: 0%

---

# Validera Microsoft Dynamics Sync {#validate-microsoft-dynamics-sync}

>[!CAUTION]
>
>Om Multi-Factor Authentication (MFA) är aktiverat för Dynamics Sync måste du inaktivera det för att Dynamics ska kunna synkroniseras korrekt med Marketo. Kontakta [Marketo Support](https://nation.marketo.com/t5/Support/ct-p/Support){target="_blank"} om du vill ha mer information.

## Kör Verifiera synkronisering i Marketo {#run-validate-sync-in-marketo}

Det är viktigt att du kör verktyget Validera synkronisering för att kontrollera att Microsoft Dynamics Sync med Marketo är rätt konfigurerat innan du skapar den slutliga anslutningen mellan dem. Processen genererar en checklista med sju konfigurationssteg som identifierar var det finns problem. Om du kontrollerar att detta var korrekt kan du spara mycket tid senare.

1. Klicka på fliken **[!UICONTROL Admin]** och sedan på länken **[!DNL Microsoft Dynamics]** i integreringsområdet.

   ![](assets/image2015-9-28-16-3a7-3a51.png)

1. Välj **[!DNL Microsoft]**.

   ![](assets/image2015-9-28-16-3a10-3a47.png)

1. Klicka på fliken **[!UICONTROL Validate Sync Setup]**.

   ![](assets/image2015-9-28-16-3a11-3a45.png)

1. Ange ditt användarnamn, lösenord och URL (klient-ID och klienthemlighet är valfria). Klicka på **[!UICONTROL Next]** när du är klar.

   ![](assets/four-1.png)

   >[!NOTE]
   >
   >Om du har synkroniserat tidigare kommer **[!UICONTROL CRM]** i det vänstra trädet att läsa **[!DNL Microsoft Dynamics]** och data i ovanstående formulär kan vara förifyllda.

1. Om allt är bra genererar Validera synkronisering en checklista full av gröna bockmarkeringar ![—](assets/check.png).

   ![](assets/image2015-9-22-15-3a58-3a12.png)

1. Om du ser ett ![-](assets/delete.png) har det steget ett problem. Se [Åtgärda problem med synkronisering av Dynamics-validering](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/validate-microsoft-dynamics-sync/fix-dynamics-validation-sync-issues.md){target="_blank"} för att identifiera och åtgärda problemet. Kör sedan synkroniseringsvalideringsstegen igen tills resultatet ser ut som bilden ovan.

   >[!CAUTION]
   >
   >Vi stöder för närvarande inte uppdatering av sandlådan för Marketo Dynamics Sync. Om du behöver uppdatera din Dynamics CRM-sandlåda krävs en ny Marketo-sandlåda. Kontakta kontoteamet (din kontoansvarige) för mer information.

>[!MORELIKETHIS]
>
>[Åtgärda problem med synkronisering av Dynamics-validering](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/validate-microsoft-dynamics-sync/fix-dynamics-validation-sync-issues.md){target="_blank"}
