---
description: Lägg till inställningen för att avbryta prenumerationen - Marketo Docs - Produktdokumentation
title: Lägg till inställningen för att avbryta prenumerationen
feature: Marketo Sales Connect
exl-id: 8aa75123-f6b5-4dfe-8fa7-f764620c04e8
source-git-commit: 26573c20c411208e5a01aa7ec73a97e7208b35d5
workflow-type: tm+mt
source-wordcount: '198'
ht-degree: 0%

---

# Lägg till inställningen för att avbryta prenumerationen {#auto-append-unsubscribe-message-setting}

Kontrollera att alla skickade e-postmeddelanden innehåller ett meddelande om att prenumerationen har avbrutits så att mottagarna enkelt kan välja att inte kommunicera. När ett meddelande om att avbeställa prenumerationen är aktiverat kommer all kommunikation som teamet skickar från Marketo Sales att innehålla ett meddelande om att avbeställa prenumerationen, inklusive e-post som skickas från webbprogrammet, Salesforce, plugin-programmet Gmail samt Outlook-pluginprogrammet.

## Saker att notera {#things-to-note}

* För e-postmeddelanden som skickas från plugin-programmen läggs prenumerationen bara till när en mall används.

* Om du använder det dynamiska fältet `{{team_unsubscribe}}` i en e-postmall och inställningen för att avsluta prenumerationen är aktiverad, kommer det dynamiska fältet för att avsluta prenumerationen att fylla i ditt meddelande _i stället för_ som läggs till i ditt meddelande om att prenumerationen har avbrutits.

## Aktivera/inaktivera Lägg till för avbeställning {#enable-disable-unsubscribe-append}

1. Klicka på kugghjulsikonen och välj **Inställningar**.

   ![](assets/auto-append-unsubscribe-message-setting-1.png)

1. Klicka på **Avsluta prenumeration** under Administratörsinställningar.

   ![](assets/auto-append-unsubscribe-message-setting-2.png)

1. Gå till fliken Meddelanden under Lägg till meddelande om prenumerationsuppgift och flytta reglaget till önskat läge.

   ![](assets/auto-append-unsubscribe-message-setting-3.png)

>[!TIP]
>
>Om du inaktiverar inställningen för att avsluta prenumerationen rekommenderar vi att du lägger till en sidfot för att avbryta prenumerationen i mallarna så att du är säker på att din kommunikation har ett avanmälningsalternativ. Du kan göra detta genom att lägga till ett eget anpassat meddelande till varje mall eller genom att använda det `{{team_unsubscribe}}` [dynamiska fältet](/help/marketo/product-docs/marketo-sales-connect/templates/dynamic-fields/dynamic-fields-glossary.md){target="_blank"}.
