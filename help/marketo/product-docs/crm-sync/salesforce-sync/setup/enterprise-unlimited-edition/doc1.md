---
description: Steg 1 av 3 - Lägg till Marketo-fält i Salesforce (Enterprise/Unlimited) - Marketo Docs - Produktdokumentation
title: Steg 1 av 3 - Lägg till Marketo-fält i Salesforce (Enterprise/Unlimited)
hide: true
hidefromtoc: true
feature: Salesforce Integration
source-git-commit: 989804463f44afbf35ab11c0f23c37b0d328e652
workflow-type: tm+mt
source-wordcount: '655'
ht-degree: 0%

---

# Steg 1 av 3: Lägg till Marketo-fält i Salesforce (Enterprise/Unlimited) {#step-of-add-marketo-fields-to-salesforce-enterprise-unlimited}

>[!PREREQUISITES]
>
>Du måste ha tillgång till Salesforce API:er för att kunna synkronisera mellan Marketo Engage och Salesforce.

Marketo använder en uppsättning fält för att samla in viss typ av marknadsföringsrelaterad information. Om du vill ha dessa data i Salesforce följer du instruktionerna nedan.

1. Skapa tre anpassade fält i Salesforce för lead- och kontaktobjekten: poäng, anskaffningsprogram och anskaffningsdatum.
1. Mappa dessa anpassade fält mellan leads och kontakter så att värdena överförs vid konvertering i Salesforce.
1. Du kan skapa ytterligare fält om det behövs (se tabellen nedan).

Alla dessa anpassade fält är valfria och behöver inte synkronisera Marketo och Salesforce. Vi rekommenderar att du skapar fält för poäng, anskaffningsprogram och anskaffningsdatum.

## Lägg till Marketo-fält i Salesforce {#add-marketo-fields-to-salesforce}

Lägg till tre anpassade fält i lead- och kontaktobjekten i Salesforce som listas ovan. Om du vill lägga till fler fält kan du läsa tabellen med tillgängliga fält i slutet av det här avsnittet.

Utför följande steg för vart och ett av de tre anpassade fälten för att lägga till dem. Börja med Score.

1. Logga in på Salesforce och klicka på Konfigurera.

   SCREENSHOT

1. Sök efter ordet &quot;Objekt&quot; i Snabbsökning

   SCREENSHOT

1. Klicka på Objekthanterare och sök efter&quot;Leads&quot;

   SCREENSHOT

1. Klicka på Lead under ETIKETT och klicka sedan på Fält och relationer till vänster.

   SCREENSHOT

1. Klicka på knappen Ny på sidan Fält och relationer

   SCREENSHOT

1. Välj lämplig fälttyp (för Poäng - tal; Anskaffningsprogram - text; Anskaffningsdatum - Datum/tid).

   SCREENSHOT

1. Klicka på Nästa.

   SCREENSHOT

1. Ange fältetikett, längd och fältnamn enligt tabellen nedan.

   TABELL

   >[!NOTE]
   >
   >Salesforce lägger till __c i fältnamn när de används för att skapa API-namn.

   SCREENSHOT

   >[!NOTE]
   >
   >Text- och nummerfält kräver en längd, men inte datum-/tidsfält. En beskrivning är valfri.

1. Klicka på Nästa.

   SCREENSHOT

1. Ange åtkomstinställningarna och klicka på Nästa:

   Ange alla roller som synliga och skrivskyddade

   Avmarkera kryssrutan Skrivskyddad för din synkroniseringsanvändares profil:

   Om du har en användare med profilen för en systemadministratör som synkroniseringsanvändare avmarkerar du kryssrutan Skrivskyddad för systemadministratörsprofilen (se nedan)
Om du har skapat en anpassad profil för synkroniseringsanvändaren avmarkerar du kryssrutan Skrivskyddad för den anpassade profilen

   SCREENSHOT

1. Välj de sidlayouter som ska visa fältet.

   SCREENSHOT

1. Klicka på Spara och ny för att gå tillbaka och skapa de två andra anpassade fälten. Klicka på Spara när du är klar med alla tre.

   SCREENSHOT

* Sök efter Kontakter i Objektshanteraren. Klicka på Fält och relationer.
* Utför steg 5 till 12 för fälten Poäng, Inköpsdatum och Anskaffningsprogram på kontaktobjektet, precis som för lead-objektet.
* Du kan också använda ovanstående procedur för ytterligare anpassade fält från den här tabellen.

  TABELL

  >[!NOTE]
  >
  >Värden i fält som automatiskt tilldelats av Marketo är inte omedelbart tillgängliga i Salesforce när det nya fältet har skapats. Marketo synkroniserar data till Salesforce vid nästa uppdatering av posten i något av systemen (dvs. en uppdatering av något av de synkroniserade fälten mellan Marketo och Salesforce).

## Mappa anpassade fält för konverteringar {#map-custom-fields-for-conversions}

Ett anpassat fält på lead-objektet i Salesforce bör mappas till ett kontaktfält på kontaktobjektet så att data överförs när en konvertering inträffar.

1. Klicka på Konfigurera i det övre högra hörnet.

   SCREENSHOT

1. Sök efter ordet &quot;Objekt&quot; i Snabbsökning

   SCREENSHOT

1. Gå till delen Anpassade leadfält och relationer och klicka på Mappa leadfält

   SCREENSHOT

1. Klicka på listrutan bredvid fältet som du vill mappa, under motsvarande flikkonto, kontakt eller affärsmöjlighet.

   SCREENSHOT

1. Välj motsvarande anpassat kontaktfält.

   SCREENSHOT

1. Upprepa stegen ovan för alla andra fält som du har skapat.

1. Klicka på Spara när du är klar.
