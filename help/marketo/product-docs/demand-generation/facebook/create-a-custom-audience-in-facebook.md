---
unique-page-id: 4720275
description: Skapa en anpassad målgrupp i Facebook - Marketo Docs - produktdokumentation
title: Skapa en anpassad målgrupp i Facebook
exl-id: a2c8d89c-16b3-44f6-a2c6-c52fe78ab39c
feature: Integrations
source-git-commit: 431bd258f9a68bbb9df7acf043085578d3d91b1f
workflow-type: tm+mt
source-wordcount: '271'
ht-degree: 0%

---

# Skapa en anpassad målgrupp i Facebook {#create-a-custom-audience-in-facebook}

>[!PREREQUISITES]
>
>* [Lägg till anpassade Facebook-målgrupper som en LaunchPoint-tjänst](/help/marketo/product-docs/demand-generation/ad-network-integrations/add-facebook-custom-audiences-as-a-launchpoint-service.md){target="_blank"} i administratörsavsnittet.
>* [Acceptera Facebook anpassade målgruppsvillkor](https://www.facebook.com/ads/manage/customaudiences/tos.php){target="_blank"} i ditt Facebook-konto.

>[!TIP]
>
>Läs mer om [anpassade målgrupper i Facebook](https://www.facebook.com/help/341425252616329){target="_blank"}.

1. Hitta och välj den smarta eller statiska lista som innehåller de leads du vill skapa målgruppen från.

   ![](assets/create-a-custom-audience-in-facebook-1.png)

1. Välj fliken **Leads** och klicka sedan på ikonen **Skicka via Lägg till Bridge** längst ned.

   ![](assets/create-a-custom-audience-in-facebook-2.png)

1. Välj **Facebook** och klicka på **Nästa**.

   ![](assets/create-a-custom-audience-in-facebook-3.png)

1. Klicka på listrutan **Målgrupp** och välj **+ Ny målgrupp**.

   ![](assets/create-a-custom-audience-in-facebook-4.png)

   >[!IMPORTANT]
   >
   >Facebook API tillåter upp till 500 anpassade målgrupper per Facebook-annonskonto.

1. Skriv in ett **målgruppsnamn**. Klicka på **Uppdatera**.

   ![](assets/create-a-custom-audience-in-facebook-5.png)

   >[!NOTE]
   >
   >Om du har flera Facebook-annonskonton visas ytterligare en listruta där du kan välja vilket annonskonto som målgruppen har skapats i.

   >[!TIP]
   >
   >Vill du byta ut en ny publik mot en befintlig som är kopplad till en annonsuppsättning eller grupp? Markera kryssrutan **Ersätt en befintlig publik**. Om du gör detta tas **inte** den målgrupp som ersätts bort.

1. När du är klar uppdateras statusdialogrutan.

   ![](assets/create-a-custom-audience-in-facebook-6.png)

   Och det är allt! I Facebook ser du den nya målgruppen i **Ads Manager** > **Publiker**.

   ![](assets/create-a-custom-audience-in-facebook-7.png)

   >[!NOTE]
   >
   >Alla listor som du flyttar över till Facebook blir statiska. Smarta listor i Marketo kommer inte att automatiskt uppdatera målgruppslistan i Facebook för att återspegla ändringar som gjorts efter överföringen.

   >[!TIP]
   >
   >Se [Facebook utbildningsväg för Marketo-kunder](https://facebook.exceedlms.com/student/enrollments/create_enrollment_from_token/BF9TqSaCvM73PP4ScjhCm4fi){target="_blank"}. Det täcker allt ni behöver veta, från att skapa en Facebook-sida till att målinrikta era Facebook-annonser med hjälp av Marketo nätverksintegreringar för annonser.

   >[!MORELIKETHIS]
   >
   >[Lägg till leads till en anpassad målgrupp i Facebook](/help/marketo/product-docs/demand-generation/facebook/add-leads-to-a-custom-audience-in-facebook.md)
