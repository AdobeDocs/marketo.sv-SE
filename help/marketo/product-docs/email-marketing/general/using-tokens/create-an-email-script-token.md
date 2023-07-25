---
unique-page-id: 1900577
description: Skapa en token för e-postskript - Marketo Docs - produktdokumentation
title: Skapa en e-postskripttoken
exl-id: c7f8c3e0-6d64-4115-b9b6-261576360ba1
feature: Tokens
source-git-commit: 431bd258f9a68bbb9df7acf043085578d3d91b1f
workflow-type: tm+mt
source-wordcount: '235'
ht-degree: 0%

---

# Skapa en e-postskripttoken {#create-an-email-script-token}

För avancerade utvecklare kan du använda [Snabbhetsskript](https://velocity.apache.org/engine/1.7/user-guide.html) i era e-postmeddelanden. Så här gör du.

1. Gå till **Marknadsföringsaktiviteter**.

   ![](assets/ma.png)

1. Sök efter och välj ett program (Händelse, Standard eller Förlovning osv.).

   ![](assets/image2014-9-17-22-3a21-3a24.png)

1. Under **Mina token** tabb, dra i en **E-postskript** token.

   ![](assets/image2014-9-17-22-3a21-3a29.png)

1. Namnge din e-postskripttoken och **klicka för att redigera** innehållet.

   ![](assets/image2014-9-17-22-3a21-3a46.png)

1. Använd trädet till höger för att dra in **Person, möjlighet**, eller **Eget objekt** variabler.

   ![](assets/five-2.png)

   >[!NOTE]
   >
   >När du använder en array (möjlighet eller anpassat objekt) begränsas du till de senaste 10 objekten som är kopplade till personen.

1. Observera att variabeln blir markerad/aktiv när du har dragit den till skriptredigeraren.

   ![](assets/image2014-9-17-22-3a22-3a33.png)

   >[!NOTE]
   >
   >Om du skriver in tokens i friform måste du kontrollera/aktivera alla motsvarande tokens i trädet, annars behandlas de som oformaterad text och fungerar inte.

1. Skriv ditt skript i Snabbhet. Här är några användbara resurser:

   * [Marketo Developers Email Scripting Documentation](https://developers.marketo.com/email-scripting/)
   * [Användarhandbok för snabbhet](https://velocity.apache.org/engine/devel/user-guide.html)
   * [Referenshandbok för hastighet](https://velocity.apache.org/engine/devel/vtl-reference-guide.html)
   * [Velocity Tools Javadoc](https://velocity.apache.org/tools/releases/2.0/javadoc/index.html)

1. När skriptet är klart klickar du på **Spara**.

   ![](assets/image2014-9-17-22-3a23-3a1.png)

1. Klicka **Spara** en gång till.

   ![](assets/image2014-9-17-22-3a23-3a13.png)

Nu kan du använda denna token i dina e-postmeddelanden. Skriptet körs varje gång ett e-postmeddelande skickas.

>[!MORELIKETHIS]
>
>[Lägg till en e-postskripttoken i din e-post](/help/marketo/product-docs/email-marketing/general/using-tokens/add-an-email-script-token-to-your-email.md)
