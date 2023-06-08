---
unique-page-id: 2360189
description: Anpassa dina URL:er för landningssidor med en CNAME (Administration) - Marketo Docs - Produktdokumentation
title: Anpassa URL:er för landningssidor med en CNAME (administration)
exl-id: a5aa1c76-15f7-4e8c-a736-77c79f65c368
source-git-commit: b71729a678ff4a676bb60803d845d0a44118f7e5
workflow-type: tm+mt
source-wordcount: '230'
ht-degree: 0%

---

# Anpassa URL:er för landningssidor med en CNAME  {#customize-your-landing-page-urls-with-a-cname}

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

1. Gå till **[!UICONTROL Admin]** område.

   ![](assets/customize-your-landing-page-urls-with-a-cname-1.png)

1. Klicka på **[!UICONTROL Landing Pages]**.

   ![](assets/customize-your-landing-page-urls-with-a-cname-2.png)

1. Under **[!UICONTROL Landing Pages]** kopierar du kontosträngen från avsnittet Inställningar.

   ![](assets/customize-your-landing-page-urls-with-a-cname-3.png)

1. Du kommer också att behöva det här senare, så notera det.

1. Skicka förfrågan till IT.

1. Be din IT-personal att installera följande CNAME (ersätt ordet [CNAME] och [KONTOSTRÄNG] med texten från föregående steg):

   [CNAME].YourCompany.com > [KONTOSTRÄNG].mktoweb.com

1. Slutför CNAME-installationen.

1. När IT-avdelningen har skapat CNAME går du tillbaka till **[!UICONTROL Admin]** område.

   ![](assets/customize-your-landing-page-urls-with-a-cname-4.png)

1. Klicka på **[!UICONTROL Landing Pages]**.

   ![](assets/customize-your-landing-page-urls-with-a-cname-5.png)

1. Under **[!UICONTROL Settings]** avsnitt, klicka **[!UICONTROL Edit]**.

   ![](assets/customize-your-landing-page-urls-with-a-cname-6.png)

1. Ange CNAME i **[!UICONTROL Domain name for Landing Pages]**, ange **[!UICONTROL Fallback page]**, ange **[!UICONTROL Homepage]** och klicka **[!UICONTROL Save]**.

   ![](assets/customize-your-landing-page-urls-with-a-cname-7.png)

På din reservsida omdirigeras personer om din Marketo-landningssida inte är tillgänglig.

Snyggt jobb! Dina landningssidor är nu märkta med din företagsdomän.
