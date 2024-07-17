---
unique-page-id: 1146987
description: Ta bort ett flödessteg - Marketo Docs - produktdokumentation
title: Ta bort ett flödessteg
exl-id: 039a1e80-48cc-47f9-9e1a-459f89bf0730
feature: Smart Campaigns
source-git-commit: 12f2399859c784095cc2c1df772c66c649106ba3
workflow-type: tm+mt
source-wordcount: '367'
ht-degree: 0%

---

# Ta bort ett flödessteg {#delete-a-flow-step}

>[!CAUTION]
>
>Om du tar bort flödessteg, _speciellt väntesteg_ från aktiva smarta kampanjer, kan det få oväntade resultat. Läs den här artikeln noggrant.

Först tar vi grunderna. Så här tar du bort ett oönskat flödessteg från en smart kampanj.

1. I den smarta kampanjen **[!UICONTROL Flow]** klickar du på ikonen **X** för att ta bort ett flödessteg.

   ![](assets/delete-a-flow-step-1.png)

1. Klicka på **[!UICONTROL Delete]**.

   ![](assets/delete-a-flow-step-2.png)

   >[!CAUTION]
   >
   >Om du tar bort, lägger till och flyttar steg i en _aktiv_-kampanj kan oväntade resultat uppstå. Överväg att skapa en ny kampanj, testa den och sedan byta kampanj.

   Ändringar kan göras i en aktiv kampanj, men kan få oförutsedda konsekvenser. Här är detaljerna:

   **Batchsmarta kampanjer**

   Om kampanjen:

   1. **Kördes aldrig**. Gör alla ändringar du vill. Det kommer inte att påverka någon förrän ni genomför kampanjen.
   1. **Är en återkommande smart kampanj**. Ändringarna kommer att påverka andra användare i framtiden, inte tidigare.
   1. **Kördes redan utan väntesteg**.Inga personer påverkas eftersom kampanjen är vilande efter körning.
   1. **Körs just nu**. Ändringar kan orsaka oväntat beteende beroende på tidpunkten och informationen för borttagningen. Vi rekommenderar att du INTE redigerar en batchkampanj som aktivt körs. Lär dig hur du [avbryter en smart kampanj som körs](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/using-smart-campaigns/abort-a-smart-campaign.md){target="_blank"} i nödfall.

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
   >1. Personer som trycker på **Steg 2** väntar en vecka innan de går vidare till **Steg 3**.
   >1. Du tar bort **Steg 2** under veckan.
   >1. Folk kommer att fortsätta vänta i 1 vecka (de kommer inte automatiskt tillbaka till flödet).
   >1. När de äntligen kommer tillbaka försöker de gå till **Steg 3**. De kommer inte att hitta den.
   >1. **VIKTIGT!** Eftersom det nu bara finns två steg kommer personerna _inte att få e-post nr 2_.
