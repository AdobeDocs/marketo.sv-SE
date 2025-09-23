---
unique-page-id: 14746470
description: Konfigurera en anpassad leveranskanal - Marketo Docs - produktdokumentation
title: Konfigurera en anpassad leveranskanal
exl-id: a31f7bfd-a4ee-4948-9bdc-b49d47054d40
feature: Marketo Sales Connect
source-git-commit: 09a656c3a0d0002edfa1a61b987bff4c1dff33cf
workflow-type: tm+mt
source-wordcount: '353'
ht-degree: 0%

---

# Konfigurera en anpassad leveranskanal {#setting-up-a-custom-delivery-channel}

Med [!DNL Marketo Sales Connect] kan du integrera med en anpassad SMTP-server för att leverera dina e-postmeddelanden. Det här är ett bra alternativ för dem som inte vill skicka massutskick från sin Gmail eller [!DNL Exchange]-leveranskanal.

Användare kan konfigurera en anpassad SMTP-server för egen användning, eller så kan administratörer konfigurera en Team SMTP som ska delas av alla [!DNL Sales Connect]-användare i din instans.

>[!NOTE]
>
>* Förutom att konfigurera SMTP-servern måste din [e-postidentitet verifieras](/help/marketo/product-docs/marketo-sales-connect/getting-started/email-settings/verify-your-email.md) innan du kan skicka e-post.
>* Vi rekommenderar att du samarbetar med IT-teamet eller SMTP-serverleverantören för att få rätt serverautentiseringsuppgifter för din SMTP-server.
>* Du kan inte ansluta din Gmail- och [!DNL Exchange]-server med autentiseringsuppgifterna för SMTP-servern. Använd vår e-postanslutningstjänst för att integrera med dessa leverantörer.

## Anpassad SMTP {#custom-smtp}

1. Logga in på [webbprogrammet](https://toutapp.com/login), klicka på kugghjulsikonen uppe till höger och välj **[!UICONTROL Settings]**.

   ![](assets/setting-up-a-custom-delivery-channel-1.png)

1. Klicka på [!UICONTROL My Account] under **[!UICONTROL Email Settings]**.

   ![](assets/setting-up-a-custom-delivery-channel-2.png)

1. Klicka på **[!UICONTROL Custom Delivery Channel]**.

   ![](assets/setting-up-a-custom-delivery-channel-3.png)

1. Ange dina [!UICONTROL SMTP Server]-inloggningsuppgifter och klicka på **[!UICONTROL Connect]**.

   ![](assets/setting-up-a-custom-delivery-channel-4.png)

   >[!NOTE]
   >
   >Om det här är din enda leveranskanal tilldelas den automatiskt till alla dina e-postidentiteter, och du gör det här. Om detta inte är den enda leveranskanalen, fortsätt till steg 5.

1. Klicka [!UICONTROL Email Settings] medan du fortfarande är i **[!UICONTROL Address and Signature]**.

   ![](assets/setting-up-a-custom-delivery-channel-5.png)

1. Leta reda på e-postidentiteten som du vill välja en leveranskanal för och klicka på **[!UICONTROL Choose Delivery Channel]**.

   ![](assets/setting-up-a-custom-delivery-channel-6.png)

1. Klicka på [!UICONTROL Deliverability] i **[!UICONTROL Edit]**-kortet.

   ![](assets/setting-up-a-custom-delivery-channel-7.png)

1. Klicka på listrutan [!UICONTROL Channel] och välj den anpassade leveranskanal som du just lade till. Klicka på **[!UICONTROL Save]**.

   ![](assets/setting-up-a-custom-delivery-channel-8.png)

   >[!NOTE]
   >
   >Om teamadministratören konfigurerar teamets SMTP-server gäller den automatiskt bara din standardidentitet för e-post och är tillgänglig som ett alternativ för dina andra e-postidentiteter.

## Team SMTP-server {#team-smtp-server}

>[!NOTE]
>
>**Administratörsbehörigheter krävs**

1. Logga in på [webbprogrammet](https://toutapp.com/login), klicka på kugghjulsikonen uppe till höger och välj **[!UICONTROL Settings]**.

   ![](assets/setting-up-a-custom-delivery-channel-9.png)

1. Klicka på [!UICONTROL Admin Settings] under **[!UICONTROL General]**.

   ![](assets/setting-up-a-custom-delivery-channel-10.png)

1. Klicka på **[!UICONTROL Team Delivery Channel]**.

   ![](assets/setting-up-a-custom-delivery-channel-11.png)

1. Ange dina [!UICONTROL SMTP Server]-inloggningsuppgifter och klicka på **[!UICONTROL Connect]**.

   ![](assets/setting-up-a-custom-delivery-channel-12.png)

   >[!NOTE]
   >
   >Teamets SMTP-server kommer att vara standardleveranskanalen för standardidentiteten för e-post för alla teammedlemmar. Dessutom kommer den att vara tillgänglig som ett alternativ för leveranskanal för alla andra e-postidentiteter.

   >[!MORELIKETHIS]
   >
   >* [E-postanslutning för Gmail-användare](/help/marketo/product-docs/marketo-sales-connect/email-plugins/gmail/email-connection-for-gmail-users.md)
   >
   >* [E-postanslutning för [!DNL Outlook] användare](/help/marketo/product-docs/marketo-sales-connect/email-plugins/msc-for-outlook/email-connection-for-outlook-users.md)
