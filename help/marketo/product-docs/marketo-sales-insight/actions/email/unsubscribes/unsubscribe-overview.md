---
description: Avbeställ prenumerationen - Marketo Docs - produktdokumentation
title: Avbeställ prenumeration - översikt
exl-id: 7598efa9-9686-4dd0-840b-f8b6de4ab2be
feature: Sales Insight Actions
source-git-commit: 09a656c3a0d0002edfa1a61b987bff4c1dff33cf
workflow-type: tm+mt
source-wordcount: '328'
ht-degree: 0%

---

# Avbeställ prenumeration - översikt {#unsubscribe-overview}

Det blir allt viktigare för organisationer att följa lagar om e-postsekretess. För att underlätta har vi förbättrat vår avprenumeration.

* Länkar för att avbryta prenumerationen placeras i alla e-postmeddelanden som skickas från [!DNL Marketo Sales] och [!DNL Salesforce] (detta gäller inte för anpassade e-postmeddelanden som skickas från [!DNL Outlook] eller Gmail)
* Administratörer kan redigera avbeställningsmeddelanden för hela teamet
* Information om att avbryta prenumerationen lagras i PDV
* Du kan avbryta prenumerationen manuellt: Klicka på Länk, [!DNL Salesforce] Synkronisera och studsa
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

Om du är administratör kan du gå till gruppen för att avbryta prenumerationen och filtrera efter [!UICONTROL Account Unsubscribes] och se alla avregistreringar som har samlats in i din persondatabas.

![](assets/unsubscribe-overview-4.png)

## Avbeställ historikkort {#unsubscribe-history-card}

Kortet [!UICONTROL Unsubscribe History] hjälper administratörer och användare att få sammanhangsberoende information om kontaktens avbeställningshistorik. Navigera dit genom att gå till fliken [!UICONTROL People] och välja en person. Det finns längst ned på fliken [!UICONTROL About] i vyn Personinformation.

>[!NOTE]
>
>Det kommer bara att finnas ett [!UICONTROL Unsubscribe History]-kort om personen någon gång har _återprenumererat_.

![](assets/unsubscribe-overview-5.png)

<table>
 <colgroup>
  <col>
  <col>
 </colgroup>
 <tbody>
  <tr>
   <td><strong>[!UICONTROL Date]</strong></td>
   <td><p>Visar det datum då prenumerationen/återprenumerationen ägde rum.</p></td>
  </tr>
  <tr>
   <td><strong>[!UICONTROL Details]</strong></td>
   <td><p>Prenumerera igen: En [!DNL Sales Connect]-administratör tog manuellt bort prenumerationen från kontaktposten. Den kan även visa information om varför kontakten avbröt prenumerationen.</p><p>Avbeställ: Kontakten avbröt prenumerationen.</p></td>
  </tr>
  <tr>
   <td><strong>[!UICONTROL Source]</strong></td>
   <td><p>[!DNL Salesforce] Synkronisering: Avbeställningen togs av en synkronisering från [!DNL Salesforce].</p><p>Manuell: Användaren klickade på knappen för att avbryta prenumerationen för att avanmäla sig.</p><p>Klicka på Länk: Mottagaren av ett e-postmeddelande klickade på länken för att avbryta prenumerationen.</p><p>"Administratörsnamn": En administratörs namn visas när åtgärden var att återprenumerera kontakter. Detta gör att användarna vet vem som har tagit bort avbeställningen.</p></td>
  </tr>
 </tbody>
</table>

>[!MORELIKETHIS]
>
>[Anpassa länkmeddelande för att avbryta prenumeration](/help/marketo/product-docs/marketo-sales-insight/actions/email/unsubscribes/customize-unsubscribe-link-message.md)
