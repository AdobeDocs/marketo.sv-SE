---
unique-page-id: 8783322
description: Verifiera [!DNL Microsoft Dynamics] synkronisering - Marketo Docs - produktdokumentation
title: Verifiera [!DNL Microsoft Dynamics] synkronisering
exl-id: 00297a8d-36c3-42f6-a9b8-4a8dd7c1f30d
feature: Microsoft Dynamics
source-git-commit: 0d37fbdb7d08901458c1744dc68893e155176327
workflow-type: tm+mt
source-wordcount: '236'
ht-degree: 0%

---

# Verifiera synkronisering av [!DNL Microsoft Dynamics] {#validate-microsoft-dynamics-sync}

>[!CAUTION]
>
>Om Multi-Factor Authentication (MFA) är aktiverat för din [!DNL Dynamics]-synkronisering måste du inaktivera det för att [!DNL Dynamics] ska kunna synkronisera korrekt med Marketo. Kontakta [Marketo Support](https://nation.marketo.com/t5/Support/ct-p/Support) om du vill ha mer information.

## Kör Verifiera synkronisering i Marketo {#run-validate-sync-in-marketo}

Det är viktigt att du kör verktyget Validera synkronisering för att kontrollera att din [!DNL Microsoft Dynamics]-synkronisering med Marketo är korrekt konfigurerad innan du skapar den slutliga anslutningen mellan dem. Processen genererar en checklista med sju konfigurationssteg som identifierar var det finns problem. Om du kontrollerar att detta var korrekt kan du spara mycket tid senare.

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
   >Om du har synkroniserat tidigare kommer **CRM** i det vänstra trädet att läsa **[!DNL Microsoft Dynamics]** och data i ovanstående formulär kan vara förifyllda.

1. Om allt är bra genererar Validera synkronisering en checklista full av gröna bockmarkeringar ![—](assets/check.png).

   ![](assets/image2015-9-22-15-3a58-3a12.png)

1. Om du ser ett ![-](assets/delete.png) har det steget ett problem. Se [Åtgärda [!DNL Dynamics] Problem med synkronisering av validering](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/validate-microsoft-dynamics-sync/fix-dynamics-validation-sync-issues.md) för att identifiera och åtgärda problemet. Kör sedan synkroniseringsvalideringsstegen igen tills resultatet ser ut som bilden ovan.

   >[!CAUTION]
   >
   >Vi stöder för närvarande inte uppdatering av sandlådan för synkronisering av [!DNL Marketo Dynamics]. Om du behöver uppdatera din [!DNL Dynamics] CRM-sandlåda krävs en ny Marketo-sandlåda. Kontakta din Customer Success Manager om du vill ha mer information.

>[!MORELIKETHIS]
>
>[Åtgärda [!DNL Dynamics] Problem med synkronisering av validering](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/validate-microsoft-dynamics-sync/fix-dynamics-validation-sync-issues.md)
