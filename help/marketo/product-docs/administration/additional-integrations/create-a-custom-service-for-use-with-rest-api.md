---
unique-page-id: 2360350
description: Skapa en anpassad tjänst för användning med ReST API - Marketo Docs - produktdokumentation
title: Skapa en anpassad tjänst för användning med ReST API
exl-id: d94f723b-2e98-4350-a9e5-bd57aff2303b
feature: Administration
source-git-commit: 2b610cc3486b745212b0b1f36018a83214d7ecd7
workflow-type: tm+mt
source-wordcount: '183'
ht-degree: 1%

---

# Skapa en anpassad tjänst för användning med ReST API {#create-a-custom-service-for-use-with-rest-api}

Om du vill integrera med Marketo via ReST API:t måste du skapa en anpassad tjänst. Så här gör du.

>[!PREREQUISITES]
>
>* [Skapa en användarroll endast för API](/help/marketo/product-docs/administration/users-and-roles/create-an-api-only-user-role.md)
>* [Skapa endast en API-användare](/help/marketo/product-docs/administration/users-and-roles/create-an-api-only-user.md)
>

>[!NOTE]
>
>**Administratörsbehörigheter krävs**

>[!TIP]
>
>Läs mer om våra utvecklares dokumentation om [REST API](https://developer.adobe.com/marketo-apis/). Vi har också [SOAP API](https://experienceleague.adobe.com/en/docs/marketo-developer/marketo/soap/soap-api) om det är vad du behöver.

## Skapa anpassad tjänst {#create-custom-service}

1. Gå till **[!UICONTROL Admin]** område.

   ![](assets/create-a-custom-service-for-use-with-rest-api-1.png)

1. Klicka **LaunchPoint**.

   ![](assets/create-a-custom-service-for-use-with-rest-api-2.png)

1. Välj **[!UICONTROL New]** och sedan **[!UICONTROL New Service]**.

   ![](assets/create-a-custom-service-for-use-with-rest-api-3.png)

1. Ange en **[!UICONTROL Display Name]** för tjänsten. Välj **[!UICONTROL API Only User]** [tidigare skapat](/help/marketo/product-docs/administration/users-and-roles/create-an-api-only-user.md).

   ![](assets/create-a-custom-service-for-use-with-rest-api-4.png)

   >[!NOTE]
   >
   >Observera att vi redan har inbyggd integrering för populära webbinärtjänster.

1. Klicka på **[!UICONTROL Create]**.

   ![](assets/create-a-custom-service-for-use-with-rest-api-5.png)

   Absolut! Tjänsten är nu skapad. Låt oss gå vidare och hämta alla autentiseringsuppgifter för åtkomst.

## Autentiseringsuppgifter för API-åtkomst {#credentials-for-api-access}

1. Gå till **[!UICONTROL Admin]** område.

   ![](assets/create-a-custom-service-for-use-with-rest-api-6.png)

1. Klicka på **[!UICONTROL LaunchPoint]**.

   ![](assets/create-a-custom-service-for-use-with-rest-api-7.png)

1. Klicka **[!UICONTROL View Details]** för anpassade [!UICONTROL LaunchPoint] tjänst skapad ovan.

   ![](assets/create-a-custom-service-for-use-with-rest-api-8.png)

1. Klicka på **[!UICONTROL Get Token]**.

   ![](assets/create-a-custom-service-for-use-with-rest-api-9.png)

1. Ange **[!UICONTROL Client Id]**, **[!UICONTROL Client Secret]**, **[!UICONTROL Authorized User]** och **[!UICONTROL Token]** till den person som ansvarar för att upprätta anslutningen.

   ![](assets/create-a-custom-service-for-use-with-rest-api-10.png)

>[!CAUTION]
>
>Dela inte den här informationen, det är bakdörren till dina data. Håll det säkert!
