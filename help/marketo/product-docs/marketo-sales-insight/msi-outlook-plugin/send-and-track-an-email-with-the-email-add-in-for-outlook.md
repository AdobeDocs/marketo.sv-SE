---
unique-page-id: 2949716
description: Skicka och spåra ett e-postmeddelande med e-posttillägget för Outlook - Marketo Docs - Produktdokumentation
title: Skicka och spåra ett e-postmeddelande med e-posttillägget för Outlook
exl-id: 81c2ce86-1528-48ad-8848-ee5a828f9ff7
source-git-commit: 8b9b2b83f5dc8908f9794d1ee387299edaae31b3
workflow-type: tm+mt
source-wordcount: '294'
ht-degree: 0%

---

# Skicka och spåra ett e-postmeddelande med e-posttillägget för Outlook {#send-and-track-an-email-with-the-email-add-in-for-outlook}

Du kan skicka och spåra e-postmeddelanden med Marketo direkt från Outlook.

>[!PREREQUISITES]
>
>Om du inte har gjort det än installerar du [Marketo e-posttillägg för Outlook](/help/marketo/product-docs/marketo-sales-insight/msi-outlook-plugin/install-the-marketo-email-add-in-for-outlook-with-a-registration-code.md).

>[!NOTE]
>
>Funktioner för Sales Insight-åtgärder, inklusive Skicka e-post, Lägg till i säljkampanj och Uppgifter, är inte tillgängliga i e-postpluginer för Sales Insight för Gmail och Outlook. För närvarande kan användare bara skicka spårbara e-postmeddelanden med eller utan en Marketo-e-postmall från sin e-postklient när de använder e-postpluginmodulerna för Sales Insight.

1. Öppna Microsoft Outlook och skapa ett nytt e-postmeddelande.

   ![](assets/image2014-9-23-16-3a6-3a46.png)

   >[!CAUTION]
   >
   >Om du inkluderar flera mottagare i e-postmeddelandet spåras alla aktiviteter under den första mottagaren.

1. Skriv e-postmeddelandet som vanligt och klicka sedan på **Send and Track**.

   ![](assets/image2014-9-23-16-3a7-3a1.png)

   >[!NOTE]
   >
   >Om du skickar ett e-postmeddelande till någon som inte finns i din Marketo-instans skapas en personpost automatiskt för dem. Deras efternamn blir alltid&quot;mktUnknown&quot; så att du enkelt kan hitta dem.

   >[!TIP]
   >
   >Om du vill använda en Marketo-mall finns mer information i [Skicka och spåra från Outlook med en mall](/help/marketo/product-docs/marketo-sales-insight/msi-outlook-plugin/send-and-track-from-outlook-using-a-marketo-template.md).

1. Ta en titt på förhandsgranskningen och klicka **Skicka**.

   ![](assets/image2014-9-23-16-3a7-3a13.png)

   >[!CAUTION]
   >
   >Antispam-tekniken avvisar ofta öppningar och klickningar som inträffar inom 20 sekunder efter att e-postmeddelandet har skickats, så vänta åtminstone så länge med att öppna/klicka under testningen.

   Om du vill se vem som har tagit emot e-postmeddelanden som skickats via Outlook skapar du en smart lista med hjälp av filtret&quot;Skickat e-post för försäljning&quot;.

   ![](assets/was-sent-sales-email.png)

Så enkelt är det! Även om det här e-postmeddelandet skickades av en säljares Outlook spåras det i Marketo.

>[!MORELIKETHIS]
>
>[Logga inkommande e-post från dina leads i Marketo](/help/marketo/product-docs/marketo-sales-insight/using-msi/log-inbound-mail-from-your-leads-in-marketo.md)
