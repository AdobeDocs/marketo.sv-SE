---
description: Fråggenerering - Marketo Docs - produktdokumentation
title: Fråggenerering
feature: Dynamic Chat
exl-id: 05e0fd4c-b8e0-47de-8ca8-d4ba07d6a06a
source-git-commit: 09a656c3a0d0002edfa1a61b987bff4c1dff33cf
workflow-type: tm+mt
source-wordcount: '292'
ht-degree: 0%

---

# Fråggenerering {#question-generation}

Se alla dina uppgifter och relevant information, t.ex. när de skapades, det totala antalet frågor, godkännandestatus och mycket annat.

## Generera frågor {#generate-questions}

1. Klicka på **[!UICONTROL Assisted responses]** under Generativ AI.

   ![](assets/question-generation-1.png)

1. Klicka på **[!UICONTROL Generate questions]**.

   ![](assets/question-generation-2.png)

1. Ge aktiviteten ett namn och ange en käll-URL (upp till 10) från vilken allt innehåll extraheras. Ange önskade ämnen/nyckelord och tryck på Retur på tangentbordet. När du är klar klickar du på **[!UICONTROL Generate]**.

   ![](assets/question-generation-3.png)

   >[!IMPORTANT]
   >
   >Om du vill vara säker på att Marketo Engage kan skrapa innehåll från de angivna URL:erna måste du först tillåtslista flera IP-adresser. [Se nedan för mer information](#ip-addresses-to-allowlist).

   >[!NOTE]
   >
   >Webbplatser/sidor måste vara offentliga (dvs. inte dolda bakom en inloggning) för att deras information ska kunna rensas.

1. Beroende på ditt innehåll kan det ta upp till 30 minuter att generera frågor och svar. Klicka på **[!UICONTROL OK]**.

   ![](assets/question-generation-4.png)

   >[!TIP]
   >
   >Klicka på Uppdatera för att se den senaste statusen för din frågegenerering.

   ![](assets/question-generation-5.png)

## Hämta frågor och svar {#download-questions-and-responses}

>[!NOTE]
>
>Genererade frågor och svar kan också visas i [svarsbiblioteket](/help/marketo/product-docs/demand-generation/dynamic-chat/generative-ai/response-library.md).

1. Leta reda på önskad åtgärd och klicka på nedladdningsikonen bredvid namnet.

   ![](assets/question-generation-6.png)

1. Leta reda på hämtningsmappen i webbläsaren och markera filen. Detta kan se annorlunda ut beroende på vilken webbläsare du använder.

   ![](assets/question-generation-7.png)

1. I Excel-filen visar **[!DNL Task details]** bara den informationen om uppgiften, inklusive instruktioner om hur du lägger till/redigerar frågor och/eller svar.

   ![](assets/question-generation-8.png)

   >[!NOTE]
   >
   >Om du bestämmer dig för att lägga till/redigera frågor och/eller svar gruppvis, [lär dig hur du överför dem hit](/help/marketo/product-docs/demand-generation/dynamic-chat/generative-ai/response-library.md).

1. Fliken **[!DNL Q&Rs]** innehåller ytterligare information, inklusive de frågor och svar som genererats.

   ![](assets/question-generation-9.png)

## IP-adresser att Tillåtslista {#ip-addresses-to-allowlist}

Om du vill kunna extrahera innehåll från dina webb-URL:er under genereringen av frågor och svar ska du leta reda på din region nedan och se till att den IP-adress som är associerad med den är tillåtslista av ditt webbteam.

<table width="450">
<thead>
  <tr>
    <th>Nordamerika</th>
    <th>Europa</th>
    <th>APAC</th>
  </tr>
</thead>
<tbody>
  <tr>
    <td>13.68.17.252</td>
    <td>20.105.150.224</td>
    <td>20.213.91.77</td>
  </tr>
</tbody>
</table>
