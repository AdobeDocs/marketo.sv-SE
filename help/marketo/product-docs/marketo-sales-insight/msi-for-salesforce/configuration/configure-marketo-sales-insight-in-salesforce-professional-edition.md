---
unique-page-id: 3571743
description: Konfigurera Marketo Sales Insight i Salesforce Professional Edition - Marketo Docs - produktdokumentation
title: Konfigurera Marketo Sales Insight i Salesforce Professional Edition
exl-id: fae63560-0bb3-46a9-94a3-cc27c1aa363e
source-git-commit: 86c32e5f7eab00a1963b9d00057af4820cddfe78
workflow-type: tm+mt
source-wordcount: '912'
ht-degree: 0%

---

# Konfigurera Marketo Sales Insight i Salesforce Professional Edition {#configure-marketo-sales-insight-in-salesforce-professional-edition}

Här är de steg du måste ta för att konfigurera Marketo Sales Insight i Salesforce Professional Edition. Kom så sätter vi igång.

>[!PREREQUISITES]
>
>* Installera Marketo i Salesforce Professional Edition.
>
>* [Installera Marketo Sales Insight-paket i Salesforce AppExchange](/help/marketo/product-docs/marketo-sales-insight/msi-for-salesforce/installation/install-marketo-sales-insight-package-in-salesforce-appexchange.md)


>[!NOTE]
>
>**Administratörsbehörigheter krävs**

## Konfigurera Sales Insight i Marketo {#configure-sales-insight-in-marketo}

1. Öppna ett nytt webbläsarfönster för att hämta inloggningsuppgifterna för Marketo Sales Insight från ditt Marketo-konto.
1. Gå till området Admin och välj **Försäljningsinsikter**.

   ![](assets/configure-marketo-sales-insight-in-salesforce-professional-edition-1-1.png)

1. Klicka **Redigera API-konfiguration**.

   ![](assets/configure-marketo-sales-insight-in-salesforce-professional-edition-2-1.png)

1. Ange en API-hemlig nyckel som du väljer och klicka på **Spara**. Använd INTE ett et-tecken (&amp;) i API-hemlighetstangenten.

   ![](assets/configure-marketo-sales-insight-in-salesforce-professional-edition-3-1.png)

   >[!NOTE]
   >
   >Din API-hemliga nyckel är som ett lösenord för din organisation och bör vara säker.

1. Klicka **Visa** på panelen Rest API Configuration för att fylla i autentiseringsuppgifterna.

   ![](assets/configure-marketo-sales-insight-in-salesforce-professional-edition-4-1.png)

1. Ett bekräftelsemeddelande visas. Klicka **OK**.

   ![](assets/configure-marketo-sales-insight-in-salesforce-professional-edition-5-1.png)

## Konfigurera säljinsikter i Salesforce {#configure-sales-insight-in-salesforce}

1. I Salesforce klickar du på **Inställningar**.

   ![](assets/configure-marketo-sales-insight-in-salesforce-professional-edition-6-1.png)

1. Sök efter&quot;fjärrwebbplats&quot; och välj **Inställningar för fjärrplats**.

   ![](assets/configure-marketo-sales-insight-in-salesforce-professional-edition-7-1.png)

1. Klicka **Ny fjärrplats**.

   ![](assets/configure-marketo-sales-insight-in-salesforce-professional-edition-8-1.png)

1. Ange namnet på fjärrplatsen (det kan vara något som &quot;MarketoSoapAPI&quot;). Ange URL för fjärrplatsen, som är din Marketo-värd-URL från panelen Konfigurera Soap API i Marketo. Klicka **Spara**. Du har nu skapat fjärrplatsinställningar för Soap API.

   ![](assets/configure-marketo-sales-insight-in-salesforce-professional-edition-9-1.png)

1. Klicka **Ny fjärrplats** igen.

   ![](assets/configure-marketo-sales-insight-in-salesforce-professional-edition-10-1.png)

1. Ange namnet på fjärrplatsen (det kan vara något som &quot;MarketoRestAPI&quot;). Ange URL för fjärrplats, som är din API-URL från konfigurationspanelen för Rest API i Marketo. Klicka **Spara**. Du har nu skapat fjärrplatsinställningar för Rest API.

## Ställ in Marketo Sales Insight {#set-up-marketo-sales-insight}

1. Logga in på din Marketo-instans och klicka på **Administratör**.

   ![](assets/login-admin-1.png)

1. Klicka **Försäljningsinsikter**.

   ![](assets/image2015-5-22-15-3a12-3a33-1.png)

1. Klicka **Redigera API-konfiguration**.

   ![](assets/image2015-5-22-15-3a15-3a0-1.png)

1. Ange en **API-hemlig nyckel** och klicka **Spara**.

   >[!CAUTION]
   >
   >Använd inte ett et-tecken (&amp;) i API-hemlig nyckel.

   ![](assets/image2015-5-27-16-3a36-3a56-1.png)

   >[!TIP]
   >
   >Låt det här fönstret vara öppet. Du behöver den här informationen senare i Salesforce.

1. Gå tillbaka till Salesforce, klicka **Inställningar**.

   ![](assets/image2015-5-22-14-3a40-3a39-1.png)

1. Sök efter fjärrplats och klicka på **Inställning för fjärrplats** under **Säkerhetskontroller**.

   ![](assets/image2014-9-24-17-3a25-3a52.png)

1. Klicka **Ny fjärrplats**.

   ![](assets/image2014-9-24-17-3a26-3a6.png)

1. Retur **Namn på fjärrplats** och **URL för fjärrwebbplats** och sedan klicka **Spara**.

   ![](assets/remote-site-1.png)

   >[!NOTE]
   >
   >Du väljer **Namn på fjärrplats** (MarketoAPI används här). The **URL för fjärrwebbplats** finns i fältet Marketo Host i dialogrutan Redigera API-konfiguration från steg 4.

## Anpassa sidlayouter {#customize-page-layouts}

1. Klicka **Inställningar**.

   ![](assets/image2015-5-22-14-3a40-3a39-1.png)

1. Sök efter&quot;sidlayout&quot; och välj **Sidlayout** under **Leads**.

   ![](assets/image2015-5-28-14-3a58-3a39-1.png)

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

1. Klicka på **Fält** till vänster. Sök och dra sedan **Engagemang** etiketten i **Marketo Sales Insight** layout.

   ![](assets/image2015-5-22-16-3a32-3a46-1.png)

1. Upprepa även ovanstående steg för dessa fält.

<table> 
 <tbody> 
  <tr> 
   <td colspan="1">Engagemang</td> 
  </tr> 
  <tr> 
   <td colspan="1" rowspan="1"><p>Relativt poängvärde</p></td> 
  </tr> 
  <tr> 
   <td colspan="1" rowspan="1"><p>Värde för nödsituationer</p></td> 
  </tr> 
  <tr> 
   <td colspan="1" rowspan="1"><p>Senaste intressanta datum</p></td> 
  </tr> 
  <tr> 
   <td colspan="1" rowspan="1"><p>Senaste intressanta tillfälle</p></td> 
  </tr> 
  <tr> 
   <td colspan="1" rowspan="1"><p>Källa för senaste intressanta stund</p></td> 
  </tr> 
  <tr> 
   <td colspan="1" rowspan="1"><p>Typ av senaste intressanta stund</p></td> 
  </tr> 
 </tbody> 
</table>

1. Klicka **Spara** när du är klar.

   ![](assets/image2014-9-24-17-3a35-3a6.png)

1. Upprepa den här processen för att lägga till Visualforce-sidavsnitt och Sales Insight-fält för **Kontakt**, **Konto** och **Möjligheter**.
1. Upprepa steg 5-7 för att lägga till Visualforce-sidavsnitt för kontakt, konto och säljprojekt. Upprepa sedan steg 8-10 för att lägga till Sales Insight-fält för **Kontakt**. Glöm inte att spara efter ändringarna.

## Mappa anpassade personfält {#map-custom-person-fields}

Marketo personfält måste mappas till Salesforce-kontaktfält för att säkerställa att konverteringen fungerar som den ska. Så här gör du.

1. Klicka **Inställningar**.

   ![](assets/image2015-5-22-14-3a40-3a39-1.png)

1. Sök efter&quot;fält&quot; i sökfältet och klicka på **Fält** under **Leads**.

   ![](assets/image2015-6-1-9-3a54-3a50-1.png)

1. Klicka **Mappa leadfält**.

   ![](assets/image2015-6-1-9-3a58-3a48-1.png)

1. Klicka på listrutan till höger för **Engagemang**.

   ![](assets/image2015-6-1-10-3a9-3a53-1.png)

1. Välj **Contact.Engagement** i listan.

   ![](assets/image2015-6-1-10-3a12-3a11-1.png)

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

   ![](assets/image2014-9-24-17-3a37-3a17.png)

## Marketo Sales Insight Config {#marketo-sales-insight-config}

1. Klicka **+** och sedan markera **Marketo Sales Insight Config**.

   ![](assets/image2014-9-24-17-3a37-3a45.png)

1. Kontrollera **Aktivera Marketo API**. Fyll sedan i [API-konfigurationsinformation i Marketo Admin](#set-up-marketo-sales-insight). Klicka **Spara ändringar** när du är klar.

   ![](assets/image2014-9-24-17-3a38-3a0.png)

   >[!NOTE]
   >
   >Om diagnostiktestet misslyckades kan du behöva [lägga till fler fält i sidlayouten](https://nation.marketo.com/docs/DOC-1115).

Och det är allt! Du bör kunna se fälten Marketo Sales Insight för Leads, Contacts, Accounts och Opportunity.

![](assets/twenty-six-1.png)

>[!NOTE]
>
>För konton kommer Sales Insight att inkludera alla e-postmeddelanden, men bara de senaste intressanta stunderna, webbaktiviteten och poängändringarna.

## Öppna Marketo Sales Insight {#access-marketo-sales-insight}

1. I Salesforce klickar du på **+** i slutet av flikfältet och klicka på **Marketo Sales Insight Config**.

1. Välj **Aktivera Marketo API** kryssrutan.

1. Kopiera inloggningsuppgifterna från Soap API-panelen på Marketo Sales Insight Admin-sida och klistra in dem i Soap API-avsnittet på Salesforce Sales Insight Configuration-sidan.

1. Kopiera inloggningsuppgifterna från panelen Rest API på Marketo Sales Insight Admin-sida och klistra in dem i delen Rest API på konfigurationssidan för Salesforce Sales Insight.

   ![](assets/configure-marketo-sales-insight-in-salesforce-professional-edition-27.png)

>[!MORELIKETHIS]
>
>* [Prioritet, Urklipp, Relativa poäng och Bästa val](/help/marketo/product-docs/marketo-sales-insight/msi-for-salesforce/features/stars-and-flames/priority-urgency-relative-score-and-best-bets.md)
>* [Lägg till Marketo-flik i Salesforce](/help/marketo/product-docs/marketo-sales-insight/msi-for-salesforce/configuration/add-marketo-tab-to-salesforce.md)
>* [Lägg till åtkomst till profiler för Sales Insight](/help/marketo/product-docs/marketo-sales-insight/msi-for-salesforce/configuration/add-sales-insight-access-to-profiles.md){target=&quot;_blank&quot;}

