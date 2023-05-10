---
unique-page-id: 2360360
description: Skapa en webkrok - Marketo Docs - produktdokumentation
title: Skapa en webbkrok
exl-id: 3e753d2d-6f33-4987-884e-8e13167cf3df
source-git-commit: a498dcc5dc95bd7f732481d30db021485cf052c0
workflow-type: tm+mt
source-wordcount: '221'
ht-degree: 0%

---

# Skapa en webbkrok {#create-a-webhook}

Använd webhooks för att dra nytta av webbtjänster från tredje part för att skicka textmeddelanden, utöka persondata med mera.

>[!AVAILABILITY]
>
>Alla kunder har inte köpt den här funktionen. Kontakta din säljare för mer information.

1. Gå till **Administratör** område.

   ![](assets/create-a-webhook-1.png)

1. Klicka **Webhooks**.

   ![](assets/create-a-webhook-2.png)

1. Klicka **Ny webkrok**.

   ![](assets/create-a-webhook-3.png)

1. Namnge och konfigurera din webkrok.

   ![](assets/create-a-webhook-4.png)

   >[!NOTE]
   >
   >Detta inkluderar ofta att du anger dina inloggningsuppgifter för en tredjepartstjänst som en URL-parameter eller i POSTEN.

   * **URL**: Ange den URL som du använder i din begäran till webbtjänsten. Så här infogar du en token, t.ex. personens e-postadress (**`{{lead.Email Address}}`**), klickar du på **Infoga token**.

   * **Mall**: Om du vill skicka information i texten i begäran anger du det via nyttolastmallen. Mallar tillåts för följande typer av begäranden: POST, DELETE, PATCH eller PUT. Du kan använda dataformat som JSON eller XML. Om du vill infoga en variabel i mallen klickar du på **Infoga token**.

   * **Begär tokenkodning**: Om tokenvärdena innehåller specialtecken (t.ex. ett et-tecken, &#39;&amp;&#39;), anger du formatet för din begäran (**JSON** eller **Formulär/URL**).

   * **Svarstyp**: Välj formatet för det svar du får från tjänsten (**JSON** eller **XML**).

   * **Typ av begäran**: Välj den HTTP-metod som ska användas (DELETE, GET, PATCH, POST, PUT).

1. Klicka **Skapa**.

   ![](assets/create-a-webhook-5.png)

>[!NOTE]
>
>Läs mer i [webhooks](https://developers.marketo.com/documentation/webhooks/) Djupdykning.
