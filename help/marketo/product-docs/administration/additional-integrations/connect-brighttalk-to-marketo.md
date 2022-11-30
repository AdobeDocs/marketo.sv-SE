---
unique-page-id: 15695874
description: Anslut BrightTALK till Marketo - Marketo Docs - produktdokumentation
title: Anslut BrightTALK till Marketo
exl-id: 5c6a12ec-301b-4dec-975c-24ec759ebb37
source-git-commit: 5f509a7aa27692e54bf129b94c657aff0f645f2b
workflow-type: tm+mt
source-wordcount: '343'
ht-degree: 0%

---

# Anslut BrightTALK till Marketo {#connect-brighttalk-to-marketo}

Lär dig hur du ansluter din BrightTALK-kanal till din Marketo-instans. För att kunna göra detta måste du vara administratör för båda.

>[!NOTE]
>
>**Administratörsbehörigheter krävs**

## Steg i BrightTALK {#steps-in-brighttalk}

1. Logga in på [business.brighttalk.com/demandcentral](https://business.brighttalk.com/demandcentral/login){target=&quot;_blank&quot;} och klicka på **Anslut nu**.
1. Under Advanced Marketo Connector klickar du på **Anslut**.
1. Du kommer till skärmen för inloggningsuppgifter och frågar efter: Klient-ID, Klienthemlighet, Identitetstjänstens URL och URL för återställningstjänst. Logga in på Marketo för att få den här informationen.

## Steg i Marketo {#steps-in-marketo}

>[!NOTE]
>
>I det här skedet måste du konfigurera en API-användarroll och API-användare för att kunna begränsa vilka behörigheter BrightStor ska ha i din Marketo-instans. Eftersom vi redan har artiklar för de stegen länkar vi dig till dem.

1. Skapa en [Användarroll endast för API](/help/marketo/product-docs/administration/users-and-roles/create-an-api-only-user-role.md){target=&quot;_blank&quot;}.

1. [Skapa en API-användare](/help/marketo/product-docs/administration/users-and-roles/create-an-api-only-user.md){target=&quot;_blank&quot;}, med den API-roll för BrightStor som du skapade under steg 4.

1. Gå tillbaka till området Admin.

   ![](assets/connect-brighttalk-to-marketo-1.png)

1. Under Integrering klickar du på **LaunchPoint**.

   ![](assets/connect-brighttalk-to-marketo-2.png)

1. Klicka på **Nytt** nedrullningsbar meny och välj **Ny tjänst**.

   ![](assets/connect-brighttalk-to-marketo-3.png)

1. Ange ett visningsnamn. Klicka på listrutan Tjänst och välj **Egen** (do _not_ välj BrightTALK).

   ![](assets/connect-brighttalk-to-marketo-4.png)

   >[!CAUTION]
   >
   >Kom ihåg att inte markera BrightTALK i listrutan. Det är ett fält som vi håller på att ta bort, och om du väljer det kan det skapa betydande problem med din Marketo/BrightTALK-integrering.

1. Ange en beskrivning. Klicka på listrutan Endast API-användare och välj den BrightStor API-användare som du skapade under steg 5. Klicka **Skapa**.

   ![](assets/connect-brighttalk-to-marketo-5.png)

1. Klicka **Visa detaljer** för den anpassade tjänst du just skapade.

   ![](assets/connect-brighttalk-to-marketo-6.png)

1. Kopiera (och spara) **Klient-ID** och **Klienthemlighet**. Klicka **Stäng**.

   ![](assets/connect-brighttalk-to-marketo-7.png)

1. Under Integrering väljer du **Webbtjänster**.

   ![](assets/connect-brighttalk-to-marketo-8.png)

1. Under Rest API kopierar (och sparar) du **Slutpunkt** och **Identitet**.

   ![](assets/connect-brighttalk-to-marketo-9.png)

## Ytterligare steg i BrightTALK {#additional-steps-in-brighttalk}

1. Gå tillbaka till konfigurationsskärmen för BrightTALK-anslutningen från steg 3 och ange de uppgifter du sparade från steg 12 och 14.

   När inloggningsuppgifterna har autentiserats har du officiellt anslutit BrightTALK till Marketo. Nästa steg är att bestämma [vilka datafält du vill synkronisera](https://support.brighttalk.com/hc/en-us/articles/115005131274-BrightTALK-Connector-for-Marketo-Choose-the-Fields-to-Sync){target=&quot;_blank&quot;}.
