---
unique-page-id: 12981050
description: Lås försäljningsmall - Marketo Docs - produktdokumentation
title: Lås försäljningsmall
exl-id: 005dde5d-ed60-444b-b7a3-b91be72a0151
source-git-commit: 72e1d29347bd5b77107da1e9c30169cb6490c432
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

1. Gå till **Administratör** och sedan klicka **Försäljningsinsikter**.

   ![](assets/1.png)

1. Under **Inställningar**, klicka **Redigera**.

   ![](assets/2.png)

1. Kontrollera **Möjlighet att låsa mallar**. Klicka **Spara**.

   ![](assets/image2017-10-9-8-3a19-3a45.png)

>[!NOTE]
>
>Som standard är den här rutan markerad och möjligheten att låsa mallar är aktiverad. Om du avmarkerar alternativet inaktiveras funktionen för låsmall i e-postredigeraren.

>[!NOTE]
>
>Om du ändrar den här inställningen som administratör ändras **not** retroaktivt påverka befintliga mallar, Det innebär att de inte låses automatiskt.

## Lås mall i e-postredigeraren {#lock-template-in-the-email-editor}

1. Välj den e-postadress som du vill låsa och klicka sedan på **Redigera utkast**.

   ![](assets/5.png)

1. I e-postredigeraren klickar du på **E-postinställningar**.

   ![](assets/6.png)

1. Kontrollera **Publicera till Marketo Sales Insight** om det inte redan är markerat. Du kan nu avmarkera **Tillåt CRM-användare att redigera e-post** för att låsa mallen. Klicka **Spara**.

   ![](assets/7.png)

   >[!NOTE]
   >
   >Som standard är den här kryssrutan markerad och CRM-användare kan redigera e-postmeddelanden.
