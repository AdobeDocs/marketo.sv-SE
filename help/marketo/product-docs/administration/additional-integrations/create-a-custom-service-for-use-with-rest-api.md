---
unique-page-id: 2360350
description: Skapa en anpassad LaunchPoint-tjänst som är länkad till en API-användare för ReST API-integrering.
title: Skapa en anpassad tjänst för användning med ReST API
exl-id: d94f723b-2e98-4350-a9e5-bd57aff2303b
feature: Administration
source-git-commit: 40f06a5391f2f7263bea0c5b8cefc1f3a607c68c
workflow-type: tm+mt
source-wordcount: '150'
ht-degree: 2%

---

# Skapa en anpassad tjänst för användning med ReST API {#create-a-custom-service-for-use-with-rest-api}

Skapa en anpassad tjänst om du vill integrera med Marketo via ReST API.

>[!PREREQUISITES]
>
>* [Skapa endast en API-användarroll](/help/marketo/product-docs/administration/users-and-roles/create-an-api-only-user-role.md)
>* [Skapa endast en API-användare](/help/marketo/product-docs/administration/users-and-roles/create-api-only-user.md)
>

>[!NOTE]
>
>**Administratörsbehörigheter krävs**

>[!TIP]
>
>Mer information om [REST API](https://developer.adobe.com/marketo-apis/) finns i dokumentationen för utvecklare.

## Skapa anpassad tjänst {#create-custom-service}

1. Gå till området **[!UICONTROL Admin]**.

   ![](assets/create-a-custom-service-for-use-with-rest-api-1.png)

1. Klicka på **[!UICONTROL LaunchPoint]**.

   ![](assets/create-a-custom-service-for-use-with-rest-api-2.png)

1. Välj **[!UICONTROL New]** och sedan **[!UICONTROL New Service]**.

   ![](assets/create-a-custom-service-for-use-with-rest-api-3.png)

1. Ange en **[!UICONTROL Display Name]** för tjänsten. Markera **[!UICONTROL API Only User]** [som skapades](/help/marketo/product-docs/administration/users-and-roles/create-api-only-user.md).

   ![](assets/create-a-custom-service-for-use-with-rest-api-4.png)

1. Klicka på **[!UICONTROL Create]**.

   ![](assets/create-a-custom-service-for-use-with-rest-api-5.png)

   Tjänsten har skapats. Hämta de autentiseringsuppgifter som ska användas för åtkomst.

## Autentiseringsuppgifter för API-åtkomst {#credentials-for-api-access}

1. Gå till området **[!UICONTROL Admin]**.

   ![](assets/create-a-custom-service-for-use-with-rest-api-6.png)

1. Klicka på **[!UICONTROL LaunchPoint]**.

   ![](assets/create-a-custom-service-for-use-with-rest-api-7.png)

1. Klicka på **[!UICONTROL View Details]** för den anpassade [!UICONTROL LaunchPoint]-tjänsten som skapats ovan.

   ![](assets/create-a-custom-service-for-use-with-rest-api-8.png)

1. Klicka på **[!UICONTROL Get Token]**.

   ![](assets/create-a-custom-service-for-use-with-rest-api-9.png)

1. Ange **[!UICONTROL Client Id]**, **[!UICONTROL Client Secret]**, **[!UICONTROL Authorized User]** och **[!UICONTROL Token]** till den person som ansvarar för att upprätta anslutningen.

   ![](assets/create-a-custom-service-for-use-with-rest-api-10.png)

>[!CAUTION]
>
>Dela inte denna information eftersom den ger åtkomst till dina data.
