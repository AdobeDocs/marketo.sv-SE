---
unique-page-id: 7504736
description: Installera Marketo för Microsoft Dynamics 2015 On-Premises Step 1 of 3 - Marketo Docs - produktdokumentation
title: Installera Marketo för Microsoft Dynamics 2015 On-Premises Step 1 of 3
exl-id: c9b6d365-15c1-4eff-938c-8433b1fe7f24
feature: Microsoft Dynamics
source-git-commit: 821d69736b1cbeac0c80718c58a7a3c471387545
workflow-type: tm+mt
source-wordcount: '264'
ht-degree: 1%

---

# Steg 1 av 3: Konfigurera Synkronisera användare för Marketo (lokal version 2015) {#step-of-configure-sync-user-for-marketo-on-premises-2015}

Innan du kan synkronisera Microsoft Dynamics 2015 On-Premises med Marketo Engage måste du först installera Marketo-lösningen i Dynamics.

>[!NOTE]
>
>När du har synkroniserat Marketo till en CRM kan du inte synkronisera en ny CRM till den befintliga Marketo-instansen.

>[!PREREQUISITES]
>
>Om du använder Microsoft Dynamics On-Premise måste du ha [Driftsättning mot Internet](https://www.microsoft.com/en-us/download/confirmation.aspx?id=41701){target="_blank"} (IFD) with [Active Directory Federation Services](https://msdn.microsoft.com/en-us/library/bb897402.aspx){target="_blank"} 2.0+ (ADFS) har konfigurerats. Obs! IFD-dokumentet laddas ned automatiskt när du klickar på länken.
>
>[Ladda ned Marketo Lead Management Solution](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/download-the-marketo-lead-management-solution.md){target="_blank"} innan du börjar.

>[!NOTE]
>
>**Dynamics-administratörsbehörigheter krävs**.
>
>Du behöver administratörsbehörighet för CRM för att kunna utföra den här synkroniseringen.

1. Logga in i Dynamics. Klicka på **[!UICONTROL Microsoft Dynamics CRM]** nedrullningsbar meny och välj **[!UICONTROL Settings]**.

   ![](assets/image2015-3-19-8-33-29.png)

1. Under **[!UICONTROL Settings]** väljer du **[!UICONTROL Solutions]**.

   ![](assets/image2015-3-19-8-33-3.png)

1. Klicka på **[!UICONTROL Import]**.

   ![](assets/image2015-3-19-8-34-8.png)

1. Klicka **[!UICONTROL Browse]** och välj den lösning du behöver [nedladdad](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/download-the-marketo-lead-management-solution.md). Klicka på **[!UICONTROL Next]**.

   ![](assets/image2015-3-19-9-20-56.png)

1. Visa lösningsinformationen och klicka på **[!UICONTROL View solution package details]**.

   ![](assets/image2015-11-18-11-12-8.png)

1. När du är klar med kontrollen av all information klickar du på **[!UICONTROL Close]**.

   ![](assets/step6.png)

1. Gå tillbaka till sidan Lösningsinformation, klicka på **[!UICONTROL Next]**.

   ![](assets/image2015-3-19-9-21-50.png)

1. Kontrollera att kryssrutan för SDK-alternativet är markerad. Klicka på **[!UICONTROL Import]**.

   ![](assets/image2015-3-19-9-19-12.png)

1. Vänta tills importen är klar.

   >[!TIP]
   >
   >Du måste aktivera popup-fönster i webbläsaren för att slutföra installationen.

   ![](assets/image2015-3-11-11-34-9.png)

1. Hämta en loggfil (om du vill) och klicka på **[!UICONTROL Close]**.

   >[!NOTE]
   >
   >Du kan se ett meddelande med texten&quot;Marketo Lead Management har slutförts med varning&quot;. Detta är helt förväntat.

   ![](assets/image2015-3-13-9-54-39.png)

1. Marketo Lead Management visas nu på **[!UICONTROL All Solutions]** sida.

   ![](assets/image2015-3-19-8-40-38.png)

1. Välj Marketo och klicka **[!UICONTROL Publish All Customizations]**.

   ![](assets/image2015-3-19-8-41-21.png)

   Snyggt jobbat! Installationen är klar.

   >[!CAUTION]
   >
   >Om du inaktiverar någon av meddelandeprocesserna i Marketo SDK avbryts installationen!

   >[!MORELIKETHIS]
   >
   >[Installera Marketo för Microsoft Dynamics 2015 On-Premises Step 2 of 3](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/connecting-to-legacy-versions/step-2-of-3-set-up-2015.md){target="_blank"}
