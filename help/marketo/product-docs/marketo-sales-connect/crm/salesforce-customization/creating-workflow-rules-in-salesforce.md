---
unique-page-id: 14745823
description: Skapa arbetsflödesregler i Salesforce - Marketo Docs - produktdokumentation
title: Skapa arbetsflödesregler i Salesforce
exl-id: 0cfce178-453b-4949-96aa-c327278a267d
feature: Marketo Sales Connect
source-git-commit: 431bd258f9a68bbb9df7acf043085578d3d91b1f
workflow-type: tm+mt
source-wordcount: '470'
ht-degree: 0%

---

# Skapa arbetsflödesregler i Salesforce {#creating-workflow-rules-in-salesforce}

När du använder Marketo Sales Insight (MSI) och Marketo Sales Connect (MSC) parallellt uppdateras inte MSI Best Bets-funktionen i Salesforce. Alla andra MSI-funktioner fungerar som vanligt (visa intressanta stunder iFrame, skicka e-post, lägga till i kampanjer osv.). I den här artikeln finns en lösning som hjälper dig att få bästa val att fungera igen.

>[!NOTE]
>
>Detta påverkar bara kunder som använder **både** MSI och MSE och som vill använda funktionen för bästa val i MSI. Om du inte behöver/använder Bästa val kan du bortse från det.

## Komma igång {#getting-started}

Du kan komma runt problemet genom att skapa nya arbetsflödesregler som kopierar värden från nya MSE-fält till de gamla MSI-fälten. Du måste skapa fyra arbetsflödesregler för Kontakt-objektet och samma fyra arbetsflödesregler för Lead-objektet i din egen Salesforce-instans. Detta kan kräva att du har CRM-administratörsbehörighet (beroende på din roll och konfiguration i CRM).

Nedan visas de rekommenderade namnen på arbetsflödesreglerna och en beskrivning av varje. Dessa gäller för objekten Kontakt och Lead:

<table> 
 <colgroup> 
  <col> 
  <col> 
 </colgroup> 
 <tbody> 
  <tr> 
   <td>Uppdatera fältet Intressant stund</td> 
   <td><p>Copy from: Last Marketo Engagement Desc<br>Copy to: Last Intressant Moment Desc</p></td> 
  </tr> 
  <tr> 
   <td>Uppdatera fält för typ av intressant stund</td> 
   <td><p>Kopiera från: Senaste Marketo Engagement Type<br>Kopiera till: Senaste intressanta stund</p></td> 
  </tr> 
  <tr> 
   <td>Uppdatera fältet Intressant stund för Source</td> 
   <td><p>Copy from: Last Marketo Engagement Source<br>Copy to: Last Intressant stund Source</p></td> 
  </tr> 
  <tr> 
   <td>Uppdatera fältet Intressant datum</td> 
   <td><p>Copy from: Last Marketo Engagement Date<br>Copy to: Last Intressant Moment Date</p></td> 
  </tr> 
 </tbody> 
</table>

## Instruktioner {#instructions}

1. När du har klickat på **Inställningar** söker du efter **Arbetsflöde** och väljer **Arbetsflödesregler**.

   ![](assets/one-1.png)

1. Välj **Ny regel**.

   ![](assets/two-1.png)

1. Klicka på listrutan Objekt, välj **Lead** och klicka sedan på **Nästa**.

   ![](assets/three-1.png)

1. Ange&quot;Uppdatera intressant tillfälligt fält&quot; som regelnamn. Markera alternativknappen **som har skapats och varje gång den redigeras**. I listrutan Regelvillkor väljer du **formel som utvärderas till true**. Sök efter och välj funktionen ISCHANGED. Markera sedan standardfältvärdet och klicka på **Infoga fält**.

   ![](assets/four-1.png)

1. I popup-fönstret Infoga fält väljer du **Senaste Marketo Engagement Desc** och klickar på **Infoga**.

   ![](assets/five-1.png)

1. Klicka på **Spara och nästa**.

   ![](assets/6.png)

1. Välj **Ny fältuppdatering** i listrutan Lägg till arbetsflödesåtgärd.

   ![](assets/seven.png)

1. I fältet Namn anger du&quot;Uppdatera intressant tillfälligt dekorfält&quot; (unikt namn genererar automatiskt). I listrutan Fält att uppdatera väljer du **Senaste intressanta tidpunkt**. Markera alternativknappen **Använd en formel för att ange det nya värdet** och klicka sedan på **Visa formelredigeraren**.

   ![](assets/eight.png)

1. Klicka på knappen **Infoga fält**.

   ![](assets/9a.png)

1. Välj **Senaste Marketo-engagemangsavdelning** och klicka på **Infoga**. På nästa sida klickar du på **Spara**.

   ![](assets/nine.png)

1. Klicka på **Klar**.

   ![](assets/twelve.png)

1. Klicka på **Aktivera** för att aktivera arbetsflödesregeln.

   ![](assets/thirteen.png)

   Efter det sista steget kan du välja att klona arbetsflödesregeln för de andra fälten i avsnittet Komma igång: Desc, Type, Source, Date. När du har slutfört de fyra arbetsflödesreglerna i Kontakt-objektet upprepar du det för Lead-objektet.
