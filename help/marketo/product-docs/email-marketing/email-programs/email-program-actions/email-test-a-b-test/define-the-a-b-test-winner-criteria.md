---
unique-page-id: 2359545
description: Definiera A/B Test Winner Criteria - Marketo Docs - Product Documentation
title: Definiera villkor för A/B-testvinnare
exl-id: be8a0887-70f4-4667-93a6-d982a16cdfdb
feature: Email Programs, A/B Testing
source-git-commit: d20a9bb584f69282eefae3704ce4be2179b29d0b
workflow-type: tm+mt
source-wordcount: '412'
ht-degree: 0%

---

# Definiera villkor för A/B-testvinnare {#define-the-a-b-test-winner-criteria}

När [lägga till ett A/B-test](/help/marketo/product-docs/email-marketing/email-programs/email-program-actions/email-test-a-b-test/add-an-a-b-test.md){target="_blank"} to your email program, you will need to pick a test type, [schedule the A/B test](/help/marketo/product-docs/email-marketing/email-programs/email-program-actions/email-test-a-b-test/schedule-the-a-b-test.md){target="_blank"}definierar sedan vinnarkriterierna. Så här avgör du vilket e-postmeddelande som vinner.

>[!PREREQUISITES]
>
>[Lägg till ett A/B-test](/help/marketo/product-docs/email-marketing/email-programs/email-program-actions/email-test-a-b-test/add-an-a-b-test.md){target="_blank"}

## Vinnarvillkor {#winner-criteria}

1. Standardvärdet **Vinnarvillkor** visas först.

   ![](assets/image2014-9-12-15-3a51-3a3.png)

   <table>
   <tr>
   <td><b>Öppnar</b></td>
   <td>En öppen registrerar när bilder hämtas till ett e-postmeddelande. Även om du inte inkluderar någon bild infogar Marketo som standard en enda spårningspixel i alla HTML-e-postmeddelanden.</td>
   </tr>
   <tr>
   <td><b>Klickningar</b></td>
   <td>Som standard är länkar i e-postmeddelanden inbäddade i att du kan se vem som klickade på länken, hur många länkar som klickades osv.</td>
   </tr>
   <tr>
   <td><b>Klicka för att öppna %</b></td>
   <td>Procentandel e-postmeddelanden som öppnades och där en länk klickades i e-postmeddelandet. Detta mäter relevansen och sammanhanget för ett e-postmeddelande genom att ta antalet unika klick dividerat med antalet unika öppningar och sedan multiplicera med 100 för att visa det som en procentandel.</td>
   </tr>
   <tr>
   <td><b>Engagement Score</b></td>
   <td>The <a href="https://experienceleague.adobe.com/docs/marketo/using/product-docs/email-marketing/drip-nurturing/reports-and-notifications/understanding-the-engagement-score.html" target="_blank">engagemangspoäng</a> hjälper er att avgöra hur effektivt ert innehåll är.</td>
   </tr>
   </table>

   >[!TIP]
   >
   >Om du väljer Engagement Score måste testet köras i minst 24 timmar. Läs mer om [förstå engagemangsmomentet](/help/marketo/product-docs/email-marketing/drip-nurturing/reports-and-notifications/understanding-the-engagement-score.md){target="_blank"}.

1. Du kan också anpassa villkoren genom att välja Anpassad konvertering och klicka på Redigera.

   ![](assets/image2014-9-12-15-3a51-3a53.png)

   >[!NOTE]
   >
   >Med anpassad konvertering kan du välja vilken händelse som helst som en konvertering genom att använda utlösare och filter.

1. Ett fönster öppnas. Hitta den utlösare du vill ha och dra den till arbetsytan.

   ![](assets/image2014-9-12-15-3a52-3a18.png)

1. Definiera utlösaren.

   ![](assets/image2014-9-12-15-3a53-3a11.png)

   >[!IMPORTANT]
   >
   >Marketo tillåter bara utlösare/filter för personer som har fått e-postmeddelandet från det här e-postprogrammet, så du behöver inte lägga till filtret&quot;Har skickats e-post&quot;. När du använder en e-postrelaterad utlösare/filter måste du dessutom se till att&quot;är någon&quot; som operator.

1. Klicka **Stäng**.

   ![](assets/image2014-9-12-15-3a53-3a36.png)

   Bra! Nu är det dags att bestämma hur vinnaren ska vara bestämd.

## Deklarera vinnare {#declare-winner}

1. Välj ett av de två tillgängliga alternativen.

   ![](assets/image2014-9-12-15-3a53-3a44.png)

   >[!NOTE]
   >
   >Om du gör en **Datum/tid** A/B-test, du kan bara välja **Manuell**.

   När A/B-testet är klart kan Marketo automatiskt skicka det vinnande e-postmeddelandet vid den schemalagda tidpunkten, eller så kan du granska resultatet och bestämma när e-postmeddelandet ska skickas.

1. Automatiskt är grymt och är standardalternativet. Klicka bara **Nästa**.

   ![](assets/image2014-9-12-15-3a54-3a35.png)

   >[!TIP]
   >
   >Välja **Manuell** skickar ut testet och väntar på att du ska utnämna en vinnare. Du får en rapport över resultaten.

Perfekt! Nu ska vi [schemalägg A/B-testet](/help/marketo/product-docs/email-marketing/email-programs/email-program-actions/email-test-a-b-test/schedule-the-a-b-test.md){target="_blank"}.
