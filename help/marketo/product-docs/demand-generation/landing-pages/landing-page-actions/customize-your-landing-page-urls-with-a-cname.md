---
unique-page-id: 2359746
description: Anpassa dina URL:er för landningssidor med en CNAME - Marketo Docs - produktdokumentation
title: Anpassa URL:er för landningssidor med en CNAME
exl-id: 2cd87785-61e5-46cd-b1e0-6fbc145014d4
source-git-commit: 72e1d29347bd5b77107da1e9c30169cb6490c432
workflow-type: tm+mt
source-wordcount: '254'
ht-degree: 0%

---

# Anpassa URL:er för landningssidor med en CNAME {#customize-your-landing-page-urls-with-a-cname}

Även om Marketo är värd för dina landningssidor kan webbadressen anpassas helt. Hur det ser ut utan CNAME:

`https://na-sj02.marketo.com/lp/mktodemoaccount126/UnsubscribePage.html`

Så här ska det se ut:

`https://go.YourCompany.com/UnsubscribePage.html`

## Välj en CNAME {#choose-a-cname}

Välj ett ord som du vill gå till början av URL:en för dina landningssidor. Det är bara ett ord och borde vara ganska kort. Exempel:

* go.YourCompany.com/NameOfPage.html
* info.YourCompany.com/NameOfPage.html
* pages.YourCompany.com/NameOfPage.html

Det enda ordet (plus YourCompany.com) kallas för CNAME. Du behöver det här senare, så notera det.

## Hitta din kontosträng {#find-your-account-string}

1. Gå till **Administratör** område och klicka på **Landningssidor**.

   ![](assets/image2014-9-18-16-3a2-3a45.png)

   >[!NOTE]
   >
   >**Administratörsbehörigheter krävs**

1. Under **Landning** **Sidor** -fliken, kopiera **Konto** **Sträng** från **Inställningar** -avsnitt.

   ![](assets/image2014-9-18-16-3a44-3a12.png)

1. Du kommer också att behöva det senare, så notera det.

## Skicka begäran till IT {#send-request-to-it}

Be din IT-personal att installera följande CNAME: (Ersätt ordet [CNAME] och [KONTOSTRÄNG] med texten från föregående steg.)

[CNAME].YourCompany.com > [KONTOSTRÄNG].mktoweb.com

## Slutför CNAME-installationen {#complete-cname-setup}

1. När IT-avdelningen har skapat CNAME går du till **Administratör** och klicka på **Landningssidor**.

   ![](assets/image2014-9-18-17-3a15-3a11.png)

1. Under **Inställningar** avsnitt, klicka på **Redigera**.

   ![](assets/image2014-9-18-17-3a15-3a18.png)

1. Ange CNAME i **Domännamn för landningssidor**, ange **Reservsida**, ange **Hemsida** och klicka **Spara**.

   ![](assets/image2014-9-18-17-3a15-3a25.png)

>[!NOTE]
>
>Din reservsida är den sida som leder om Marketo landningssida inte är tillgänglig.

Snyggt jobb! Dina landningssidor är nu märkta med din företagsdomän.
