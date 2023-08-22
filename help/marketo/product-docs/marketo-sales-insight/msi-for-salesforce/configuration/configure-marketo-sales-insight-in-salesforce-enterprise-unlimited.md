---
unique-page-id: 2360368
description: Konfigurera Marketo Sales Insight i Salesforce Enterprise/Unlimited - Marketo Docs - produktdokumentation
title: Konfigurera Marketo Sales Insight i Salesforce Enterprise/Unlimited
exl-id: a33ed396-8d26-403f-b6d8-fe7c55ce76ba
feature: Marketo Sales Insights
source-git-commit: 9d1b18b2aebde00ae715a072580a8f128d07923e
workflow-type: tm+mt
source-wordcount: '847'
ht-degree: 0%

---

# Konfigurera Marketo Sales Insight i Salesforce Enterprise/Unlimited {#configure-marketo-sales-insight-in-salesforce-enterprise-unlimited}

Här är de steg du måste utföra för att konfigurera Marketo Sales Insight i Salesforce Enterprise/Unlimited Editions. Kom så sätter vi igång.

>[!PREREQUISITES]
>
>[Installera Marketo Sales Insight-paket i Salesforce-AppExchange](/help/marketo/product-docs/marketo-sales-insight/msi-for-salesforce/installation/install-marketo-sales-insight-package-in-salesforce-appexchange.md)

>[!NOTE]
>
>**Administratörsbehörigheter krävs**

## Konfigurera Sales Insight i Marketo {#configure-sales-insight-in-marketo}

1. Hämta dina MSI-autentiseringsuppgifter i Marketo. Gå till området Admin och välj **Försäljningsinsikter**.

   ![](assets/configure-marketo-sales-insight-in-salesforce-professional-edition-1.png)

1. Klicka **Redigera API-konfiguration**.

   ![](assets/configure-marketo-sales-insight-in-salesforce-professional-edition-2.png)

1. Ange en API-hemlig nyckel som du väljer och klicka på **Spara**. Använd INTE ett et-tecken (&amp;) i API-hemlighetsnyckeln.

   ![](assets/configure-marketo-sales-insight-in-salesforce-professional-edition-3.png)

   >[!NOTE]
   >
   >Din API-hemliga nyckel är som ett lösenord för din organisation och bör vara säker.

1. Klicka **Visa** på panelen Rest API Configuration för att fylla i autentiseringsuppgifterna.

   ![](assets/configure-marketo-sales-insight-in-salesforce-professional-edition-4.png)

1. Ett bekräftelsemeddelande visas. Klicka **OK**.

   ![](assets/configure-marketo-sales-insight-in-salesforce-professional-edition-5.png)

   >[!TIP]
   >
   >Låt det här fönstret vara öppet. Du behöver den här informationen senare i Salesforce.

## Konfigurera säljinsikter i Salesforce {#configure-sales-insight-in-salesforce}

1. I Salesforce klickar du på **Inställningar**.

   ![](assets/configure-marketo-sales-insight-in-salesforce-professional-edition-6.png)

1. Sök efter&quot;fjärrwebbplats&quot; och välj **Inställningar för fjärrplats**.

   ![](assets/configure-marketo-sales-insight-in-salesforce-professional-edition-7.png)

1. Klicka **Ny fjärrplats**.

   ![](assets/configure-marketo-sales-insight-in-salesforce-professional-edition-8.png)

1. Ange namnet på fjärrplatsen (det kan vara något som &quot;MarketoSoapAPI&quot;). Ange URL för fjärrplatsen, som är din Marketo-värd-URL från panelen Konfigurera Soap API i Marketo. Klicka **Spara**. Du har nu skapat fjärrplatsinställningar för Soap API.

   ![](assets/configure-marketo-sales-insight-in-salesforce-professional-edition-9.png)

1. Klicka **Ny fjärrplats** igen.

   ![](assets/configure-marketo-sales-insight-in-salesforce-professional-edition-10.png)

1. Ange namnet på fjärrplatsen (det kan vara något som &quot;MarketoAPI&quot;). Ange URL för fjärrplats, som är din API-URL från konfigurationspanelen för Rest API i Marketo. Klicka **Spara**. Du har nu skapat fjärrplatsinställningar för Rest API.

   >[!NOTE]
   >
   >_Du_ välj **Namn på fjärrplats** (MarketoAPI används här). The **URL för fjärrwebbplats** finns i fältet Marketo Host i dialogrutan Edit API Configuration från steg 3 i avsnittet Configure Sales Insight in Marketo.

## Anpassa sidlayouter {#customize-page-layouts}

1. Klicka **Inställningar**.

   ![](assets/image2015-5-22-14-3a40-3a39.png)

1. Sök efter&quot;sidlayout&quot; och välj **Sidlayout** under **Leads**.

   ![](assets/image2015-5-28-14-3a58-3a39.png)

1. Klicka **Visualforce-sidor** till vänster. Dra **Avsnitt** till layouten under Anpassade länkar.

   ![](assets/image2014-9-24-17-3a32-3a53.png)

1. Ange&quot;Marketo Sales Insight&quot; som **Avsnittsnamn**. Välj **1 kolumn** och klicka **OK**.

   ![](assets/image2014-9-24-17-3a33-3a23.png)

1. Dra och släpp **Lead** till det nya avsnittet.

   ![](assets/image2014-9-24-17-3a33-3a45.png)

   >[!TIP]
   >
   >Namnet på den här rutan ändras beroende på objekttypen. Om du till exempel ändrar sidlayouten för Kontakter står Kontakt.

1. Dubbelklicka på **Lead** -block som du just har lagt till.

   ![](assets/image2014-9-24-17-3a34-3a0.png)

1. Redigera höjd till **450** pixlar och klicka **OK**.

   ![](assets/image2014-9-24-17-3a34-3a26.png)

   >[!NOTE]
   >
   >Kontrollera **Visa rullningslister** om du behöver tillgång till genomskärningsaktiviteter.

   >[!TIP]
   >
   >Vi rekommenderar en höjd på 410 pixlar för objekten Konton och Affärsmöjligheter.

1. Klicka på **Fält** till vänster. Sök och dra sedan **Akut** etiketten i **Marketo Sales Insight** layout.

   ![](assets/configure-marketo-sales-insight-in-salesforce-professional-edition-18.png)

1. Upprepa även ovanstående steg för dessa fält.

   <table> 
    <tbody> 
     <tr> 
      <td>Senaste intressanta stund</td> 
     </tr> 
     <tr> 
      <td>Senaste intressanta datum</td> 
     </tr> 
     <tr> 
      <td>Senaste intressanta tillfälle</td> 
     </tr> 
     <tr> 
      <td>Källa för senaste intressanta stund</td> 
     </tr> 
     <tr> 
      <td>Typ av senaste intressanta stund</td> 
     </tr> 
     <tr> 
      <td>Senaste aktivitet efter försäljning</td> 
     </tr> 
     <tr> 
      <td>Senaste åtagande per försäljning</td> 
     </tr> 
     <tr> 
      <td>Kontakt-ID för MSI</td> 
     </tr> 
     <tr> 
      <td>Relativa poäng</td> 
     </tr> 
     <tr> 
      <td>Relativt poängvärde</td> 
     </tr> 
     <tr> 
      <td>Akut</td> 
     </tr> 
     <tr> 
      <td>Värde för nödsituationer</td> 
     </tr> 
     <tr> 
      <td>Visa i Marketo</td> 
     </tr> 
    </tbody> 
   </table>

1. Klicka **Spara** när du är klar.

   ![](assets/image2014-9-24-17-3a35-3a6.png)

1. Upprepa steg 5-7 för att lägga till Visualforce-sidavsnitt och Sales Insight-fält för **Kontakt**, **Konto** och **Möjligheter**.

1. Upprepa steg 8-10 för att lägga till fält för Sales Insight från listan nedan för **Kontakt**. Var noga med att spara ändringarna.

<table> 
    <tbody> 
     <tr> 
      <td>Senaste intressanta stund</td> 
     </tr> 
     <tr> 
      <td>Senaste intressanta datum</td> 
     </tr> 
     <tr> 
      <td>Senaste intressanta tillfälle</td> 
     </tr> 
     <tr> 
      <td>Källa för senaste intressanta stund</td> 
     </tr> 
     <tr> 
      <td>Typ av senaste intressanta stund</td> 
     </tr> 
     <tr> 
      <td>Senaste Marketo-aktivitet per försäljning</td> 
     </tr> 
     <tr> 
      <td>Senaste Marketo-engagemang från försäljning</td> 
     </tr> 
     <tr> 
      <td>MKTO Lead Score</td> 
     </tr> 
     <tr> 
      <td>Relativa poäng</td> 
     </tr> 
     <tr> 
      <td>Relativt poängvärde</td> 
     </tr> 
     <tr> 
      <td>Sales Insight - Öppnar hela kontaktlistsidan</td> 
     </tr> 
     <tr> 
      <td>Akut</td> 
     </tr> 
     <tr> 
      <td>Värde för nödsituationer</td> 
     </tr> 
    </tbody> 
   </table>

## Mappa anpassade personfält {#map-custom-person-fields}

Marketo personfält måste mappas till Salesforce-kontaktfält för att konverteringen ska fungera korrekt. Så här gör du.

1. Klicka **Inställningar**.

   ![](assets/image2015-5-22-14-3a40-3a39.png)

1. Sök efter&quot;fält&quot; i sökfältet och klicka på **Fält** under **Leads**.

   ![](assets/image2015-6-1-9-3a54-3a50.png)

1. Klicka **Mappa leadfält**.

   ![](assets/image2015-6-1-9-3a58-3a48.png)

1. Klicka på listrutan till höger för **Engagemang**.

   ![](assets/image2015-6-1-10-3a9-3a53.png)

1. Välj **Contact.Engagement** i listan.

   ![](assets/image2015-6-1-10-3a12-3a11.png)

1. Upprepa och mappa även dessa fält.

   <table> 
    <tbody> 
     <tr> 
      <th colspan="1" rowspan="1">Anpassat fält för Marketo-person</th> 
      <th colspan="1" rowspan="1">Anpassat fält för Salesforce-kontakt</th> 
     </tr> 
     <tr> 
      <td colspan="1" rowspan="1"><p>Engagemang</p></td> 
      <td colspan="1" rowspan="1"><p>Contact.Engagement</p></td> 
     </tr> 
     <tr> 
      <td colspan="1" rowspan="1"><p>Relativt poängvärde</p></td> 
      <td colspan="1" rowspan="1"><p>Kontakt.Relativt poängvärde</p></td> 
     </tr> 
     <tr> 
      <td colspan="1" rowspan="1"><p>Värde för nödsituationer</p></td> 
      <td colspan="1" rowspan="1"><p>Contact.Emergency Value</p></td> 
     </tr> 
     <tr> 
      <td colspan="1" rowspan="1"><p>Senaste intressanta datum</p></td> 
      <td colspan="1" rowspan="1"><p>Kontakt.Senaste intressanta datum</p></td> 
     </tr> 
     <tr> 
      <td colspan="1" rowspan="1"><p>Senaste intressanta tillfälle</p></td> 
      <td colspan="1" rowspan="1"><p>Kontakt.Senaste intressanta tillfälle</p></td> 
     </tr> 
     <tr> 
      <td colspan="1" rowspan="1"><p>Källa för senaste intressanta stund</p></td> 
      <td colspan="1" rowspan="1"><p>Kontakt.Senaste intressanta tidskälla</p></td> 
     </tr> 
     <tr> 
      <td colspan="1" rowspan="1"><p>Typ av senaste intressanta stund</p></td> 
      <td colspan="1" rowspan="1"><p>Kontakt.Senaste intressanta stund</p></td> 
     </tr> 
    </tbody> 
   </table>

1. Klicka **Spara** när du är klar.

## Marketo Sales Insight Configuration Tab {#marketo-sales-insight-configuration-tab}

1. Klicka på **+** i slutet av flikfältet och klicka på **Marketo Sales Insight Config**.

1. Kopiera inloggningsuppgifterna från Soap API-panelen i [Marketo Sales Insight Admin page](/help/marketo/product-docs/marketo-sales-insight/msi-for-salesforce/configuration/configure-marketo-sales-insight-in-salesforce-professional-edition.md#set-up-marketo-sales-insight){target="_blank"} och klistra in dem i Soap API-avsnittet på Salesforce Sales Insight Configuration-sidan.

1. Kopiera inloggningsuppgifterna från panelen Rest API i [Marketo Sales Insight Admin page](/help/marketo/product-docs/marketo-sales-insight/msi-for-salesforce/configuration/configure-marketo-sales-insight-in-salesforce-professional-edition.md#set-up-marketo-sales-insight){target="_blank"} och klistra in dem i delen Rest API på sidan Konfiguration av Salesforce Sales Insight.

   ![](assets/configure-marketo-sales-insight-in-salesforce-enterprise-edition-25.png)

Och det är allt! Du bör kunna se fälten Marketo Sales Insight för Leads, Contacts, Accounts och Opportunity.

>[!NOTE]
>
>Om diagnostiktestet misslyckades kan du behöva [lägga till fler fält i sidlayouten](https://nation.marketo.com/docs/DOC-1115){target="_blank"}.

>[!NOTE]
>
>För konton kommer Sales Insight att inkludera alla e-postmeddelanden, men bara de senaste intressanta stunderna, webbaktiviteten och poängändringarna.

>[!MORELIKETHIS]
>
>* [Prioritet, Urklipp, Relativa poäng och Bästa val](/help/marketo/product-docs/marketo-sales-insight/msi-for-salesforce/features/stars-and-flames/priority-urgency-relative-score-and-best-bets.md)
>* [Lägg till fliken Marketo i Salesforce](/help/marketo/product-docs/marketo-sales-insight/msi-for-salesforce/configuration/add-marketo-tab-to-salesforce.md)
>* [Lägg till åtkomst till profiler för Sales Insight](/help/marketo/product-docs/marketo-sales-insight/msi-for-salesforce/configuration/add-sales-insight-access-to-profiles.md){target="_blank"}
