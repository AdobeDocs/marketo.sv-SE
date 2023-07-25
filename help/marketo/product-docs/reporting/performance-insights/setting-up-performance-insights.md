---
unique-page-id: 12981145
description: Ställa in prestandainsikter - Marketo Docs - produktdokumentation
title: Konfigurera prestandainsikter
exl-id: f87bbaba-c2c1-4b83-9e07-f8a5d1f1738b
feature: Reporting
source-git-commit: 431bd258f9a68bbb9df7acf043085578d3d91b1f
workflow-type: tm+mt
source-wordcount: '307'
ht-degree: 0%

---

# Konfigurera prestandainsikter {#setting-up-performance-insights}

Följ stegen nedan för att konfigurera MPI.

## Inställningar för affärsmöjlighet {#opportunity-setup}

1. Klicka **Administratör**.

   ![](assets/admin.png)

1. Klicka **Analys av intäktscykler**.

   ![](assets/two-2.png)

   >[!NOTE]
   >
   >Om du inte har RCA måste du välja **Programanalys** för steg 2.

1. Klicka på under Attribution **Redigera**.

   ![](assets/three-1.png)

1. Attributinställningar visas.

   ![](assets/four-2.png)

   Om attribuering är explicit kontrollerar du att säljprojektskontaktrollen har fyllts i (antingen via slutpunkten för säljprojektsrollen eller via CRM-integrering).

   Om Attribution är implicit kontrollerar du att företagsfältet på leadet/kontakten är samma som kontonamnet för affärsmöjligheten.

   >[!NOTE]
   >
   >Se till att rätt fält fylls i för alla affärsmöjligheter:
   >
   >* Affärsmöjlighet - belopp
   >* Är stängd
   >* Är vunnen
   >* Skapad den (kan inte anges i ditt fall)
   >* Stängt datum (detta kan inte anges i ditt fall)
   >* Typ av affärsmöjlighet

## Programinställningar {#program-setup}

Uppdatera programkostnaderna i minst 12 månader. Du kan göra detta manuellt eller med program-API:t. I det här exemplet gör vi det manuellt.

1. Klicka **Marknadsföringsaktiviteter**.

   ![](assets/ma.png)

1. Hitta och välj program.

   ![](assets/select-program.png)

1. Klicka på **Inställningar** -fliken.

   ![](assets/setup-tab.png)

1. Dra **Periodkostnad** på arbetsytan.

   ![](assets/period-cost.png)

1. Ställ in programmånaden för minst 12 månader sedan och klicka på **OK**.

   ![](assets/set-period.png)

1. Ange periodkostnad och klicka på **Spara**.

   ![](assets/set-cost.png)

Granska sedan analysbeteendet för att ange om en viss kanal ska inkluderas i analysen. Ange analysbeteende (normal, inkluderande, operativ).

1. Klicka **Administratör**.

   ![](assets/admin.png)

1. Klicka **Taggar**.

   ![](assets/tags.png)

1. Klicka på **+** för att expandera kanallistan.

   ![](assets/channel.png)

1. Dubbelklicka på den önskade kanalen.

   ![](assets/channel-click.png)

1. Klicka på **Analysbeteende** och välj önskat beteende.

   ![](assets/edit-channel.png)

1. Ange kriterier för framgång.

   ![](assets/success.png)

1. Klicka **Spara**.

   ![](assets/save.png)

## Koppla programmet till personen {#tie-the-program-to-the-person}

1. Kontrollera att inköpsprogrammet och förvärvsdatumet har angetts för varje person i databasen för att First Touch Attribution ska fungera.
1. Se till att era program är framgångslägen för era medarbetare.

>[!NOTE]
>
>Ändringarna görs inte omedelbart. En nattetid krävs innan ändringarna träder i kraft.
