---
unique-page-id: 2360360
description: Skapa en webkrok - Marketo Docs - produktdokumentation
title: Skapa en webbkrok
exl-id: 3e753d2d-6f33-4987-884e-8e13167cf3df
source-git-commit: 25a574719eb6c064d33b6a1cebafe2668ed1330d
workflow-type: tm+mt
source-wordcount: '209'
ht-degree: 0%

---

# Skapa en webbkrok {#create-a-webhook}

Använd webhooks för att dra nytta av webbtjänster från tredje part för att skicka textmeddelanden, utöka persondata med mera.

>[!AVAILABILITY]
>
>Alla kunder har inte köpt den här funktionen. Kontakta din säljare för mer information.

1. Gå till **Administratör** och klicka **Webhooks**.

   ![](assets/image2014-9-24-14-3a52-3a57.png)

1. Klicka **Ny webkrok**.

   ![](assets/image2014-9-24-14-3a53-3a9.png)

1. Namnge och konfigurera din webkrok.

   ![](assets/image2014-9-24-14-3a53-3a19.png)

   >[!NOTE]
   >
   >Detta inkluderar ofta att du anger dina inloggningsuppgifter för en tredjepartstjänst som en URL-parameter eller i POSTEN.

   * **URL**: Ange den URL som du använder i din begäran till webbtjänsten. Så här infogar du en token, t.ex. personens e-postadress (**`{{lead.Email Address}}`**), klickar du på **Infoga token**.

   * **Mall**: Om du vill skicka information i POSTENS brödtext anger du mallen. Använd valfritt dataformat som stöder HTTP-POST, inklusive XML, JSON eller SOAP. Om du vill infoga en variabel i mallen klickar du på **Infoga token**.

   * **Begär tokenkodning**: Om tokenvärdena innehåller specialtecken (t.ex. ett et-tecken, &#39;&amp;&#39;), anger du formatet för din begäran (**JSON** eller **Formulär/URL**).

   * **Svarstyp**: Välj formatet för det svar du får från tjänsten (**JSON** eller **XML**).

   * **Typ av begäran**: Välj den HTTP-metod som ska användas (DELETE, GET, PATCH, POST, PUT).

   Klicka **Skapa**.

   ![](assets/image2014-9-24-14-3a53-3a35.png)

>[!NOTE]
>
>Läs mer i [webhooks](https://developers.marketo.com/documentation/webhooks/) Djupdykning.
