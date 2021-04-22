---
unique-page-id: 15695874
description: Anslut BrightTALK till Marketo - Marketo Docs - produktdokumentation
title: Anslut BrightTALK till Marketo
exl-id: 5c6a12ec-301b-4dec-975c-24ec759ebb37
translation-type: tm+mt
source-git-commit: 72e1d29347bd5b77107da1e9c30169cb6490c432
workflow-type: tm+mt
source-wordcount: '335'
ht-degree: 0%

---

# Anslut BrightTALK till Marketo {#connect-brighttalk-to-marketo}

Lär dig hur du ansluter din BrightTALK-kanal till din Marketo-instans. För att kunna göra detta måste du vara administratör för båda.

>[!NOTE]
>
>**Administratörsbehörigheter krävs**

## Steg i BrightTALK {#steps-in-brighttalk}

1. Logga in på [business.brighttalk.com/demandcentral](https://business.brighttalk.com/demandcentral/login) och klicka på **Anslut nu**.
1. Klicka på **Anslut** under Avancerad Marketo Connector.
1. Du kommer till skärmen för inloggningsuppgifter och frågar efter: Klient-ID, Klienthemlighet, Identitetstjänstens URL och URL för återställningstjänst. Logga in på Marketo för att få den här informationen.

## Steg i Marketo {#steps-in-marketo}

>[!NOTE]
>
>I det här skedet måste du konfigurera en API-användarroll och API-användare för att kunna begränsa vilka behörigheter BrightStor ska ha i din Marketo-instans. Eftersom vi redan har artiklar för de stegen länkar vi dig till dem.

1. Skapa en [API Endast användarroll](/help/marketo/product-docs/administration/users-and-roles/create-an-api-only-user-role.md).
1. [Skapa en API-användare](/help/marketo/product-docs/administration/users-and-roles/create-an-api-only-user.md) med den API-roll för BrightStor som du skapade under steg 4.
1. Gå tillbaka till området Admin.

   ![](assets/one.png)

1. Klicka på **LaunchPoint** under Integrering.

   ![](assets/two.png)

1. Klicka på listrutan **Ny** och välj **Ny tjänst**.

   ![](assets/three.png)

1. Ange ett visningsnamn. Klicka på listrutan Tjänst och välj **Egen** (gör _inte_ välj BrightTALK).

   ![](assets/four.png)

   >[!CAUTION]
   >
   >Kom ihåg att inte markera BrightTALK i listrutan. Det är ett fält som vi håller på att ta bort, och om du väljer det kan det skapa betydande problem med din Marketo/BrightTALK-integrering.

1. Ange en beskrivning. Klicka på listrutan Endast API-användare och välj den BrightStor API-användare som du skapade under steg 5. Klicka på **Skapa**.

   ![](assets/five.png)

1. Klicka på **Visa information** för den anpassade tjänst du just skapade.

   ![](assets/six.png)

1. Kopiera (och spara) **Klient-ID** och **Klienthemlighet**. Klicka på **Stäng**.

   ![](assets/eight-1.png)

1. Välj **Webbtjänster** under Integrering.

   ![](assets/nine-1.png)

1. Under Rest API kopierar (och sparar) du **Endpoint** och **Identity**.

   ![](assets/ten.png)

## Ytterligare steg i BrightTALK {#additional-steps-in-brighttalk}

1. Gå tillbaka till konfigurationsskärmen för BrightTALK-anslutningen från steg 3 och ange de uppgifter du sparade från steg 12 och 14.

   När inloggningsuppgifterna har autentiserats har du officiellt anslutit BrightTALK till Marketo. Nästa steg är att bestämma [vilka datafält du vill synkronisera](https://support.brighttalk.com/hc/en-us/articles/115005131274-BrightTALK-Connector-for-Marketo-Choose-the-Fields-to-Sync).
