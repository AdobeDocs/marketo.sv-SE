---
description: Connect Dynamic Chat to Marketo - Marketo Docs - Product Documentation
title: Connect Dynamic Chat to Marketo
exl-id: bad6c2dc-d4e7-4f98-bf6d-743043f96e4e
source-git-commit: bb2620ab72987cf857a7144aca21e94a11f29d90
workflow-type: tm+mt
source-wordcount: '262'
ht-degree: 0%

---

# Ansluta Dynamic Chat till Marketo {#connect-dynamic-chat-to-marketo}

After you&#39;ve completed the [initial setup](/help/marketo/product-docs/demand-generation/dynamic-chat/initial-setup.md), it&#39;s time to perform the one-time sync connecting Dynamic Chat to your Marketo subscription.

1. I Min Marketo klickar du på **Dynamiskt chatt** platta.

   ![](assets/connect-dynamic-chat-to-marketo-1.png)

   >[!NOTE]
   >
   >Om du inte ser rutan kan du kontakta Marketo Admin.

1. Om du tidigare har använt ett program med en Adobe ID kommer du direkt till Dynamic Chat. Om inte, [konfigurera din Adobe ID](https://helpx.adobe.com/manage-account/using/create-update-adobe-id.html).

1. Om du vill ansluta din Marketo-instans väljer du **Integreringar**.

   ![](assets/connect-dynamic-chat-to-marketo-2.png)

1. På Marketo-kortet klickar du **Initiera synkronisering**.

   ![](assets/connect-dynamic-chat-to-marketo-3.png)

1. Välj upp till 50 standardfält eller anpassade fält som ska synkroniseras med dynamiskt chatt. Klicka **Nästa** när det är klart.

   ![](assets/connect-dynamic-chat-to-marketo-4.png)

   >[!CAUTION]
   >
   >At this time, attribute selections **cannot** be changed after the initial sync. När synkroniseringen är klar kan du bara gå tillbaka och lägga till fler (om du väljer mindre än 50).

1. Make sure you have the correct selections (reminder: you cannot remove attributes post-sync, so click **Edit Selections** if you need to change any in this step). Click **Confirm** when done to initiate the sync.

   ![](assets/connect-dynamic-chat-to-marketo-5.png)

>[!NOTE]
>
>It can take anywhere from 2 to 24 hours for the sync to complete, depending on the size of your database.

## Link Your Adobe Org and Marketo {#link-your-adobe-org-and-marketo}

Nu är det dags att länka Adobe och Marketo.

1. Logga in på [experience.adobe.com](https://experience.adobe.com).

1. Kopiera Org-ID:t från det nedre högra hörnet på hemsidan, _minus_ &quot;@AdobeOrg.&quot;

   ![](assets/connect-dynamic-chat-to-marketo-6.png)

1. I Marketo går du till **Administratör** avsnitt och markera **Organisationsmappning för Adobe**.

   ![](assets/connect-dynamic-chat-to-marketo-7.png)

1. Klicka **Redigera**.

   ![](assets/connect-dynamic-chat-to-marketo-8.png)

1. Klistra in det Org-ID som du kopierade i steg 2 och klicka på **OK**.

   ![](assets/connect-dynamic-chat-to-marketo-9.png)

>[!MORELIKETHIS]
>
>[Initial Setup](/help/marketo/product-docs/demand-generation/dynamic-chat/initial-setup.md)
