---
unique-page-id: 15695874
description: Connect BrightTALK to Marketo - Marketo Docs - Produktdokumentation
title: Anslut BrightTALK till Marketo
translation-type: tm+mt
source-git-commit: 23428a6e0ba9b2108a8f2f7dd6a69929dd069834
workflow-type: tm+mt
source-wordcount: '341'
ht-degree: 0%

---


# Anslut BrightTALK till Marketo {#connect-brighttalk-to-marketo}

Lär dig hur du ansluter din BrightTALK-kanal till din Marketo-instans. För att kunna göra detta måste du vara administratör för båda.

>[!NOTE]
>
>**Administratörsbehörigheter krävs**

## Steg i BrightTALK {#steps-in-brighttalk}

1. Logga in på [business.brighttalk.com/demandcentral](http://business.brighttalk.com/demandcentral/login) och klicka på **Anslut nu**.
1. Klicka på **Anslut** under Advanced Marketo Connector.
1. Du kommer till skärmen för inloggningsuppgifter och frågar efter: Klient-ID, Klienthemlighet, Identitetstjänstens URL och URL för återställningstjänst. Logga in på Marketo för att få den här informationen.

## Steg i Marketo {#steps-in-marketo}

>[!NOTE]
>
>Nu måste du konfigurera en API-roll och API-användare för att begränsa vilka behörigheter BrightStor ska ha i din Marketo-instans. Eftersom vi redan har artiklar för de stegen länkar vi dig till dem.

1. Skapa en [API Endast användarroll](http://docs.marketo.com/x/iwMk).
1. [Skapa en API-användare](http://docs.marketo.com/x/jwMk) med den API-roll för BrightStor som du skapade under steg 4.
1. Gå tillbaka till området Admin.

   ![](assets/one.png)

1. Klicka på **LaunchPoint** under Integrering.

   ![](assets/two.png)

1. Klicka på listrutan **Ny** och välj **Ny tjänst**.

   ![](assets/three.png)

1. Ange ett visningsnamn. Klicka på listrutan Tjänst och välj **Egen** (gör **inte** välj BrightTALK).

   ![](assets/four.png)

   >[!CAUTION]
   >
   >Kom ihåg att inte markera BrightTALK i listrutan. Det är ett fält som vi håller på att ta bort, och om vi väljer det kan det skapa betydande problem med er integrering med Marketo/BrightTALK.

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

## Steg i BrightTALK {#steps-in-brighttalk-1}

1. Gå tillbaka till konfigurationsskärmen för BrightTALK-anslutningen från steg 3 och ange de uppgifter du sparade från steg 12 och 14.

   När inloggningsuppgifterna har autentiserats har du officiellt anslutit BrightTALK till Marketo. Nästa steg är att bestämma [vilka datafält du vill synkronisera](http://support.brighttalk.com/hc/en-us/articles/115005131274-BrightTALK-Connector-for-Marketo-Choose-the-Fields-to-Sync).

