---
unique-page-id: 10617187
description: Sekretessinställningar - Marketo Docs - produktdokumentation
title: Sekretessinställningar
exl-id: 1fde9011-02a9-4ec9-bfa4-c56a52ce1eed
translation-type: tm+mt
source-git-commit: 72e1d29347bd5b77107da1e9c30169cb6490c432
workflow-type: tm+mt
source-wordcount: '521'
ht-degree: 0%

---

# Sekretessinställningar {#understanding-privacy-settings}

## Översikt {#overview}

Marketo ger marknadsförarna ett sätt att få webbbesökarnas samtycke att spåra dem. Det finns två sätt att avanmäla dig, eller så kan du välja att spåras med anonymiserad IP.

* Webbbesökare väljer funktionen Do Not Track (DNT) i sin webbläsare (och marknadsföraren följer webbbesökarens begäran om Do Not Track)
* Webbbesökare använder en avanmälningscookie som tillhandahålls av en marknadsförare på en webbplats

Marknadsföraren kan också spåra användare, men använda en anonym IP-adress.

Dessa metoder kan påverka Marketo värde och funktionalitet inom vissa områden. Om marknadsföraren *inte* ändrar något i Marketo-konfigurationen är dock Marketo-funktionen densamma.

## Webbläsarinställningar för Do Not Track {#browser-settings-for-do-not-track}

Webbbesökarna kan ställa in sin webbläsare så att de inte kan spåras av någon webbplats genom att välja&quot;Do Not Track&quot; (DNT). Detta förhindrar spårning för just den webbläsaren och enheten. Mer information finns i webbläsarens sekretessinställningar.

I Munchkin kan en marknadsförare [avgöra om webbläsarens DNT-inställning ska stödjas eller ignoreras.](/help/marketo/product-docs/administration/settings/edit-do-not-track-browser-support-settings.md)

Vid webbanpassning kan en marknadsförare bestämma om han/hon ska [ha stöd för eller ignorera webbläsarens DNT-inställning](/help/marketo/product-docs/web-personalization/getting-started/setting-web-personalization-to-do-not-track.md).

## Välj ut från en specifik webbplats {#opt-out-from-a-specific-website}

Du kan också tillåta webbplatsbesökare att välja bort webbplatsspårning från din webbplats, oavsett om inställningarna **Webbläsare spårar inte** är konfigurerade eller inte. På så sätt kan besökaren ange sina spårningsinställningar direkt från webbplatsen.

För att kunna göra detta måste du lägga till en parameter i en länk för avanmälan på en webbsida som har aktiverad automatisk spårning. Det kan vara vilken webbsida som helst, men webbsidans länk måste innehålla följande parameter:

?marketo_opt_out=true

Nedan visas exempel på en webbsida med en länk för att avanmäla sig och en landningssida för när länken har klickats. Din kommer att variera.

Här är en webbsida med en knapp med parametern &quot;?marketo_opt_out=true&quot; i länken opt-out.

![](assets/opt-out-1.png)

Du kan skapa och publicera en landningssida som en uppföljningssida för när du klickar på länken med parametern&quot;?marketo_opt_out=true&quot;.

![](assets/opt-out-2.png)

När du klickar på länken lägger Marketo till en cookie med namnet **mkto_opt_out** i besökarens webbläsare som inaktiverar Munchkin-spårning för den besökare som klickar på länken med ovanstående parameter.

Verifiera att du är en cookie och klicka på länken för att bekräfta att cookien kan placeras. Kontrollera sedan dina webbläsarcookies för att bekräfta att **mkto_opt_out**-cookien har lagts till.

![](assets/opt-out-3.png)

>[!NOTE]
>
>Detta fungerar för närvarande endast med Munchkin version 152 och senare.

## Anmäl dig till {#opt-in}

Marknadsförarna kan ge användare möjlighet att anmäla sig genom att använda Marketo funktioner för e-post, formulär, landningssidor och andra metoder.

## Spåra med hjälp av en anonym IP {#tracking-using-an-anonymized-ip}

Marknadsförarna kan skydda sin integritet genom att spåra användare med en anonym IP-adress. Det gör du genom att lägga till den här koden i RTP- eller Munchkin Javascript-filen som är inbäddad på webbplatsen.

* För Munchkin lägger du bara till {&quot;anonymizeIP&quot;,true} i init-funktionen.

   >[!NOTE]
   >
   >Om du använder den här parametern måste Munchkin V2 vara aktiverat. Kontakta [Marketo Support](https://nation.marketo.com/community/support_solutions) om du vill aktivera den för din prenumeration.

* För Webbanpassning (RTP) lägger du till detta i javascript-filen:

`anonymize IP : before calling rtp('send','view'); add rtp('set', 'settings', {'anonymizeIP' : true});`
