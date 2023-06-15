---
description: Uppdatera aktivitetstypfält vid loggning av aktiviteter till Salesforce - Marketo Docs - produktdokumentation
title: Uppdatera aktivitetstypfält vid loggning av aktiviteter till Salesforce
source-git-commit: 46c48172a58cf6bd2e9772ef57510fd7d808adc2
workflow-type: tm+mt
source-wordcount: '420'
ht-degree: 0%

---

# Uppdatera aktivitetstypfält vid loggning av aktiviteter till Salesforce {#update-activity-type-field-when-logging-activities-to-salesforce}

Åtgärder kan automatiskt synkronisera dina e-post- och samtalsaktiviteter till Salesforce för att kunna användas för rapportering och öka synligheten i aktivitetshistoriken. När du loggar aktiviteter ska du kontrollera att fältet Aktivitetstyp är korrekt uppdaterat till E-post, Ring eller Svara, beroende på vilken typ av aktivitet som loggas.

>[!NOTE]
>
>Loggning av e-postmeddelanden via BCC kommer inte att visa listan Uppgiftstyp, utan fyller i textfältet automatiskt som e-post eftersom de levereras till Salesforce via din BCC-adress.

## Saker att veta {#things-to-know}

* En anslutning till Salesforce krävs för att uppgiftstypen ska kunna uppdateras.
* Det ska inte finnas något standardtypvärde valt i listrutan Aktivitetstyp.
* Anrop, svar och e-post måste alla finnas i listrutan Aktivitetstyp (skiftläge).
* Arbetsflöden eller utlösare i Salesforce som uppdaterar fältet Aktivitetstyp kan störa den här processen.

## Inställningar {#setup}

Kontrollera först att du har rätt plocklistevärden på plats. Du behöver hjälp av din Salesforce-administratör för att göra ändringar i din lista.

Kontrollera först vilka värden du saknar i din aktivitetstypsväljare (ej e-post, samtal eller svar). Du kan behöva hjälp av din Salesforce-administratör för att granska detta och göra ändringar i din lista över aktivitetstyper. Om du vill göra de här ändringarna följer du stegen nedan.

### I Salesforce Lightning {#salesforce-lightning}

1. Navigera till [Salesforce.com](https://salesforce.com){target="_blank"}.
1. Klicka på kugghjulsikonen i det övre högra hörnet och välj **Inställningar** > **Objektshanteraren**.
1. Skriv &quot;task&quot; i rutan &#39;Quick Find&#39;.
1. Klicka på i den vänstra panelen **Fält och relationer**.
1. Klicka på fältetikett **Typ**.
1. Klicka på under Picklist-värdet för uppgiftstyp **Nytt**.
1. Skriv namnet på de värden för uppgiftstypväljaren som saknas (&quot;E-post,&quot;Ring&quot;,&quot;Svara&quot;).
1. Klicka **Spara**.

### I Salesforce Classic {#salesforce-classic}

1. Navigera till [Salesforce.com](https://salesforce.com){target="_blank"}.
1. Klicka **Inställningar** > **Bygge** > **Anpassa** > **Verksamhet** > **Aktivitetsfält**.
1. Klicka **Typ**.
1. Klicka på under Picklist-värdet för uppgiftstyp **Nytt**.
1. Skriv namnet på de värden för uppgiftstypväljaren som saknas (&quot;E-post,&quot;Ring&quot;,&quot;Svara&quot;).
1. Klicka **Spara**.

Nu när detta är på plats börjar du se textfältet fylla i motsvarande värde för loggade e-postmeddelanden, samtal och svar. Dessa värden _not_ fylls i på påminnelseuppgifter för Sales Insight Actions.

>[!NOTE]
>
>Om du inte ser Svara som ett värde lägger du till det genom att klicka på **Nytt**. Svara är inte ett standardvärde i Salesforce.

>[!MORELIKETHIS]
>
>* [Loggningsattribut för försäljningsaktivitet till Salesforce](/help/marketo/product-docs/marketo-sales-insight/actions/crm/salesforce-package-configuration/logging-sales-activity-attributes-to-salesforce.md){target="_blank"}
>* [Konfigurera detaljanpassning av Salesforce-aktivitet](/help/marketo/product-docs/marketo-sales-insight/actions/crm/salesforce-integration/configure-salesforce-activity-detail-customization.md){target="_blank"}
>* [Synkroniseringsinställningar för Salesforce](/help/marketo/product-docs/marketo-sales-insight/actions/crm/salesforce-integration/salesforce-sync-settings.md){target="_blank"}
