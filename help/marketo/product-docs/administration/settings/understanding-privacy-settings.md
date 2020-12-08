---
unique-page-id: 10617187
description: Understanding Privacy Settings - Marketo Docs - Product Documentation
title: Sekretessinställningar
translation-type: tm+mt
source-git-commit: efadb7eb3845012c273e1a60f9cd98ac884eb543
workflow-type: tm+mt
source-wordcount: '534'
ht-degree: 0%

---


# Sekretessinställningar {#understanding-privacy-settings}

## Översikt {#overview}

Marketo ger marknadsförarna ett sätt att få webbbesökarnas samtycke att spåra dem. Det finns två sätt att avanmäla dig, eller så kan du välja att spåras med anonymiserad IP.

* Webbbesökare väljer funktionen Do Not Track (DNT) i sin webbläsare (och marknadsföraren följer webbbesökarens begäran om Do Not Track)
* Webbbesökare använder en avanmälningscookie som tillhandahålls av en marknadsförare på en webbplats

Marknadsföraren kan också spåra användare, men använda en anonym IP-adress.

Dessa metoder kan påverka Marketos värde och funktionalitet inom specifika områden. Men om marknadsföraren *inte* ändrar något i Marketos konfiguration ändras inte Marketo-funktionen.

## Webbläsarinställningar för Do Not Track {#browser-settings-for-do-not-track}

Webbbesökarna kan ställa in sin webbläsare så att de inte kan spåras av någon webbplats genom att välja&quot;Do Not Track&quot; (DNT). Detta förhindrar spårning för just den webbläsaren och enheten. Mer information finns i webbläsarens sekretessinställningar.

I Munchkin kan en marknadsförare [avgöra om webbläsarens DNT-inställning](edit-do-not-track-browser-support-settings.md)ska stödjas eller ignoreras.

Vid webbanpassning kan en marknadsförare bestämma om han eller hon ska [stödja eller ignorera webbläsarens DNT-inställning](/help/marketo/product-docs/web-personalization/getting-started/setting-web-personalization-to-do-not-track.md).

## Avanmäl dig från en viss webbplats {#opt-out-from-a-specific-website}

Du kan också tillåta besökare att avanmäla sig från webbplatsspårning från din webbplats, oavsett om inställningarna för **webbläsarspårning** har konfigurerats eller inte. På så sätt kan besökaren ange sina spårningsinställningar direkt från webbplatsen.

För att kunna göra detta måste du lägga till en parameter i en länk för avanmälan på en webbsida som har aktiverad automatisk spårning. Det kan vara vilken webbsida som helst, men webbsidans länk måste innehålla följande parameter:

?marketo_opt_out=true

Nedan visas exempel på en webbsida med en länk för att avanmäla sig och en landningssida för när länken har klickats. Din kommer att variera.

Här är en webbsida med en knapp med parametern &quot;?marketo_opt_out=true&quot; i länken opt-out.

![](assets/opt-out-1.png)

Du kan skapa och publicera en landningssida som en uppföljningssida för när du klickar på länken med parametern&quot;?marketo_opt_out=true&quot;.

![](assets/opt-out-2.png)

När du klickar på länken lägger Marketo till en cookie med namnet **mkto_opt_out** i besökarens webbläsare som inaktiverar Munchkin-spårning för den besökare som klickar på länken med ovanstående parameter.

Verifiera att du är en cookie och klicka på länken för att bekräfta att cookien kan placeras. Kontrollera sedan dina cookies i webbläsaren för att bekräfta att **cookien mkto_opt_out** har lagts till.

![](assets/opt-out-3.png)

>[!NOTE]
>
>Detta fungerar för närvarande endast med Munchkin version 152 och senare.

## Anmäl dig {#opt-in}

Marknadsförarna kan göra det möjligt för användare att anmäla sig genom att använda Marketos funktioner för e-post, formulär, landningssidor och andra metoder.

## Spåra med hjälp av en anonym IP {#tracking-using-an-anonymized-ip}

Marknadsförarna kan skydda sin integritet genom att spåra användare med en anonym IP-adress. Det gör du genom att lägga till den här koden i RTP- eller Munchkin Javascript-filen som är inbäddad på webbplatsen.

* För Munchkin lägger du bara till {&quot;anonymizeIP&quot;,true} i init-funktionen.

   >[!NOTE]
   >
   >Om du använder den här parametern måste Munchkin V2 vara aktiverat. Kontakta [Marketo Support](http://nation.marketo.com/community/support_solutions)om du vill aktivera det för din prenumeration.

* För Webbanpassning (RTP) lägger du till detta i javascript-filen:

anonymisera IP: innan du anropar rtp(&#39;send&#39;,&#39;view&#39;); add rtp(&#39;set&#39;, &#39;settings&#39;, {&#39;anonymizeIP&#39; : true});

