---
unique-page-id: 2359418
description: Importera en lista med människor - Marketo Docs - Produktdokumentation
title: Importera en lista med personer
translation-type: tm+mt
source-git-commit: d7d6aee63144c472e02fe0221c4a164183d04dd4
workflow-type: tm+mt
source-wordcount: '496'
ht-degree: 0%

---


# Importera en lista med personer {#import-a-list-of-people}

## Uppdrag: Importera en kalkylbladslista med deltagande i affärsprogram till din databas {#mission-import-a-spreadsheet-list-of-trade-show-attendees-into-your-database}

>[!PREREQUISITES]
>
>[Konfigurera och lägga till en person](/help/marketo/getting-started/quick-wins/get-set-up-and-add-a-person.md)

I den här självstudiekursen får du lära dig att importera personer från en kalkylbladsfil till Marketo.

## Steg 1: Hämta och redigera ett kalkylblad {#step-download-and-edit-a-spreadsheet}

1. Börja med att ladda ned vår övningskalkylbladsfil ([**tradeshow-Attendees.csv**](https://docs.marketo.com/display/docs/assets/tradeshow-attendees.csv)) till datorn.

   ![](assets/image2014-9-24-12-3a5-3a0.png)

   >[!NOTE]
   >
   >Använd följande format när du importerar ett datum: **9/21/20** (månad/dag/år).

   >[!NOTE]
   >
   >Alla datum-/tidfält som importeras behandlas som centraltid. Om du har datum-/tidsfält i en annan tidszon kan du använda en Excel-formel för att omvandla den till Central Time (USA/Chicago).

1. Lägg till ditt eget förnamn, efternamn, e-postadress och jobbtitel och spara sedan filen på datorn.

   ![](assets/image2014-9-24-12-3a5-3a30.png)

>[!NOTE]
>
>Ange din riktiga e-postadress i CSV-filen så att du kan ta emot de närliggande e-postmeddelanden du skickar i nästa uppdrag.

## Steg 2: Skapa ett program {#step-create-a-program}

1. Gå till **Marknadsföringsaktiviteter**.

   ![](assets/ma-2.png)

1. Välj mappen **Learning** och klicka sedan på **Nytt program** under **Nytt**.

   ![](assets/image2014-9-24-12-3a21-3a13.png)

1. **Ge** programmet namnet&quot;My Tradeshow Program&quot; och välj&quot;Event&quot; som  **programtyp**.

   ![](assets/image2014-9-24-12-3a21-3a25.png)

1. Välj **Tradeshow** för **Channel** och klicka på **Create**.

   ![](assets/image2014-9-24-12-3a21-3a39.png)

>[!NOTE]
>
>Händelseprogram inträffar vid specifika datum. Läs mer om [**Händelser**](/help/marketo/product-docs/demand-generation/events/understanding-events/understanding-event-programs.md).

## Steg 3: Importera ditt kalkylblad till Marketo {#step-import-your-spreadsheet-into-marketo}

1. I **My Tradeshow Program** klickar du på **Nytt** och väljer **Ny lokal resurs**.

   ![](assets/seven-3.png)

1. Klicka på **Lista**.

   ![](assets/image2014-9-24-12-3a22-3a56.png)

1. **Ge** listan namnet&quot;Deltagare i mässa&quot; och klicka på  **Skapa**.

   ![](assets/image2014-9-24-12-3a23-3a9.png)

1. Klicka på **Visa åtgärder** och välj **Importera lista** i listan **Deltagare**.

   ![](assets/ten-2.png)

   >[!CAUTION]
   >
   >Om du använder en egen CSV-fil måste du se till att den är kodad UTF-8, UTF-16, Shift-JIS eller EUC-JP.

   >[!NOTE]
   >
   >Storleksgränsen för CSV-filer är 100 MB.

1. **Bläddra** till  **filen tradeshow-Attendees.** csvkalkylblad på datorn och klicka på  **Nästa**.

   ![](assets/eleven-2.png)

   >[!NOTE]
   >
   >Om du väljer **Hoppa över nya personer och uppdateringar** i listimportläget påverkas inte befintliga personposter och du loggar inga aktiviteter. Använd det här läget om du vill ha en snabb, förfiltrerad statisk lista över befintliga personer som kan användas i dina marknadsföringsaktiviteter. Om du väljer det här läget:
   >
   > * Hoppa över skapande av ny person
   > * Hoppa över uppdateringar av personfält
   > * Hoppa över aktivitetsloggning


1. Koppla listkolumnsfälten till deras respektive Marketo-fält och klicka på **Nästa**.

   ![](assets/image2014-9-24-12-3a24-3a49.png)

   >[!TIP]
   >
   >Kolumnrubrikerna ska alltid matcha fältet exakt (skiftlägeskänsligt) för att uppnå bästa resultat för automatisk mappning. Om du använder anpassade fält och inte ser dem i listrutan går du tillbaka och [skapar dem](/help/marketo/product-docs/administration/field-management/create-a-custom-field-in-marketo.md) så att de kan bli alternativ.

   >[!NOTE]
   >
   >Om det finns fält som du inte vill importera väljer du **Ignorera** i listrutan Marketfält.

1. Välj **My Tradeshow Program** för **förvärvsprogrammet** och klicka sedan på **Importera**.

   ![](assets/image2014-9-24-12-3a25-3a1.png)

1. Vänta tills dina personer har importerats och stäng sedan popup-fönstret för importförloppet.

   ![](assets/image2014-9-24-12-3a25-3a13.png)

1. Gå tillbaka i **Mitt utbildningsprogram** och klicka på fliken **Medlemmar**. Du kommer att se alla de personer du just importerat.

   ![](assets/fifteen-1.png)

>[!NOTE]
>
>Du kan analysera hur ditt program fungerar genom att spåra programmedlemskap. Läs mer om [**Program**](/help/marketo/product-docs/core-marketo-concepts/programs/creating-programs/understanding-programs.md).

## Uppdraget är klart {#mission-complete}

Nu är deltagarna i ditt varumärke medlemmar i ditt Marketo-program!

<br> 

[◄ 4: Automatiskt svar för e-post](/help/marketo/getting-started/quick-wins/email-auto-response.md)

[Uppdrag 6: Drip, Drip, Sköldhet ►](/help/marketo/getting-started/quick-wins/drip-drip-nurture.md)
