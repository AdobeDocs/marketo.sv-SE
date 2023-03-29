---
description: Konfigurera detaljanpassning av Salesforce-aktivitet - Marketo Docs - produktdokumentation
title: Konfigurera detaljanpassning av Salesforce-aktivitet
exl-id: 534ebdb5-7a5b-48eb-98f7-2d05a9eae8e8
source-git-commit: b490b10c5544defaad50163fa29bfd0c2ca0d902
workflow-type: tm+mt
source-wordcount: '706'
ht-degree: 0%

---

# Konfigurera detaljanpassning av Salesforce-aktivitet {#configure-salesforce-activity-detail-customization}

>[!PREREQUISITES]
>
>* Salesforce och Sales Insight Actions [måste vara ansluten](/help/marketo/product-docs/marketo-sales-insight/actions/crm/salesforce-integration/connect-your-sales-insight-actions-account-to-salesforce.md)
>* Logga e-postaktivitet via API [måste vara aktiverat](/help/marketo/product-docs/marketo-sales-insight/actions/crm/salesforce-integration/salesforce-sync-settings.md)


Med anpassning av aktivitetsdetalj kan administratörer konfigurera den information som ska logga in i Salesforce-aktivitetsfältet - Ämne när en Sales Insight-aktivitet/påminnelseaktivitet synkroniseras med Salesforce.

>[!NOTE]
>
>* Uppdateringar som görs i ämnesfältet i Sales Insight Actions för en påminnelseuppgift återspeglas i motsvarande Salesforce-uppgifts ämnesfält, om du använder `{{activity_subject}}` dynamiskt fält i anpassning av aktivitetsdetalj.
>* Radbrytningar stöds inte vid loggning av information till Salesforce-objektfältet. Eventuella radbrytningar i redigeraren för anpassning av aktivitetsinformation tas bort när en ny rubrik för en försäljningsuppgift uppdateras.


![](assets/configure-salesforce-activity-detail-customization-1.png)

![](assets/configure-salesforce-activity-detail-customization-2.png)

<table>
 <tr>
  <td><strong>1</td>
  <td>Påminnelseuppgift för InMail</td>
 </tr>
 <tr>
  <td><strong>2</td>
  <td>E-postaktivitet</td>
 </tr>
 <tr>
  <td><strong>3</td>
  <td>Samtalsaktivitet</td>
 </tr>
</table>

Funktionen kan användas för att låsa upp följande fördelar:

* Genom att anpassa vilken information som visas i ämnesfältet är det enkelt att skanna aktivitetsinformationen för försäljning i Salesforce.
* Administratörer kan tagga ämnesfältet med en unik identifierare, t.ex.&quot;Mkto_sales&quot;, så att aktiviteter från Sales Insight Actions enkelt kan identifieras och skiljas från andra e-postaktiviteter, samtalsaktiviteter och uppgifter.
* Minska behovet av anpassade aktivitetsfält. Salesforce tillämpar begränsningar för antalet anpassade aktivitetsfält, som kan begränsa vilka data som är tillgängliga för användning i rapporter. Genom att använda dynamiska aktivitetsfält för att lägga till nyckeldata på ämnesraden kan du minska antalet anpassade aktivitetsfält som du behöver skapa i Salesforce-instansen.
* Ämnesfältet med aktiviteter och uppgifter följer ett konsekvent mönster som definieras av Sales Insight Actions Admin.

>[!NOTE]
>
>Om du loggar e-postsvar som aktiviteter till Salesforce kommer de inte att använda inställningarna för anpassning av aktivitetsinformation i Salesforce. I stället loggar de som&quot;Svara: E-postämne.&quot;

## Dynamiska aktivitetsfält som stöds {#activity-dynamic-fields-supported}

Dynamiska aktivitetsfält refererar till information om dina försäljningsaktiviteter för att fylla i data. Idag kan de användas med anpassning av aktivitetsinformation för Salesforce.

>[!NOTE]
>
>Om det inte finns något värde för att fylla i det dynamiska fältet för en viss aktivitet/uppgift fylls inga data i för det dynamiska fältet när Salesforce-aktiviteten - Ämnesfältet uppdateras.

<table>
 <tr>
  <th>Fält</th>
  <th>Beskrivning</th>
 </tr>
 <tr>
  <td>{{activity_type}}</td>
  <td>Fyller i uppgiftstypen som Email, Call, InMail eller Custom.</td>
 </tr>
 <tr>
  <td>{{activity_subject}}</td>
  <td><p>Fyller i föremålet för uppgiften.</p>
      <p>Om det är ett e-postmeddelande fylls ämnesraden i i e-postmeddelandet.</p>
      <p>Vid anrop, inMail eller anpassad fylls ett värde i om en påminnelseuppgift skapades med ett värde i aktivitetsnamnet/ämnesfältet.</p></td>
 </tr>
 <tr>
  <td>{{sales_campaign_name}}</td>
  <td>Om aktiviteten initierades från en försäljningskampanj fylls försäljningskampanjens namn i.</td>
 </tr>
 <tr>
  <td>{{sales_campaign_day}}</td>
  <td>Om aktiviteten initierades från en försäljningskampanj fylls försäljningskampanjens dagnummer som aktiviteten inträffade på.</td>
 </tr>
 <tr>
  <td>{{sales_campaign_step}}</td>
  <td>Om aktiviteten initierades från en försäljningskampanj fylls stegnumret i under försäljningskampanjdagen som aktiviteten inträffade på.</td>
 </tr>
 <tr>
  <td>{{call_result}}</td>
  <td>Om aktiviteten är ett anrop och ett samtalsresultat väljs fylls värdet för anropsresultatet i.</td>
 </tr>
 <tr>
  <td>{{call_reason}}</td>
  <td>Om aktiviteten är ett samtal och en anropsorsak väljs fylls anropsorsaksvärdet i.</td>
 </tr>
</table>

## Konfigurera detaljanpassning av Salesforce-aktivitet {#configuring-salesforce-activity-detail-customization}

>[!NOTE]
>
>**Administratörsbehörighet krävs.**

När du konfigurerar din aktivitetsinformation bör du tänka på vilka data som är mest relevanta för försäljningen när du granskar aktivitetshistorik i Salesforce.

1. Klicka på kugghjulsikonen och välj **Inställningar**.

   ![](assets/configure-salesforce-activity-detail-customization-3.png)

1. Klicka **Salesforce**.

   ![](assets/configure-salesforce-activity-detail-customization-4.png)

1. Klicka **Synkronisera inställningar**.

   ![](assets/configure-salesforce-activity-detail-customization-5.png)

1. I redigeraren Anpassa aktivitetsinformation lägger du till eventuell ledig text. Den text du lägger till är icke-dynamisk och förblir oförändrad för ämnesfältet för alla uppgifter som synkroniseras med Salesforce.

   ![](assets/configure-salesforce-activity-detail-customization-6.png)

   >[!TIP]
   >
   >Även om det inte är obligatoriskt att radbryta tillagd text inom raka hakparenteser kan det vara lättare för en del att skilja mellan data när de fylls i i ett ämnesfält i Salesforce. Exempel: `[Sales Insight Actions] - {{Activity_type}}`

1. Lägg till ytterligare dynamiska fält genom att klicka på **Lägg till dynamiskt fält** -knappen.

   ![](assets/configure-salesforce-activity-detail-customization-7.png)

1. Markera önskade dynamiska fält.

   ![](assets/configure-salesforce-activity-detail-customization-8.png)

1. Klicka **Spara**.

   ![](assets/configure-salesforce-activity-detail-customization-9.png)

>[!NOTE]
>
>Salesforce har en begränsning på 255 tecken. Om din aktivitetsinformation överstiger det, kommer den att trunkeras för att säkerställa att informationen lagras i Salesforce-objektfältet.

>[!MORELIKETHIS]
>
>* [Synkronisera inställningar](/help/marketo/product-docs/marketo-sales-insight/actions/crm/salesforce-integration/salesforce-sync-settings.md)
>* [Synkronisering av påminnelseaktivitet med Salesforce](/help/marketo/product-docs/marketo-sales-insight/actions/tasks/reminder-task-sync-with-salesforce.md)

