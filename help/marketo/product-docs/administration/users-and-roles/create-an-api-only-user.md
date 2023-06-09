---
unique-page-id: 2360207
description: Skapa en användare med endast API - Marketo Docs - produktdokumentation
title: Skapa endast en API-användare
exl-id: 23c92255-07a8-41c2-b7b8-8e495d135671
source-git-commit: 2d28d4b473815952231356691b1e9310c61a20f1
workflow-type: tm+mt
source-wordcount: '154'
ht-degree: 3%

---

# Skapa endast en API-användare {#create-an-api-only-user}

Om du vill integrera med Marketo via [REST API](https://developers.marketo.com/documentation/rest/){target="_blank"}måste du skapa en användare med enbart API. Så här gör du.

>[!PREREQUISITES]
>
>[Skapa en användarroll endast för API](/help/marketo/product-docs/administration/users-and-roles/create-an-api-only-user-role.md){target="_blank"}

>[!NOTE]
>
>**Administratörsbehörigheter krävs**

1. Gå till **[!UICONTROL Admin]** område.

   ![](assets/create-an-api-only-user-1.png)

1. Klicka på **[!UICONTROL Users & Roles]**.

   ![](assets/create-an-api-only-user-2.png)

1. Klicka på **[!UICONTROL Invite New User]**.

   ![](assets/create-an-api-only-user-3.png)

1. Ange e-post, förnamn och efternamn för den användare som bara är API. Klicka på **[!UICONTROL Next]**.

   ![](assets/create-an-api-only-user-4.png)

   >[!TIP]
   >
   >Lägg till en valfri orsak eller ett förfallodatum för åtkomst. Utgångsdatumet är praktiskt för korttidsanställda.

1. Välj **[!UICONTROL API Only]** roll och kontrollera **[!UICONTROL API Only]** kryssrutan. Klicka på **[!UICONTROL Next]**.

   ![](assets/create-an-api-only-user-5.png)

1. Klicka på **[!UICONTROL Send]**.

   ![](assets/create-an-api-only-user-6.png)

>[!NOTE]
>
>Popup-fönstret säger: &quot;En inbjudan krävs inte bara för API&quot;, men det betyder inte att du har gjort något fel. Det innebär bara att vi skapar rollen utan att behöva skicka ett e-postmeddelande med en inbjudan.

Okej då! Nu ska vi skapa en anpassad tjänst.

>[!MORELIKETHIS]
>
>[Skapa en anpassad tjänst för användning med ReST API](/help/marketo/product-docs/administration/additional-integrations/create-a-custom-service-for-use-with-rest-api.md){target="_blank"}
