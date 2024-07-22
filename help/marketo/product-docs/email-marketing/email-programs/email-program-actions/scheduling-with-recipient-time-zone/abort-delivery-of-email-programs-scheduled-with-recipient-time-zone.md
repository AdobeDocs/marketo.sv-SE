---
unique-page-id: 13795727
description: Avbryt leverans av e-postprogram som schemalagts med mottagartidszon - Marketo Docs - produktdokumentation
title: Avbryt leverans av e-postprogram som schemalagts med mottagartidszon
exl-id: e69afa4a-32fb-4791-a9b6-683d64d610d6
feature: Email Programs
source-git-commit: 431bd258f9a68bbb9df7acf043085578d3d91b1f
workflow-type: tm+mt
source-wordcount: '220'
ht-degree: 0%

---

# Avbryt leverans av e-postprogram som schemalagts med mottagartidszon {#abort-delivery-of-email-programs-scheduled-with-recipient-time-zone}

I nödfall kan du avbryta leveransen av ett e-postprogram som redan har börjat köras med Mottagarens tidszon aktiverad.

Eftersom e-postprogram som schemaläggs med mottagartidszon kan köras i upp till 24 timmar kommer eventuella efterföljande utskick att avbrytas om leveransen avbryts.

1. Markera det e-postprogram som du vill avbryta och klicka sedan på **Avbryt leverans** under rutan Godkännande på kontrollpanelen.

   ![](assets/ptz-abortdelivery.png)

1. Bekräfta att du vill avbryta leveransen genom att klicka på **Avbryt**.

   ![](assets/image2018-2-23-11-3a20-3a27.png)

1. När du har avbrutit funktionen kommer rutnätet **Results** i ditt e-postprogram att se ut som det nedan. Eventuella efterföljande utskick avbryts och visas som&quot;E-postbaserad mjuk&quot; i kolumnen **Aktivitetstyp**.

   ![](assets/image2018-2-23-11-3a22-3a11.png)

   >[!NOTE]
   >
   >Avbrutna e-postmeddelanden visas **inte** som ett mjukt studs *förrän* den tid de ursprungligen var schemalagda att levereras i sina respektive tidszoner. Fram tills dess visas de som&quot;Skicka e-post&quot;.

1. I rutnätet kan du klicka på valfritt e-postmeddelande för att visa aktivitetsinformation. Om du avbryter en sändning ser popup-fönstret med information ut så här:

   ![](assets/image2018-2-23-11-3a30-3a46.png)

>[!MORELIKETHIS]
>
>* [Förstå mottagarens tidszon](/help/marketo/product-docs/email-marketing/email-programs/email-program-actions/scheduling-with-recipient-time-zone/understanding-recipient-time-zone.md)
>* [Schemalägg e-postprogram med mottagartidszon](/help/marketo/product-docs/email-marketing/email-programs/email-program-actions/scheduling-with-recipient-time-zone/schedule-email-programs-with-recipient-time-zone.md)
