---
description: Konfigurera ON24-integrering med Marketo - Marketo Docs - produktdokumentation
title: Konfigurera ON24-integreringen med Marketo
exl-id: 395ffa37-b87d-4eb4-bf9f-72aa96dc819c
feature: Events
source-git-commit: e3f61755dccd9bea1378a429fc428b440fc3ecb4
workflow-type: tm+mt
source-wordcount: '263'
ht-degree: 0%

---

# Konfigurera ON24-integreringen med Marketo{#set-up-the-on24-integration-with-marketo}

Så här konfigurerar du din ON24-händelseintegrering.

## Skapa en roll enbart för API {#create-an-api-only-role}

1. Klicka på **Admin** i Min Marketo.

   ![](assets/set-up-the-on24-integration-with-marketo-1.png)

1. Klicka på **Användare och roller** under Säkerhet.

   ![](assets/set-up-the-on24-integration-with-marketo-2.png)

1. Klicka på fliken **Roller** och sedan på **Ny roll**.

   ![](assets/set-up-the-on24-integration-with-marketo-3.png)

1. Ange ett rollnamn. Öppna menyn **Åtkomst-API** och välj&quot;Read-Write Custom Object&quot; och&quot;Read-Write Person&quot;. Klicka på **Skapa**.

   ![](assets/set-up-the-on24-integration-with-marketo-4.png)

## Skapa en ny användare {#create-a-new-user}

1. Klicka på fliken **Användare** och sedan på **Bjud in ny användare** i Användare och roller.

   ![](assets/set-up-the-on24-integration-with-marketo-5.png)

1. Ange den nya användarens information och klicka på **Nästa**.

   ![](assets/set-up-the-on24-integration-with-marketo-6.png)

1. Välj den roll för endast ON24 API som du nyss skapade. Markera kryssrutan **Endast API**. Klicka på **Nästa**.

   ![](assets/set-up-the-on24-integration-with-marketo-7.png)

1. Klicka på **Skicka**.

   ![](assets/set-up-the-on24-integration-with-marketo-8.png)

>[!NOTE]
>
>Ingen inbjudan krävs för användare med endast API.

## Konfigurera ON24-anslutning {#set-up-on24-connection}

1. Klicka på **LaunchPoint** i administratörsavsnittet.

   ![](assets/set-up-the-on24-integration-with-marketo-9.png)

1. Klicka på **Ny** och sedan på **Ny tjänst**.

   ![](assets/set-up-the-on24-integration-with-marketo-10.png)

1. Välj ett visningsnamn. Klicka på listrutan **Tjänst** och välj **Egen**. Ange en beskrivning. Klicka på listrutan Endast API-användare och välj den användare som du skapade [ i stegen ovan](#create-a-new-user). Klicka på **Skapa**.

   ![](assets/set-up-the-on24-integration-with-marketo-11.png)

1. Hitta den anpassade LaunchPoint-tjänst som du just skapade och klicka på Visa detaljer.

   ![](assets/set-up-the-on24-integration-with-marketo-12.png)

1. Markera, högerklicka, kopiera och spara klient-ID:t (du behöver det senare). Upprepa för Klienthemlighet.

   ![](assets/set-up-the-on24-integration-with-marketo-13.png)

1. Klicka på Webbtjänster i trädet till vänster.

   ![](assets/set-up-the-on24-integration-with-marketo-14.png)

1. Under REST API markerar du, högerklickar, kopierar och sparar den första delen av Identity (fram till &#39;m&#39; på .com).

   ![](assets/set-up-the-on24-integration-with-marketo-15.png)

1. Navigera med ditt sparade klient-ID, klienthemlighet och identitet till ditt ON24-konto. Resten av stegen utförs där och finns i [ON24-dokumentationen](https://support.on24.com/hc/en-us/articles/21420762650523-Data-Integration-Setup-Instructions-When-Using-Marketo-Registration-Option-1){target="_blank"}.
