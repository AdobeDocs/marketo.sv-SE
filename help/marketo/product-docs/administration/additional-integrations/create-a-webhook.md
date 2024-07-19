---
unique-page-id: 2360360
description: Skapa en [!DNL Webhook] - Marketo Docs - produktdokumentation
title: Skapa en  [!DNL Webhook]
exl-id: 3e753d2d-6f33-4987-884e-8e13167cf3df
feature: Administration, Webhooks
source-git-commit: 23a7b8cb1cd07c0194c08d30218602a52d03df5b
workflow-type: tm+mt
source-wordcount: '181'
ht-degree: 1%

---

# Skapa en [!DNL Webhook] {#create-a-webhook}

Använd [!DNL Webhooks] om du vill dra nytta av webbtjänster från tredje part för att skicka textmeddelanden, utöka persondata och mycket mer.

1. Gå till området **[!UICONTROL Admin]**.

   ![](assets/create-a-webhook-1.png)

1. Klicka på **[!UICONTROL Webhooks]**.

   ![](assets/create-a-webhook-2.png)

1. Klicka på **[!UICONTROL New Webhook]**.

   ![](assets/create-a-webhook-3.png)

1. Namnge och konfigurera [!DNL Webhook].

   ![](assets/create-a-webhook-4.png)

   >[!NOTE]
   >
   >Detta inkluderar ofta att du anger dina inloggningsuppgifter för en tredjepartstjänst som en URL-parameter eller i POSTEN.

   * **[!UICONTROL URL]**: Ange den URL som du använder i din begäran till webbtjänsten. Om du vill infoga en token, till exempel personens e-postadress (**`{{lead.Email Address}}`**), klickar du på **[!UICONTROL Insert Token]** i din begäran.

   * **[!UICONTROL Template]**: Om du vill överföra information i begärans innehåll anger du det via nyttolastmallen. Mallar tillåts för följande typer av begäranden: POST, DELETE, PATCH eller PUT. Du kan använda dataformat som JSON eller XML. Om du vill infoga en token i mallen klickar du på **[!UICONTROL Insert Token]**.

   * **[!UICONTROL Request Token Encoding]**: Om tokenvärdena innehåller specialtecken (t.ex. ett et-tecken (&amp;)) anger du formatet för din begäran (**JSON** eller **Form/Url**).

   * **[!UICONTROL Response type]**: Välj formatet för det svar du får från tjänsten (**JSON** eller **XML**).

   * **[!UICONTROL Request Type]**: Välj den HTTP-metod som ska användas (DELETE, GET, PATCH, POST, PUT).

1. Klicka på **[!UICONTROL Create]**.

   ![](assets/create-a-webhook-5.png)

>[!NOTE]
>
>Läs mer i djupdykningen [[!DNL Webhooks]](https://experienceleague.adobe.com/en/docs/marketo-developer/marketo/webhooks/webhooks){target="_blank"}.
