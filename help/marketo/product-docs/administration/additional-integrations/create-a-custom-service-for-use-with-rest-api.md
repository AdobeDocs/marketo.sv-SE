---
unique-page-id: 2360350
description: Skapa en anpassad tjänst för användning med ReST API - Marketo Docs - produktdokumentation
title: Skapa en anpassad tjänst för användning med ReST API
translation-type: tm+mt
source-git-commit: 47b2fee7d146c3dc558d4bbb10070683f4cdfd3d
workflow-type: tm+mt
source-wordcount: '228'
ht-degree: 0%

---


# Skapa en anpassad tjänst för användning med ReST API {#create-a-custom-service-for-use-with-rest-api}

Om du vill integrera med Marketo via ReST API:t måste du skapa en anpassad tjänst. Så här gör du.

>[!NOTE]
>
>**Förutsättningar**
>
>* [Skapa en användarroll endast för API](../../../product-docs/administration/users-and-roles/create-an-api-only-user-role.md)
>* [Skapa endast en API-användare](../../../product-docs/administration/users-and-roles/create-an-api-only-user.md)

>



>[!NOTE]
>
>**Administratörsbehörigheter krävs**

>[!NOTE]
>
>**Djupdykning**
>
>Läs mer i dokumentationen för våra utvecklare om [ReST API](http://developers.marketo.com/documentation/rest/). Vi har också [SOAP API](http://developers.marketo.com/documentation/soap/) om det är det du behöver.

>[!NOTE]
>
>Du kan inte skapa en anpassad tjänst om du har Spark-nivån Marketo.

## Skapa anpassad tjänst {#create-custom-service}

1. Gå till **Admin** och klicka på **LaunchPoint**.

   ![](assets/image2014-9-19-10-3a38-3a15.png)

1. Klicka på **Ny tjänst** under **Ny**.

   ![](assets/image2014-9-19-10-3a38-3a22.png)

1. Ange ett **visningsnamn** för tjänsten. Markera den **API-version som du** tidigare skapade [som endast är användar](../../../product-docs/administration/users-and-roles/create-an-api-only-user.md).

   >[!NOTE]
   >
   >**Påminnelse**
   >
   >Observera att vi redan har inbyggd integrering för populära webbinärtjänster.

   ![](assets/image2014-9-19-10-3a38-3a32.png)

1. Klicka på **Skapa**.

   ![](assets/image2014-9-19-10-3a39-3a28.png)

   Absolut! Tjänsten är nu skapad. Låt oss gå vidare och hämta alla autentiseringsuppgifter för åtkomst.

## Autentiseringsuppgifter för API-åtkomst {#credentials-for-api-access}

1. Gå till **Admin** och klicka på **LaunchPoint**.

   ![](assets/image2014-9-19-10-3a42-3a11.png)

1. Klicka på **Visa detaljer** för den anpassade LaunchPoint-tjänsten som skapas ovan.

   ![](assets/image2014-9-19-10-3a42-3a16.png)

1. Klicka på **Hämta token**.

   ![](assets/image2014-9-19-10-3a42-3a24.png)

1. Ange klient-ID**, **klienthemlighet**, **auktoriserad användare** och **token** för den person som ansvarar för att upprätta anslutningen.

   ![](assets/image2014-9-19-10-3a42-3a38.png)

>[!CAUTION]
>
>Dela inte denna information; det är bakdörren till era data. Håll det säkert!

