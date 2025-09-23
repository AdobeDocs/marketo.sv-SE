---
unique-page-id: 10096656
description: Skapa en händelse med Marketo ON24-adaptern - Marketo Docs - produktdokumentation
title: Skapa en händelse med Marketo ON24-adaptern
exl-id: a240ff72-b12f-4e3a-8e14-94fddb02f944
feature: Events
source-git-commit: 09a656c3a0d0002edfa1a61b987bff4c1dff33cf
workflow-type: tm+mt
source-wordcount: '284'
ht-degree: 0%

---

# Skapa en händelse med Marketo ON24-adaptern {#create-an-event-with-the-marketo-on-adapter}

Du bör känna till byggstenarna och den rekommenderade sekvensen för att skapa händelser i Marketo. Du bör också ha kunskaper om följande Marketo-koncept:

* [Marketo-program](/help/marketo/product-docs/core-marketo-concepts/programs/creating-programs/understanding-programs.md){target="_blank"} samt händelser och skillnaderna mellan dem
* [Kanaler](/help/marketo/product-docs/administration/tags/create-a-program-channel.md){target="_blank"}
* [Lokal Assets](/help/marketo/product-docs/core-marketo-concepts/programs/creating-programs/understanding-local-assets-in-a-program.md){target="_blank"}
* [Underordnade kampanjer](/help/marketo/product-docs/demand-generation/events/create-an-event/create-an-event-with-the-marketo-on24-adapter/configure-event-settings-and-sync-marketo-with-your-webinar.md){target="_blank"} och [Programstatus](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/program-flow-actions/change-program-status.md){target="_blank"}

>[!NOTE]
>
>Mer information om Marketo API:er finns i [Marketo API-dokumentationen](https://experienceleague.adobe.com/sv/docs/marketo-developer/marketo/rest/rest-api){target="_blank"}.

## Förutsättningar {#prerequisites}

Följande krävs för att använda integreringen Marketo ON24:

* **Prenumeration på ON24-webbsändningar** - Om du inte har någon prenumeration kontaktar du ON24 direkt. **OBS!**: ON24 Hosted Edition krävs. Händelsehantering ON24 krävs inte.

* **Administratörsbehörighet till ON24** - Du behöver den här anslutningen för att kunna använda och skapa gäster i ON24-systemet.
* **ON24-anslutningsreferenser** - Du måste ange den här informationen i Marketo för att kunna aktivera integreringen: Användarnamn, Lösenord, Klient-ID och Klientnyckel. Kontakta din kontohanterare för ON24 eller support för ON24 om du behöver hjälp med dina uppgifter.
* **Registreringsformulär** - Använd ett Marketo-formulär eller ett icke-Marketo-formulär tillsammans med rätt API för att säkerställa att registreringsdata och registreringsinformation skickas till Marketo.
* **Underordnad registreringskampanj** - En underordnad registreringskampanj i din Marketo-händelse måste skapas och konfigureras på rätt sätt för att din Event Partner-integrering ska fungera.

## Processflöde {#process-flow}

Så här skapar du en händelse med Marketo On24-adaptern:

1. [Skapa webbinariet i ON24](/help/marketo/product-docs/demand-generation/events/create-an-event/create-an-event-with-the-marketo-on24-adapter/create-your-webinar-event-in-on24.md){target="_blank"}
1. [Konfigurera händelseinställningar och synkronisera Marketo med ditt webbinarium](/help/marketo/product-docs/demand-generation/events/create-an-event/create-an-event-with-the-marketo-on24-adapter/configure-event-settings-and-sync-marketo-with-your-webinar.md){target="_blank"}
1. [Skapa underordnade kampanjer och lokala Assets](/help/marketo/product-docs/demand-generation/events/create-an-event/create-an-event-with-the-marketo-on24-adapter/create-child-campaigns-and-local-assets.md){target="_blank"}
1. [Testa din ON24-händelseintegrering](/help/marketo/product-docs/demand-generation/events/create-an-event/create-an-event-with-the-marketo-on24-adapter/test-your-on24-event-integration.md){target="_blank"}
1. [Exempel på ON24-händelseintegrering](/help/marketo/product-docs/demand-generation/events/create-an-event/create-an-event-with-the-marketo-on24-adapter/example-on24-event-integration.md){target="_blank"}
1. [Om status för webbinarium](/help/marketo/product-docs/demand-generation/events/create-an-event/create-an-event-with-the-marketo-on24-adapter/understanding-webinar-program-statuses.md){target="_blank"}
1. [ON24 - händelseregistreringsuppdateringar](/help/marketo/product-docs/demand-generation/events/create-an-event/create-an-event-with-the-marketo-on24-adapter/on24-event-registration-updates.md){target="_blank"}
