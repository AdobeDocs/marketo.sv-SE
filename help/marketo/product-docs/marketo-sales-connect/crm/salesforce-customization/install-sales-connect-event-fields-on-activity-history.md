---
unique-page-id: 14352475
description: Installera händelsefält för anslutning av försäljning på aktivitetshistorik - Marketo Docs - produktdokumentation
title: Installera händelsefält för försäljningsanslutning i aktivitetshistorik
exl-id: c1bdb5a6-04f0-4579-84b6-33f4a301128f
feature: Marketo Sales Connect
source-git-commit: 431bd258f9a68bbb9df7acf043085578d3d91b1f
workflow-type: tm+mt
source-wordcount: '269'
ht-degree: 0%

---

# Installera händelsefält för försäljningsanslutning i aktivitetshistorik {#install-sales-connect-event-fields-on-activity-history}

När du har installerat Enterprise-paketet i Salesforce kan du installera fälten för Sales Connect-händelser i din aktivitetshistorik. Händelsefält för Sales Connect innehåller information som vyer, klick och kampanjer. På så sätt kan du få information om dina e-postmeddelanden direkt importerade till Salesforce.

Se till att du samarbetar med din Salesforce-administratör när du utför de här stegen. I det här exemplet ska vi installera fälten på **Sidlayout för leads**. Du kan även installera fälten på sidlayouterna för kontakt, konto och säljprojekt. Kom ihåg att när du loggar e-postmeddelanden till konton och säljprojekt måste du ha kontakten som du skickar som en kontaktroll.

1. Klicka **Inställningar**.
1. Klicka **Anpassa**.
1. Klicka **Leads**.
1. Klicka **Sidlayouter**.
1. Klicka **Redigera** bredvid sidlayouten som du vill ändra.

   >[!NOTE]
   >
   >Sales Connect kommer att installera vissa sidlayouter åt dig, men om du redan har en standardlayout som teamet använder måste du installera den där. Du kan ta bort sidlayouterna Sales Connect om du inte vill använda dem.

1. Bläddra nedåt till avsnittet Aktivitetshistorik.
1. Klicka på den skiftnyckel som du vill redigera.
1. Markera de Sales Connect-fält som du vill ta med i avsnittet Aktivitetshistorik. Om du inte ser Sales Connect-fält här kan du ha installerat fel Salesforce-paket.
1. Klicka **Lägg till** om du vill flytta de önskade fälten.
1. Klicka **OK**.
1. Klicka **Spara**.

   Dina användare kan nu se värdefull information och uppdateringar om sina e-postmeddelanden i Salesforce!
