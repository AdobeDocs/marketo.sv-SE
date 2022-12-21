---
unique-page-id: 2360245
description: Ta bort avanmälan av text från Admin Email Section - Marketo Docs - Product Documentation
title: Ta bort Avbeställ text från Admin Email Section
exl-id: 2961a9b6-8b35-4227-bf8a-a07b2664a6c4
source-git-commit: 2776969be44ba1a3d795e99986d10cf0470fb9e9
workflow-type: tm+mt
source-wordcount: '165'
ht-degree: 0%

---

# Ta bort Avbeställ text från Admin Email Section {#remove-unsubscribe-text-from-the-admin-email-section}

Det enda skälet till att du bör ta bort det avbrutna prenumerationen helt från området&quot;Admin > E-post&quot; är om du väljer att skapa länken för att avbryta prenumerationen i e-postmallarna. Textrutan har en validering som inte tillåter att du sparar utan innehåll. Du kan kringgå detta genom att lägga till en liten HTML-kommentar. Kommentaren HTML visas inte i e-postklienten eftersom den återger e-postmeddelandet i HTML och kommentarerna utelämnas. Så här gör du.

1. Gå till **Administratör** område.

   ![](assets/remove-unsubscribe-text-from-the-admin-email-section-1.png)

1. Klicka **E-post**.

   ![](assets/remove-unsubscribe-text-from-the-admin-email-section-2.png)

1. Markera all text och tryck på **Ta bort** nyckel.

   >[!CAUTION]
   >
   >Innan du tar bort kopierar/klistrar du in detta i ett textdokument som en säkerhetskopia.

1. Skriv in `<!--This is a comment -->`.

   ![](assets/remove-unsubscribe-text-from-the-admin-email-section-3.png)

1. Klicka **Spara ändringar**.

   ![](assets/remove-unsubscribe-text-from-the-admin-email-section-4.png)

>[!NOTE]
>
>För **Avbeställ text** du måste lägga till ett enda tecken. Använd ett streck eller en punkt.
