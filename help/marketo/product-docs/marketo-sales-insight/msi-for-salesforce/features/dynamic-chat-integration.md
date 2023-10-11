---
description: Integrering med Dynamic Chat - Marketo Docs - produktdokumentation
title: Integrering med Dynamic Chat
exl-id: b2e3b4da-9ca7-4299-9c50-f52e0de91e36
feature: Marketo Sales Insights
source-git-commit: 6e81a8891f7d6e5916549d453a694b42e08cd496
workflow-type: tm+mt
source-wordcount: '396'
ht-degree: 0%

---

# Integrering med Dynamic Chat {#dynamic-chat-integration}

Läs mer om integrationen mellan Dynamic Chat och Sales Insight.

>[!PREREQUISITES]
>
>* Ditt SFDC-paket för Sales Insight måste vara av version [2.4.0 eller senare](/help/marketo/product-docs/marketo-sales-insight/msi-for-salesforce/upgrading/upgrading-your-msi-package.md){target="_blank"}
>
>* Du måste ha [Integrering med Dynamic Chat](/help/marketo/product-docs/demand-generation/dynamic-chat/dynamic-chat-overview.md){target="_blank"} konfigurera
>
>* Se till att du använder din Sales Insight [Driftsinställningar](/help/marketo/product-docs/marketo-sales-insight/msi-for-salesforce/configuration/marketo-sales-insight-configuration-tab-in-salesforce.md#operational-settings){target="_blank"}, you have the "API Secret Key" field populated. If you don't, learn how to retrieve it [here](/help/marketo/product-docs/marketo-sales-insight/msi-for-salesforce/configuration/configure-marketo-sales-insight-in-salesforce-enterprise-unlimited.md#configure-sales-insight-in-marketo){target="_blank"}.

## Marketo Sales Insight Configuration Tab {#marketo-sales-insight-configuration-tab}

Följ stegen nedan för att aktivera integreringen av Dynamic Chat.

1. Logga in på ditt Salesforce-konto, klicka på + i slutet av flikfältet och klicka på **Marketo Sales Insight Config**.

1. Klicka för att ta bort&quot;Visualforce-panelen&quot;.

   ![](assets/dynamic-chat-integration-1.png)

1. Välj **Aktivera Dynamic Chat-data** kryssrutan.

   ![](assets/dynamic-chat-integration-2.png)

## Översikt över funktioner {#feature-overview}

Följande Dynamic Chat-aktiviteter kan utnyttjas av Sales Insight-användare..

Engaged Dialog: Loggade in Marketo and populated in Sales Insight when a visitor clicks on a chatbot and interages with the Dialog.

* Dialogrutenamn
* Sidans URL
* Status (initierad/släppt/slutförd)

Schemalagd avtalad tid: Inloggad i Marketo och ifylld i Sales Insight när en besökare har schemalagt en avtalad tid via chatbot.

* Dialogrutenamn
* Agent
* Sidans URL
* Schemalagd den (infoga datum- och tidsstämpel)
* Status (schemalagd, schemalagd, annullerad)

Uppnått mål: Inloggad i Marketo och ifylld i Sales Insight när en besökare når ett mål i något dialogflöde.

* Dialogrutenamn
* Målnamn
* Sidans URL

Interagera med dokument: Inloggad i Marketo och ifylld i Sales Insight när en besökare interagerar med ett dokument som delas via chatbot.

* Dialogrutenamn
* Dokument
* Status

Chattaktiviteter är tillgängliga i Insights Dashboard.

![](assets/dynamic-chat-integration-3.png)

Fliken Chatt finns på panelerna Lead och Kontakt. Det innehåller kolumnerna Aktivitetstyp, Dialogrutenamn och Datum.

![](assets/dynamic-chat-integration-4.png)

Du kan lära dig mer om en aktivitetstyp genom att klicka på den.

![](assets/dynamic-chat-integration-5.png)

På samma sätt innehåller panelerna Namn, Aktivitetstyp, Dialogrutenamn och Datum.

![](assets/dynamic-chat-integration-6.png)

Fliken Chatt finns även på fliken Global Marketo. Den innehåller tre aktivitetstyper (engagerad dialog, schemalagd avtalad tid, uppnått mål) tillsammans med följande kolumner:

* Person
* Konto
* Typ av aktivitet (engagerad dialog, schemalagd avtalad tid, uppnått mål)
* Dialogrutenamn
* Datum- och tidsstämpel

Återigen kan du lära dig mer om en aktivitetstyp genom att klicka på den.

![](assets/dynamic-chat-integration-7.png)

>[!NOTE]
>
>Om kryssrutan&quot;Aktivera Dynamic Chat data&quot; är inaktiverad kommer följande funktioner att inaktiveras:
>
>* Rad med chattaktiviteter på Instrumentpanelen för insikter (smart rutnät och listvy varje vecka)
>* Fliken Chatt på panelerna Lead, Kontakt, Konto och Möjligheter
>* Fliken Chatt på fliken Global Marketo
>
>Det går inte att inaktivera endast en av dessa funktioner.

