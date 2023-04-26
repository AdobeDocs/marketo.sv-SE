---
description: E-postverifiering - Marketo Docs - produktdokumentation
title: E-postverifiering
exl-id: 976e46a7-8c85-45ed-86c1-0c5cdb2d5c3e
source-git-commit: c45b3ab94b806b53768891613f15b8e9b694a440
workflow-type: tm+mt
source-wordcount: '167'
ht-degree: 0%

---

# E-postverifiering {#email-verification}

Adobe Marketo Engage-prenumerationer kräver att alla användare som inte är API-baserade, inklusive administratörer för Marketo Engage, verifierar sin e-postadress. Användare med enkel inloggning (SSO) som inte har tilldelats en administratörsroll, eller som har tilldelats en roll med behörigheten Åsidosätt enkel inloggning, kommer automatiskt att få sin e-post verifierad när prenumerationen har aktiverats med funktionen för e-postverifiering.

**Användarinbjudan**

När en administratör bjuder in en användare verifieras den användaren automatiskt när han/hon klickar på länken för inbjudan. SSO-användare som inte har tilldelats rollen Admin verifieras automatiskt.

**Ändra en e-postadress**

När en användares e-postadress ändras blir den inte verifierad. Ett e-postmeddelande skickas till dem där de kan verifiera igen. Användarna kan skicka om e-postmeddelandet manuellt genom att klicka på **Skicka verifiering igen**.

![](assets/email-verification-1.png)

![](assets/email-verification-2.png)

**Användare och roller**

I kolumnen Admin > Användare &amp; roller visas verifieringsstatusen för varje användare i kolumnen E-poststatus.

![](assets/email-verification-3.png)

Om du vill skicka ett bekräftelsemeddelande till en overifierad användare igen markerar du användarens post och klickar på knappen **Verifiera e-post** -knappen.
