---
unique-page-id: 17727995
description: Email CC - Marketo Docs - produktdokumentation
title: Email CC
exl-id: 00550e98-916d-4e66-91f8-7394c242a29b
feature: Email Editor
source-git-commit: 431bd258f9a68bbb9df7acf043085578d3d91b1f
workflow-type: tm+mt
source-wordcount: '547'
ht-degree: 0%

---

# Email CC {#email-cc}

Med Email CC kan angivna e-postmeddelanden skickas via Marketo till CC-mottagare.

Den här funktionen är tillgänglig för alla e-postresurser från Marketo, oavsett hur e-postmeddelandet skickas (batch- eller utlösarkampanj). CC-mottagaren får en exakt kopia av e-postmeddelandet som skickas till den valda Marketo-personen. Därför kan alla aktiviteter (öppningar, klickningar osv.) loggas i aktivitetsloggen för Marketo-personen på raden &quot;Till&quot; i e-postmeddelandet. Leveransaktivitet (skickad, levererad, hård studsning osv.) _annat än &quot;mjuk studs&quot;_ kommer **not** registrera eftersom Marketo inte kan skilja leveranshändelser för Marketo-personen från CC-mottagarnas. Marketo kommer endast att kunna CC för upp till 100 000 personer åt gången. Om din smarta lista överstiger 100 kB och det är absolut nödvändigt att alla personer på den får CC rekommenderar vi att du delar upp din lista.

>[!NOTE]
>
>Email CC var inte utformat för att användas med A/B-tester. Du kan använda det i alla fall om du vill, men eftersom det tekniskt inte stöds, kan Marketo Support inte hjälpa till med felsökningen.

## Konfigurera e-post-CC {#set-up-email-cc}

1. I Min Marketo klickar du på **Administratör**.

   ![](assets/one.png)

1. Välj **E-post**.

   ![](assets/two.png)

1. Klicka **Redigera inställningar för e-postkopia**.

   ![](assets/three.png)

1. Välj upp till 25 Marketo lead- eller företagsfält (av typen &quot;E-post&quot;) som ska vara tillgängliga som CC-adresser i e-postmeddelanden. Klicka **Spara** när det är klart.

   ![](assets/four.png)

## Använda Email CC {#using-email-cc}

1. Välj e-post och klicka **Redigera utkast**.

   ![](assets/five.png)

1. Klicka **E-postinställningar**.

   ![](assets/six.png)

1. Välj upp till fem fält som du vill använda för CC-användare. I det här exemplet vill vi bara ha Lead Owner CC&#39;d. Klicka **Spara** när det är klart.

   ![](assets/seven.png)

   Så enkelt är det! När du skickar e-postmeddelandet i exemplet ovan kommer lead-ägaren för de valda mottagarna att vara CC.

   >[!NOTE]
   >
   >Om en ogiltig e-postadress finns i ett CC-fält hoppas den över.

   För snabb identifiering visar e-postsammanfattningsvyn om/vilka e-postfält som har valts.

   ![](assets/eight.png)

   Om e-postmeddelandet har godkänts men Marketo Admin inaktiverar ett eller flera av CC-fälten innan e-postmeddelandet skickas, **de personerna inte får något e-postmeddelande**. I så fall kommer e-postsammanfattningsvyn att visa alla fält som inaktiverats efter godkännande men som skickats i förväg:

   ![](assets/removal.png)

   >[!NOTE]
   >
   >Du ser även ovanstående fel i avsnittet E-postinställningar i e-postutkastet.

## Efter Skicka {#after-the-send}

* Om en CC-mottagare klickar på en spårad länk i e-postmeddelandet, kommer klickaktiviteten (som alla andra interaktionsaktiviteter) att associeras med e-postmeddelandets huvudmottagare. Dessutom kan de klicka sig fram till en sida med Marketo webbspårningskod (munchkin.js), vilket gör att de kodas som huvudmottagare.

>[!TIP]
>
>Du kan välja att [inaktivera vissa eller alla spårningslänkar](/help/marketo/product-docs/email-marketing/general/functions-in-the-editor/disable-tracking-for-an-email-link.md) i ett mejl.

* När en e-postkampanj har körts innehåller aktiviteten Skicka e-post en lista med alla CC-adresser som har inkluderats för varje mottagare av e-postmeddelandet. Om några CC-adresser hoppades över på grund av att prenumerationen avbrutits, kommer även den att registreras i aktiviteten.
* Avbeställ länkarna och sidorna fungerar normalt i e-postmeddelanden från CC. Detta gör att CC-mottagare kan avbeställa prenumerationen om de vill (och följa reglerna för skräppostskydd), och en post för den här åtgärden lagras i Marketo-databasen.
* Personer som är listade som avbeställda i din Marketo-databas kommer att **not** ta emot e-postmeddelanden via CC.
