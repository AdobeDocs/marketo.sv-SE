---
description: Steg 1 av 3 - Installera Marketo Solution with Server to Server Connection - Marketo Docs - produktdokumentation
title: Steg 1 av 3 - Installera Marketo Solution med Server to Server Connection
exl-id: bf6f87c1-5ba5-490b-bcce-365120af3730
feature: Microsoft Dynamics
source-git-commit: 0d37fbdb7d08901458c1744dc68893e155176327
workflow-type: tm+mt
source-wordcount: '234'
ht-degree: 2%

---

# Steg 1 av 3: Installera Marketo Solution med Server to Server Connection {#step-1-of-3-install-the-marketo-solution-s2s}

Innan du kan synkronisera [!DNL Microsoft Dynamics 365] och Marketo måste du först installera Marketo-lösningen i [!DNL Dynamics]. **[!DNL Dynamics]Administratörsbehörigheter krävs.**

>[!CAUTION]
>
>Aktivera inte anpassad entitetssynkronisering innan den inledande synkroniseringen har slutförts. Du meddelas via e-post när den första synkroniseringen är klar.

>[!NOTE]
>
>När du har synkroniserat Marketo till en CRM kan du inte utföra en ny synkronisering utan att ersätta instansen.

>[!PREREQUISITES]
>
>[Hämta Marketo Lead Management Solution](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/download-the-marketo-lead-management-solution.md){target="_blank"}

1. Logga in på **[[!DNL Microsoft Office 365]](https://login.microsoftonline.com/)**.

   ![](assets/image2015-3-16-15-3a58-3a55.png)

1. Klicka på menyn ![](assets/image2015-3-16-16-3a1-3a13.png) och välj **[!UICONTROL CRM]**.

   ![](assets/image2015-3-16-16-3a0-3a10.png)

1. Klicka på menyn ![](assets/image2015-5-13-10-3a5-3a8.png). I listrutan väljer du **[!UICONTROL Settings]** och sedan **[!UICONTROL Solutions]**.

   ![](assets/image2015-5-13-10-3a4-3a1.png)

1. Klicka på **[!UICONTROL Import]**.

   ![](assets/image2015-3-19-8-3a34-3a8.png)

1. Klicka på **[!UICONTROL Choose File]**. Välj den Marketo Lead Management-lösning som du [hämtade](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/download-the-marketo-lead-management-solution.md). Klicka på **[!UICONTROL Next]**.

   ![](assets/image2015-10-9-14-3a44-3a14.png)

1. Visa lösningsinformationen och klicka på **[!UICONTROL View solution package details]**.

   ![](assets/image2015-10-9-15-3a4-3a16.png)

1. När du har kontrollerat alla detaljer klickar du på **[!UICONTROL Close]**.

   ![](assets/image2015-10-9-14-3a57-3a3.png)

1. Gå tillbaka till sidan [!UICONTROL Solution Information] och klicka på **[!UICONTROL Next]**.

   ![](assets/image2015-10-9-14-3a59-3a24.png)

1. Kontrollera att kryssrutan för alternativet SDK är markerad. Klicka på **[!UICONTROL Import]**.

   ![](assets/image2015-10-9-15-3a7-3a12.png)

   >[!TIP]
   >
   >Du måste aktivera popup-fönster i webbläsaren för att slutföra installationen.

1. Vänta nu tills importen är klar.

   ![](assets/image2015-3-11-11-3a34-3a9.png)

1. Klicka på **[!UICONTROL Close]**.

   >[!NOTE]
   >
   >Du kan se ett meddelande med texten&quot;Marketo Lead Management har slutförts med varning&quot;. Detta är helt förväntat.

   ![](assets/image2015-3-13-9-3a54-3a39.png)

1. [!UICONTROL Marketo Lead Management] visas nu i listan över lösningar.

   ![](assets/image2015-3-19-8-3a40-3a38.png)

1. Markera **[!UICONTROL Marketo Lead Management]** och klicka på **[!UICONTROL Publish All Customizations]**.

   ![](assets/image2015-3-19-8-3a41-3a21.png)

   Hög fem! Installationen är klar.

   >[!MORELIKETHIS]
   >
   >[Steg 2 av 3: Konfigurera Marketo-lösningen med S2S-anslutning](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/microsoft-dynamics-365-with-s2s-connection/step-2-of-3-set-up.md){target="_blank"}
