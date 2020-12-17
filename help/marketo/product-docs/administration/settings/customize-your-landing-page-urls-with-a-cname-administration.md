---
unique-page-id: 2360189
description: Anpassa dina URL:er för landningssidor med en CNAME (Administration) - Marketo Docs - Produktdokumentation
title: Anpassa URL:er för landningssidor med en CNAME (administration)
translation-type: tm+mt
source-git-commit: e149133a5383faaef5e9c9b7775ae36e633ed7b1
workflow-type: tm+mt
source-wordcount: '251'
ht-degree: 0%

---


# Anpassa URL:er för landningssidor med en CNAME (administration) {#customize-your-landing-page-urls-with-a-cname-administration}

Även om Marketo är värd för dina landningssidor bör URL:en anpassas för ditt företag.

>[!NOTE]
>
>Ingen CNAME:
>
>https://na-sj02.marketo.com/lp/mktodemoaccount126/UnsubscribePage.html
>
>CNAME:
>
>https://go.**Ditt företag**.com/UnsuscribePage.html

>[!NOTE]
>
>**Administratörsbehörigheter krävs**

Kom så sätter vi igång!

1. Välj en CNAME.

   Det är den främre delen av URL:en. Exempel:

   * **go**.YourCompany.com/NameOfPage.html
   * **info**.YourCompany.com/NameOfPage.html
   * **sidor**.YourCompany.com/NameOfPage.html

   Det enda ordet (plus YourCompany.com) kallas för CNAME. Du behöver det här senare så notera det.

1. Hitta din kontosträng.

1. Gå till området **Admin** och klicka på **Startsidor**.

   ![](assets/image2014-9-16-13-3a9-3a44.png)

1. Under fliken **Landningssidor** kopierar du kontosträngen från avsnittet Inställningar.

   ![](assets/image2014-9-16-13-3a9-3a57.png)

1. Du kommer också att behöva det här senare, så notera det.

1. Skicka förfrågan till IT.

1. Be din IT-personal att installera följande CNAME (ersätt ordet [CNAME] och [KONTOSTRING] med texten från föregående steg):

   [CNAME].YourCompany.com >  [ACCOUNT STRING].mktoweb.com

1. Slutför CNAME-installationen.

1. När IT-avdelningen har skapat CNAME går du till **Admin** och klickar på **landningssidor**.

   ![](assets/image2014-9-16-13-3a10-3a14.png)

1. Klicka på **Redigera** under **Inställningar**.

   ![](assets/image2014-9-16-13-3a10-3a31.png)

1. Ange ditt CNAME-konto i **Domännamn för landningssidor**, ange din **återställningssida**, ange din **startsida** och klicka på **Spara**.

   ![](assets/image2014-9-16-13-3a10-3a45.png)

På din reservsida omdirigeras personer om din Marketo-landningssida inte är tillgänglig.

Snyggt jobb! Dina landningssidor är nu märkta med din företagsdomän.
