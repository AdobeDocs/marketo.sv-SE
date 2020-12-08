---
unique-page-id: 2359746
description: Anpassa URL:er för landningssidor med en CNAME - Marketo Docs - produktdokumentation
title: Anpassa URL:er för landningssidor med en CNAME
translation-type: tm+mt
source-git-commit: 00887ea53e395bea3a11fd28e0ac98b085ef6ed8
workflow-type: tm+mt
source-wordcount: '273'
ht-degree: 0%

---


# Anpassa URL:er för landningssidor med en CNAME {#customize-your-landing-page-urls-with-a-cname}

Även om Marketo är värd för dina landningssidor kan URL:en anpassas helt. Hur det ser ut utan CNAME:
`<pre data-theme="Confluence">http://na-sj02.marketo.com/lp/mktodemoaccount126/UnsubscribePage.html</pre>` Så här ska det se ut:
`<pre data-theme="Confluence"> http://go.YourCompany.com/UnsubscribePage.html</pre>`

## Välj en CNAME {#choose-a-cname}

Välj ett ord som du vill gå till början av URL:en för dina landningssidor. Det är bara ett ord och borde vara ganska kort. Exempel:

* gå. [YourCompany.com/NameOfPage.html](http://YourCompany.com/NameOfPage.html)
* info. [YourCompany.com/NameOfPage.html](http://YourCompany.com/NameOfPage.html)
* sidor. [YourCompany.com/NameOfPage.html](http://YourCompany.com/NameOfPage.html)

Det enda ordet (plus [YourCompany.com](http://YourCompany.com)) kallas för CNAME. Du behöver det här senare så notera det.

## Hitta din kontosträng {#find-your-account-string}

1. Gå till området **Admin** och klicka på **landningssidor.**

   ![](assets/image2014-9-18-16-3a2-3a45.png)

   >[!NOTE]
   >
   >**Administratörsbehörigheter krävs**

1. Under fliken **Landningssidor** **Sidor** kopierar du **kontots** **sträng** från avsnittet **Inställningar** .

   ![](assets/image2014-9-18-16-3a44-3a12.png)

1. Du kommer också att behöva det senare, så notera det.

## Skicka begäran till IT {#send-request-to-it}

Be din IT-personal att installera följande CNAME: (Ersätt ordet [CNAME] och [KONTOSTRÄNG] med texten från föregående steg.)

[CNAME]. [YourCompany.com](http://yourcompany.com/) > [ACCOUNT STRING]. [mktoweb.com](http://mktoweb.com/)

## Slutför CNAME-installationen {#complete-cname-setup}

1. När IT-avdelningen har skapat CNAME går du till **Admin** och klickar på **Landing** **Pages**.

   ![](assets/image2014-9-18-17-3a15-3a11.png)

1. Klicka på **Redigera** under **Inställningar**.

   ![](assets/image2014-9-18-17-3a15-3a18.png)

1. Ange ditt CNAME-värde i **Domännamn** **för** **Landing** **Pages** ******** ******** ****, ange dinFallback¥page¥, ange din Homepage¥ och klicka på¥Save¥¥.

   ![](assets/image2014-9-18-17-3a15-3a25.png)

>[!NOTE]
>
>Din reservsida är sidan som leads omdirigeras till om Marketo Landing Page inte är tillgänglig.

Snyggt jobb! Dina landningssidor är nu märkta med din företagsdomän.