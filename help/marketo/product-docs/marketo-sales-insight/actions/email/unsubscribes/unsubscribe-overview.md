---
description: Avbeställ prenumerationen - Marketo Docs - produktdokumentation
title: Avbeställ prenumeration - översikt
exl-id: 7598efa9-9686-4dd0-840b-f8b6de4ab2be
feature: Sales Insight Actions
source-git-commit: 431bd258f9a68bbb9df7acf043085578d3d91b1f
workflow-type: tm+mt
source-wordcount: '348'
ht-degree: 0%

---

# Avbeställ prenumeration - översikt {#unsubscribe-overview}

Det blir allt viktigare för organisationer att följa lagar om e-postsekretess. För att underlätta har vi förbättrat vår avprenumeration.

* Länkar för att avbryta prenumerationen placeras på alla e-postmeddelanden som skickas från Marketo Sales och Salesforce (detta gäller inte för anpassade e-postmeddelanden som skickas från Outlook eller Gmail)
* Administratörer kan redigera avbeställningsmeddelanden för hela teamet
* Information om att avbryta prenumerationen lagras i PDV
* Du kan avbryta prenumerationen manuellt: Klicka på Länk, Salesforce-synkronisering och Studsa
* Ny startsida för länk för avanmälan

## Avbeställ Landing Page {#unsubscribe-link-landing-page}

När en person klickar på länken för att avbryta prenumerationen kommer han/hon att hamna på en startsida där han/hon kan välja vad han/hon vill avbeställa och varför.

![](assets/unsubscribe-overview-1.png)

Den här informationen sparas i vyn med personinformation och kan visas senare.

## Avbeställ grupp {#unsubscribe-group}

Se och hantera alla personer som inte har prenumererat på ett och samma ställe.

![](assets/unsubscribe-overview-2.png)

Använd sökfältet för att söka efter personer som inte har prenumererat.

![](assets/unsubscribe-overview-3.png)

Om du är administratör kan du gå till gruppen för att avbryta prenumerationen och filtrera efter Avsluta abonnemang och se alla avregistreringar som har samlats in i din persondatabas.

![](assets/unsubscribe-overview-4.png)

## Avbeställ historikkort {#unsubscribe-history-card}

Med historikkortet för att avbryta prenumerationen kan administratörer och användare få sammanhangsberoende information om kontaktens avbeställningshistorik. Navigera dit genom att gå till fliken Personer och välja en person. Det finns längst ned på fliken Om i vyn Personinformation.

>[!NOTE]
>
>Det finns bara ett historikkort för att avsluta prenumerationen om personen har _återkallat prenumerationen_ vid något tillfälle.

![](assets/unsubscribe-overview-5.png)

<table> 
 <colgroup> 
  <col> 
  <col> 
 </colgroup> 
 <tbody> 
  <tr> 
   <td><strong>Datum</strong></td> 
   <td><p>Visar det datum då prenumerationen/återprenumerationen ägde rum.</p></td> 
  </tr> 
  <tr> 
   <td><strong>Information</strong></td> 
   <td><p>Prenumerera igen: En Sales Connect-administratör tog manuellt bort prenumerationen från kontaktposten. Den kan även visa information om varför kontakten avbröt prenumerationen.</p><p>Avbeställ: Kontakten avbröt prenumerationen.</p></td> 
  </tr> 
  <tr> 
   <td><strong>Källa</strong></td> 
   <td><p>Salesforce-synkronisering: Avbeställningen togs av en synkronisering från Salesforce.</p><p>Manuell: Användaren klickade på knappen för att avbryta prenumerationen för att avanmäla sig.</p><p>Klicka på Länk: Mottagaren av ett e-postmeddelande klickade på länken för att avbryta prenumerationen.</p><p>"Administratörsnamn": En administratörs namn visas när åtgärden var att återprenumerera kontakter. Detta gör att användarna vet vem som har tagit bort avbeställningen.</p></td> 
  </tr> 
 </tbody> 
</table>

>[!MORELIKETHIS]
>
>[Anpassa länkmeddelande för att avbryta prenumeration](/help/marketo/product-docs/marketo-sales-insight/actions/email/unsubscribes/customize-unsubscribe-link-message.md)
