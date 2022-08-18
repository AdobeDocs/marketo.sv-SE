---
description: Konfigurera reCAPTCHA v3 - Marketo Docs - Produktdokumentation
title: Konfigurera reCAPTCHA v3
hide: true
hidefromtoc: true
exl-id: 235a2688-59a8-4827-a929-a07f3ae06988
source-git-commit: 24942664d613fa2851bad7a0dd3862027deacf37
workflow-type: tm+mt
source-wordcount: '0'
ht-degree: 0%

---

# Konfigurera reCAPTCHA v3 {#setting-up-recaptcha-v3}

Intro Text

## Inledande konfiguration av reCAPTCHA v3 {#initial-recaptcha-v3-setup}

Text: Beskriv v3 - följande steg utförs utanför Marketo Engage.

1. Gå till [https://www.google.com/recaptcha/about/](https://www.google.com/recaptcha/about/){target=&quot;_blank&quot;} och klicka på v3 Admin Console.

1. Logga in/registrera dig med ett Google-konto.

1. Klicka på knappen Skapa (+-tecken) för att skapa en ny nyckel.

1. Skapa en etikett som identifierar vilken nyckel som ska användas för Marketo Engage.

1. Välj typ **reCAPTCHA v3**. Marketo Engage stöder för närvarande inte reCAPTCHA v2.

1. Lägg till varje domän som används av Marketo Engage-prenumerationen. Domäner som inte anges här returnerar fel i formulär där reCAPTCHA är aktiverat.

   * 123-ABC-456.mktoweb.com
   * app-pod.marketo.com
   * alla domäner och alias för landningssidor som konfigurerats i prenumerationen

1. Ange en ägare och ytterligare e-postadress som ska ta emot varningar om den här tjänsten.

1. Godkänn villkoren för reCAPTCHA.

1. Klicka **Skicka**.

>[!NOTE]
>
>Ha webbplatsnyckeln och den hemliga nyckeln till hands för Marketo Engage-konfigurationen.

## Konfigurera CAPTCHA i Marketo Engage {#setting-up-captcha-in-marketo-engage}

1. I Marketo klickar du på **Administratör**.

   ![](assets/setting-up-recaptcha-v3-1.png)

1. Välj **CAPTCHA** i trädet.

   ![](assets/setting-up-recaptcha-v3-2.png)

1. Klicka **Redigera** på CAPTCHA-inställningar.

   ![](assets/setting-up-recaptcha-v3-3.png)

1. Klicka på listrutan CAPTCHA och välj reCAPTCHA v3.

   ![](assets/setting-up-recaptcha-v3-4.png)

1. Infoga hemlig nyckel och platsnyckel. Klicka **Spara** när det är klart.

   ![](assets/setting-up-recaptcha-v3-5.png)
