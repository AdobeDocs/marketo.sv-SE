---
description: Dynamic Chat-integrering - Marketo Docs - produktdokumentation
title: Dynamisk chattintegrering
hide: true
hidefromtoc: true
source-git-commit: ea2ee32a4c8805154f17717d515bb994dbfbe982
workflow-type: tm+mt
source-wordcount: '304'
ht-degree: 0%

---

# Dynamisk chattintegrering {#dynamic-chat-integration}

Läs mer om Dynamic Chat-integrationen med Sales Insight.

>[!PREREQUISITES]
>
>* Ditt SFDC-paket för Sales Insight måste vara av version [1,9 eller senare](/help/marketo/product-docs/marketo-sales-insight/msi-for-salesforce/upgrading/upgrading-your-msi-package.md){target=&quot;_blank&quot;}
>
>* Du måste ha [Dynamisk chattintegrering](/help/marketo/product-docs/demand-generation/dynamic-chat/dynamic-chat-overview.md){target=&quot;_blank&quot;} har konfigurerats


## Marketo Sales Insight Configuration tab {#marketo-sales-insight-configuration-tab}

1. Logga in på ditt Salesforce-konto, klicka på + i slutet av flikfältet och klicka på **Marketo Sales Insight Config**.

1. Klicka för att ta bort&quot;Visualforce-panelen&quot;.

   ![](assets/dynamic-chat-integration-1.png)

1. Välj **Aktivera dynamiska chattdata** kryssrutan.

   ![](assets/dynamic-chat-integration-2.png)

## Funktionsöversikt {#feature-overview}

De dynamiska chattaktiviteterna nedan kan utnyttjas av Sales Insight-användare.

Engaged Dialog: Inloggad i Marketo och ifylld i Sales Insight när en besökare klickar på en chattbot och engagerar sig i dialogrutan.

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

Fliken Chatt finns på panelerna Lead och Kontakt. Det innehåller kolumnerna Aktivitetstyp, Dialogrutenamn och Datum.

![](assets/dynamic-chat-integration-3.png)

Du kan läsa mer om en aktivitetstyp genom att klicka på den.

![](assets/dynamic-chat-integration-4.png)

På samma sätt innehåller panelerna Namn, Aktivitetstyp, Dialogrutenamn och Datum.

![](assets/dynamic-chat-integration-5.png)

Fliken Chatt finns även på fliken Global Marketo. Det innehåller tre aktivitetstyper (engagerad dialog, schemalagd avtalad tid, uppnått mål) tillsammans med följande kolumner:

* Person
* Konto
* Typ av aktivitet (engagerad dialog, schemalagd avtalad tid, uppnått mål)
* Dialogrutenamn
* Datum- och tidsstämpel

Återigen kan du lära dig mer om en aktivitetstyp genom att klicka på den.

![](assets/dynamic-chat-integration-6.png)

>[!NOTE]
>
>Aktiviteten&quot;Interagera med dokument&quot; kommer att vara tillgänglig i MSI i en kommande version.
