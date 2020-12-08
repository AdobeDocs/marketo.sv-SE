---
unique-page-id: 2360360
description: Skapa en webkrok - Marketo Docs - Produktdokumentation
title: Skapa en webbkrok
translation-type: tm+mt
source-git-commit: 5c9683c6b00ccbf9e9d606fd4513432c9872ad00
workflow-type: tm+mt
source-wordcount: '251'
ht-degree: 0%

---


# Skapa en webbkrok {#create-a-webhook}

>[!NOTE]
>
>**FYI**
>
>Marketo standardiserar nu språk för alla prenumerationer, så du kan se lead/leads i din prenumeration och person/personer på docs.marketo.com. Dessa termer betyder samma sak. det påverkar inte artikelinstruktionerna. Det finns andra förändringar också. [Läs mer](http://docs.marketo.com/display/DOCS/Updates+to+Marketo+Terminology).

Använd webhooks för att dra nytta av webbtjänster från tredje part för att skicka textmeddelanden, utöka persondata med mera.

>[!NOTE]
>
>**Tillgänglighet**
>
>Alla kunder har inte köpt den här funktionen. Kontakta din säljare för mer information.

1. Gå till **Admin **och klicka på **Webhooks**.

   ![](assets/image2014-9-24-14-3a52-3a57.png)

1. Klicka på **Ny webkrok**.

   ![](assets/image2014-9-24-14-3a53-3a9.png)

1. Namnge och konfigurera din webkrok.

   ![](assets/image2014-9-24-14-3a53-3a19.png)

   >[!NOTE]
   >
   >Detta inkluderar ofta att du anger dina inloggningsuppgifter för en tredjepartstjänst som en URL-parameter eller i POSTEN.

   * **URL**: Ange den URL som du använder för att POST din förfrågan till webbtjänsten. Om du vill infoga en token, t.ex. personens e-postadress (**`{{lead.Email Address}}`**), klickar du på **Infoga token** i din begäran.

   * **Mall**: Om du vill skicka information i POSTENS brödtext anger du mallen. Använd valfritt dataformat som stöder HTTP-POST, inklusive XML, JSON eller SOAP. Om du vill infoga en token i mallen klickar du på **Infoga token**.

   * **Begär tokenkodning**: Om tokenvärdena innehåller specialtecken (t.ex. ett et-tecken (&amp;)) anger du formatet för din begäran (**JSON** eller **Form/Url**).

   * **Svarstyp**: Välj formatet för det svar du får från tjänsten (**JSON** eller **XML**).

   Klicka på Skapa.

   ![](assets/image2014-9-24-14-3a53-3a35.png)

>[!NOTE]
>
>**Djupdykning**
>
>Läs mer i [webhookarnas](http://developers.marketo.com/documentation/webhooks/) djupdykning.

