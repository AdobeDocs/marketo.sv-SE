---
unique-page-id: 2950524
description: Distribuera sociala medier på din webbplats - Marketo Docs - produktdokumentation
title: Distribuera sociala medier på din webbplats
exl-id: bccfa461-29c1-4cf1-8e6a-2186c36bdf7e
feature: Social
source-git-commit: 97324d932b65020d041f728928d3792140bea71c
workflow-type: tm+mt
source-wordcount: '265'
ht-degree: 0%

---

# Distribuera sociala medier på din webbplats {#deploy-social-on-your-website}

Bädda in sociala appar på icke-Marketo-sidor.

>[!IMPORTANT]
>
>Den 31 juli 2024 började vi ta bort den här funktionen. Du kommer inte att kunna skapa nya resurser. Befintliga tillgångar kommer att fortsätta att fungera fram till 31 januari 2025. [Läs mer](https://nation.marketo.com/t5/employee-blogs/marketo-engage-social-features-deprecation/ba-p/351977){target="_blank"}

>[!AVAILABILITY]
>
>Alla användare i Marketo Engage har inte köpt den här funktionen. Kontakta kontoteamet (din kontoansvarige) för mer information.

Ni kan distribuera sociala appar på er egen webbplats för att engagera er målgrupp och föra in alla i den större konversationen i sociala nätverk. När man delar kampanjer och innehåll med sina vänner i sociala nätverk genererar man mer trafik på er webbplats.

1. Välj en godkänd social app, till exempel en YouTube Video eller Social Button.

   ![](assets/image2015-5-12-11-3a43-3a24.png)

1. Välj **Bädda in kod** från åtgärder för sociala appar.

   ![](assets/image2015-5-12-12-3a59-3a46.png)

1. Kopiera koden för webbplatsens sidhuvud (`<head>`) och brödtext (`<body>`).

   ![](assets/image2015-5-12-13-3a3-3a34.png)

1. Klistra in det första kodfragmentet i webbplatsens sidhuvud.

   ![](assets/socialonsite-embedhead.png)

1. Klistra in det andra kodfragmentet på varje sida, där du vill att din sociala app ska visas på sidan.

   ![](assets/socialonsite-embedwidget.png)

1. Om du behöver ange storleken på den sociala appen till specifika dimensioner på sidan lägger du till alternativen **outerHeight** och **outerWidth** i det andra kodfragmentet. Du kan till exempel lägga till `options='{"outerHeight":400, "outerWidth":600}'`, som i:

   ![](assets/socialonsite-resizewidget2.png)

   Din sociala Marketo-app lägger nu till innehåll och interaktivitet på din webbplats och bjuder in fans, besökare och befintliga kunder att sprida ordet om dig. Samtidigt läggs deras profildata till i databasen och mätvärden för social påverkan spåras.

   >[!MORELIKETHIS]
   >
   >* [Knappen Anpassa social app](/help/marketo/product-docs/demand-generation/social/configuring-social-actions/customize-social-app-button.md)
   >* [Ange krav för social delning](/help/marketo/product-docs/demand-generation/social/social-functions/set-social-share-requirement.md)
   >* [Publish landningssidor till Facebook](/help/marketo/product-docs/demand-generation/facebook/publish-landing-pages-to-facebook.md)
