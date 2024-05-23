---
description: Fråggenerering - Marketo Docs - produktdokumentation
title: Fråggenerering
feature: Dynamic Chat
exl-id: 05e0fd4c-b8e0-47de-8ca8-d4ba07d6a06a
source-git-commit: b2ceefb068005d916027fb71be0dc4e25849ae23
workflow-type: tm+mt
source-wordcount: '295'
ht-degree: 0%

---

# Fråggenerering {#question-generation}

Se alla dina uppgifter och relevant information, t.ex. när de skapades, det totala antalet frågor, godkännandestatus och mycket annat.

## Generera frågor {#generate-questions}

1. Under Generative AI klickar du på **[!UICONTROL Assisted responses]**.

   ![](assets/question-generation-1.png)

1. Klicka på **[!UICONTROL Generate questions]**.

   ![](assets/question-generation-2.png)

1. Ge aktiviteten ett namn och ange en käll-URL (upp till 10) från vilken allt innehåll extraheras. Ange önskade ämnen/nyckelord och tryck på Retur på tangentbordet. När du är klar klickar du **[!UICONTROL Generate]**.

   ![](assets/question-generation-3.png)

   >[!IMPORTANT]
   >
   >Om du vill vara säker på att Marketo Engage kan skrapa innehåll från de angivna URL:erna måste du först tillåtslista flera IP-adresser. [Mer information finns nedan](#ip-addresses-to-allowlist).

1. Beroende på ditt innehåll kan det ta upp till 30 minuter att generera frågor och svar. Klicka på **[!UICONTROL OK]**.

   ![](assets/question-generation-4.png)

   >[!TIP]
   >
   >Klicka på Uppdatera för att se den senaste statusen för din frågegenerering.

   ![](assets/question-generation-5.png)

## Hämta frågor och svar {#download-questions-and-responses}

>[!NOTE]
>
>Genererade frågor och svar visas också i [Svarsbibliotek](/help/marketo/product-docs/demand-generation/dynamic-chat/generative-ai/response-library.md).

1. Leta reda på önskad åtgärd och klicka på nedladdningsikonen bredvid namnet.

   ![](assets/question-generation-6.png)

1. Leta reda på hämtningsmappen i webbläsaren och markera filen. Detta kan se annorlunda ut beroende på vilken webbläsare du använder.

   ![](assets/question-generation-7.png)

1. I Excel-filen **[!DNL Task details]** visar just det, olika detaljer om uppgiften, inklusive anvisningar om hur du lägger till/redigerar frågor och/eller svar.

   ![](assets/question-generation-8.png)

   >[!NOTE]
   >
   >Om du bestämmer dig för att lägga till/redigera frågor och/eller svar gruppvis, [lära dig hur du överför dem igen här](/help/marketo/product-docs/demand-generation/dynamic-chat/generative-ai/response-library.md).

1. The **[!DNL Q&Rs]** På -fliken finns ytterligare information, bland annat frågor och svar som genererats.

   ![](assets/question-generation-9.png)

## IP-adresser att Tillåtslista {#ip-addresses-to-allowlist}

Om du vill kunna extrahera innehåll från dina webb-URL:er under genereringen av frågor och svar, ska du leta reda på din region nedan och se till att alla IP-adresser som är kopplade till den är tillåtslista av ditt webbteam.

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
    <td>20.10.235.188</td>
    <td>20.76.246.248</td>
    <td>20.167.0.195</td>
  </tr>
  <tr>
    <td>20.10.235.189</td>
    <td>20.76.247.92</td>
    <td>20.248.128.31</td>
  </tr>
  <tr>
    <td>20.10.235.246</td>
    <td>20.76.247.134</td>
    <td>20.167.1.48</td>
  </tr>
  <tr>
    <td>20.10.235.248</td>
    <td>20.76.247.244</td>
    <td>20.167.1.63</td>
  </tr>
  <tr>
    <td>20.10.235.255</td>
    <td>20.93.168.10</td>
    <td>20.167.1.92</td>
  </tr>
  <tr>
    <td>20.10.236.96</td>
    <td>20.93.168.44</td>
    <td>20.167.1.155</td>
  </tr>
  <tr>
    <td>20.119.144.14</td>
    <td>20.105.224.16</td>
    <td>20.211.64.11</td>
  </tr>
  <tr>
    <td>13.68.17.252</td>
    <td>20.105.150.224</td>
    <td>20.213.91.77</td>
  </tr>
</tbody>
</table>
