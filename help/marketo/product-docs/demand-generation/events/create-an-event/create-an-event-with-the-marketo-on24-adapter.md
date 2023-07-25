---
unique-page-id: 10096656
description: Skapa en händelse med Marketo ON24-adaptern - Marketo Docs - produktdokumentation
title: Skapa en händelse med Marketo ON24-adaptern
exl-id: a240ff72-b12f-4e3a-8e14-94fddb02f944
feature: Events
source-git-commit: 431bd258f9a68bbb9df7acf043085578d3d91b1f
workflow-type: tm+mt
source-wordcount: '284'
ht-degree: 0%

---

# Skapa en händelse med Marketo ON24-adaptern {#create-an-event-with-the-marketo-on-adapter}

Du bör känna till byggstenarna och den rekommenderade sekvensen för att skapa händelser i Marketo. Du bör också ha kunskaper om följande Marketo-koncept:

* [Marketo-program](/help/marketo/product-docs/core-marketo-concepts/programs/creating-programs/understanding-programs.md){target="_blank"} samt händelser och skillnaderna mellan dem
* [Kanaler](/help/marketo/product-docs/administration/tags/create-a-program-channel.md){target="_blank"}
* [Lokala resurser](/help/marketo/product-docs/core-marketo-concepts/programs/creating-programs/understanding-local-assets-in-a-program.md){target="_blank"}
* [Underordnade kampanjer](/help/marketo/product-docs/demand-generation/events/create-an-event/create-an-event-with-the-marketo-on24-adapter/configure-event-settings-and-sync-marketo-with-your-webinar.md){target="_blank"} and [Program Statuses](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/program-flow-actions/change-program-status.md){target="_blank"}

>[!NOTE]
>
>Se [Marketo API-dokumentation](https://developers.marketo.com/documentation/rest/){target="_blank"} om du vill ha mer information om Marketo API:er.

## Förutsättningar {#prerequisites}

Följande krävs för att använda integreringen Marketo ON24:

* **Prenumeration på ON24-webbsändningar** - Om du inte har någon prenumeration kontaktar du ON24 direkt. **ANMÄRKNING**: ON24 Hosted Edition krävs. Händelsehantering ON24 krävs inte.

* **Administratörsrättigheter till ON24** - Du behöver den här anslutningen för att kunna använda den och skapa gäster i ON24-systemet.
* **On24-anslutningsreferenser** - Du måste ange den här informationen i Marketo för att aktivera integreringen: Användarnamn, lösenord, klient-ID och klientnyckel. Kontakta din kontohanterare för ON24 eller support för ON24 om du behöver hjälp med dina uppgifter.
* **Registreringsformulär** - Använd ett Marketo-formulär eller ett icke-Marketo-formulär tillsammans med rätt API för att säkerställa att registreringsdata och registreringsinformation skickas till Marketo.
* **Registrera underordnad kampanj** - En registrering av en underordnad kampanj i ditt Marketo Event-evenemang måste skapas och konfigureras på rätt sätt för att integreringen av din Event Partner ska fungera.

## Processflöde {#process-flow}

Följ de här stegen för att skapa en händelse med Marketo On24-adaptern:

1. [Skapa ett webbinarium i ON24](/help/marketo/product-docs/demand-generation/events/create-an-event/create-an-event-with-the-marketo-on24-adapter/create-your-webinar-event-in-on24.md){target="_blank"}
1. [Konfigurera händelseinställningar och synkronisera Marketo med ditt webbinarium](/help/marketo/product-docs/demand-generation/events/create-an-event/create-an-event-with-the-marketo-on24-adapter/configure-event-settings-and-sync-marketo-with-your-webinar.md){target="_blank"}
1. [Skapa underordnade kampanjer och lokala resurser](/help/marketo/product-docs/demand-generation/events/create-an-event/create-an-event-with-the-marketo-on24-adapter/create-child-campaigns-and-local-assets.md){target="_blank"}
1. [Testa din ON24-händelseintegrering](/help/marketo/product-docs/demand-generation/events/create-an-event/create-an-event-with-the-marketo-on24-adapter/test-your-on24-event-integration.md){target="_blank"}
1. [Exempel på händelseintegrering ON24](/help/marketo/product-docs/demand-generation/events/create-an-event/create-an-event-with-the-marketo-on24-adapter/example-on24-event-integration.md){target="_blank"}
1. [Om status för webbinarium](/help/marketo/product-docs/demand-generation/events/create-an-event/create-an-event-with-the-marketo-on24-adapter/understanding-webinar-program-statuses.md){target="_blank"}
1. [ON24 - Händelseregistreringsuppdateringar](/help/marketo/product-docs/demand-generation/events/create-an-event/create-an-event-with-the-marketo-on24-adapter/on24-event-registration-updates.md){target="_blank"}
