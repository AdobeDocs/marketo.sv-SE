---
unique-page-id: 14745823
description: Skapa arbetsflödesregler i Salesforce - Marketo Docs - produktdokumentation
title: Skapa arbetsflödesregler i Salesforce
exl-id: 0cfce178-453b-4949-96aa-c327278a267d
feature: Marketo Sales Connect
source-git-commit: 09a656c3a0d0002edfa1a61b987bff4c1dff33cf
workflow-type: tm+mt
source-wordcount: '393'
ht-degree: 1%

---

# Skapa arbetsflödesregler i Salesforce {#creating-workflow-rules-in-salesforce}

När du använder Marketo Sales Insight (MSI) och Marketo Sales Connect (MSC) parallellt uppdateras inte MSI Best Bets-funktionen i [!DNL Salesforce]. Alla andra MSI-funktioner fungerar som vanligt (visa intressanta stunder iFrame, skicka e-post, lägga till i kampanjer osv.). I den här artikeln finns en lösning som hjälper dig att få bästa val att fungera igen.

>[!NOTE]
>
>Detta påverkar bara kunder som använder **både** MSI och MSE och som vill använda funktionen för bästa val i MSI. Om du inte behöver/använder Bästa val kan du bortse från det.

## Komma igång {#getting-started}

Du kan komma runt problemet genom att skapa nya arbetsflödesregler som kopierar värden från nya MSE-fält till de gamla MSI-fälten. Du måste skapa fyra arbetsflödesregler för Kontakt-objektet och samma fyra arbetsflödesregler för Lead-objektet i din egen [!DNL Salesforce]-instans. Detta kan kräva att du har CRM-administratörsbehörighet (beroende på din roll och konfiguration i CRM).

Nedan visas de rekommenderade namnen på arbetsflödesreglerna och en beskrivning av varje. Dessa gäller för objektet [!UICONTROL Contact] och [!UICONTROL Lead]:

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

1. När du har klickat på **[!UICONTROL Setup]** söker du efter **Arbetsflöde** och väljer **[!UICONTROL Workflow Rules]**.

   ![](assets/one-1.png)

1. Välj **[!UICONTROL New Rule]**.

   ![](assets/two-1.png)

1. Klicka på listrutan [!UICONTROL Object] och välj **[!UICONTROL Lead]**. Klicka sedan på **[!UICONTROL Next]**.

   ![](assets/three-1.png)

1. Ange&quot;Update Intressant stund Desc Field&quot; som [!UICONTROL Rule Name]. Markera alternativknappen **[!UICONTROL created, and every time it’s edited]**. Välj [!UICONTROL Rule Criteria] i listrutan **[!UICONTROL formula evaluates to true]**. Sök efter och välj funktionen ISCHANGED. Markera sedan standardfältvärdet och klicka på **[!UICONTROL Insert Field]**.

   ![](assets/four-1.png)

1. I popup-fönstret [!UICONTROL Insert Field] väljer du **[!UICONTROL Last Marketo Engagement Desc]** och klickar på **[!UICONTROL Insert]**.

   ![](assets/five-1.png)

1. Klicka på **[!UICONTROL Save & Next]**.

   ![](assets/6.png)

1. Välj [!UICONTROL Add Workflow Action] i listrutan **[!UICONTROL New Field Update]**.

   ![](assets/seven.png)

1. I fältet [!UICONTROL Name] anger du&quot;Update Intressant stund Desc Field&quot; ([!UICONTROL Unique Name] genererar automatiskt). Välj [!UICONTROL Field to Update] i listrutan **[!UICONTROL Last Interesting Moment Desc]**. Markera alternativknappen **[!UICONTROL Use a formula to set new value]** och klicka sedan på **[!UICONTROL Show Formula Editor]**.

   ![](assets/eight.png)

1. Klicka på knappen **[!UICONTROL Insert Field]**.

   ![](assets/9a.png)

1. Välj **[!UICONTROL Last Marketo Engagement Desc]** och klicka på **[!UICONTROL Insert]**. Klicka på **[!UICONTROL Save]** på nästa sida.

   ![](assets/nine.png)

1. Klicka på **[!UICONTROL Done]**.

   ![](assets/twelve.png)

1. Klicka på **[!UICONTROL Activate]** för att aktivera arbetsflödesregeln.

   ![](assets/thirteen.png)

   Efter det sista steget kan du välja att klona arbetsflödesregeln för de andra fälten i avsnittet [!UICONTROL Getting Started]: Desc, Type, Source, Date. När du har slutfört de fyra arbetsflödesreglerna i [!UICONTROL Contact]-objektet upprepar du det samma för [!UICONTROL Lead]-objektet.
