---
unique-page-id: 2360245
description: Ta bort standardinnehållet för avanmälan från Admin Email genom att använda en HTML-kommentar när du skapar länken i mallar.
title: Ta bort Avbeställ text från Admin Email Section
exl-id: 2961a9b6-8b35-4227-bf8a-a07b2664a6c4
feature: Email Setup
source-git-commit: e894ece3a643113fd3e1d8df9f8addefea5553f5
workflow-type: tm+mt
source-wordcount: '165'
ht-degree: 1%

---

# Ta bort Avbeställ text från Admin > E-postavsnitt {#remove-unsubscribe-text-from-the-admin-email-section}

Den enda anledningen till att du någonsin helt bör ta bort innehållet som inte längre är prenumerant i området **[!UICONTROL Admin]** > **[!UICONTROL Email]** är om du väljer att skapa länken för att avbryta prenumerationen i e-postmallarna. Textrutan har en validering som inte tillåter att du sparar utan innehåll. Du kan kringgå detta genom att lägga till en liten HTML-kommentar. HTML-kommentaren visas inte i e-postklienten eftersom den återger e-postmeddelandet i HTML och kommentarerna utelämnas. Så här gör du.

1. Gå till området **[!UICONTROL Admin]**.

   ![](assets/remove-unsubscribe-text-from-the-admin-email-section-1.png)

1. Klicka på **[!UICONTROL Email]**.

   ![](assets/remove-unsubscribe-text-from-the-admin-email-section-2.png)

1. Markera all text och tryck på **[!UICONTROL Delete]**.

   >[!CAUTION]
   >
   >Innan du tar bort kopierar/klistrar du in detta i ett textdokument som en säkerhetskopia.

1. Skriv in `<!--This is a comment -->`.

   ![](assets/remove-unsubscribe-text-from-the-admin-email-section-3.png)

1. Klicka på **[!UICONTROL Save Changes]**.

   ![](assets/remove-unsubscribe-text-from-the-admin-email-section-4.png)

>[!NOTE]
>
>För **Avbeställ text** måste du lägga till ett enda tecken. Använd streck eller punkt.
