---
unique-page-id: 2360207
description: Skapa en endast API-användare - Marketo Docs - produktdokumentation
title: Skapa endast en API-användare
translation-type: tm+mt
source-git-commit: e149133a5383faaef5e9c9b7775ae36e633ed7b1
workflow-type: tm+mt
source-wordcount: '165'
ht-degree: 0%

---


# Skapa endast en API-användare {#create-an-api-only-user}

Om du vill integrera med Marketo via [REST API](http://developers.marketo.com/documentation/rest/)måste du skapa en användare med enbart API. Så här gör du.

>[!PREREQUISITES]
>
>* [Skapa en användarroll endast för API](create-an-api-only-user-role.md)

>



>[!NOTE]
>
>**Administratörsbehörigheter krävs**

1. Klicka på **Användare och roller under** Admin **.**

   ![](assets/image2014-9-17-9-3a31-3a31.png)

1. Klicka på **Bjud in ny användare**.

   ![](assets/image2014-9-17-9-3a32-3a3.png)

1. Ange e-post, förnamn och efternamn för den användare som bara är API. Klicka på **Nästa**.

   ![](assets/image2016-5-24-10-3a53-3a7.png)

   >[!TIP]
   >
   >Lägg till en valfri orsak eller ett förfallodatum för åtkomst. Utgångsdatumet är praktiskt för korttidsanställda.

1. Markera rollen Endast **** API och markera kryssrutan Endast **** API. Klicka på **Nästa**.

   ![](assets/four.png)

1. Klicka på **Skicka**.

   ![](assets/image2016-5-24-11-3a8-3a20.png)

>[!NOTE]
>
>Popup-fönstret säger: &quot;En inbjudan krävs inte bara för API&quot;, men det betyder inte att du har gjort något fel. Det innebär bara att vi skapar rollen utan att behöva skicka ett e-postmeddelande med en inbjudan.

Okej då! Nu ska vi skapa en anpassad tjänst.

>[!NOTE]
>
>**Relaterade artiklar**
>
>* [Skapa en anpassad tjänst för användning med ReST API](../../../product-docs/administration/additional-integrations/create-a-custom-service-for-use-with-rest-api.md)

>



