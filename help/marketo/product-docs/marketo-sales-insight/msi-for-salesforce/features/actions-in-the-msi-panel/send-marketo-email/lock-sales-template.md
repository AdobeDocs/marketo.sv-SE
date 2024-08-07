---
unique-page-id: 12981050
description: Lås försäljningsmall - Marketo Docs - produktdokumentation
title: Lås försäljningsmall
exl-id: 005dde5d-ed60-444b-b7a3-b91be72a0151
feature: Marketo Sales Insights
source-git-commit: 431bd258f9a68bbb9df7acf043085578d3d91b1f
workflow-type: tm+mt
source-wordcount: '214'
ht-degree: 0%

---

# Lås försäljningsmall {#lock-sales-template}

För att förhindra CRM-användare från att redigera säljmallar kan administratörer låsa mallar, vilket gör att användare kan låsa mallar individuellt från e-postredigeraren.

>[!CAUTION]
>
>Den här funktionen fungerar endast för Salesforce och är inte kompatibel med Microsoft Dynamics eller andra CRM. Mallar som öppnas från Outlook- eller Gmail-plugin-program kommer inte att låsas eftersom redigeraren inte styrs av Marketo.

## Aktivera låsmall {#enable-lock-template}

>[!NOTE]
>
>**Administratörsbehörigheter krävs**

1. Gå till **Admin** och klicka sedan på **Sales Insight**.

   ![](assets/1.png)

1. Klicka på **Redigera** under **Inställningar**.

   ![](assets/2.png)

1. Markera **Aktivera möjligheten att låsa mallar**. Klicka på **Spara**.

   ![](assets/image2017-10-9-8-3a19-3a45.png)

>[!NOTE]
>
>Som standard är den här rutan markerad och möjligheten att låsa mallar är aktiverad. Om du avmarkerar alternativet inaktiveras funktionen för låsmall i e-postredigeraren.

>[!NOTE]
>
>Om du ändrar den här inställningen som administratör kommer **inte** att påverka befintliga mallar retroaktivt. Det innebär att de inte låses automatiskt.

## Lås mall i e-postredigeraren {#lock-template-in-the-email-editor}

1. Markera det e-postmeddelande som du vill låsa och klicka sedan på **Redigera utkast**.

   ![](assets/5.png)

1. Klicka på **E-postinställningar** i e-postredigeraren.

   ![](assets/6.png)

1. Kontrollera **Publish till Marketo Sales Insight** om den inte redan är markerad. Du kan nu avmarkera **Tillåt CRM-användare att redigera e-post** för att låsa mallen. Klicka på **Spara**.

   ![](assets/7.png)

   >[!NOTE]
   >
   >Som standard är den här kryssrutan markerad och CRM-användare kan redigera e-postmeddelanden.
