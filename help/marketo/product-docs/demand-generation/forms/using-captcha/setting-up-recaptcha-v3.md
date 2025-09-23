---
description: Konfigurera reCAPTCHA v3 - Marketo Docs - Produktdokumentation
title: Konfigurera reCAPTCHA v3
exl-id: 235a2688-59a8-4827-a929-a07f3ae06988
feature: Forms
source-git-commit: 09a656c3a0d0002edfa1a61b987bff4c1dff33cf
workflow-type: tm+mt
source-wordcount: '304'
ht-degree: 0%

---

# Konfigurerar [!UICONTROL reCAPTCHA v3] {#setting-up-recaptcha-v3}

ReCAPTCHA v3 är en friktionslös upplevelse som gör att man kan få fram inskickade formulär baserat på hur misstänkt de är utan att behöva använda text, bilder eller knappar. [Läs mer](https://developers.google.com/search/blog/2018/10/introducing-recaptcha-v3-new-way-to){target="_blank"}.

## Hämta din [!UICONTROL Data Center] och [!UICONTROL Munchkin ID] {#retrieve-your-data-center-and-munchkin-id}

För steg 6 i det inledande konfigurationsavsnittet för [!UICONTROL reCAPTCHA v3] nedan behöver du din Marketo Engage-prenumerations [!UICONTROL Data Center] och [!UICONTROL Munchkin ID]. Så här hittar du dem.

1. Klicka på **[!UICONTROL Admin]** i Marketo.

   ![](assets/setting-up-recaptcha-v3-1.png)

1. Klicka på **[!UICONTROL My Account]**.

   ![](assets/setting-up-recaptcha-v3-2.png)

1. Bläddra ned till [!UICONTROL Support Information].

   ![](assets/setting-up-recaptcha-v3-3.png)

## Inledande [!UICONTROL reCAPTCHA v3]-konfiguration {#initial-recaptcha-v3-setup}

Följande steg utförs utanför Marketo.

1. Gå till [https://www.google.com/recaptcha/about/](https://www.google.com/recaptcha/about/){target="_blank"} och klicka på v3 Admin Console.

1. Logga in/registrera dig med ett Google-konto.

1. Klicka på knappen [!UICONTROL Create] (+-tecken) för att skapa en ny nyckel.

1. Skapa en etikett som identifierar vilken nyckel som ska användas för Marketo Engage.

1. Välj typen **[!UICONTROL reCAPTCHA v3]**. Marketo Engage stöder för närvarande inte reCAPTCHA v2.

1. Lägg till de domäner som Marketo Engage-prenumerationen använder. Domäner som inte anges här returnerar fel i formulär där reCAPTCHA är aktiverat. Kom ihåg att ersätta orden &#39;datacenter&#39; och &#39;munchkinID&#39; med [data i din prenumeration](#retrieve-your-data-center-and-munchkin-id).

   * app-datacenter.marketo.com
   * munchkinID.mktoweb.com
   * alla domäner och alias för landningssidor som konfigurerats i prenumerationen

   >[!NOTE]
   >
   >Om till exempel ditt kontos [!UICONTROL Data Center] är &quot;sjst&quot; är domänen du tillåtslista `app-sjst.marketo.com`. Om [!UICONTROL Munchkin ID] är 123-ABC-789 är domänen du tillåtslista `123-ABC-789.mktoweb.com`.

1. Ange en ägare och ytterligare e-postadress som ska ta emot varningar om den här tjänsten.

1. Godkänn villkoren för reCAPTCHA.

1. Klicka på **[!UICONTROL Submit]**.

   >[!NOTE]
   >
   >Ha webbplatsnyckeln och den hemliga nyckeln till hands för Marketo Engage-konfigurationen.

## Konfigurera CAPTCHA i Marketo Engage {#setting-up-captcha-in-marketo-engage}

>[!IMPORTANT]
>
>När du har utfört de här stegen och [aktiverat CAPTCHA i ditt första Marketo-formulär](/help/marketo/product-docs/demand-generation/forms/using-captcha/enable-captcha-in-marketo-forms.md){target="_blank"} måste du testa formuläret omedelbart, eftersom alla typer av felkonfigurationer i reCAPTCHA-inställningarna kan bryta formuläret.

1. Klicka på **[!UICONTROL Admin]** i Marketo.

   ![](assets/setting-up-recaptcha-v3-4.png)

1. Välj **[!UICONTROL CAPTCHA]** i trädet.

   ![](assets/setting-up-recaptcha-v3-5.png)

1. Klicka på **[!UICONTROL Edit]** på inställningarna för [!UICONTROL CAPTCHA].

   ![](assets/setting-up-recaptcha-v3-6.png)

1. Klicka på listrutan [!UICONTROL CAPTCHA] och välj [!UICONTROL reCAPTCHA v3].

   ![](assets/setting-up-recaptcha-v3-7.png)

1. Infoga **[!UICONTROL Secret Key]** och **[!UICONTROL Site Key]**. Klicka på **[!UICONTROL Save]** när du är klar.

   ![](assets/setting-up-recaptcha-v3-8.png)

>[!MORELIKETHIS]
>
>[Aktivera CAPTCHA i Marketo Forms](/help/marketo/product-docs/demand-generation/forms/using-captcha/enable-captcha-in-marketo-forms.md)
