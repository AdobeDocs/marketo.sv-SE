---
unique-page-id: 12983101
description: Mappa anpassade fält till Marketo - Marketo Docs - produktdokumentation
title: Mappa anpassade fält till Marketo
exl-id: c52c9bcb-6448-4ebe-b87f-9e3a48e3d27d
feature: Integrations
source-git-commit: 09a656c3a0d0002edfa1a61b987bff4c1dff33cf
workflow-type: tm+mt
source-wordcount: '234'
ht-degree: 1%

---

# Mappa anpassade fält till Marketo {#map-custom-fields-to-marketo}

Du kanske vill samla in mer än standardinformationen som lagras i [!DNL Facebook] som standard, till exempel hur ofta någon använder din onlineleveranstjänst. Du kan uppnå detta genom att [skapa anpassade frågor](https://www.facebook.com/business/help/774623835981457?helpref=uf_permalink) i dina [!DNL Facebook] leads-annonser.

**Marketo börjar dock inte automatiskt samla in dessa data**. Om du vill att Marketo ska kunna börja hämta anpassade fältvärden måste **du** mappa dessa anpassade fält till ett fält i Marketo.

Så här konfigurerar du detta i området LaunchPoint i Admin.

>[!NOTE]
>
>**Administratörsbehörigheter krävs**

1. Gå till området Admin och klicka på **[!UICONTROL LaunchPoint]**. Sök efter och redigera **[!UICONTROL Facebook Lead Ads]** under Installerade tjänster.

   ![](assets/image2017-10-24-9-3a32-3a16.png)

1. Klicka på **[!UICONTROL Next]**.

   ![](assets/image2017-10-24-14-3a55-3a13.png)

1. Lämna det auktoriserade kontot som det är - gör **inga** ändringar. Klicka på **[!UICONTROL Next]**.

   ![](assets/image2017-10-24-14-3a56-3a48.png)

1. Som tidigare lämnar du de markerade sidorna som de är - gör **inga** ändringar. Klicka på **[!UICONTROL Next]**.

   ![](assets/image2017-10-24-15-3a0-3a54.png)

1. Här mappar du det anpassade fältet [!DNL Facebook] till ditt Marketo-fält. Klicka på **[!UICONTROL Add].**

   ![](assets/image2017-10-24-9-3a33-3a49.png)

1. Ange namnet på det anpassade fältet [!DNL Facebook] på den nya raden.

   ![](assets/image2017-10-24-9-3a37-3a3.png)

   >[!NOTE]
   >
   >Endast fält som har sparats i [!DNL Facebook] formulärmallar visas som alternativ här.

1. Klicka i kolumnen **[!UICONTROL Marketo Field]**. Skriv för att söka efter fältet som du vill mappa till. När du har markerat ett fält klickar du på **[!UICONTROL Save]**.

   ![](assets/image2017-10-24-11-3a16-3a42.png)

   >[!NOTE]
   >
   >Om du inte redan har ett fält i Marketo att mappa fältet [!DNL Facebook] till kan du lära dig hur du [skapar anpassade fält](/help/marketo/product-docs/administration/field-management/create-a-custom-field-in-marketo.md).

>[!CAUTION]
>
>Du **måste** gå igenom den här processen för alla nya [!DNL Facebook]-fält för att Marketo ska kunna samla in data.
