---
unique-page-id: 4719287
description: Redigera ursprungliga fältmappningar - Marketo Docs - produktdokumentation
title: Redigera ursprungliga fältmappningar
exl-id: 320613d1-3845-4e05-a704-0db0f8027dc8
feature: Salesforce Integration
source-git-commit: 756a38ba87dd5af9ee783e9709056d444d4f415b
workflow-type: tm+mt
source-wordcount: '259'
ht-degree: 0%

---

# Redigera ursprungliga fältmappningar {#edit-initial-field-mappings}

>[!NOTE]
>
>Den här funktionen är bara tillgänglig före den första synkroniseringen till Salesforce. När knappen **[!UICONTROL Sync Now]** trycks ned kan detta inte längre göras.

Under den första synkroniseringen till Salesforce kombinerar Marketo Engage automatiskt anpassade fält med liknande namn till ett enda fält på Marketo-sidan för att säkerställa att data kan utbytas med både lead- och kontaktobjekt i CRM. I den här artikeln beskrivs hur du anpassar mappningarna.

## Mappa omappade fält {#map-unmapped-fields}

När du ser ett fält i mappen [!UICONTROL Unmapped Fields] betyder det att det inte är mappat till ett liknande fält på lead eller kontakt i Salesforce. Du kan fixa det där.

1. Klicka på **[!UICONTROL Edit Mappings]**.

![](assets/image2014-12-9-13-3a31-3a0.png)

1. Öppna mappen **[!UICONTROL Unmapped Custom Fields]**.

   ![](assets/two.png)

1. Dra ett omappat anpassat fält till ett annat för att mappa dem tillsammans.

   >[!NOTE]
   >
   >Du kan bara redigera anpassade fältkopplingar. Standardfältkopplingar kan inte ändras.

   ![](assets/three.png)

1. Klicka på **[!UICONTROL Finish Mappings]** när du är klar.

   ![](assets/four.png)

## Bryt befintlig mappning {#break-existing-mapping}

Om du har fält med liknande namn på lead- och kontaktobjektet mappas de automatiskt av Marketo. Du kan anse att de är olika och att de har olika data. Bryt mappningen så här.

1. Klicka på **[!UICONTROL Edit Mappings]**.

   ![](assets/image2014-12-9-13-3a31-3a37.png)

1. Markera ett mappat fält och klicka på **[!UICONTROL Break Mapping]** för att separera fälten.

   ![](assets/image2014-12-9-13-3a31-3a47.png)

1. Klicka på **[!UICONTROL Finish Mappings]** när du är klar.

   ![](assets/image2014-12-9-13-3a31-3a58.png)

   Snyggt! Du är nästan klar med den inledande synkroniseringen.

## Återställ schema {#reset-schema}

1. Om du gör några ändringar i schemat i Salesforce medan du arbetar med mappningarna kan du dra in ändringarna genom att klicka på **[!UICONTROL Reset Schema]**.

   * Alla mappningsändringar återställs!
   * Om du återställer schemat läggs bara fält till, inte tas bort (även om du döljer dem för synkroniseringsanvändaren).

   ![](assets/image2014-12-9-13-3a32-3a8.png)
