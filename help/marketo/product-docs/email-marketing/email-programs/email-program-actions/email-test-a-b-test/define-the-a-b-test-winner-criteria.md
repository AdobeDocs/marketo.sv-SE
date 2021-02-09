---
unique-page-id: 2359545
description: Definiera A/B Test Winner Criteria - Marketo Docs - Product Documentation
title: Definiera villkor för A/B-testvinnare
translation-type: tm+mt
source-git-commit: 8d45a28e1c2adad3e04645f7150f1757414092f0
workflow-type: tm+mt
source-wordcount: '401'
ht-degree: 0%

---


# Definiera A/B-test för vinnarvillkor {#define-the-a-b-test-winner-criteria}

När [du lägger till ett A/B-test](/help/marketo/product-docs/email-marketing/email-programs/email-program-actions/email-test-a-b-test/add-an-a-b-test.md) i ditt e-postprogram måste du välja en testtyp, [schemalägga A/B-testet](/help/marketo/product-docs/email-marketing/email-programs/email-program-actions/email-test-a-b-test/schedule-the-a-b-test.md) och sedan definiera vinnarvillkoren. Så här avgör du vilket e-postmeddelande som vinner.

>[!PREREQUISITES]
>
>[Lägg till ett A/B-test](/help/marketo/product-docs/email-marketing/email-programs/email-program-actions/email-test-a-b-test/add-an-a-b-test.md)

## Vinnarvillkor {#winner-criteria}

1. Standardalternativen för **Vinnarvillkor** visas först.

   ![](assets/image2014-9-12-15-3a51-3a3.png)

   | **Öppnar** | En öppen registrerar när bilder hämtas till ett e-postmeddelande. Även om du inte inkluderar en bild infogar Marketo som standard en enda spårningspixel i alla HTML-e-postmeddelanden. |
   |---|---|
   | **Klickningar** | Som standard är länkar i e-postmeddelanden inbäddade i spårning, vilket gör att du kan se vem som klickade på länken, hur många länkar som klickades osv. |
   | **Klicka för att öppna %** | Procentandel e-postmeddelanden som öppnades och där en länk klickades i e-postmeddelandet. Detta mäter relevansen och sammanhanget för ett e-postmeddelande genom att ta antalet unika klick dividerat med antalet unika öppningar och sedan multiplicera med 100 för att visa det som en procentandel. |
   | **Engagement Score** | Med [engagemangspoängen](/help/marketo/product-docs/email-marketing/drip-nurturing/reports-and-notifications/understanding-the-engagement-score.md) kan du avgöra hur effektivt ditt innehåll är. |

   >[!TIP]
   >
   >Om du väljer Engagement Score måste testet köras i minst 24 timmar. Läs mer om [att förstå engagemangspoängen](/help/marketo/product-docs/email-marketing/drip-nurturing/reports-and-notifications/understanding-the-engagement-score.md).

1. Du kan också anpassa villkoren genom att välja Anpassad konvertering och klicka på Redigera.

   ![](assets/image2014-9-12-15-3a51-3a53.png)

   >[!NOTE]
   >
   >Med anpassad konvertering kan du välja vilken händelse som helst som en konvertering genom att använda utlösare och filter.

1. Ett fönster öppnas. Hitta den utlösare du vill ha och dra den till arbetsytan.

   ![](assets/image2014-9-12-15-3a52-3a18.png)

1. Definiera utlösaren.

   ![](assets/image2014-9-12-15-3a53-3a11.png)

   >[!NOTE]
   >
   >Marketo tillåter endast utlösare för personer som har fått e-postmeddelandet från det här e-postprogrammet. Du behöver inte lägga till filtret&quot;Skickat e-post&quot;.

1. Klicka på **Stäng**.

   ![](assets/image2014-9-12-15-3a53-3a36.png)

   Bra! Nu är det dags att bestämma hur vinnaren ska vara bestämd.

## Deklarera vinnare {#declare-winner}

1. Välj ett av de två tillgängliga alternativen.

   ![](assets/image2014-9-12-15-3a53-3a44.png)

   >[!NOTE]
   >
   >Om du gör ett **datum/tid** A/B-test kan du bara välja **Manuell**.

   När A/B-testet är klart kan Marketo automatiskt skicka det vinnande e-postmeddelandet vid den schemalagda tidpunkten, eller så kan du granska resultatet och bestämma när e-postmeddelandet ska skickas.

1. Automatiskt är grymt och är standardalternativet. Klicka bara på **Nästa**.

   ![](assets/image2014-9-12-15-3a54-3a35.png)

   >[!TIP]
   >
   >Om du väljer **Manuell** skickas testet ut och du väntar på att du ska deklarera en vinnare. Du får en rapport över resultaten.

Perfekt! Nu ska vi [schemalägga A/B-testet](/help/marketo/product-docs/email-marketing/email-programs/email-program-actions/email-test-a-b-test/schedule-the-a-b-test.md).
