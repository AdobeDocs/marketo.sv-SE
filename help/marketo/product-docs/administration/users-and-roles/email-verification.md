---
description: E-postverifiering - Marketo Docs - produktdokumentation
title: E-postverifiering
exl-id: 976e46a7-8c85-45ed-86c1-0c5cdb2d5c3e
source-git-commit: 44cca5ebad831cc39babac87ac9ebbf53df6c795
workflow-type: tm+mt
source-wordcount: '255'
ht-degree: 0%

---

# E-postverifiering {#email-verification}

Adobe Marketo Engage-prenumerationer kräver att alla användare som inte är API-baserade, inklusive administratörer för Marketo Engage, verifierar sin e-postadress. Användare med enkel inloggning (SSO) som inte har tilldelats en administratörsroll, eller som har tilldelats en roll med behörigheten Åsidosätt enkel inloggning, kommer automatiskt att få sin e-post verifierad när prenumerationen har aktiverats med funktionen för e-postverifiering.

## Användarinbjudan {#user-invite}

När en administratör bjuder in en användare verifieras den användaren automatiskt när han/hon klickar på länken för inbjudan. SSO-användare som inte har tilldelats rollen Admin verifieras automatiskt.

## Ändra en e-postadress {#changing-an-email-address}

När en användares e-postadress ändras blir den inte verifierad. Ett e-postmeddelande skickas till dem där de kan verifiera igen. Användarna kan skicka om e-postmeddelandet manuellt genom att klicka på **Skicka verifiering igen**.

![](assets/email-verification-1.png)

![](assets/email-verification-2.png)

## Användare och roller {#users-and-roles}

I **Administratör** > **Användare och roller** visas verifieringsstatusen för varje användare i kolumnen E-poststatus.

![](assets/email-verification-3.png)

## Inloggnings-ID för flera användare {#multiple-user-login-ids}

Endast ett användarkonto kan kopplas till en e-postadress. Om det finns flera användarkonton som är associerade med en enda e-postadress måste konflikten lösas i Marketo Engage och alla användarinloggningar som är associerade med e-postadressen visas, liksom tre lösningsalternativ:<p>
`1` Använd den aktuella e-postadressen för det aktuella användarens inloggnings-ID<p>
`2` Använd ett nytt e-postmeddelande för det aktuella användarens inloggnings-ID<p>
`3` Fördröj beslutet tills nästa inloggning

![](assets/email-verification-4.png)

## Verifierings-e-post {#verification-email}

Inbjudna användare får följande mejl:

![](assets/email-verification-5.png)

>[!NOTE]
>
>Om du vill skicka ett bekräftelsemeddelande till en overifierad användare igen markerar du användarens post och klickar på knappen **Verifiera e-post** -knappen.
