---
unique-page-id: 4719287
description: Redigera ursprungliga fältmappningar - Marketo Docs - Produktdokumentation
title: Redigera ursprungliga fältmappningar
translation-type: tm+mt
source-git-commit: 00887ea53e395bea3a11fd28e0ac98b085ef6ed8
workflow-type: tm+mt
source-wordcount: '279'
ht-degree: 0%

---


# Redigera ursprungliga fältmappningar {#edit-initial-field-mappings}

>[!NOTE]
>
>**Påminnelse**
>
>Den här funktionen är bara tillgänglig före den första synkroniseringen till Salesforce! När knappen **Synkronisera nu** trycks ned kan detta inte göras längre.

Under den första synkroniseringen till Salesforce kombinerar Marketo automatiskt anpassade fält med liknande namn till ett enda fält på Marketo-sidan för att säkerställa att data kan utbytas med både lead- och kontaktobjekt i CRM. I den här artikeln beskrivs hur du anpassar mappningarna.

## Mappa omappade fält {#map-unmapped-fields}

När du ser ett fält i mappen Omappade fält betyder det att det inte är mappat till ett liknande fält på lead eller kontakt i Salesforce. Du kan fixa det där.

1. Klicka på Redigera mappningar.

![](assets/image2014-12-9-13-3a31-3a0.png)

1. Öppna mappen **Omappade anpassade fält** .

   ![](assets/two.png)

1. Dra ett omappat anpassat fält till ett annat för att mappa dem tillsammans.

   >[!NOTE]
   >
   >Du kan bara redigera anpassade fältkopplingar. Standardfältkopplingar kan inte ändras.

   ![](assets/three.png)

1. Klicka på **Avsluta mappningar** när du är klar.

   ![](assets/four.png)

## Bryt befintlig mappning {#break-existing-mapping}

Om du har fält med liknande namn på leadet och kontaktobjektet Marketo mappas de automatiskt. Du kan anse att de är olika och att de har olika data. Bryt mappningen så här.

1. Klicka på **Redigera mappningar**.

   ![](assets/image2014-12-9-13-3a31-3a37.png)

1. Markera ett mappat fält och klicka på **Brytmappning** för att separera fälten.

   ![](assets/image2014-12-9-13-3a31-3a47.png)

1. Klicka på **Avsluta mappningar** när du är klar.

   ![](assets/image2014-12-9-13-3a31-3a58.png)

   Snyggt! Du är nästan klar med den inledande synkroniseringen.

## Återställ schema {#reset-schema}

1. Om du gör några ändringar i schemat i Salesforce medan du arbetar med mappningarna kan du dra in ändringarna genom att klicka på **Återställ schema**.

   * Alla mappningsändringar återställs!
   * Om du återställer schemat läggs bara fält till, inte tas bort (även om du döljer dem för synkroniseringsanvändaren).

   ![](assets/image2014-12-9-13-3a32-3a8.png)

