---
unique-page-id: 1146987
description: Ta bort ett flödessteg - Marketo Docs - Produktdokumentation
title: Ta bort ett flödessteg
translation-type: tm+mt
source-git-commit: d7d6aee63144c472e02fe0221c4a164183d04dd4
workflow-type: tm+mt
source-wordcount: '378'
ht-degree: 0%

---


# Ta bort ett flödessteg {#delete-a-flow-step}

>[!CAUTION]
>
>Om du tar bort flödessteg, *speciellt väntesteg* från aktiva smarta kampanjer, kan det få oväntade resultat. **Läs den här artikeln noggrant.**

Först gör vi grunderna. Så här tar du bort ett oönskat flödessteg från en smart kampanj. 1. Klicka på X-ikonen i det smarta kampanjflödet för att ta bort eventuella flödessteg.

![](assets/image2014-9-22-13-3a52-3a20.png)

1. Klicka på **Ta bort**.

   ![](assets/image2014-9-22-13-3a55-3a25.png)

   Enkelt och enkelt, eller hur? För det mesta..

   >[!CAUTION]
   >
   >Att ta bort, lägga till och flytta steg i en **aktiv**-kampanj kan definitivt ge oväntade resultat. Överväg att skapa en ny kampanj, testa den och sedan byta kampanj.

   Ändringar kan göras i en aktiv kampanj, men kan få oförutsedda konsekvenser. Här är detaljerna:

   **Smarta gruppkampanjer**

   Om kampanjen:

   1. **Aldrig sprang.** Gör alla ändringar du vill. Det kommer inte att påverka någon förrän ni genomför kampanjen.
   1. **Är en återkommande smart kampanj.** Ändringarna kommer att påverka andra användare i framtiden, inte i tidigare körningar.
   1. **Kördes redan UTAN väntesteg.** Ingen kommer att påverkas eftersom kampanjen är vilande efter att ha körts.
   1. **Kör just nu.** Ändringar kan orsaka oväntat beteende beroende på tidpunkten och informationen för borttagningen. Vi rekommenderar att du INTE redigerar en batchkampanj som aktivt körs. Lär dig hur du avbryter en smart kampanj[ som körs i nödfall.](../../../../product-docs/core-marketo-concepts/smart-campaigns/using-smart-campaigns/abort-a-smart-campaign.md)

   1. **Kördes redan med väntesteg.** Flera detaljer om den här.\
      När en person går in i ett vänteläge sänker personen längden och anger vilket NUMBER-STEG han/hon ska gå tillbaka till. Se exemplet nedan.

   **Utlös smarta kampanjer**

   1. **Inga väntesteg.** Om du tar bort ett normalt steg påverkas bara personer som kör kampanjen i framtiden.
   1. **Med väntesteg.** Se exemplet nedan för batchkampanjer. Samma logik gäller.

   >[!NOTE]
   >
   >**Exempel**
   >
   >    
   >    
   >1. En smart kampanj består av tre steg.
   >
   >   * STEG 1. Skicka e-post nr 1
   >   * STEG 2. Vänta en vecka
   >   * STEG 3. Skicka e-post nr 2
   >
   >1. Personer som trycker på **Steg 2** väntar en vecka innan de går vidare till **Steg 3**.
   >1. Du tar bort **Steg 2** under veckan.
   >1. Folk kommer att fortsätta vänta 1 vecka. (De kommer inte automatiskt tillbaka till flödet.)
   >1. När de slutligen kommer tillbaka försöker de gå till **Steg 3**. De kommer inte att hitta den.
   >1. **VIKTIGT:** Eftersom det nu bara finns två steg kommer  *personerna inte att få e-post nr 2.*


Göra ändringar i en aktiv kampanj

Förstå den här funktionen så får ni överordnad smarta kampanjer. Hej!
