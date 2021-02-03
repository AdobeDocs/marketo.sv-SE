---
unique-page-id: 10096656
description: Skapa en händelse med marknadsföringskortet ON24 - Marketo Docs - produktdokumentation
title: Skapa en händelse med Marketo ON24-adaptern
translation-type: tm+mt
source-git-commit: ed83438ae5660d172e845f25c4d72d599574bd91
workflow-type: tm+mt
source-wordcount: '296'
ht-degree: 0%

---


# Skapa en händelse med Marketo ON24-adaptern {#create-an-event-with-the-marketo-on-adapter}

## Innan du börjar {#before-you-begin}

Du bör känna till byggblocken och den rekommenderade sekvensen för att skapa händelser i Marketo. Du bör också ha kunskap om följande Marketo-koncept:

* [Marketo-](/help/marketo/product-docs/core-marketo-concepts/programs/creating-programs/understanding-programs.md) program samt Event och skillnaderna mellan dem
* [Kanaler](/help/marketo/product-docs/administration/tags/create-a-program-channel.md)
* [Lokala resurser](/help/marketo/product-docs/core-marketo-concepts/programs/creating-programs/understanding-local-assets-in-a-program.md)
* [Underordnade ](/help/marketo/product-docs/demand-generation/events/create-an-event/create-an-event-with-the-marketo-on24-adapter/configure-event-settings-and-sync-marketo-with-your-webinar.md) kampanjer och  [programstatus](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/program-flow-actions/change-program-status.md)

>[!NOTE]
>
>Mer information om Marketo API:er finns i [dokumentationen för Marketo API](https://developers.marketo.com/documentation/rest/).

## Förutsättningar {#prerequisites}

Följande krävs för att använda Marketo ON24-integreringen:

* **Prenumeration på ON24-webbsändningar**  - Om du inte har någon prenumeration kontaktar du ON24 direkt. **OBS**: ON24 Hosted Edition krävs. Händelsehantering ON24 krävs inte.

* **Administratörsrättigheter till ON24**  - Du behöver detta för att använda den här anslutningen och skapa gäster i ON24-systemet.
* **ON24-anslutningsreferenser**  - Du måste ange den här informationen i Marketo för att kunna aktivera integreringen: Användarnamn, lösenord, klient-ID och klientnyckel. Kontakta din kontohanterare för ON24 eller support för ON24 om du behöver hjälp med dina uppgifter.
* **Registreringsformulär**  - Använd ett Marketo-formulär eller ett icke-Marketo-formulär tillsammans med rätt API för att säkerställa att registreringsdata och registreringsinformation skickas till Marketo.
* **Underordnad kampanj**  för registrering - En underordnad kampanj för registrering i din Marketo-händelse måste skapas och konfigureras på rätt sätt för att integreringen av din Event Partner ska fungera.

## Processflöde {#process-flow}

Följ de här stegen för att skapa en händelse med marknadsföringskortet On24:

1. [Ange dina ON24-autentiseringsuppgifter i Marketo](/help/marketo/product-docs/demand-generation/events/create-an-event/create-an-event-with-the-marketo-on24-adapter/enter-your-on24-credentials-in-marketo.md)
1. [Skapa ett webbinarium i ON24](/help/marketo/product-docs/demand-generation/events/create-an-event/create-an-event-with-the-marketo-on24-adapter/create-your-webinar-event-in-on24.md)
1. [Konfigurera händelseinställningar och synkronisera markeringar med ditt webbinarium](/help/marketo/product-docs/demand-generation/events/create-an-event/create-an-event-with-the-marketo-on24-adapter/configure-event-settings-and-sync-marketo-with-your-webinar.md)
1. [Skapa underordnade kampanjer och lokala resurser](/help/marketo/product-docs/demand-generation/events/create-an-event/create-an-event-with-the-marketo-on24-adapter/create-child-campaigns-and-local-assets.md)
1. [Testa din ON24-händelseintegrering](/help/marketo/product-docs/demand-generation/events/create-an-event/create-an-event-with-the-marketo-on24-adapter/test-your-on24-event-integration.md)
1. [Exempel på händelseintegrering ON24](/help/marketo/product-docs/demand-generation/events/create-an-event/create-an-event-with-the-marketo-on24-adapter/example-on24-event-integration.md)
1. [Om status för webbinarium](/help/marketo/product-docs/demand-generation/events/create-an-event/create-an-event-with-the-marketo-on24-adapter/understanding-webinar-program-statuses.md)
1. [ON24 - Händelseregistreringsuppdateringar](/help/marketo/product-docs/demand-generation/events/create-an-event/create-an-event-with-the-marketo-on24-adapter/on24-event-registration-updates.md)
