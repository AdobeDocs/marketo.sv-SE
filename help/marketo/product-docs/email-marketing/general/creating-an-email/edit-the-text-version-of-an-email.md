---
unique-page-id: 11372054
description: Redigera textversionen av ett e-postmeddelande - Marketo Docs - produktdokumentation
title: Redigera textversionen av ett e-postmeddelande
exl-id: 6973ccdd-6ae1-4051-ab7e-ff7da40baf97
feature: Email Editor
source-git-commit: 94b458ee7138f90bd243d2d2a8b761dabff23a66
workflow-type: tm+mt
source-wordcount: '233'
ht-degree: 0%

---

# Redigera textversionen av ett e-postmeddelande {#edit-the-text-version-of-an-email}

När du skapar ett e-postmeddelande kanske du vill att textversionen ska skrivas på ett annat sätt än HTML. Som standard kopierar Marketo automatiskt textinnehållet i textelement som finns i e-postmeddelandet till textversionen. Så här redigerar du det.

>[!NOTE]
>
>Det här är inte en artikel om att skapa ett e-postmeddelande med endast text. Mer information finns i [Skapa ett e-postmeddelande med endast text](/help/marketo/product-docs/email-marketing/general/creating-an-email/create-a-text-only-email.md).

1. Klicka på fliken **Text** längst ned i e-postmeddelandet i e-postredigeraren.

   ![](assets/one-5.png)

1. Avmarkera **Kopiera automatiskt från HTML** om du vill göra ändringar.

   ![](assets/two-5.png)

1. Dubbelklicka på textområdet.

   ![](assets/three-4.png)

1. Redigera. När du är klar stänger du bara redigeraren eller går tillbaka till HTML. Ändringarna sparas automatiskt.

   ![](assets/four-4.png)

   Om du bara har statiskt innehåll kan texten redigeras i ett stort block (se steg 3). Om du har dynamiskt innehåll bryts texten upp i olika redigerbara avsnitt, vilket visas nedan.

   ![](assets/five-3.png)

>[!CAUTION]
>
>Om du väljer **Kopiera från HTML**, eller om du väljer **Kopiera automatiskt från HTML** i e-postmeddelanden som innehåller dynamiskt innehåll, anges flaggan Granskad till _true_ för alla segment (vilket ger den gröna bockmarkeringen som anger att den har granskats) i både HTML- och textversionen av e-postmeddelandet. Om du utför någon av ovanstående åtgärder måste du kontrollera innehållet innan du skickar iväg det.
