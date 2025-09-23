---
unique-page-id: 14352475
description: Installera händelsefält för anslutning av försäljning på aktivitetshistorik - Marketo Docs - produktdokumentation
title: Installera händelsefält för försäljningsanslutning i aktivitetshistorik
exl-id: c1bdb5a6-04f0-4579-84b6-33f4a301128f
feature: Marketo Sales Connect
source-git-commit: 09a656c3a0d0002edfa1a61b987bff4c1dff33cf
workflow-type: tm+mt
source-wordcount: '239'
ht-degree: 2%

---

# Installera händelsefält för försäljningsanslutning i aktivitetshistorik {#install-sales-connect-event-fields-on-activity-history}

När du har installerat Enterprise-paketet i [!DNL Salesforce] kan du installera [!UICONTROL Sales Connect]-händelsefält i aktivitetshistoriken. [!UICONTROL Sales Connect] händelsefält innehåller information som vyer, klick och kampanjer. Det gör att du kan importera information om dina e-postmeddelanden direkt till [!DNL Salesforce].

Se till att du samarbetar med din [!DNL Salesforce]-administratör när du utför de här stegen. I det här exemplet kommer vi att installera fälten på **sidlayouten Leads**. Du kan även installera fälten på sidlayouterna för kontakt, konto och säljprojekt. Kom ihåg att när du loggar e-postmeddelanden till konton och säljprojekt måste du ha kontakten som du skickar som en kontaktroll.

1. Klicka på **[!UICONTROL Setup]**.
1. Klicka på **[!UICONTROL Customize]**.
1. Klicka på **[!UICONTROL Leads]**.
1. Klicka på **[!UICONTROL Page Layouts]**.
1. Klicka på **[!UICONTROL Edit]** bredvid sidlayouten som du vill ändra.

   >[!NOTE]
   >
   >[!DNL Sales Connect] kommer att installera vissa sidlayouter åt dig, men om du redan har en standardlayout som används av ditt team bör du installera den där. Du kan ta bort sidlayouterna [!DNL Sales Connect] om du inte vill använda dem.

1. Rulla ned till avsnittet [!UICONTROL Activity History].
1. Klicka på den skiftnyckel som du vill redigera.
1. Markera de [!UICONTROL Sales Connect] fält som du vill ta med i avsnittet [!UICONTROL Activity History]. Om du inte ser [!UICONTROL Sales Connect] fält här kan du ha installerat fel [!DNL Salesforce]-paket.
1. Klicka på **[!UICONTROL Add]** om du vill flytta över de önskade fälten.
1. Klicka på **[!UICONTROL OK]**.
1. Klicka på **[!UICONTROL Save]**.

   Dina användare kan nu se värdefull information och uppdateringar om sina e-postmeddelanden i [!DNL Salesforce]!
