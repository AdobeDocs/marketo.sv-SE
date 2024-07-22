---
description: E-postverifiering - Marketo Docs - produktdokumentation
title: E-postverifiering
exl-id: 976e46a7-8c85-45ed-86c1-0c5cdb2d5c3e
feature: Users and Roles
source-git-commit: c5d5fd490fe2800dc7a34d02c73d728e115646a0
workflow-type: tm+mt
source-wordcount: '459'
ht-degree: 0%

---

# E-postverifiering {#email-verification}

Adobe Marketo Engage-prenumerationer kräver att alla användare som inte är API-baserade, inklusive administratörer för Marketo Engage, verifierar sin e-postadress.

## Varför den här funktionen introducerades {#why-this-feature-was-introduced}

Marketo Engage fortsätter lanseringen av e-postverifiering som förberedelse för migrering av kunder till Adobe Business Platform, inklusive användarmigrering till Adobe ID:n. Den här funktionen förbättrar säkerheten för befintliga användarkonton i Marketo Engage. För att en Marketo Engage-användare ska kunna vara kopplad till rätt Adobe ID måste befintliga Marketo Engage-användare verifiera sin e-postadress. En Marketo Engage-användare måste ha en verifierad e-postadress för att kunna migreras till en Adobe ID. Om en Marketo Engage-användare inte verifierar sin e-postadress kan de inte migreras till en Adobe ID och förlorar åtkomsten till en Marketo-prenumeration när användarmigreringen för prenumerationen är klar.

## Användarinbjudan {#user-invite}

När en administratör bjuder in en användare verifieras den användaren automatiskt när han/hon klickar på länken för inbjudan.

>[!IMPORTANT]
>
>Undantaget ovan är _i en prenumeration som endast är avsedd för enkel inloggning_. Administratörer får en ny användarinbjudan, men icke-administratörsanvändare kommer inte att göra det. Användare som inte är administratörer måste fortfarande gå igenom e-postverifieringsprocessen för att säkerställa att deras register migreras. Användarna kan skicka verifieringslänken via e-post genom att gå till **Admin** > **Mitt konto** > **Kontoinställningar** och klicka på **Skicka verifiering igen**.

![](assets/email-verification-1.png)

## Verifierings-e-post {#verification-email}

Användarna får e-postmeddelandet nedan när e-postverifiering aktiveras för en prenumeration, eller om det aktiveras av en administratör/användare.

En aktiv användarsession krävs för e-postverifiering. Användaren måste först logga in på sin Marketo-prenumeration med sin identitetsleverantörs-URL (IdP). När en session har etablerats klickar de _sedan_ på länken **Verifiera e-postadress** i e-postmeddelandet.

![](assets/email-verification-2.png)

>[!TIP]
>
>Om du vill skicka ett bekräftelsemeddelande till en overifierad användare igen markerar du användarens post och klickar på knappen **[!UICONTROL Verify Email]**.

## Ändra en e-postadress {#changing-an-email-address}

När en användares e-postadress ändras blir den inte verifierad. Ett e-postmeddelande skickas till dem där de kan verifiera igen. Användarna kan skicka om e-postmeddelandet manuellt genom att klicka på **[!UICONTROL Resend Verification]**.

![](assets/email-verification-3.png)

![](assets/email-verification-4.png)

## Användare och roller {#users-and-roles}

I kolumnen **[!UICONTROL Admin]** > **[!UICONTROL Users & Roles]** visar e-poststatus verifieringsstatusen för varje användare.

![](assets/email-verification-5.png)

## Inloggnings-ID för flera användare {#multiple-user-login-ids}

Endast ett användarkonto kan kopplas till en e-postadress. Om det finns flera användarkonton som är associerade med en enda e-postadress måste konflikten lösas i Marketo Engage och alla användarinloggningar som är associerade med e-postadressen visas, liksom tre lösningsalternativ:

* Använd den aktuella e-postadressen för det aktuella användarens inloggnings-ID
* Använd ett nytt e-postmeddelande för det aktuella användarens inloggnings-ID
* Fördröj beslutet tills nästa inloggning

  ![](assets/email-verification-6.png)

>[!NOTE]
>
>Även om ett användarkonto måste kopplas till en enda adress kan ett användarkonto användas för många prenumerationer via Universal ID.
