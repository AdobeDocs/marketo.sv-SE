---
unique-page-id: 3571805
description: Steg 1 av 3 - Installera Marketo Solution (2011 On-Premises) - Marketo Docs - produktdokumentation
title: Steg 1 av 3 - Installera Marketo Solution (On-Premises 2011)
exl-id: 6e559b10-5273-4dc2-b98d-49c509cbeff7
feature: Microsoft Dynamics
source-git-commit: 0d37fbdb7d08901458c1744dc68893e155176327
workflow-type: tm+mt
source-wordcount: '253'
ht-degree: 1%

---

# Steg 1 av 3: Installera Marketo Solution (2011 On-Premises) {#step-of-install-the-marketo-solution-on-premises}

Innan du kan synkronisera [!DNL Microsoft Dynamics] On-Premises och Marketo måste du först installera Marketo-lösningen i [!DNL Dynamics].

>[!NOTE]
>
>När du har synkroniserat Marketo till en CRM kan du inte utföra en ny synkronisering utan att ersätta instansen.

>[!PREREQUISITES]
>
>Du måste ha [Internet Facing Deployment](https://learn.microsoft.com/en-us/dynamics365/customerengagement/on-premises/deploy/configure-an-internet-facing-deployment){target="_blank"} (IFD) med [Active Directory Federation Services](https://msdn.microsoft.com/en-us/library/bb897402.aspx){target="_blank"} 2.0, 2.1 eller 3.0 (ADFS) konfigurerat. **Obs!** IFD-dokumentet hämtas automatiskt när du klickar på länken.
>
>[Ladda ned Marketo Lead Management Solution](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/download-the-marketo-lead-management-solution.md){target="_blank"} innan du startar.

>[!NOTE]
>
>**[!DNL Dynamics]Administratörsbehörigheter krävs.**
>
>Du behöver administratörsbehörighet för CRM för att kunna utföra den här synkroniseringen.

1. Logga in på **[!DNL Dynamics]**, välj **[!UICONTROL Settings]** i den nedre vänstra menyn.

   ![](assets/image2015-4-2-11-3a32-3a53.png)

1. Välj **[!UICONTROL Solutions]** i trädet.

   ![](assets/image2015-4-2-11-3a35-3a28.png)

1. Klicka på **[!UICONTROL Import]**.

   ![](assets/image2015-4-2-11-3a37-3a33.png)

1. Klicka på **[!UICONTROL Browse]**. Välj den Marketo Lead Management-lösning som du [hämtade](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/download-the-marketo-lead-management-solution.md). Klicka på **[!UICONTROL Next]**.

   ![](assets/image2015-4-2-11-3a40-3a33.png)

1. Visa lösningsinformationen och klicka på **[!UICONTROL View solution package details]**.

   ![](assets/image2015-11-18-11-3a12-3a8.png)

1. När du har kontrollerat alla detaljer klickar du på **[!UICONTROL Close]**.

   ![](assets/image2015-10-9-14-3a57-3a3.png)

1. Klicka på **[!UICONTROL Next]** på sidan Lösningsinformation.

   ![](assets/image2015-4-2-11-3a41-3a48.png)

1. Kontrollera att kryssrutan för meddelandealternativ i SDK är markerad. Klicka på **[!UICONTROL Next]**.

   ![](assets/image2015-4-2-11-3a42-3a37.png)

   >[!TIP]
   >
   >Du måste aktivera popup-fönster i webbläsaren för att slutföra installationen.

1. Vänta nu tills importen är klar. Ställ dig upp och sträck lite.

   ![](assets/image2015-4-2-11-3a43-3a51.png)

1. Klicka på **[!UICONTROL Close]**.

   >[!NOTE]
   >
   >Du kan se ett meddelande med texten&quot;Marketo Lead Management har slutförts med varning&quot;. Detta är helt förväntat.

   ![](assets/image2015-4-2-11-3a44-3a44.png)

1. [!UICONTROL Marketo Lead Management] visas nu på sidan **[!UICONTROL All Solutions]**.

   ![](assets/image2015-4-2-11-3a46-3a55.png)

1. Markera [!UICONTROL Marketo Lead Management] och klicka på **[!UICONTROL Publish All Customizations]**.

   ![](assets/image2015-4-2-11-3a48-3a21.png)

>[!CAUTION]
>
>Om du inaktiverar någon av meddelandeprocesserna i Marketo SDK avbryts installationen!

>[!MORELIKETHIS]
>
>[Steg 2 av 3: Konfigurera Marketo Sync-användare i [!DNL Dynamics] (2011 On-Premises)](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/connecting-to-legacy-versions/step-2-of-3-set-up-2011.md)
