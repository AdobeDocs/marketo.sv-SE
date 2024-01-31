---
description: E-postverifiering - Marketo Docs - produktdokumentation
title: E-postverifiering
exl-id: 976e46a7-8c85-45ed-86c1-0c5cdb2d5c3e
feature: Users and Roles
source-git-commit: 5ef17e8c3988706a4d95332312ffb035f35bb269
workflow-type: tm+mt
source-wordcount: '410'
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
>Undantaget ovan är att i en prenumeration med enbart enkel inloggning får administratörer en ny användarinbjudan, men inte administratörer. Icke-administratörer måste gå igenom e-postverifieringsprocessen för att säkerställa migrering av sina användarposter. En administratör kan skicka e-postverifieringslänken genom att klicka på **Skicka e-postverifiering igen** intill användarnamnet.

## Verifierings-e-post {#verification-email}

Användarna får följande mejl när e-postverifiering aktiveras för en prenumeration, eller om den aktiveras av en administratör/användare:

![](assets/email-verification-1.png)

>[!NOTE]
>
>Om du vill skicka ett bekräftelsemeddelande till en overifierad användare igen markerar du användarens post och klickar på knappen **[!UICONTROL Verify Email]** -knappen.

## Ändra en e-postadress {#changing-an-email-address}

När en användares e-postadress ändras blir den inte verifierad. Ett e-postmeddelande skickas till dem där de kan verifiera igen. Användarna kan skicka om e-postmeddelandet manuellt genom att klicka på **[!UICONTROL Resend Verification]**.

![](assets/email-verification-2.png)

![](assets/email-verification-3.png)

## Användare och roller {#users-and-roles}

I **[!UICONTROL Admin]** > **[!UICONTROL Users & Roles]** visas verifieringsstatusen för varje användare i kolumnen E-poststatus.

![](assets/email-verification-4.png)

## Inloggnings-ID för flera användare {#multiple-user-login-ids}

Endast ett användarkonto kan kopplas till en e-postadress. Om det finns flera användarkonton som är associerade med en enda e-postadress måste konflikten lösas i Marketo Engage och alla användarinloggningar som är associerade med e-postadressen visas, liksom tre lösningsalternativ:

* Använd den aktuella e-postadressen för det aktuella användarens inloggnings-ID
* Använd ett nytt e-postmeddelande för det aktuella användarens inloggnings-ID
* Fördröj beslutet tills nästa inloggning

  ![](assets/email-verification-5.png)

>[!NOTE]
>
>Även om ett användarkonto måste kopplas till en enda adress kan ett användarkonto användas för många prenumerationer via Universal ID.
