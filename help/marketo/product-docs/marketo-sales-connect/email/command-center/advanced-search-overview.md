---
unique-page-id: 37356329
description: Advanced Search Overview - Marketo Docs - Product Documentation
title: Översikt över avancerad sökning
exl-id: bb6e2c9f-b44a-43ba-94ae-ae30e182bcc8
feature: Marketo Sales Connect
source-git-commit: 09a656c3a0d0002edfa1a61b987bff4c1dff33cf
workflow-type: tm+mt
source-wordcount: '376'
ht-degree: 2%

---

# Översikt över avancerad sökning {#advanced-search-overview}

Genom att använda den avancerade sökningen för att rikta dig till potentiella kunder som har visat, klickat eller svarat på e-postmeddelanden kan du skapa en målinriktad lista över de mest engagerade potentiella kunderna.

## Använda avancerad sökning {#how-to-access-advanced-search}

1. Klicka på **[!UICONTROL Command Center]**.

   ![](assets/one.png)

1. Klicka på **[!UICONTROL Emails]**.

   ![](assets/two.png)

1. Välj lämplig flik.

   ![](assets/three.png)

1. Klicka på **[!UICONTROL Advanced Search]**.

   ![](assets/four.png)

## Filter {#filters}

**Datum**

Välj datumintervall för sökningen. Förinställda datum uppdateras beroende på vilken e-poststatus du väljer ([!UICONTROL Sent], [!UICONTROL Undelivered], [!UICONTROL Pending]).

![](assets/date.png)

**Vem**

Filtrera efter e-postmottagare/avsändare i avsnittet [!UICONTROL Who].

![](assets/who.png)

| Nedrullningsbar meny | Beskrivning |
|---|---|
| **[!UICONTROL View As]** | Filtrera efter en specifik avsändare i din [!DNL Sales Connect]-instans (det här alternativet är endast tillgängligt för administratörer). |
| **[!UICONTROL By Group]** | Filtrera e-postmeddelanden efter en viss grupp mottagare. |
| **[!UICONTROL By Person]** | Filtrera efter en viss mottagare. |

**När**

Välj efter skapat datum, leveransdatum, misslyckat datum eller schemalagt datum. Vilka alternativ som är tillgängliga varierar beroende på vilken e-poststatus du väljer ([!UICONTROL Sent], [!UICONTROL Undelivered], [!UICONTROL Pending]).

![](assets/when.png)

**Kampanjer**

Filtrera e-postmeddelanden efter kampanjdeltagande.

![](assets/campaigns.png)

**Status**

Det finns tre e-poststatusar att välja mellan. Typen/aktivitetsalternativen ändras baserat på vald status.

![](assets/status.png)

***Status: Skickat***

![](assets/status-sent.png)

Filtrerar efter din skickade e-postaktivitet. Du kan välja vyer/inga vyer, klicka/klicka utan klick och/eller svar/inga svar.

***Status: Väntande***

![](assets/status-pending.png)

Filtrerar efter alla väntande e-postmeddelanden.

| Status | Beskrivning |
|---|---|
| **[!UICONTROL Scheduled]** | E-postmeddelanden som har schemalagts från dispositionsfönstret ([!DNL Salesforce] eller Web App), e-postplugin-program eller en kampanj. |
| **[!UICONTROL Drafts]** | E-postmeddelanden som är i utkastläge. E-postmeddelanden kräver en ämnesrad och en mottagare för att kunna sparas som ett utkast. |
| **[!UICONTROL In Progress]** | E-postmeddelanden som håller på att skickas. E-postmeddelanden får inte vara kvar i det här läget i mer än några sekunder. |

***Status: Olevererad***

![](assets/status-undelivered.png)

Filtrerar efter e-postmeddelanden som aldrig levererats.

| Status | Beskrivning |
|---|---|
| **[!UICONTROL Failed]** | När ett e-postmeddelande inte kan skickas från [!DNL Sales Connect] (vanliga orsaker är bland annat: e-postmeddelanden skickas till kontakter som avbrutit prenumerationen/blockerats, eller om det uppstod ett problem med att fylla i de dynamiska fälten). |
| **[!UICONTROL Bounced]** | Ett e-postmeddelande markeras som studsat när det avvisas av mottagarens server. Endast e-postmeddelanden som skickades via [!DNL Sales Connect] servrar visas här. |
| **[!UICONTROL Spam]** | När e-postmeddelandet har markerats som skräppost (vanlig term för oombedd e-post) av mottagaren. Endast e-postmeddelanden som skickades via [!DNL Sales Connect] servrar visas här. |

## Sparade sökningar {#saved-searches}

Så här skapar du en sparad sökning.

1. Klicka på **[!UICONTROL Save Filters As]** när alla filter är på plats.

   ![](assets/save-search-1.png)

1. Ge sökningen ett namn och klicka på **[!UICONTROL Save]**.

   ![](assets/save-search-2.png)

   Dina sparade sökningar visas i sidofältet till vänster.

   ![](assets/advanced-search-overview-15.png)
