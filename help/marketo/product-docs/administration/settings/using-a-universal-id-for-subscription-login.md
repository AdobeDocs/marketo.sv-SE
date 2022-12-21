---
unique-page-id: 10100311
description: Använda ett universellt ID för prenumerationsinloggning - Marketo Docs - produktdokumentation
title: Använda ett universellt ID för prenumerationsinloggning
exl-id: 75cf1323-0468-49e9-83ca-e55aa30744ac
source-git-commit: d5c1c1d0ce2a521898eaa4f6610bf1ce04b4f66b
workflow-type: tm+mt
source-wordcount: '586'
ht-degree: 0%

---

# Använda ett universellt ID för prenumerationsinloggning {#using-a-universal-id-for-subscription-login}

Med ett universellt ID kan du komma åt flera Marketo-prenumerationer med en enda inloggning och snabbt växla mellan prenumerationer. Du kan dock använda olika inloggningar för dina prenumerationer om du vill.

Med Universal ID kan du fortfarande skapa supportärenden för varje enskild prenumeration.

Prenumerationsnivåinställningarna gäller för användare som använder Universal ID, till exempel roller, behörigheter och lösenordsprinciper. Ändringar på användarprofilnivå återspeglas i alla prenumerationer, till exempel förnamn, efternamn och e-postadress.

## Konfigurera ett universellt ID {#setting-up-a-universal-id}

Alla Marketo-prenumerationer har den valfria funktionen Universal ID. Från varje enskild instans måste din Marketo-administratör bjuda in dig till alla dina olika prenumerationer med samma inloggning. Marketo kan inte sammanfoga dina befintliga inloggningar automatiskt.

>[!NOTE]
>
>Om du har flera inloggnings-ID:n för prenumeration kan du även ha flera communityprofiler. Var noga med att välja ID:t för ditt universella ID som är anslutet till profilen som du vill använda, och det är för din produktionsinstans, inte din sandlåda.

## Loggar in {#logging-in}

När du loggar in för att acceptera en inbjudan till en andra prenumeration med ett universellt ID visas inloggningssidan för anmälan. Här måste du markera en kryssruta för att godkänna villkoren. När du har accepterat visas sidan för normal återställning, inte den här, för alla efterföljande inloggningar. Genom att acceptera villkoren tillåter du att Marketo distribuerar dina grundläggande profildata (som förnamn, efternamn och e-postadress) till datacentralerna på olika platser där din prenumeration finns.

![](assets/new-login-reduced-hands-name.png)

>[!TIP]
>
>ID:n som du inte längre använder finns kvar såvida inte prenumerationsadministratören tar bort dem. Vi rekommenderar att du behåller dem, om du till exempel har en privat rapport som du själv har tilldelats, som bara kan nås med det ID:t. I det här fallet är det bra att flytta dessa privata rapporter till ditt nya Universal ID och sedan ta bort ditt befintliga ID.

## Lösenord {#passwords}

Med Universal ID för flera prenumerationer tillämpar Marketo automatiskt den striktaste lösenordsprincipen. Om vissa prenumerationer till exempel kräver en minimilängd för lösenord och andra inte gör det, kommer minimilängden att gälla för alla prenumerationer.

Med ett universellt ID för flera prenumerationer kan bara du ändra lösenordet.

>[!NOTE]
>
>Marketo ber användare som vill använda ett universellt ID att återställa sitt lösenord om den aktuella prenumerationens lösenord inte uppfyller lösenordsprincipen för den andra prenumerationen som de bjuds in till.

## Växla mellan prenumerationer {#switching-between-subscriptions}

Med ett universellt ID kan du se den prenumeration du är inloggad på och välja andra prenumerationer som du har inloggningsåtkomst till. I de flesta fall kan du växla mellan dem utan att behöva logga ut och in igen.

![](assets/image2016-11-3-15-3a10-3a16.png)

När du loggar ut och in igen loggar Marketo automatiskt in dig på den prenumeration du senast var inloggad på. Du kan sedan byta till en annan prenumeration om det behövs.

## Community-profiler {#community-profiles}

Om du har flera prenumerationer kan du ha flera communityprofiler. Vi rekommenderar att du väljer den inloggning som är länkad till din mest aktiva community-profil.

## Mobilplattform {#mobile-platform}

Användare med ett universellt ID kan se sina data på Marketo Moments och iPad-programmet för händelseincheckning från den prenumeration som de senast loggat in på. Du kan inte ändra prenumerationer från själva mobilplattformen.

>[!MORELIKETHIS]
>
>* [Lägg till enkel inloggning på en portal](/help/marketo/product-docs/administration/additional-integrations/add-single-sign-on-to-a-portal.md)
>* [Begränsa användarinloggning till enbart enkel inloggning](/help/marketo/product-docs/administration/additional-integrations/restrict-user-login-to-sso-only.md)
>* [Bjud in Marketo-användare till två instanser med Universal ID](https://nation.marketo.com/t5/Knowledgebase/Inviting-Marketo-Users-to-Two-Instances-with-Universal-ID-UID/ta-p/251122)

