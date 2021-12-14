---
description: Konfigurera detaljanpassning av Salesforce-aktivitet - Marketo Docs - produktdokumentation
title: Konfigurera detaljanpassning av Salesforce-aktivitet
hide: true
hidefromtoc: true
exl-id: 4b20ca29-18d6-4026-9bf9-77656ad1442d
source-git-commit: 87f43fb58b5739c0465a1a74fb60cdf5c5f6b759
workflow-type: tm+mt
source-wordcount: '573'
ht-degree: 0%

---

# Konfigurera detaljanpassning av Salesforce-aktivitet {#configure-salesforce-activity-detail-customization}

Med anpassning av aktivitetsdetalj kan administratörer konfigurera den information som ska logga in i Salesforce-aktivitetsfältet - Ämne när en Sales Connect-aktivitet/påminnelseaktivitet synkroniseras med Salesforce.

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
* Administratörer kan tagga ämnesfältet med en unik identifierare, t.ex.&quot;Mkto_sales&quot;, så att aktiviteter från Sales Connect enkelt kan identifieras och skiljas från andra e-postaktiviteter, samtalsaktiviteter och uppgifter.
* Minska behovet av anpassade aktivitetsfält. Salesforce tillämpar begränsningar för antalet anpassade aktivitetsfält, som kan begränsa vilka data som är tillgängliga för användning i rapporter. Genom att använda dynamiska aktivitetsfält för att lägga till nyckeldata på ämnesraden kan du minska antalet anpassade aktivitetsfält som du behöver skapa i Salesforce-instansen.
* Ämnesfältet med aktiviteter och uppgifter följer ett konsekvent mönster som definieras av Sales Connect Admin.

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

PICC

1. Klicka **Salesforce**.

PICC

1. Klicka **Synkronisera inställningar**.

PICC

1. I redigeraren Anpassa aktivitetsinformation lägger du till eventuell ledig text. Den ändras inte för ämnesfältet för alla uppgifter som synkroniseras med Salesforce.

1. Lägg till alla dynamiska fält som du vill lägga till genom att klicka på knappen för dynamiskt fält och välja de dynamiska fält som du vill använda i listan.

1. Klicka **Spara**.

>[!NOTE]
>
>Salesforce har en begränsning på 255 tecken. Om din aktivitetsinformation överstiger det, kommer den att trunkeras för att säkerställa att informationen kan lagras i Salesforce-objektfältet.

>[!MORELIKETHIS]
>
>* [Synkronisera inställningar](/help/marketo/product-docs/marketo-sales-connect/crm/salesforce-integration/salesforce-sync-settings.md)
>* [Synkronisering av påminnelseaktivitet med Salesforce](/help/marketo/product-docs/marketo-sales-connect/tasks/reminder-task-sync-with-salesforce.md)
>* [Anpassa Sales Connect för CRM](/help/marketo/product-docs/marketo-sales-connect/crm/salesforce-customization/sales-connect-customizations-for-crm.md)

