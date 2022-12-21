---
unique-page-id: 12983101
description: Mappa anpassade fält till Marketo - Marketo Docs - produktdokumentation
title: Mappa anpassade fält till Marketo
exl-id: c52c9bcb-6448-4ebe-b87f-9e3a48e3d27d
source-git-commit: 72e1d29347bd5b77107da1e9c30169cb6490c432
workflow-type: tm+mt
source-wordcount: '258'
ht-degree: 0%

---

# Mappa anpassade fält till Marketo {#map-custom-fields-to-marketo}

Du kanske vill samla in mer än standardinformationen som Facebook lagrar som standard, till exempel hur ofta någon använder din onlinebutik. Du kan uppnå detta genom att [skapa anpassade frågor](https://www.facebook.com/business/help/774623835981457?helpref=uf_permalink) i era Facebook ledande annonser.

Men **Marketo kommer inte att börja samla in dessa data automatiskt**. För att Marketo ska kunna börja hämta anpassade fältvärden måste du **måste** mappa dessa anpassade fält till ett fält i Marketo.

Så här konfigurerar du detta i området LaunchPoint i Admin.

>[!NOTE]
>
>**Administratörsbehörigheter krävs**

1. Gå till området Admin och klicka på **LaunchPoint**. Under Installerade tjänster kan du söka efter och redigera **Facebook Lead Ads**.

   ![](assets/image2017-10-24-9-3a32-3a16.png)

1. Klicka **Nästa**.

   ![](assets/image2017-10-24-14-3a55-3a13.png)

1. Lämna det auktoriserade kontot som det är - gör **not** göra ändringar. Klicka **Nästa**.

   ![](assets/image2017-10-24-14-3a56-3a48.png)

1. Som tidigare lämnar du de markerade sidorna som de är - gör **not** göra ändringar. Klicka **Nästa**.

   ![](assets/image2017-10-24-15-3a0-3a54.png)

1. Här mappar du det anpassade Facebook-fältet till ditt Marketo-fält. Klicka **Lägg till.**

   ![](assets/image2017-10-24-9-3a33-3a49.png)

1. Ange namnet på ditt anpassade Facebook-fält på den nya raden.

   ![](assets/image2017-10-24-9-3a37-3a3.png)

   >[!NOTE]
   >
   >Endast fält som har sparats i Facebook formulärmallar visas som alternativ här.

1. Klicka på **Marketo Field** kolumn. Skriv för att söka efter fältet som du vill mappa till. När du har markerat ett fält klickar du på **Spara**.

   ![](assets/image2017-10-24-11-3a16-3a42.png)

   >[!NOTE]
   >
   >Om du inte redan har ett fält i Marketo att mappa fältet Facebook till kan du lära dig hur [skapa anpassade fält](/help/marketo/product-docs/administration/field-management/create-a-custom-field-in-marketo.md).

>[!CAUTION]
>
>Du **måste** gå igenom den här processen för alla nya fält i Facebook så att Marketo kan samla in data.
