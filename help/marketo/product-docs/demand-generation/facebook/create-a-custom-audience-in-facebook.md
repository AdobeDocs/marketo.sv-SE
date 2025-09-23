---
unique-page-id: 4720275
description: Skapa en anpassad målgrupp i Facebook - Marketo Docs - produktdokumentation
title: Skapa en anpassad målgrupp i Facebook
exl-id: a2c8d89c-16b3-44f6-a2c6-c52fe78ab39c
feature: Integrations
source-git-commit: 09a656c3a0d0002edfa1a61b987bff4c1dff33cf
workflow-type: tm+mt
source-wordcount: '219'
ht-degree: 0%

---

# Skapa en anpassad målgrupp i [!DNL Facebook] {#create-a-custom-audience-in-facebook}

>[!PREREQUISITES]
>
>* [Lägg till [!DNL Facebook] anpassade målgrupper som en LaunchPoint-tjänst](/help/marketo/product-docs/demand-generation/ad-network-integrations/add-facebook-custom-audiences-as-a-launchpoint-service.md){target="_blank"} i administratörsavsnittet.
>* [Acceptera  [!DNL Facebook]s anpassade målgruppsvillkor](https://www.facebook.com/ads/manage/customaudiences/tos.php){target="_blank"} i ditt [!DNL Facebook]-konto.

>[!TIP]
>
>Läs mer om [anpassade målgrupper i [!DNL Facebook]](https://www.facebook.com/help/341425252616329){target="_blank"}.

1. Hitta och välj den smarta eller statiska lista som innehåller de leads du vill skapa målgruppen från.

   ![](assets/create-a-custom-audience-in-facebook-1.png)

1. Välj fliken **[!UICONTROL Leads]** och klicka sedan på ikonen **Skicka via Lägg till Bridge** längst ned.

   ![](assets/create-a-custom-audience-in-facebook-2.png)

1. Markera **[!UICONTROL Facebook]** och klicka på **[!UICONTROL Next]**.

   ![](assets/create-a-custom-audience-in-facebook-3.png)

1. Klicka på listrutan **[!UICONTROL Audience]** och välj **[!UICONTROL + New Audience]**.

   ![](assets/create-a-custom-audience-in-facebook-4.png)

   >[!IMPORTANT]
   >
   >Facebook-API:t tillåter upp till 500 anpassade målgrupper per Facebook-annonskonto.

1. Skriv in en **[!UICONTROL Audience Name]**. Klicka på **[!UICONTROL Update]**.

   ![](assets/create-a-custom-audience-in-facebook-5.png)

   >[!NOTE]
   >
   >Om du har flera [!DNL Facebook] annonskonton visas en extra listruta där du kan välja vilket annonskonto som målgruppen har skapats i.

   >[!TIP]
   >
   >Vill du byta ut en ny publik mot en befintlig som är kopplad till en annonsuppsättning eller grupp? Markera kryssrutan **[!UICONTROL Replace an existing audience]**. Om du gör detta tas **inte** den målgrupp som ersätts bort.

1. När du är klar uppdateras statusdialogrutan.

   ![](assets/create-a-custom-audience-in-facebook-6.png)

   Och det är allt! På Facebook ser du den nya målgruppen i **Ads Manager** > **Publiker**.

   ![](assets/create-a-custom-audience-in-facebook-7.png)

   >[!NOTE]
   >
   >Alla listor som du flyttar över till [!DNL Facebook] blir statiska. Smarta listor i Marketo kommer inte att automatiskt uppdatera målgruppslistan i [!DNL Facebook] för att återspegla ändringar som gjorts efter överföringen.

   >[!MORELIKETHIS]
   >
   >[Lägg till leads till en anpassad målgrupp i [!DNL Facebook]](/help/marketo/product-docs/demand-generation/facebook/add-leads-to-a-custom-audience-in-facebook.md)
