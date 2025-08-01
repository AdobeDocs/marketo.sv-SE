---
description: Konfigurera en anpassad leveranskanal för ditt team - Marketo Docs - produktdokumentation
title: Konfigurera en anpassad leveranskanal för ditt team
exl-id: e7ba524c-a0d2-4c2b-95ba-20b9d830f18c
feature: Sales Insight Actions
source-git-commit: 0d37fbdb7d08901458c1744dc68893e155176327
workflow-type: tm+mt
source-wordcount: '159'
ht-degree: 0%

---

# Konfigurera en anpassad leveranskanal för ditt team {#set-up-a-custom-delivery-channel-for-your-team}

>[!NOTE]
>
>**Administratörsbehörigheter krävs**

>[!NOTE]
>
>* Förutom att konfigurera SMTP-servern måste din [e-postidentitet verifieras](/help/marketo/product-docs/marketo-sales-insight/actions/getting-started/email-settings/verify-your-email.md) innan du kan skicka e-post.
>* Vi rekommenderar att du samarbetar med IT-teamet eller SMTP-serverleverantören för att få rätt serverautentiseringsuppgifter för din SMTP-server.
>* Du kan inte ansluta din Gmail- och [!DNL Exchange]-server med autentiseringsuppgifterna för SMTP-servern. Använd vår e-postanslutningstjänst för att integrera med dessa leverantörer.

1. Klicka på kugghjulsikonen och välj **[!UICONTROL Settings]**.

   ![](assets/set-up-a-custom-delivery-channel-for-your-team-1.png)

1. Klicka på [!UICONTROL Admin Settings] under **[!UICONTROL General]**.

   ![](assets/set-up-a-custom-delivery-channel-for-your-team-2.png)

1. Klicka på fliken **[!UICONTROL Team Delivery Channel]**.

   ![](assets/set-up-a-custom-delivery-channel-for-your-team-3.png)

1. Ange autentiseringsuppgifterna för SMTP-servern och klicka på **[!UICONTROL Connect]**.

   ![](assets/set-up-a-custom-delivery-channel-for-your-team-4.png)

   >[!NOTE]
   >
   >Teamets SMTP-server kommer att vara standardleveranskanalen för standardidentiteten för e-post för alla teammedlemmar. Dessutom kommer den att vara tillgänglig som ett alternativ för leveranskanal för alla andra e-postidentiteter.

   >[!MORELIKETHIS]
   >
   >* [E-postanslutning för Gmail-användare](/help/marketo/product-docs/marketo-sales-connect/email-plugins/gmail/email-connection-for-gmail-users.md)
   >* [E-postanslutning för [!DNL Outlook] användare](/help/marketo/product-docs/marketo-sales-connect/email-plugins/msc-for-outlook/email-connection-for-outlook-users.md)
