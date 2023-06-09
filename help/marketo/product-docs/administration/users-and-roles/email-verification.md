---
description: E-postverifiering - Marketo Docs - produktdokumentation
title: E-postverifiering
exl-id: 976e46a7-8c85-45ed-86c1-0c5cdb2d5c3e
source-git-commit: 2d28d4b473815952231356691b1e9310c61a20f1
workflow-type: tm+mt
source-wordcount: '403'
ht-degree: 0%

---

# E-postverifiering {#email-verification}

Adobe Marketo Engage-prenumerationer kräver att alla användare som inte är API-baserade, inklusive administratörer för Marketo Engage, verifierar sin e-postadress. Användare med enkel inloggning (SSO) som inte har tilldelats en administratörsroll, eller som har tilldelats en roll med behörigheten Åsidosätt enkel inloggning, kommer automatiskt att få sin e-post verifierad när prenumerationen har aktiverats med funktionen för e-postverifiering.

## Varför den här funktionen introducerades {#why-this-feature-was-introduced}

Marketo Engage fortsätter lanseringen av e-postverifiering som förberedelse för migrering av kunder till Adobe Business Platform, inklusive användarmigrering till Adobe ID:n. Den här funktionen förbättrar säkerheten för befintliga användarkonton i Marketo Engage. För att en Marketo Engage-användare ska kunna vara kopplad till rätt Adobe ID måste befintliga Marketo Engage-användare verifiera sin e-postadress. En Marketo Engage-användare måste ha en verifierad e-postadress för att kunna migreras till en Adobe ID. Om en Marketo Engage-användare inte verifierar sin e-postadress kan de inte migreras till en Adobe ID och förlorar åtkomsten till en Marketo-prenumeration när användarmigreringen för prenumerationen är klar.

## Användarinbjudan {#user-invite}

När en administratör bjuder in en användare verifieras den användaren automatiskt när han/hon klickar på länken för inbjudan. SSO-användare som inte har tilldelats rollen Admin verifieras automatiskt.

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
