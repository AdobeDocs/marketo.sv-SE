---
unique-page-id: 1900597
description: Definiera en målgrupp genom att importera en lista - Marketo Docs - produktdokumentation
title: Definiera en publik genom att importera en lista
exl-id: 9a63f4a5-1d76-4671-9622-19eb368d196f
feature: Email Programs
source-git-commit: 09a656c3a0d0002edfa1a61b987bff4c1dff33cf
workflow-type: tm+mt
source-wordcount: '363'
ht-degree: 0%

---

# Definiera en publik genom att importera en lista {#define-an-audience-by-importing-a-list}

>[!PREREQUISITES]
>
>[Skapa en e-postadress för ett e-postprogram](/help/marketo/product-docs/email-marketing/email-programs/email-program-actions/create-an-email-for-an-email-program.md)

När du har skapat ett e-postprogram vill du berätta vem du vill skicka e-postmeddelandet till. Du kan göra detta genom att [skapa en smart lista](/help/marketo/product-docs/core-marketo-concepts/smart-lists-and-static-lists/creating-a-smart-list/create-a-smart-list.md) eller genom att importera en lista. Så här uppnår du detta genom att importera en lista.

>[!NOTE]
>
>Det går bara att definiera målgruppen när e-postprogrammet inte har godkänts.
>
>Alla datum-/tidfält som importeras behandlas som centraltid. Om du har datum-/tidsfält i en annan tidszon kan du använda en Excel-formel för att omvandla den till Central Time (USA/Chicago).

1. Gå till **[!UICONTROL Marketing Activities]**.

   ![](assets/login-marketing-activities-1.png)

1. Välj ditt e-postprogram och klicka sedan på **[!UICONTROL Import List]** under rutan **[!UICONTROL Audience]**.

   ![](assets/importlist.png)

1. Listimportfönstret öppnas, klicka på **[!UICONTROL Browse]** och välj den fil du vill importera. När du har valt din lista över personer klickar du på **[!UICONTROL Next]**.

   ![](assets/importlist1.png)

   >[!CAUTION]
   >
   >Kontrollera att listan är kodad UTF-8, UTF-16, Shift-JIS eller EUC-JP och att filstorleken inte överstiger 50 MB.

1. Kontrollera att fälten i filen är korrekt mappade och klicka på **[!UICONTROL Next]**.

   ![](assets/image2014-9-12-11-3a10-3a7.png)

   >[!TIP]
   >
   >Marketo kommer att komma ihåg mappningarna för framtida importer!

1. Ange en **[!UICONTROL Name]** för listan och klicka på **[!UICONTROL Import]**.

   ![](assets/image2014-9-12-11-3a10-3a13.png)

1. När importen är klar går du tillbaka till huvudprogramfliken. Du får se hur många som är kvalificerade.

   ![](assets/myemailprogram-1.jpg)

>[!NOTE]
>
>**Definition**
>
>Märkte du numret för spärrad? Det här numret är en delmängd av de kvalificerade personerna och representerar personer som inte kan skicka det här e-postmeddelandet eftersom de är:
>
>* Avprenumererad
>* Marknadsföring har pausats
>* Blocklist
>* Ogiltig e-postadress
>* Tom e-postadress
>
>Klicka på numret om du vill se en detaljerad lista över personer som blockerats från utskick.
>
>Använd knappen ![—](assets/image2014-10-23-16-3a32-3a36-1.png) på **[!UICONTROL Audience]**-panelen för att se hur många personer som är kvalificerade att ta emot e-postmeddelandet baserat på villkoren i den smarta listan. Ta bort det blockerade numret från personnumret för att få det totala antalet personer som ska få e-postmeddelandet.

>[!TIP]
>
>Du behöver inte vänta på att listimporten ska slutföras. Du kan fortsätta arbeta om du vill.

Fantastisk! Nu är det dags att välja ett befintligt e-postmeddelande eller att skapa ett nytt e-postmeddelande som ska skickas till dessa personer.

>[!MORELIKETHIS]
>
>* [Välj en befintlig e-postadress](/help/marketo/product-docs/email-marketing/email-programs/email-program-actions/choose-an-existing-email.md)
>* [Skapa en e-postadress för ett e-postprogram](/help/marketo/product-docs/email-marketing/email-programs/email-program-actions/create-an-email-for-an-email-program.md)
