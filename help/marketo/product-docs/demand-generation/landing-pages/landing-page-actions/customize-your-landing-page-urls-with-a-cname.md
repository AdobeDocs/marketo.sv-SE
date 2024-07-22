---
unique-page-id: 2359746
description: Anpassa dina URL:er för landningssidor med en CNAME - Marketo Docs - produktdokumentation
title: Anpassa URL:er för landningssidor med en CNAME
exl-id: 2cd87785-61e5-46cd-b1e0-6fbc145014d4
feature: Landing Pages
source-git-commit: 431bd258f9a68bbb9df7acf043085578d3d91b1f
workflow-type: tm+mt
source-wordcount: '237'
ht-degree: 0%

---

# Anpassa URL:er för landningssidor med en CNAME {#customize-your-landing-page-urls-with-a-cname}

Även om Marketo är värd för dina landningssidor kan URL:en anpassas helt. Hur det ser ut utan CNAME:

`https://na-sj02.marketo.com/lp/mktodemoaccount126/UnsubscribePage.html`

Så här ska det se ut:

`https://go.YourCompany.com/UnsubscribePage.html`

## Välj en CNAME {#choose-a-cname}

Välj ett ord som du vill gå till början av URL:en för dina landningssidor. Det är bara ett ord och borde vara ganska kort. Exempel:

* go.YourCompany.com/NameOfPage.html
* info.YourCompany.com/NameOfPage.html
* pages.YourCompany.com/NameOfPage.html

Det enda ordet (plus YourCompany.com) kallas för CNAME. Du behöver det här senare, så notera det.

## Hitta ditt Munchkin-ID {#find-your-munchkin-id}

1. Gå till området **Admin**.

   ![](assets/customize-your-landing-page-urls-with-a-cname-1.png)

1. Klicka på **Mitt konto**.

   ![](assets/customize-your-landing-page-urls-with-a-cname-2.png)

   >[!NOTE]
   >
   >**Administratörsbehörigheter krävs**

1. Bläddra ned till &quot;Support Information&quot; och kopiera ditt Munchkin-ID.

   ![](assets/customize-your-landing-page-urls-with-a-cname-3.png)

## Skicka begäran till IT {#send-request-to-it}

Be din IT-personal att installera följande CNAME: (Ersätt ordet [CNAME] och [Munchkin ID] med texten från föregående steg.)

[CNAME].YourCompany.com > [Munchkin ID].mktoweb.com

## Slutför CNAME-installationen {#complete-cname-setup}

1. Gå till **Admin** när din IT-avdelning har skapat CNAME.

   ![](assets/customize-your-landing-page-urls-with-a-cname-4.png)

1. Klicka på **Landningssidor**.

   ![](assets/customize-your-landing-page-urls-with-a-cname-5.png)

1. Klicka på **Redigera** under avsnittet **Inställningar**.

   ![](assets/customize-your-landing-page-urls-with-a-cname-6.png)

1. Ange ditt CNAME-konto i **Domännamn för landningssidor**, ange din **återställningssida**, ange din **startsida** och klicka på **Spara**.

   ![](assets/customize-your-landing-page-urls-with-a-cname-7.png)

>[!NOTE]
>
>Din reservsida är den sida som leder om Marketo landningssida inte är tillgänglig.

Snyggt jobb! Dina landningssidor är nu märkta med din företagsdomän.
