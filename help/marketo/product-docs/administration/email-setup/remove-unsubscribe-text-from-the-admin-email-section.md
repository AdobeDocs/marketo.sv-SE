---
unique-page-id: 2360245
description: Ta bort text från avsnittet "Admin -> E-post" - Marketo Docs - Produktdokumentation
title: Ta bort Avbeställ text från avsnittet "Admin -> E-post"
translation-type: tm+mt
source-git-commit: 47b2fee7d146c3dc558d4bbb10070683f4cdfd3d
workflow-type: tm+mt
source-wordcount: '164'
ht-degree: 0%

---


# Ta bort Avbeställ text från avsnittet &quot;Admin -> E-post&quot; {#remove-unsubscribe-text-from-the-admin-email-section}

Det enda skälet till att du bör ta bort det avbrutna prenumerationen helt från området&quot;Admin > E-post&quot; är om du väljer att skapa länken för att avbryta prenumerationen i e-postmallarna. Textrutan har en validering som inte tillåter att du sparar utan innehåll. Du kan kringgå detta genom att lägga till en liten HTML-kommentar. HTML-kommentaren visas inte i e-postklienten eftersom den återger e-postmeddelandet i HTML och kommentarerna utelämnas. Så här gör du.

1. Gå till **Admin** och klicka på **E-post**.

   ![](assets/image2016-8-26-13-3a57-3a9.png)

1. Markera all text och tryck på **Delete **tangent.

   >[!CAUTION]
   >
   >Innan du tar bort kopierar/klistrar du in detta i ett textdokument som en säkerhetskopia.

1. Skriv in **<!--This is a comment -->**.

   ![](assets/image2016-8-26-13-3a53-3a15.png)

1. Klicka på **Spara ändringar**.

   ![](assets/image2016-8-26-13-3a59-3a40.png)

>[!NOTE]
>
>För **Unsubscribe Text **måste du lägga till ett enda tecken. Använd ett streck eller en punkt.

