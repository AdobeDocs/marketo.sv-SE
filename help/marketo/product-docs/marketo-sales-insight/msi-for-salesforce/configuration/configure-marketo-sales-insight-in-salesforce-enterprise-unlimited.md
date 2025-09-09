---
unique-page-id: 2360368
description: Lär dig konfigurera Marketo Sales Insight i Salesforce Enterprise/Unlimited editions.
title: Konfigurera Marketo Sales Insight i Salesforce Enterprise/Unlimited
exl-id: a33ed396-8d26-403f-b6d8-fe7c55ce76ba
feature: Marketo Sales Insights
source-git-commit: 07b2e888c31c6e98a3207fad5d277261f7f193af
workflow-type: tm+mt
source-wordcount: '801'
ht-degree: 1%

---

# Konfigurera [!DNL Marketo Sales Insight] i [!DNL Salesforce] Enterprise/Unlimited {#configure-marketo-sales-insight-in-salesforce-enterprise-unlimited}

Konfigurera Marketo Sales Insight i Salesforce Enterprise/Unlimited editions genom att utföra följande steg.

>[!PREREQUISITES]
>
>[Installera [!DNL Marketo Sales Insight] Paket i [!DNL Salesforce] AppExchange](/help/marketo/product-docs/marketo-sales-insight/msi-for-salesforce/installation/install-marketo-sales-insight-package-in-salesforce-appexchange.md)

>[!NOTE]
>
>**Administratörsbehörighet krävs.**

## Konfigurera Sales Insight i Marketo Engage {#configure-sales-insight-in-marketo}

1. Om du vill få dina Marketo Sales Insight-inloggningsuppgifter i Marketo Engage går du till **[!UICONTROL Admin]**-området och väljer **[!UICONTROL Sales Insight]**.

   ![](assets/configure-marketo-sales-insight-in-salesforce-professional-edition-1.png)

1. Klicka på **[!UICONTROL Edit API Configuration]**.

   ![](assets/configure-marketo-sales-insight-in-salesforce-professional-edition-2.png)

1. Ange en API-hemlig nyckel som du väljer och klicka på **[!UICONTROL Save]**. Använd INTE ett et-tecken (`&`) i API-hemlig nyckel.

   ![](assets/configure-marketo-sales-insight-in-salesforce-professional-edition-3.png)

   >[!NOTE]
   >
   >Den hemliga API-nyckeln är som ett lösenord för din organisation och bör vara säker.

1. Om du vill fylla i inloggningsuppgifterna klickar du på **[!UICONTROL View]** på panelen _[!UICONTROL Rest API Configuration]_.

   ![](assets/configure-marketo-sales-insight-in-salesforce-professional-edition-4.png)

1. När du ser en bekräftelsedialogruta klickar du på **[!UICONTROL OK]**.

   ![](assets/configure-marketo-sales-insight-in-salesforce-professional-edition-5.png)

   >[!TIP]
   >
   >Låt det här fönstret vara öppet. Du behöver den här informationen senare för att konfigurera Salesforce.

## Fyll i nya referenser för Rest API {#populate-new-rest-api-credentials}

1. När du fyller i Rest API-autentiseringsuppgifter för första gången ändras knappen _Visa_ till _Redigera_. Klicka på knappen **Redigera**.

   ![](assets/configure-marketo-sales-insight-in-salesforce-professional-edition-5a.png)

1. Ett meddelande visas som bekräftar att du vill återskapa API-autentiseringsuppgifter. Klicka på **Spara**.

   ![](assets/configure-marketo-sales-insight-in-salesforce-professional-edition-5b.png){width="800" zoomable="yes"}

1. När de nya autentiseringsuppgifterna har fyllts i uppdaterar du dem på fliken _Marketo Config_ i din Salesforce-instans.

   ![](assets/configure-marketo-sales-insight-in-salesforce-professional-edition-5c.png)

## Konfigurera [!DNL Sales Insight] i [!DNL Salesforce] {#configure-sales-insight-in-salesforce}

1. Klicka på **[!UICONTROL Setup]** i Salesforce.

   ![](assets/configure-marketo-sales-insight-in-salesforce-professional-edition-6.png)

1. Sök efter fjärrplats och välj **[!UICONTROL Remote Site Settings]**.

   ![](assets/configure-marketo-sales-insight-in-salesforce-professional-edition-7.png)

1. Klicka på **[!UICONTROL New Remote Site]**.

   ![](assets/configure-marketo-sales-insight-in-salesforce-professional-edition-8.png)

1. Ange namnet på fjärrplatsen (det kan vara något som liknar `MarketoSoapAPI`). Ange URL:en för fjärrplatsen, som är din Marketo-värd-URL från panelen _[!UICONTROL Soap API Configuration]_i Marketo Engage. Klicka på&#x200B;**[!UICONTROL Save]**. Du har nu skapat fjärrplatsinställningar för Soap API.

   ![](assets/configure-marketo-sales-insight-in-salesforce-professional-edition-9.png)

1. Klicka på **[!UICONTROL New Remote Site]** igen.

   ![](assets/configure-marketo-sales-insight-in-salesforce-professional-edition-10.png)

1. Ange namnet på fjärrplatsen (det kan vara något som liknar `MarketoAPI`). Ange URL:en för fjärrplatsen, som är din API-URL från panelen _[!UICONTROL Rest API Configuration]_i Marketo Engage. Klicka på&#x200B;**[!UICONTROL Save]**. Du har nu skapat fjärrplatsinställningar för Rest API.

   >[!NOTE]
   >
   >_Du_ väljer **[!UICONTROL Remote Site Name]** (`MarketoAPI` används här). **[!UICONTROL Remote Site URL]** finns i fältet Marketo-värd i dialogrutan Redigera API-konfiguration från steg 3 i avsnittet Konfigurera säljinsikter i Marketo.

## Ge användare av Sales Insight-profilen åtkomst till Salesforce standardobjekt {#grant-sales-insight-users-profile-access}

På grund av Salesforce säkerhetsförbättringar kan AppExchange-paket inte längre ge behörighet till standardobjekt, och åtkomst måste beviljas till relevanta Salesforce-objekt från Salesforce-användarprofilen. Följ de här stegen om du vill ge de behörigheter som krävs.

1. Klicka på **[!UICONTROL Setup]**.

1. Sök efter profiler i Snabbsökning.

1. Klicka på **[!UICONTROL Edit]** bredvid profilen som dina Salesforce-användare använder.

1. Aktivera _[!UICONTROL Standard Object Permission]_-åtkomst för följande objekt under avsnittet **[!UICONTROL Read]**: [!UICONTROL Lead], [!UICONTROL Contact], [!UICONTROL Account] och [!UICONTROL Opportunity].

1. Klicka på **[!UICONTROL Save]**.

## Anpassa sidlayouter {#customize-page-layouts}

1. Klicka på **[!UICONTROL Setup]**.

   ![](assets/image2015-5-22-14-3a40-3a39.png)

1. Sök efter sidlayout och välj **[!UICONTROL Page Layout]** under **[!UICONTROL Leads]**.

   ![](assets/image2015-5-28-14-3a58-3a39.png)

1. Klicka på **[!UICONTROL Visualforce Pages]** till vänster. Dra **[!UICONTROL Section]** till layouten under avsnittet _[!UICONTROL Custom Links]_.

   ![](assets/image2014-9-24-17-3a32-3a53.png)

1. Ange&quot;Marketo Sales Insight&quot; som **[!UICONTROL Section Name]**, välj **[!UICONTROL 1-Column]** och klicka på **[!UICONTROL OK]**.

   ![](assets/image2014-9-24-17-3a33-3a23.png)

1. Dra och släpp **[!UICONTROL Lead]** i det nya avsnittet.

   ![](assets/image2014-9-24-17-3a33-3a45.png)

   >[!TIP]
   >
   >Namnet på den här rutan ändras baserat på objekttypen. Om du till exempel ändrar sidlayouten för Kontakter visas Kontakt.

1. Dubbelklicka på **[!UICONTROL Lead]**-blocket som du nyss lade till.

   ![](assets/image2014-9-24-17-3a34-3a0.png)

1. Redigera höjden till **450** pixlar och klicka på **[!UICONTROL OK]**.

   ![](assets/image2014-9-24-17-3a34-3a26.png)

   >[!NOTE]
   >
   >Kontrollera **[!UICONTROL Show scrollbars]** om du behöver åtkomst till genomskärningsaktiviteter.

   >[!TIP]
   >
   >Den rekommenderade höjden för objekten Konton och säljprojekt är 410 pixlar.

1. Klicka på **[!UICONTROL Fields]** till vänster. Sök och dra sedan etiketten **[!UICONTROL Urgency]** till layouten **[!UICONTROL Marketo Sales Insight]**.

   ![](assets/configure-marketo-sales-insight-in-salesforce-professional-edition-18.png)

1. Upprepa även ovanstående steg för dessa fält.

   * Senaste intressanta stund
   * Senaste intressanta datum
   * Senaste intressanta tillfälle
   * Senaste intressanta stund Source
   * Typ av senaste intressanta stund
   * Senaste aktivitet efter försäljning
   * Senaste åtagande per försäljning
   * Kontakt-ID för MSI
   * Relativa poäng
   * Relativt poängvärde
   * Akut
   * Värde för nödsituationer
   * Visa i Marketo

1. Klicka på **[!UICONTROL Save]** när du är klar.

   ![](assets/image2014-9-24-17-3a35-3a6.png)

1. Upprepa steg 5-7 för att lägga till Visualforce-sidavsnitt och Sales Insight-fält för **[!UICONTROL Contact]**, **[!UICONTROL Account]** och **[!UICONTROL Opportunity]**.

1. Upprepa steg 8-10 för att lägga till dessa Sales Insight-fält för **[!UICONTROL Contact]**. Var noga med att spara ändringarna.

   * Senaste intressanta stund
   * Senaste intressanta datum
   * [!UICONTROL Last Interesting Moment Desc]
   * [!UICONTROL Last Interesting Moment Source]
   * [!UICONTROL Last Interesting Moment Type]
   * [!UICONTROL Last Marketo Activity by Sales]
   * [!UICONTROL Last Marketo Engagement by Sales]
   * [!UICONTROL MKTO Lead Score]
   * [!UICONTROL Relative Score]
   * [!UICONTROL Relative Score Value]
   * [!UICONTROL Sales Insight] - Öppnar sidan med fullständig kontaktlista
   * [!UICONTROL Urgency]
   * [!UICONTROL Urgency Value]

## Mappa anpassade personfält {#map-custom-person-fields}

Marketo personfält måste mappas till Salesforce kontaktfält för att konverteringen ska fungera korrekt. Följ de här stegen för att mappa dem.

1. Klicka på **[!UICONTROL Setup]**.

   ![](assets/image2015-5-22-14-3a40-3a39.png)

1. Sök efter&quot;fält&quot; i sökfältet och klicka på **[!UICONTROL Fields]** under **[!UICONTROL Leads]**.

   ![](assets/image2015-6-1-9-3a54-3a50.png)

1. Klicka på **[!UICONTROL Map Lead Fields]**.

   ![](assets/image2015-6-1-9-3a58-3a48.png)

1. Klicka på listrutan till höger för **[!UICONTROL Engagement]**.

   ![](assets/image2015-6-1-10-3a9-3a53.png)

1. Välj **[!UICONTROL Contact.Engagement]** i listan.

   ![](assets/image2015-6-1-10-3a12-3a11.png)

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

1. Klicka på **[!UICONTROL Save]** när du är klar.

## Konfigurationsfliken för Marketo Sales Insight {#marketo-sales-insight-configuration-tab}

1. I Salesforce klickar du på **+** i slutet av flikfältet och sedan på **[!UICONTROL Marketo Sales Insight Config]**.

1. Kopiera autentiseringsuppgifterna från Soap API-panelen på [Marketo Sales Insight Admin-sidan](/help/marketo/product-docs/marketo-sales-insight/msi-for-salesforce/configuration/configure-marketo-sales-insight-in-salesforce-professional-edition.md#set-up-marketo-sales-insight){target="_blank"} och klistra in dem i Soap API-avsnittet på konfigurationssidan för [!DNL Salesforce] [!DNL Sales Insight] .

1. Kopiera autentiseringsuppgifterna från panelen Rest API på [Marketo Sales Insight Admin-sidan](/help/marketo/product-docs/marketo-sales-insight/msi-for-salesforce/configuration/configure-marketo-sales-insight-in-salesforce-professional-edition.md#set-up-marketo-sales-insight){target="_blank"} och klistra in dem i delen Rest API på konfigurationssidan för [!DNL Salesforce] [!DNL Sales Insight] .

   ![](assets/configure-marketo-sales-insight-in-salesforce-enterprise-edition-25.png)

Du bör kunna se fälten Marketo Sales Insight för Leads, Contacts, Accounts och Opportunity.

>[!NOTE]
>
>Om diagnostiktestet misslyckas kan problemet åtgärdas genom att [lägga till fler fält i sidlayouten](https://nation.marketo.com:443/t5/knowledgebase/how-to-repair-marketo-sales-insight-setup-configuration-problems/ta-p/248218){target="_blank"}.

>[!NOTE]
>
>För konton inkluderar Sales Insight alla e-postmeddelanden, men bara de senaste intressanta stunderna, webbaktiviteten och poängändringarna.

>[!MORELIKETHIS]
>
>* [Prioritet, brådskande, Relativ poäng och Bästa val](/help/marketo/product-docs/marketo-sales-insight/msi-for-salesforce/features/stars-and-flames/priority-urgency-relative-score-and-best-bets.md)
>* [Lägg till Marketo-flik i [!DNL Salesforce]](/help/marketo/product-docs/marketo-sales-insight/msi-for-salesforce/configuration/add-marketo-tab-to-salesforce.md)
>* [Lägg till åtkomst till profiler för Sales Insight](/help/marketo/product-docs/marketo-sales-insight/msi-for-salesforce/configuration/add-sales-insight-access-to-profiles.md){target="_blank"}
