---
unique-page-id: 3571743
description: Lär dig konfigurera Marketo Sales Insight i Salesforce Professional Edition.
title: Konfigurera Marketo Sales Insight i Salesforce Professional Edition
exl-id: fae63560-0bb3-46a9-94a3-cc27c1aa363e
feature: Marketo Sales Insights
source-git-commit: 68abebb5e1f9dc0780aedcff51d46ed12d5b4d0a
workflow-type: tm+mt
source-wordcount: '684'
ht-degree: 1%

---

# Konfigurera Marketo Sales Insight i Salesforce Professional Edition {#configure-marketo-sales-insight-in-salesforce-professional-edition}

Konfigurera Marketo Sales Insight i Salesforce Professional Edition genom att utföra följande steg.

>[!PREREQUISITES]
>
>* Installera Marketo i Salesforce Professional Edition.
>
>* [Installera Marketo Sales Insight-paket i Salesforce-AppExchange](/help/marketo/product-docs/marketo-sales-insight/msi-for-salesforce/installation/install-marketo-sales-insight-package-in-salesforce-appexchange.md){target="_blank"}

>[!NOTE]
>
>**Administratörsbehörighet krävs.**

## Konfigurera säljinsikter i Marketo Engage {#configure-sales-insight-in-marketo}

1. Öppna ett nytt webbläsarfönster om du vill hämta inloggningsuppgifterna för Marketo Sales Insight från ditt Marketo-konto.

1. Gå till området **[!UICONTROL Admin]** och välj **[!UICONTROL Sales Insight]**.

   ![](assets/configure-marketo-sales-insight-in-salesforce-professional-edition-1-1.png)

1. Klicka på **[!UICONTROL Edit API Configuration]**.

   ![](assets/configure-marketo-sales-insight-in-salesforce-professional-edition-2-1.png)

1. Ange en API-hemlig nyckel som du väljer och klicka på **[!UICONTROL Save]**. Använd INTE ett et-tecken (`&`) i API-hemlig nyckel.

   ![](assets/configure-marketo-sales-insight-in-salesforce-professional-edition-3-1.png)

   >[!NOTE]
   >
   >Den hemliga API-nyckeln är som ett lösenord för din organisation och bör vara säker.

1. Om du vill fylla i inloggningsuppgifterna klickar du på **[!UICONTROL View]** på panelen _[!UICONTROL Rest API Configuration]_.

   ![](assets/configure-marketo-sales-insight-in-salesforce-professional-edition-4-1.png)

1. När du ser en bekräftelsedialogruta klickar du på **[!UICONTROL OK]**.

   ![](assets/configure-marketo-sales-insight-in-salesforce-professional-edition-5-1.png)

## Konfigurera säljinsikter i Salesforce {#configure-sales-insight-in-salesforce}

1. Klicka på **[!UICONTROL Setup]** i Salesforce.

   ![](assets/configure-marketo-sales-insight-in-salesforce-professional-edition-6-1.png)

1. Sök efter fjärrplats och välj **[!UICONTROL Remote Site Settings]**.

   ![](assets/configure-marketo-sales-insight-in-salesforce-professional-edition-7-1.png)

1. Klicka på **[!UICONTROL New Remote Site]**.

   ![](assets/configure-marketo-sales-insight-in-salesforce-professional-edition-8-1.png)

1. Ange namnet på fjärrplatsen (det kan vara något som liknar `MarketoSoapAPI`). Ange URL för fjärrplatsen, som är din Marketo-värd-URL från konfigurationspanelen för Soap API i Marketo Engage. Klicka på **[!UICONTROL Save]**. Du har nu skapat fjärrplatsinställningar för Soap API.

   ![](assets/configure-marketo-sales-insight-in-salesforce-professional-edition-9-1.png)

1. Klicka på **[!UICONTROL New Remote Site]** igen.

   ![](assets/configure-marketo-sales-insight-in-salesforce-professional-edition-10-1.png)

1. Ange namnet på fjärrplatsen (det kan vara något som &quot;MarketoRestAPI&quot;). Ange URL för fjärrplats, som är din API-URL från konfigurationspanelen för Rest API i Marketo. Klicka på **[!UICONTROL Save]**. Du har nu skapat fjärrplatsinställningar för Rest API.

## Bevilja åtkomst till Salesforce-standardobjekt för Sales Insight-användarprofiler {#grant-sales-insight-users-profile-access}

På grund av säkerhetsförbättringarna i Salesforce kan AppExchangar inte längre ge behörighet till standardobjekt, och åtkomst måste beviljas till relevanta Salesforce-objekt från Salesforce-användarens profil. Bevilja de nödvändiga behörigheterna genom att följa dessa steg.

1. Klicka på **[!UICONTROL Setup]**.

1. Sök efter profiler i Snabbsökning.

1. Klicka på **[!UICONTROL Edit]** bredvid profilen som dina Salesforce-användare använder.

1. Aktivera läsåtkomst för följande objekt under avsnittet Standardobjektbehörighet: Lead, Kontakt, Konto och Möjlighet.

1. Klicka på **[!UICONTROL Save]**.

## Anpassa sidlayouter {#customize-page-layouts}

1. Klicka på **[!UICONTROL Setup]**.

   ![](assets/image2015-5-22-14-3a40-3a39-1.png)

1. Sök efter sidlayout och välj **[!UICONTROL Page Layout]** under **[!UICONTROL Leads]**.

   ![](assets/image2015-5-28-14-3a58-3a39-1.png)

1. Klicka på **[!UICONTROL Visualforce Pages]** till vänster. Dra **[!UICONTROL Section]** till layouten under avsnittet Anpassade länkar.

   ![](assets/image2014-9-24-17-3a32-3a53.png)

1. Ange&quot;Marketo Sales Insight&quot; som **[!UICONTROL Section Name]**. Markera **[!UICONTROL 1-Column]** och klicka på **[!UICONTROL OK]**.

   ![](assets/image2014-9-24-17-3a33-3a23.png)

1. Dra och släpp **Lead** i det nya avsnittet.

   ![](assets/image2014-9-24-17-3a33-3a45.png)

   >[!TIP]
   >
   >Namnet på den här rutan ändras baserat på objekttypen. Om du till exempel ändrar sidlayouten för Kontakter visas Kontakt.

1. Dubbelklicka på **[!UICONTROL Lead]**-blocket som du nyss lade till.

   ![](assets/image2014-9-24-17-3a34-3a0.png)

1. Redigera höjden till 450 pixlar och klicka på **[!UICONTROL OK]**.

   ![](assets/image2014-9-24-17-3a34-3a26.png)

   >[!NOTE]
   >
   >Kontrollera **[!UICONTROL Show scrollbars]** om du behöver åtkomst till genomskärningsaktiviteter.

   >[!TIP]
   >
   >Den rekommenderade höjden för objekten Konton och säljprojekt är 410 pixlar.

1. Klicka på **[!UICONTROL Fields]** till vänster. Sök och dra sedan etiketten **[!UICONTROL Engagement]** till layouten **[!UICONTROL Marketo Sales Insight]**.

   ![](assets/image2015-5-22-16-3a32-3a46-1.png)

1. Upprepa föregående steg för följande fält:

   * [!UICONTROL Engagement]
   * [!UICONTROL Relative Score Value]
   * [!UICONTROL Urgency Value]
   * [!UICONTROL Last Interesting Moment Date]
   * [!UICONTROL Last Interesting Moment Desc]
   * [!UICONTROL Last Interesting Moment Source]
   * [!UICONTROL Last Interesting Moment Type]

1. Klicka på **[!UICONTROL Save]** när du är klar.

   ![](assets/image2014-9-24-17-3a35-3a6.png)

1. Om du vill lägga till Visualforce-sidavsnitt för **[!UICONTROL Contact]**, **[!UICONTROL Account]** och **[!UICONTROL Opportunity]** upprepar du steg 5-7.

1. Upprepa steg 8-10 för att lägga till fält för Sales Insight för **[!UICONTROL Contact]**. Glöm inte att spara efter ändringarna.

## Mappa anpassade personfält {#map-custom-person-fields}

Marketo personfält måste mappas till Salesforce-kontaktfält för att konverteringen ska fungera korrekt. Följ de här stegen för att mappa dem.

1. Klicka på **[!UICONTROL Setup]**.

   ![](assets/image2015-5-22-14-3a40-3a39-1.png)

1. Sök efter&quot;fält&quot; i sökfältet och klicka på **[!UICONTROL Fields]** under **[!UICONTROL Leads]**.

   ![](assets/image2015-6-1-9-3a54-3a50-1.png)

1. Klicka på **[!UICONTROL Map Lead Fields]**.

   ![](assets/image2015-6-1-9-3a58-3a48-1.png)

1. Klicka på listrutan till höger för **[!UICONTROL Engagement]**.

   ![](assets/image2015-6-1-10-3a9-3a53-1.png)

1. Välj **[!UICONTROL Contact.Engagement]** i listan.

   ![](assets/image2015-6-1-10-3a12-3a11-1.png)

1. Upprepa och mappa även dessa fält.

   | Anpassat fält för Marketo-person | Anpassat fält för Salesforce-kontakt |
   |--- |--- |
   | `Engagement` | `Contact.Engagement` |
   | `Relative Score Value` | `Contact.Relative Score Value` |
   | `Urgency Value` | `Contact.Urgency Value` |
   | `Last Interesting Moment Date` | `Contact.Last Interesting Moment Date` |
   | `Last Interesting Moment Desc` | `Contact.Last Interesting Moment Desc` |
   | `Last Interesting Moment Source` | `Contact.Last Interesting Moment Source` |
   | `Last Interesting Moment Type` | `Contact.Last Interesting Moment Type` |

   {style="table-layout:auto"}

1. Klicka på **[!UICONTROL Save]** när du är klar.

   ![](assets/image2014-9-24-17-3a37-3a17.png)

## Konfigurationsfliken för Marketo Sales Insight {#marketo-sales-insight-configuration-tab}

1. Klicka på **+** i slutet av flikfältet i Salesforce och klicka på **[!UICONTROL Marketo Sales Insight Config]**.

1. Kopiera autentiseringsuppgifterna från Soap API-panelen på [Marketo Sales Insight Admin-sidan](/help/marketo/product-docs/marketo-sales-insight/msi-for-salesforce/configuration/configure-marketo-sales-insight-in-salesforce-professional-edition.md#set-up-marketo-sales-insight){target="_blank"} och klistra in dem i Soap API-avsnittet på Salesforce Sales Insight Configuration-sidan.

1. Kopiera inloggningsuppgifterna från panelen **[!UICONTROL Rest API]** på [Marketo Sales Insight Admin-sidan](/help/marketo/product-docs/marketo-sales-insight/msi-for-salesforce/configuration/configure-marketo-sales-insight-in-salesforce-professional-edition.md#set-up-marketo-sales-insight){target="_blank"} och klistra in dem i delen Rest API på konfigurationssidan för Salesforce Sales Insight.

   ![](assets/configure-marketo-sales-insight-in-salesforce-professional-edition-27.png)

Du bör kunna se fälten Marketo Sales Insight för Leads, Contacts, Accounts och Opportunity.

>[!NOTE]
>
>Om diagnostiktestet misslyckas kan [problemet åtgärdas genom att fler fält läggs till i sidlayouten](https://nation.marketo.com/t5/knowledgebase/how-to-repair-marketo-sales-insight-setup-configuration-problems/ta-p/248218){target="_blank"}.

>[!NOTE]
>
>För konton inkluderar Sales Insight alla e-postmeddelanden, men bara de senaste intressanta stunderna, webbaktiviteten och poängändringarna.

>[!MORELIKETHIS]
>
>* [Prioritet, brådskande, Relativ poäng och Bästa val](/help/marketo/product-docs/marketo-sales-insight/msi-for-salesforce/features/stars-and-flames/priority-urgency-relative-score-and-best-bets.md){target="_blank"}
>* [Lägg till Marketo-flik i Salesforce](/help/marketo/product-docs/marketo-sales-insight/msi-for-salesforce/configuration/add-marketo-tab-to-salesforce.md){target="_blank"}
>* [Lägg till åtkomst till profiler för Sales Insight](/help/marketo/product-docs/marketo-sales-insight/msi-for-salesforce/configuration/add-sales-insight-access-to-profiles.md){target="_blank"}
