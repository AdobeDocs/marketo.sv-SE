---
description: Konfigurera reCAPTCHA v3 - Marketo Docs - Produktdokumentation
title: Konfigurera reCAPTCHA v3
exl-id: 235a2688-59a8-4827-a929-a07f3ae06988
source-git-commit: 457b4aadac47b0a8614c3e6025d2e1ae287b5ecc
workflow-type: tm+mt
source-wordcount: '354'
ht-degree: 0%

---

# Konfigurera reCAPTCHA v3 {#setting-up-recaptcha-v3}

ReCAPTCHA v3 är en friktionslös upplevelse som gör att man kan få fram inskickade formulär baserat på hur misstänkt de är utan att behöva använda text, bilder eller knappar. [Läs mer](https://developers.google.com/search/blog/2018/10/introducing-recaptcha-v3-new-way-to){target=&quot;_blank&quot;}.

## Hämta ditt datacenter- och Munchkin-ID {#retrieve-your-data-center-and-munchkin-id}

För steg 6 i det inledande konfigurationsavsnittet för reCAPTCHA v3 nedan behöver du Marketo Engage prenumerationens datacenter och Munchkin-ID. Så här hittar du dem.

1. I Marketo klickar du på **Administratör**.

   ![](assets/setting-up-recaptcha-v3-1.png)

1. Klicka **Mitt konto**.

   ![](assets/setting-up-recaptcha-v3-2.png)

1. Bläddra ned till supportinformation.

   ![](assets/setting-up-recaptcha-v3-3.png)

## Inledande konfiguration av reCAPTCHA v3 {#initial-recaptcha-v3-setup}

Följande steg utförs utanför Marketo.

1. Gå till [https://www.google.com/recaptcha/about/](https://www.google.com/recaptcha/about/){target=&quot;_blank&quot;} och klicka på v3 Admin Console.

1. Logga in/registrera dig med ett Google-konto.

1. Klicka på knappen Skapa (+-tecken) för att skapa en ny nyckel.

1. Skapa en etikett som identifierar vilken nyckel som ska användas för Marketo Engage.

1. Välj typ **reCAPTCHA v3**. Marketo Engage stöder för närvarande inte reCAPTCHA v2.

1. Lägg till varje domän som används av Marketo Engage-prenumerationen. Domäner som inte anges här returnerar fel i formulär där reCAPTCHA är aktiverat. Kom ihåg att ersätta orden &#39;datacenter&#39; och &#39;munchkinID&#39; med [data i din prenumeration](#retrieve-your-data-center-and-munchkin-id).

   * app-datacenter.marketo.com
   * munchkinID.mktoweb.com
   * alla domäner och alias för landningssidor som konfigurerats i prenumerationen

   >[!NOTE]
   >
   >Om ditt kontos datacenter till exempel är &quot;sjst&quot; är domänen du tillåtslista den `app-sjst.marketo.com`. Om ditt Munchkin-ID är 123-ABC-789 blir domänen du tillåtslista `123-ABC-789.mktoweb.com`.

1. Ange en ägare och ytterligare e-postadress som ska ta emot varningar om den här tjänsten.

1. Godkänn villkoren för reCAPTCHA.

1. Klicka **Skicka**.

   >[!NOTE]
   >
   >Ha webbplatsnyckeln och den hemliga nyckeln till hands för Marketo Engage-konfigurationen.

## Konfigurera CAPTCHA i Marketo Engage {#setting-up-captcha-in-marketo-engage}

>[!IMPORTANT]
>
>När du har utfört dessa steg och [aktivera CAPTCHA i ditt första Marketo-formulär](/help/marketo/product-docs/demand-generation/forms/using-captcha/enable-captcha-in-marketo-forms.md){target=&quot;_blank&quot;} måste du testa formuläret omedelbart, eftersom alla typer av felkonfigurationer i reCAPTCHA-inställningarna kan göra att formuläret bryts.

1. I Marketo klickar du på **Administratör**.

   ![](assets/setting-up-recaptcha-v3-4.png)

1. Välj **CAPTCHA** i trädet.

   ![](assets/setting-up-recaptcha-v3-5.png)

1. Klicka **Redigera** på CAPTCHA-inställningar.

   ![](assets/setting-up-recaptcha-v3-6.png)

1. Klicka på listrutan CAPTCHA och välj reCAPTCHA v3.

   ![](assets/setting-up-recaptcha-v3-7.png)

1. Infoga hemlig nyckel och platsnyckel. Klicka **Spara** när det är klart.

   ![](assets/setting-up-recaptcha-v3-8.png)
