---
unique-page-id: 2359428
description: Omdirigera en landningssida - Marketo Docs - produktdokumentation
title: Omdirigera en landningssida
exl-id: 5c9205aa-e970-4d72-a4e3-48593da4181c
source-git-commit: 80512816eaf0a70a3f10a50c34aeea14edd9046b
workflow-type: tm+mt
source-wordcount: '124'
ht-degree: 0%

---

# Omdirigera en landningssida {#redirect-a-landing-page}

## Uppdrag: Omdirigera en landningssida till en annan webbsida {#mission-redirect-a-landing-page-to-a-different-web-page}

>[!NOTE]
>
>**Administratörsbehörigheter krävs**

>[!PREREQUISITES]
>
>* [Landningssida med ett formulär](/help/marketo/getting-started/quick-wins/landing-page-with-a-form.md){target="_blank"}
>* [Anpassa URL:en till landningssidan med en CNAME](/help/marketo/product-docs/demand-generation/landing-pages/landing-page-actions/customize-your-landing-page-urls-with-a-cname.md){target="_blank"}


## Steg 1: Starta en ny omdirigeringsregel {#step-start-a-new-redirect-rule}

1. Gå till **[!UICONTROL Admin]** område.

   ![](assets/redirect-a-landing-page-1.png)

1. Gå till **[!UICONTROL Landing Pages]**.

   ![](assets/redirect-a-landing-page-2.png)

1. Klicka på **[!UICONTROL Rules]** tabbtangenten och sedan klicka **[!UICONTROL New]** och **[!UICONTROL New Redirect Rule]**.

   ![](assets/redirect-a-landing-page-3.png)

## Steg 2: Definiera omdirigeringsregeln {#step-define-the-redirect-rule}

1. Klicka på den första **[!UICONTROL Original URL]** och välja Marketo CNAME.

   ![](assets/redirect-a-landing-page-4.png)

   >[!NOTE]
   >
   >Kom ihåg att du bara kan dirigera om landningssidor som börjar med din Marketo [CNAME](/help/marketo/product-docs/demand-generation/landing-pages/landing-page-actions/customize-your-landing-page-urls-with-a-cname.md){target="_blank"}.

1. Klicka på den andra **[!UICONTROL Original URL]** och välj den landningssida som du vill omdirigera.

   ![](assets/redirect-a-landing-page-5.png)

1. För **[!UICONTROL Redirect URL]** markera sidan som du vill omdirigera till och klicka på **[!UICONTROL Create]**.

   ![](assets/redirect-a-landing-page-6.png)

## Uppdraget är slutfört {#mission-complete}

Grattis! Du har omdirigerat en landningssida.

<br> 

[◄ 9: Uppdatera lead-data](/help/marketo/getting-started/quick-wins/update-person-data.md)
