---
description: Gör en marknadsföringskampanj synlig i Sales Insight Actions - Marketo Docs - Product Documentation
title: Gör en marknadsföringskampanj synlig i försäljningsinsikter
exl-id: 223baca3-159e-4f0d-b26f-f4c924a39fc3
feature: Sales Insight Actions
source-git-commit: c6132bf5b393df38700ad9dd6f0c6414860e8bb6
workflow-type: tm+mt
source-wordcount: '300'
ht-degree: 0%

---

# Gör en marknadsföringskampanj synlig i försäljningsinsikter {#make-a-marketing-campaign-visible-in-sales-insight-actions}

Kampanjer kan bara delas om de är synliga.

Med Sales Insight Actions får användarna tillgång till en ny försäljningsapp som heter toutapp.com. Den här appen ger dem en ny uppsättning åtgärdsfunktioner, men ärver även funktionen _Lägg till i marknadsföringskampanj_ som finns i huvudversionen av försäljningsinsikter. Detta är viktigt att tänka på, eftersom dina Marketo-kampanjer måste konfigureras annorlunda beroende på var du vill att användarna ska få tillgång till funktionen Lägg till i marknadsföringskampanj (toutapp.com eller MSI SFDC-paketupplevelsen). Mer information finns i kommentaren i steg 4.

1. Välj (eller skapa) den kampanj du vill dela.

   ![](assets/make-a-marketing-campaign-visible-sia-1.png)

1. Klicka på fliken **Smart lista**.

   ![](assets/make-a-marketing-campaign-visible-sia-2.png)

1. Lägg till _Kampanjen är begärd_-utlösare.

   ![](assets/make-a-marketing-campaign-visible-sia-3.png)

1. Välj is **Webbtjänstens API** som källa.

   ![](assets/make-a-marketing-campaign-visible-sia-4.png)

   >[!NOTE]
   >
   >Om du vill visa marknadsföringskampanjen för användare som använder _Lägg till i marknadsföringskampanj_ från webbappen toutapp.com (detta gäller även om du har webbappen inbäddad i CRM via Marketo Sales Outbox-objektet), anger du den begärda källan för Campaign till&quot;Web Service API&quot;. Om du vill att marknadsföringskampanjen ska visas när en användare använder åtgärderna på MSI-panelen i Salesforce på lead-, kontakt-, konto- eller gruppåtgärdsknapparna på lead- och kontaktlistorna, uppdaterar du den begärda källan för Campaign till&quot;Sales Insight&quot;

1. Klicka på fliken **Flöde**.

   ![](assets/make-a-marketing-campaign-visible-sia-5.png)

1. Lägg till flödesåtgärden _Intressant stund_.

   ![](assets/make-a-marketing-campaign-visible-sia-6.png)

1. Välj **Webb** som Typ.

   ![](assets/make-a-marketing-campaign-visible-sia-7.png)

1. Skriv ett meddelande till ditt säljteam i rutan _Beskrivning_. I det här exemplet använder vi tokens för att ange formuläret som fylldes i.

   ![](assets/make-a-marketing-campaign-visible-sia-8.png)

1. Klicka på fliken **Schema** och **Aktivera** kampanjen.

   ![](assets/make-a-marketing-campaign-visible-sia-9.png)
