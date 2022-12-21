---
unique-page-id: 13795727
description: Avbryt leverans av e-postprogram som schemalagts med mottagartidszon - Marketo Docs - produktdokumentation
title: Avbryt leverans av e-postprogram som schemalagts med mottagartidszon
exl-id: e69afa4a-32fb-4791-a9b6-683d64d610d6
source-git-commit: 72e1d29347bd5b77107da1e9c30169cb6490c432
workflow-type: tm+mt
source-wordcount: '219'
ht-degree: 0%

---

# Avbryt leverans av e-postprogram som schemalagts med mottagartidszon {#abort-delivery-of-email-programs-scheduled-with-recipient-time-zone}

I nödfall kan du avbryta leveransen av ett e-postprogram som redan har börjat köras med Mottagarens tidszon aktiverad.

Eftersom e-postprogram som schemaläggs med mottagartidszon kan köras i upp till 24 timmar kommer eventuella efterföljande utskick att avbrytas om du avbryter leveransen av programmet.

1. Välj det e-postprogram som du vill avbryta och klicka sedan på **Avbryt leverans** under rutan Godkännande på kontrollpanelen.

   ![](assets/ptz-abortdelivery.png)

1. Bekräfta att du vill avbryta leveransen genom att klicka på **Avbryt**.

   ![](assets/image2018-2-23-11-3a20-3a27.png)

1. Efter avbeställningen visas **Resultat** kommer ditt e-postprogram att se ut som det nedan. Eventuella efterföljande utskick avbryts och visas som&quot;Mejlbaserad mjuk&quot; i dialogrutan **Typ av aktivitet** kolumn.

   ![](assets/image2018-2-23-11-3a22-3a11.png)

   >[!NOTE]
   >
   >Avbrutna e-postmeddelanden kommer att **not** visa upp som ett mjukt studs *tills* den tidpunkt då de ursprungligen var planerade att levereras i sina respektive tidszoner. Fram tills dess visas de som&quot;Skicka e-post&quot;.

1. I rutnätet kan du klicka på valfritt e-postmeddelande för att visa aktivitetsinformation. Om du avbryter en sändning ser popup-fönstret med information ut så här:

   ![](assets/image2018-2-23-11-3a30-3a46.png)

>[!MORELIKETHIS]
>
>* [Förstå mottagartidszon](/help/marketo/product-docs/email-marketing/email-programs/email-program-actions/scheduling-with-recipient-time-zone/understanding-recipient-time-zone.md)
>* [Schemalägg e-postprogram med mottagartidszon](/help/marketo/product-docs/email-marketing/email-programs/email-program-actions/scheduling-with-recipient-time-zone/schedule-email-programs-with-recipient-time-zone.md)

