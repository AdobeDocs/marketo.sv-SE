---
unique-page-id: 2359418
description: Importera en lista med människor - Marketo Docs - produktdokumentation
title: Importera en lista med personer
exl-id: a85ec787-7b22-4666-84fd-d7bf23d32cd4
source-git-commit: a3da3f466e6131fdd3507b7b567fac91ad9c5b6c
workflow-type: tm+mt
source-wordcount: '490'
ht-degree: 0%

---

# Importera en lista med personer {#import-a-list-of-people}

## Uppdrag: Importera en kalkylbladslista med deltagande i affärsprogram till databasen {#mission-import-a-spreadsheet-list-of-trade-show-attendees-into-your-database}

>[!PREREQUISITES]
>
>[Konfigurera och lägga till en person](/help/marketo/getting-started/quick-wins/get-set-up-and-add-a-person.md)

I den här självstudiekursen får du lära dig hur du importerar personer från en kalkylbladsfil till Marketo.

## Steg 1: Hämta och redigera ett kalkylblad {#step-download-and-edit-a-spreadsheet}

1. Börja med att ladda ned en övningsfil ([**tradeshow-Attendees.csv**](/help/marketo/getting-started/assets/tradeshow-attendees.csv)) till datorn.

   ![](assets/image2014-9-24-12-3a5-3a0.png)

   >[!NOTE]
   >
   >Använd följande format när du importerar ett datum: **9/21/20** (månad/dag/år).

   >[!NOTE]
   >
   >Alla datum-/tidfält som importeras behandlas som centraltid. Om du har datum-/tidsfält i en annan tidszon kan du använda en Excel-formel för att omvandla den till Central Time (USA/Chicago).

1. Lägg till ditt eget förnamn, efternamn, faktisk e-postadress (så att du kan ta emot de närliggande e-postmeddelanden du skickar i nästa uppdrag) och befattning. Spara filen på datorn.

   ![](assets/image2014-9-24-12-3a5-3a30.png)

   >[!CAUTION]
   >
   >Marketo gör det **not** har stöd för e-postadresser som innehåller känslolägesikoner.

## Steg 2: Skapa ett program {#step-create-a-program}

1. Gå till **Marknadsföringsaktiviteter** område.

   ![](assets/ma-2.png)

1. Välj **Utbildning** mapp, sedan under **Nytt** klicka **Nytt program**.

   ![](assets/image2014-9-24-12-3a21-3a13.png)

1. **Namn** Programmet&quot;My Tradeshow Program&quot; och välj&quot;Event&quot; för **Programtyp**.

   ![](assets/image2014-9-24-12-3a21-3a25.png)

1. Välj **Varumärke** för **Kanal** och klicka **Skapa**.

   ![](assets/image2014-9-24-12-3a21-3a39.png)

>[!NOTE]
>
>Händelseprogram inträffar vid specifika datum. Läs mer om [**Händelser**](/help/marketo/product-docs/demand-generation/events/understanding-events/understanding-event-programs.md).

## Steg 3: Importera kalkylblad till Marketo {#step-import-your-spreadsheet-into-marketo}

1. I **Mitt Tradeshow Program**, klicka **Nytt** och markera **Ny lokal resurs**.

   ![](assets/seven-3.png)

1. Klicka **Lista**.

   ![](assets/image2014-9-24-12-3a22-3a56.png)

1. **Namn** i listan&quot;Tradeshow Attendees&quot; och klickar på **Skapa**.

   ![](assets/image2014-9-24-12-3a23-3a9.png)

1. I **Deltagare i mässor** lista, klicka på **Liståtgärder** och markera **Importera lista**.

   ![](assets/ten-2.png)

   >[!CAUTION]
   >
   >Om du använder en egen CSV-fil måste du se till att den är kodad UTF-8, UTF-16, Shift-JIS eller EUC-JP.

   >[!NOTE]
   >
   >Storleksgränsen för CSV-filer är 100 MB.

1. **Bläddra** till **tradeshow-Attendees.csv** kalkylbladsfil på datorn och klicka på **Nästa**.

   ![](assets/eleven-2.png)

   >[!NOTE]
   >
   >I listimportläge väljer du **Hoppa över nya personer och uppdateringar** innebär att du inte kommer att påverka befintliga personposter eller logga några aktiviteter. Använd det här läget om du vill ha en snabb, förfiltrerad statisk lista över befintliga personer som kan användas i dina marknadsföringsaktiviteter. Om du väljer det här läget:
   >
   > * Hoppa över skapande av ny person
   > * Hoppa över uppdateringar av personfält
   > * Hoppa över aktivitetsloggning


1. Mappa listkolumnfälten till deras respektive Marketo-fält och klicka på **Nästa**.

   ![](assets/image2014-9-24-12-3a24-3a49.png)

   >[!TIP]
   >
   >Kolumnrubrikerna ska alltid matcha fältet exakt (skiftlägeskänsligt) för att uppnå bästa resultat för automatisk mappning. Om du använder anpassade fält och inte ser dem i listrutan går du tillbaka och [skapa dem](/help/marketo/product-docs/administration/field-management/create-a-custom-field-in-marketo.md) så att de kan bli alternativ.

   >[!NOTE]
   >
   >Om det finns fält som du inte vill importera väljer du **Ignorera** i listrutan Marketo Field.

1. Välj **Mitt Tradeshow Program** för **Anskaffningsprogram** och sedan klicka **Importera**.

   ![](assets/image2014-9-24-12-3a25-3a1.png)

1. Vänta tills dina personer har importerats och stäng sedan popup-fönstret för importförloppet.

   ![](assets/image2014-9-24-12-3a25-3a13.png)

1. Tillbaka in **Mitt Tradeshow Program** klickar du på **Medlemmar** -fliken. Du kommer att se alla de personer du just importerat.

   ![](assets/fifteen-1.png)

>[!NOTE]
>
>Du kan analysera hur ditt program fungerar genom att spåra programmedlemskap. Läs mer om [**Program**](/help/marketo/product-docs/core-marketo-concepts/programs/creating-programs/understanding-programs.md).

## Uppdraget är slutfört {#mission-complete}

Deltagarna i ditt varumärke är nu medlemmar i ditt Marketo-program!

<br> 

[◄ 4: Automatiskt svar för e-post](/help/marketo/getting-started/quick-wins/email-auto-response.md)

[Uppdrag 6: Drip, Drip, Sköldhet ►](/help/marketo/getting-started/quick-wins/drip-drip-nurture.md)
