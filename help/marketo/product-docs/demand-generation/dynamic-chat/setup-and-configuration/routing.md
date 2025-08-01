---
description: Routning - Marketo Docs - produktdokumentation
title: Routning
feature: Dynamic Chat
exl-id: e20193b9-55c1-40f2-9e42-5b5dc9b88144
source-git-commit: 26573c20c411208e5a01aa7ec73a97e7208b35d5
workflow-type: tm+mt
source-wordcount: '338'
ht-degree: 0%

---

# Routning {#routing}

Möten som bokats i Dynamic Chat kan dirigeras på två sätt. Rundar av eller använder en anpassad regel.

Runda av: Möten tilldelas agenter sekventiellt. Så om du har fem agenter och agent tre tog det senaste mötet, så får agent fyra nästa, följt av agent fem, sen till agent ett.

Anpassad regel: Du kan välja särskilda agenter för att få möten baserat på de attribut du väljer.

>[!NOTE]
>
>Kontodirigering har högsta prioritet. När en besökare når punkten i konversationen för att antingen boka ett möte eller initiera en live-chatt, kontrolleras [Kontoroutning](#account-routing) först innan andra routningsalternativ övervägs.

## Skapa en anpassad regel {#create-a-custom-rule}

I det här exemplet skickar vi alla möten från de härledda delstaterna CA, OR och WA till agent John.

1. Klicka på **Routningsregler** under Konfiguration.

   ![](assets/routing-1.png)

1. Fliken **Anpassade regler** öppnas som standard.

   ![](assets/routing-2.png)

1. Klicka på **Skapa regel**.

   ![](assets/routing-3.png)

1. Ge din regel ett namn. Du kan också lägga till en beskrivning och ange dess prioritetsnivå. Klicka på **Nästa**.

   ![](assets/routing-4.png)

1. Välj önskad(a) agent(er).

   ![](assets/routing-5.png)

1. Dra över önskade attribut.

   ![](assets/routing-6.png)

1. Sök efter och välj önskade värden.

   ![](assets/routing-7.png)

1. När alla dina önskade värden är markerade klickar du på **Spara**.

   ![](assets/routing-8.png)

## Kontodirigering {#account-routing}

Identifiera och överför ditt målkonto och respektive säljare och skicka besökare som kommer från dessa konton direkt till respektive kontoägare.

![](assets/routing-9.png)

>[!PREREQUISITES]
>
>Innan _Kontoroutning_ visas i Dynamic Chat måste behörigheter aktiveras i Admin Console. Se [Aktivera behörigheter](#enable-permissions) nedan.

### Aktivera behörigheter {#enable-permissions}

+++ Aktivera behörighet för kontoroutning

1. Logga in på [https://adminconsole.adobe.com/](https://adminconsole.adobe.com/){target="_blank"}.

1. Under _Produkter_ väljer du **Dynamic Chat**.

   ![](assets/routing-10.png)

1. Välj önskad profil under _Produktprofiler_.

   ![](assets/routing-11.png)

1. Klicka på fliken **Behörigheter**.

   ![](assets/routing-12.png)

1. Klicka på redigeringsikonen (![ikonen Redigera](assets/icon-routing-edit.png)) bredvid _Konfiguration_.

   ![](assets/routing-13.png)

1. Klicka på **+** bredvid _Visa kontodirigering_.

   ![](assets/routing-14.png){width="600" zoomable="yes"}

1. Klicka på **Spara** när du är klar.

+++

### Lägg till ett konto {#add-an-account}

I det här exemplet dirigerar vi alla anställda från Lego direkt till agent Steven.

1. Klicka på **+ Lägg till konto** på fliken Kontoroutning.

   ![](assets/routing-15.png)

   >[!TIP]
   >
   >Du kan skapa flera konton samtidigt genom att klicka på **Överför kontolista** och överföra en CSV-fil.

1. Ange företagets namn, domän och välj önskad agent.

   ![](assets/routing-16.png)
