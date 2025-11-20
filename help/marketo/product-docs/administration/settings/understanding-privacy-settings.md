---
unique-page-id: 10617187
description: Sekretessinställningar - Marketo Docs - produktdokumentation
title: Sekretessinställningar
exl-id: 1fde9011-02a9-4ec9-bfa4-c56a52ce1eed
feature: Administration
source-git-commit: eccf4a66f5d3c581a82a363918b40ae37aa73576
workflow-type: tm+mt
source-wordcount: '479'
ht-degree: 0%

---

# Sekretessinställningar {#understanding-privacy-settings}

## Översikt {#overview}

Marketo ger marknadsförarna ett sätt att få webbbesökarnas samtycke att spåra dem. Det finns två sätt att avanmäla dig, eller så kan du välja att spåras med anonymiserad IP.

* Webbbesökare väljer funktionen Do Not Track (DNT) i sin webbläsare (och marknadsföraren följer webbbesökarens begäran om Do Not Track)
* Webbbesökare använder en avanmälningscookie som tillhandahålls av en marknadsförare på en webbplats

Marknadsföraren kan också spåra användare, men använda en anonym IP-adress.

Dessa metoder kan påverka Marketo värde och funktionalitet inom vissa områden. Om marknadsföraren _inte_ ändrar något i Marketo-konfigurationen ändras inte funktionerna i Marketo.

## Webbläsarinställningar för Do Not Track {#browser-settings-for-do-not-track}

Webbbesökarna kan ställa in sin webbläsare så att de inte kan spåras av någon webbplats genom att välja&quot;Do Not Track&quot; (DNT). Detta förhindrar spårning för just den webbläsaren och enheten. Mer information finns i webbläsarens sekretessinställningar.

I [!DNL Munchkin] kan en markör [bestämma om webbläsarens DNT-inställning ska stödjas eller ignoreras](/help/marketo/product-docs/administration/settings/edit-do-not-track-browser-support-settings.md).

I Web Personalization kan en marknadsförare bestämma om han/hon ska [ha stöd för eller ignorera webbläsarens DNT-inställning](/help/marketo/product-docs/web-personalization/getting-started/setting-web-personalization-to-do-not-track.md).

## Avanmäl dig från en viss webbplats {#opt-out-from-a-specific-website}

Du kan också tillåta besökare att avanmäla sig från webbplatsspårning från din webbplats, oavsett om inställningarna för **Spåra inte webbläsare** har konfigurerats eller inte. På så sätt kan besökaren ange sina spårningsinställningar direkt från webbplatsen.

För att kunna göra detta måste du lägga till en parameter i en länk för avanmälan på en webbsida där [!DNL Munchkin]-spårning är aktiverat. Det kan vara vilken webbsida som helst, men webbsidans länk måste innehålla följande parameter:

?marketo_opt_out=true

Nedan visas exempel på en webbsida med en länk för att avanmäla sig och en landningssida för när länken har klickats. Din kommer att variera.

Här är en webbsida med en knapp med parametern &quot;?marketo_opt_out=true&quot; i länken opt-out.

![](assets/understanding-privacy-settings-1.png)

Du kan skapa och publicera en landningssida som en uppföljningssida för när du klickar på länken med parametern&quot;?marketo_opt_out=true&quot;.

![](assets/understanding-privacy-settings-2.png)

När du klickar på länken lägger Marketo till en cookie med namnet **mkto_opt_out** i besökarens webbläsare som inaktiverar [!DNL Munchkin]-spårning för den besökare som klickar på länken med ovanstående parameter.

Verifiera att du är en cookie och klicka på länken för att bekräfta att cookien kan placeras. Kontrollera sedan dina cookies i webbläsaren för att bekräfta att cookien **mkto_opt_out** har lagts till.

![](assets/understanding-privacy-settings-3.png)

>[!NOTE]
>
>Detta fungerar för närvarande bara med [!DNL Munchkin] version 152 och senare.

## Anmäl dig {#opt-in}

Marknadsförarna kan ge användare möjlighet att anmäla sig genom att använda Marketo funktioner för e-post, formulär, landningssidor och andra metoder.

## Spåra med hjälp av en anonym IP-adress {#tracking-using-an-anonymized-ip}

Marknadsförarna kan skydda sin integritet genom att spåra användare med en anonym IP-adress. Om du vill göra det lägger du till den här koden i RTP- eller [!DNL Munchkin] JavaScript-koden som är inbäddad på webbplatsen.

* För [!DNL Munchkin] lägger du bara till `{"anonymizeIP",true}` i funktionen [init](https://experienceleague.adobe.com/sv/docs/marketo-developer/marketo/javascriptapi/leadtracking/configuration){target="_blank"}.

* För Web Personalization (RTP) lägger du till detta i javascript:

`anonymize IP : before calling rtp('send','view'); add rtp('set', 'settings', {'anonymizeIP' : true});`
