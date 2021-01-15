---
unique-page-id: 2360207
description: Skapa en endast API-användare - Marketo Docs - produktdokumentation
title: Skapa endast en API-användare
translation-type: tm+mt
source-git-commit: f79909ce8f2e37bf0748596774fe47ac03618696
workflow-type: tm+mt
source-wordcount: '163'
ht-degree: 0%

---


# Skapa en endast API-användare {#create-an-api-only-user}

Om du vill integrera med Marketo via [REST API](https://developers.marketo.com/documentation/rest/) måste du skapa en användare som bara har API. Så här gör du.

>[!PREREQUISITES]
>
>[Skapa en användarroll endast för API](/help/marketo/product-docs/administration/users-and-roles/create-an-api-only-user-role.md)


>[!NOTE]
>
>**Administratörsbehörigheter krävs**

1. Under **Admin** klickar du på **Användare och roller.**

   ![](assets/image2014-9-17-9-3a31-3a31.png)

1. Klicka på **Bjud in ny användare**.

   ![](assets/image2014-9-17-9-3a32-3a3.png)

1. Ange e-post, förnamn och efternamn för den användare som bara är API. Klicka på **Nästa**.

   ![](assets/image2016-5-24-10-3a53-3a7.png)

   >[!TIP]
   >
   >Lägg till en valfri orsak eller ett förfallodatum för åtkomst. Utgångsdatumet är praktiskt för korttidsanställda.

1. Markera rollen **Endast API** och markera kryssrutan **Endast API**. Klicka på **Nästa**.

   ![](assets/four.png)

1. Klicka på **Skicka**.

   ![](assets/image2016-5-24-11-3a8-3a20.png)

>[!NOTE]
>
>Popup-fönstret säger: &quot;En inbjudan krävs inte bara för API&quot;, men det betyder inte att du har gjort något fel. Det innebär bara att vi skapar rollen utan att behöva skicka ett e-postmeddelande med en inbjudan.

Okej då! Nu ska vi skapa en anpassad tjänst.

>[!MORELIKETHIS]
>
>[Skapa en anpassad tjänst för användning med ReST API](/help/marketo/product-docs/administration/additional-integrations/create-a-custom-service-for-use-with-rest-api.md)
