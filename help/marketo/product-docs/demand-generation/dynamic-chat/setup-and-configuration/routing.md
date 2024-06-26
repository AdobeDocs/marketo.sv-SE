---
description: Routning - Marketo Docs - produktdokumentation
title: Routning
feature: Dynamic Chat
exl-id: 93d1a96d-c101-4a1c-898c-dcadb5cdce85
source-git-commit: 38274b4859ae38c018ee73d4f1715fdf6a78e815
workflow-type: tm+mt
source-wordcount: '268'
ht-degree: 0%

---

# Routning {#routing}

Möten som bokats i Dynamic Chat kan dirigeras på två sätt. Rundar av eller använder en anpassad regel.

Runda av: Möten tilldelas agenter sekventiellt. Så om du har fem agenter och agent tre tog det senaste mötet, så får agent fyra nästa, följt av agent fem, sen till agent ett.

Anpassad regel: Du kan välja särskilda agenter för att få möten baserat på de attribut du väljer.

>[!NOTE]
>
>Kontodirigering har högsta prioritet. När en besökare når punkten i konversationen för att antingen boka ett möte eller starta en live-chatt, [Kontodirigering](#account-routing) kontrolleras först innan andra routningsalternativ beaktas.

## Skapa en anpassad regel {#create-a-custom-rule}

I det här exemplet skickar vi alla möten från de härledda delstaterna CA, OR och WA till agent John.

1. Under Konfiguration klickar du på **Routningsregler**.

   ![](assets/routing-1.png)

1. Klicka på **Anpassade regler** -fliken.

   ![](assets/routing-2.png)

1. Klicka **Skapa regel**.

   ![](assets/routing-3.png)

1. Ge din regel ett namn. Du kan också lägga till en beskrivning och ange dess prioritetsnivå. Klicka **Nästa**.

   ![](assets/routing-4.png)

1. Välj önskad(a) agent(er).

   ![](assets/routing-5.png)

1. Dra över önskade attribut.

   ![](assets/routing-6.png)

1. Sök efter och välj önskade värden.

   ![](assets/routing-7.png)

1. När alla önskade värden är markerade klickar du på **Spara**.

   ![](assets/routing-8.png)

## Kontodirigering {#account-routing}

Identifiera och överför ditt målkonto och respektive säljare och skicka besökare som kommer från dessa konton direkt till respektive kontoägare.

![](assets/routing-9.png)

### Lägg till ett konto {#add-an-account}

I det här exemplet dirigerar vi alla anställda från Lego direkt till agent Steven.

1. Klicka på fliken Kontoroutning **+ Lägg till konto**.

   ![](assets/routing-10.png)

   >[!TIP]
   >
   >Du kan skapa flera konton samtidigt genom att klicka på **Ladda upp kontolista** och ladda upp en CSV-fil.

1. Ange företagets namn, domän och välj önskad agent.

   ![](assets/routing-11.png)
