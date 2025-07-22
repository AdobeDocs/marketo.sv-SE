---
unique-page-id: 12981050
description: Lås försäljningsmall - Marketo Docs - produktdokumentation
title: Lås försäljningsmall
exl-id: 005dde5d-ed60-444b-b7a3-b91be72a0151
feature: Marketo Sales Insights
source-git-commit: 0d37fbdb7d08901458c1744dc68893e155176327
workflow-type: tm+mt
source-wordcount: '183'
ht-degree: 1%

---

# Lås försäljningsmall {#lock-sales-template}

För att förhindra CRM-användare från att redigera säljmallar kan administratörer låsa mallar, vilket gör att användare kan låsa mallar individuellt från e-postredigeraren.

>[!CAUTION]
>
>Den här funktionen fungerar endast för [!DNL Salesforce] och är inte kompatibel med [!DNL Microsoft Dynamics] eller andra CRM-system. Mallar som används från plugin-programmen [!DNL Outlook] eller Gmail kommer inte att låsas eftersom redigeraren inte styrs av Marketo.

## Aktivera låsmall {#enable-lock-template}

>[!NOTE]
>
>**Administratörsbehörigheter krävs**

1. Gå till **[!UICONTROL Admin]** och klicka sedan på **[!UICONTROL Sales Insight]**.

   ![](assets/1.png)

1. Klicka på **[!UICONTROL Settings]** under **[!UICONTROL Edit]**.

   ![](assets/2.png)

1. Kontrollera **[!UICONTROL Enable ability to lock templates]**. Klicka på **[!UICONTROL Save]**.

   ![](assets/image2017-10-9-8-3a19-3a45.png)

>[!NOTE]
>
>Som standard är den här rutan markerad och möjligheten att låsa mallar är aktiverad. Om du avmarkerar alternativet inaktiveras funktionen för låsmall i e-postredigeraren.

>[!NOTE]
>
>Om du ändrar den här inställningen som administratör kommer **inte** att påverka befintliga mallar retroaktivt. Det innebär att de inte låses automatiskt.

## Lås mall i e-postredigeraren {#lock-template-in-the-email-editor}

1. Välj den e-postadress som du vill låsa och klicka sedan på **[!UICONTROL Edit Draft]**.

   ![](assets/5.png)

1. Klicka på **[!UICONTROL Email Settings]** i e-postredigeraren.

   ![](assets/6.png)

1. Kontrollera **[!UICONTROL Publish to Marketo Sales Insight]** om det inte redan är markerat. Du kan nu avmarkera **[!UICONTROL Allow CRM user to edit email]** för att låsa mallen. Klicka på **[!UICONTROL Save]**.

   ![](assets/7.png)

   >[!NOTE]
   >
   >Som standard är den här kryssrutan markerad och CRM-användare kan redigera e-postmeddelanden.
