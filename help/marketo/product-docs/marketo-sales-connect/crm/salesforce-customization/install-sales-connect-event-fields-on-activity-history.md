---
unique-page-id: 14352475
description: Installera händelsefält för anslutning av försäljning på aktivitetshistorik - Marketo-dokument - produktdokumentation
title: Installera händelsefält för försäljningsanslutning i aktivitetshistorik
translation-type: tm+mt
source-git-commit: 47b2fee7d146c3dc558d4bbb10070683f4cdfd3d
workflow-type: tm+mt
source-wordcount: '269'
ht-degree: 0%

---


# Installera händelsefält för försäljningsanslutning i aktivitetshistorik {#install-sales-connect-event-fields-on-activity-history}

När du har installerat Enterprise-paketet i Salesforce kan du installera fälten för Sales Connect-händelser i din aktivitetshistorik. Händelsefält för Sales Connect innehåller information som vyer, klick och kampanjer. På så sätt kan du få information om dina e-postmeddelanden direkt importerade till Salesforce.

Se till att du samarbetar med din Salesforce-administratör när du utför de här stegen. I det här exemplet ska vi installera fälten på **sidlayouten** Leads. Du kan även installera fälten på sidlayouterna för kontakt, konto och säljprojekt. Kom ihåg att när du loggar e-postmeddelanden till konton och säljprojekt måste du ha kontakten som du skickar som en kontaktroll.

1. Klicka på **Konfigurera**.
1. Klicka på **Anpassa**.
1. Klicka på **Leads**.
1. Klicka på **Sidlayouter**.
1. Klicka på **Redigera** bredvid den sidlayout som du vill ändra.

   >[!NOTE]
   >
   >Sales Connect kommer att installera vissa sidlayouter åt dig, men om du redan har en standardlayout som teamet använder måste du installera den där. Du kan ta bort sidlayouterna Sales Connect om du inte vill använda dem.

1. Bläddra nedåt till avsnittet Aktivitetshistorik.
1. Klicka på den skiftnyckel som du vill redigera.
1. Markera de Sales Connect-fält som du vill ta med i avsnittet Aktivitetshistorik. Om du inte ser Sales Connect-fält här kan du ha installerat fel Salesforce-paket.
1. Klicka på **Lägg** till om du vill flytta fälten.
1. Klicka på **OK**.
1. Klicka på **Spara**.

   Dina användare kan nu se värdefull information och uppdateringar om sina e-postmeddelanden i Salesforce!

