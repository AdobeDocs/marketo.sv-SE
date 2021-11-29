---
description: Konfigurera en anpassad leveranskanal - Marketo Docs - produktdokumentation
title: Konfigurera en anpassad leveranskanal
hide: true
hidefromtoc: true
source-git-commit: 55afdc537d0a5d0b6114f478c4dd2ded09c84e34
workflow-type: tm+mt
source-wordcount: '409'
ht-degree: 0%

---

# Konfigurera en anpassad leveranskanal {#setting-up-a-custom-delivery-channel}

Med Marketo Sales Connect kan ni integrera med en anpassad SMTP-server för att leverera e-postmeddelanden. Detta är ett bra alternativ för dem som inte vill skicka massutskick via Gmail eller Exchange.

Användare kan konfigurera en anpassad SMTP-server för egen användning, eller så kan administratörer konfigurera en Team SMTP som ska delas av alla Sales Connect-användare i din instans.

>[!NOTE]
>
>* Förutom att konfigurera SMTP-servern kan du [mejlidentitet måste verifieras](/help/marketo/product-docs/marketo-sales-connect/getting-started/email-settings/verify-your-email.md) innan du kan skicka e-post.
>* Vi rekommenderar att du samarbetar med IT-teamet eller SMTP-serverleverantören för att få rätt serverautentiseringsuppgifter för din SMTP-server.
>* Du kan inte ansluta Gmail- och Exchange-servern med autentiseringsuppgifterna för SMTP-servern. Använd vår e-postanslutningstjänst för att integrera med dessa leverantörer.


## Anpassad SMTP {#custom-smtp}

1. Logga in på [webbprogram](https://toutapp.com/login), klicka på kugghjulsikonen längst upp till höger och välj **Inställningar**.

PICC

1. Under Mitt konto klickar du på **E-postinställningar**.

PICC

1. Klicka **Anpassad leveranskanal**.

PICC

1. Ange dina autentiseringsuppgifter för SMTP-servern och klicka på **Anslut**.

PICC

>[!NOTE]
>
>Om det här är din enda leveranskanal tilldelas den automatiskt till alla dina e-postidentiteter, och du gör det här. Om detta inte är den enda leveranskanalen, fortsätt till steg 5.

1. Klicka på Fortsätt i e-postinställningarna **Adress och signatur**.

PICC

1. Leta reda på e-postadressen som du vill välja en leveranskanal för och klicka på **Välj leveranskanal**.

PICC

1. Klicka på Leveranskort **Redigera**.

PICC

1. Klicka på listrutan Kanal och välj den anpassade leveranskanal som du just lade till. Klicka **Spara**.

PICC

>[!NOTE]
>
>Om teamadministratören konfigurerar teamets SMTP-server gäller den automatiskt bara din standardidentitet för e-post och är tillgänglig som ett alternativ för dina andra e-postidentiteter.

## Team SMTP-server {#team-smtp-server}

>[!NOTE]
>
>**Administratörsbehörigheter krävs**

1. Logga in på [webbprogram](https://toutapp.com/login), klicka på kugghjulsikonen längst upp till höger och välj **Inställningar**.

PICC

1. Under Administratörsinställningar klickar du på **Allmänt**.

PICC

1. Klicka **Teamleveranskanal**.

PICC

1. Ange dina autentiseringsuppgifter för SMTP-servern och klicka på **Anslut**.

PICC

>[!NOTE]
>
>Teamets SMTP-server kommer att vara standardleveranskanalen för standardidentiteten för e-post för alla teammedlemmar. Dessutom kommer den att vara tillgänglig som ett alternativ för leveranskanal för alla andra e-postidentiteter.

>[!MORELIKETHIS]
>
>* [E-postanslutning för Gmail-användare](/help/marketo/product-docs/marketo-sales-connect/email-plugins/gmail/email-connection-for-gmail-users.md)
>* [E-postanslutning för Outlook-användare](/help/marketo/product-docs/marketo-sales-connect/email-plugins/msc-for-outlook/email-connection-for-outlook-users.md)

