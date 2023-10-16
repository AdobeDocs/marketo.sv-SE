---
unique-page-id: 1146987
description: Ta bort ett flödessteg - Marketo Docs - produktdokumentation
title: Ta bort ett flödessteg
exl-id: 039a1e80-48cc-47f9-9e1a-459f89bf0730
feature: Smart Campaigns
source-git-commit: 9e51ece12742152040dbbcb6a1584fba28e863ff
workflow-type: tm+mt
source-wordcount: '361'
ht-degree: 0%

---

# Ta bort ett flödessteg {#delete-a-flow-step}

>[!CAUTION]
>
>Tar bort flödessteg, _särskilt väntesteg_ från aktiva smarta kampanjer kan få oväntade resultat. Läs den här artikeln noggrant.

Först tar vi grunderna. Så här tar du bort ett oönskat flödessteg från en smart kampanj.

1. I Smart Campaign **[!UICONTROL Flow]** klickar du på **X** om du vill ta bort ett flödessteg.

![](assets/image2014-9-22-13-3a52-3a20.png)

1. Klicka på **[!UICONTROL Delete]**.

   ![](assets/image2014-9-22-13-3a55-3a25.png)

   Enkelt och enkelt, eller hur? För det mesta..

   >[!CAUTION]
   >
   >Ta bort, lägga till och flytta steg i en _aktiv_ kampanjen kan definitivt få oväntade resultat. Överväg att skapa en ny kampanj, testa den och sedan byta kampanj.

   Ändringar kan göras i en aktiv kampanj, men kan få oförutsedda konsekvenser. Här är detaljerna:

   **Batchsmarta kampanjer**

   Om kampanjen:

   1. **Aldrig körd**. Gör alla ändringar du vill. Det kommer inte att påverka någon förrän ni genomför kampanjen.
   1. **Är en återkommande smart kampanj**. Ändringarna kommer att påverka andra användare i framtiden, inte tidigare.
   1. **Kördes redan UTAN väntesteg** Ingen kommer att påverkas eftersom kampanjen är vilande efter att ha körts.
   1. **Körs just nu**. Ändringar kan orsaka oväntat beteende beroende på tidpunkten och informationen för borttagningen. Vi rekommenderar att du INTE redigerar en batchkampanj som aktivt körs. Lär dig hur man gör i krissituationer [avbryta en aktiv smart kampanj](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/using-smart-campaigns/abort-a-smart-campaign.md){target="_blank"}.

   1. **Kördes redan med väntesteg.** Flera detaljer om den här.\
      När en person går in i ett vänteläge sänker personen längden och anger vilket NUMBER-STEG han/hon ska gå tillbaka till. Se exemplet nedan.

   **Utlös smarta kampanjer**

   1. **Inga väntesteg**. Om du tar bort ett normalt steg påverkas bara personer som kör kampanjen i framtiden.
   1. **Med väntesteg**. Se exemplet nedan för batchkampanjer. Samma logik gäller.

   >[!NOTE]
   >
   >**Exempel**
   >
   >1. En Smart Campaign består av tre steg.
   >    * STEG 1. Skicka e-post nr 1
   >    * STEG 2. Vänta en vecka
   >    * STEG 3. Skicka e-post nr 2
   >
   >1. Folk som träffade **Steg 2** väntar 1 vecka innan du går vidare till **Steg 3**.
   >1. Du tar bort **Steg 2** under veckan.
   >1. Folk kommer att fortsätta vänta i 1 vecka (de kommer inte automatiskt tillbaka till flödet).
   >1. När de äntligen kommer tillbaka försöker de att gå till **Steg 3**. De kommer inte att hitta den.
   >1. **VIKTIGT!** Eftersom det nu bara finns två steg _får inte e-post nr 2_.
