---
unique-page-id: 2949716
description: Skicka och spåra ett e-postmeddelande med e-posttillägget för  [!DNL Outlook] - Marketo Docs - produktdokumentation
title: Skicka och spåra ett e-postmeddelande med e-posttillägget för  [!DNL Outlook]
exl-id: 81c2ce86-1528-48ad-8848-ee5a828f9ff7
feature: Marketo Sales Insights
source-git-commit: 09a656c3a0d0002edfa1a61b987bff4c1dff33cf
workflow-type: tm+mt
source-wordcount: '279'
ht-degree: 0%

---

# Skicka och spåra ett e-postmeddelande med e-posttillägget för [!DNL Outlook] {#send-and-track-an-email-with-the-email-add-in-for-outlook}

Du kan skicka och spåra e-postmeddelanden med Marketo direkt från [!DNL Outlook].

>[!PREREQUISITES]
>
>Installera [Marketo-e-posttillägget för [!DNL Outlook]](/help/marketo/product-docs/marketo-sales-insight/msi-outlook-plugin/install-the-marketo-email-add-in-for-outlook-with-a-registration-code.md) om du inte har gjort det än.

>[!NOTE]
>
>Funktioner för Sales Insight-åtgärder, inklusive Skicka e-post, Lägg till i säljkampanj och Uppgifter, är inte tillgängliga i e-postpluginer för Sales Insight för Gmail och Outlook. För närvarande kan användare bara skicka spårbara e-postmeddelanden med eller utan en Marketo-e-postmall från sin e-postklient när de använder e-postpluginmodulerna för Sales Insight.

1. Öppna Microsoft Outlook och skapa ett nytt e-postmeddelande.

   ![](assets/image2014-9-23-16-3a6-3a46.png)

   >[!CAUTION]
   >
   >Om du inkluderar flera mottagare i e-postmeddelandet spåras alla aktiviteter under den första mottagaren.

1. Skriv e-postmeddelandet som vanligt och klicka sedan på **[!UICONTROL Send and Track]**.

   ![](assets/image2014-9-23-16-3a7-3a1.png)

   >[!NOTE]
   >
   >Om du skickar ett e-postmeddelande till någon som inte finns i din Marketo-instans skapas en personpost automatiskt för dem. Deras efternamn blir alltid&quot;mktUnknown&quot; så att du enkelt kan hitta dem.

   >[!TIP]
   >
   >Om du vill använda en Marketo-mall läser du [Skicka och spåra från [!DNL Outlook] Använda en mall](/help/marketo/product-docs/marketo-sales-insight/msi-outlook-plugin/send-and-track-from-outlook-using-a-marketo-template.md).

1. Titta på förhandsgranskningen och klicka på **[!UICONTROL Send]**.

   ![](assets/image2014-9-23-16-3a7-3a13.png)

   >[!CAUTION]
   >
   >Antispam-tekniken avvisar ofta öppningar och klickningar som inträffar inom 20 sekunder efter att e-postmeddelandet har skickats, så vänta åtminstone så länge med att öppna/klicka under testningen.

   Om du vill se vem som har tagit emot dina e-postmeddelanden som skickats via [!DNL Outlook] skapar du en smart lista med hjälp av filtret [!UICONTROL Was Sent Sales Email].

   ![](assets/was-sent-sales-email.png)

Så enkelt är det! Även om det här e-postmeddelandet skickades av en säljares [!DNL Outlook] spåras det i Marketo.

>[!MORELIKETHIS]
>
>[Logga inkommande e-post från dina leads i Marketo](/help/marketo/product-docs/marketo-sales-insight/using-msi/log-inbound-mail-from-your-leads-in-marketo.md)
