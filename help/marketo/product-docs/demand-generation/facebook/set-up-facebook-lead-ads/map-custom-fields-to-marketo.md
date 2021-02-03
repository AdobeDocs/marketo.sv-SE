---
unique-page-id: 12983101
description: Mappa anpassade fält till Marketo - Marketo Docs - Produktdokumentation
title: Mappa anpassade fält till markering
translation-type: tm+mt
source-git-commit: ed83438ae5660d172e845f25c4d72d599574bd91
workflow-type: tm+mt
source-wordcount: '258'
ht-degree: 0%

---


# Mappa anpassade fält till markering {#map-custom-fields-to-marketo}

Du kanske vill samla in mer än standardinformationen som lagras på Facebook som standard, till exempel hur ofta någon använder din onlinetjänst. Du kan uppnå detta genom att [skapa anpassade frågor](https://www.facebook.com/business/help/774623835981457?helpref=uf_permalink) i dina Facebook-annonser.

Men **Marketo börjar inte automatiskt samla in dessa data**. För att Marketo ska kunna börja hämta anpassade fältvärden måste du **mappa dessa anpassade fält till ett fält i Marketo.**

Så här konfigurerar du detta i området LaunchPoint i Admin.

>[!NOTE]
>
>**Administratörsbehörigheter krävs**

1. Gå till området Admin och klicka på **LaunchPoint**. Under Installerade tjänster kan du söka efter och redigera **Facebook-annonser**.

   ![](assets/image2017-10-24-9-3a32-3a16.png)

1. Klicka på **Nästa**.

   ![](assets/image2017-10-24-14-3a55-3a13.png)

1. Låt det behöriga kontot vara som det är - gör **inte** några ändringar. Klicka på **Nästa**.

   ![](assets/image2017-10-24-14-3a56-3a48.png)

1. Som tidigare lämnar du de markerade sidorna som de är - gör **inte** några ändringar. Klicka på **Nästa**.

   ![](assets/image2017-10-24-15-3a0-3a54.png)

1. Här mappar du det anpassade Facebook-fältet till ditt Marketo-fält. Klicka på **Lägg till.**

   ![](assets/image2017-10-24-9-3a33-3a49.png)

1. Ange namnet på det anpassade Facebook-fältet på den nya raden.

   ![](assets/image2017-10-24-9-3a37-3a3.png)

   >[!NOTE]
   >
   >Endast fält som har sparats i Facebook-formulärmallar visas som alternativ här.

1. Klicka i kolumnen **Marketo-fält**. Skriv för att söka efter fältet som du vill mappa till. När du har markerat ett fält klickar du på **Spara**.

   ![](assets/image2017-10-24-11-3a16-3a42.png)

   >[!NOTE]
   >
   >Om du inte redan har ett fält i Marketo att mappa Facebook-fältet till, lär du dig hur du [skapar anpassade fält](/help/marketo/product-docs/administration/field-management/create-a-custom-field-in-marketo.md).

>[!CAUTION]
>
>Du **måste** gå igenom den här processen för alla nya Facebook-fält för att Marketo ska kunna samla in data.
