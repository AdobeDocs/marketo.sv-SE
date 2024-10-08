---
unique-page-id: 2949711
description: Installera Marketo e-posttillägg för Outlook med en registreringskod - Marketo Docs - Produktdokumentation
title: Installera Marketo e-posttillägg för Outlook med en registreringskod
exl-id: d7a877c2-f71e-44da-b323-04f6cdb44eb0
feature: Marketo Sales Insights
source-git-commit: 40fe81d465d04be97ae5e216250b7e06e6d3791e
workflow-type: tm+mt
source-wordcount: '532'
ht-degree: 0%

---

# Installera Marketo e-posttillägg för Outlook med en registreringskod {#install-the-marketo-email-add-in-for-outlook-with-a-registration-code}

Om användarna har tillgång till administratörsinställningarna på sina bärbara datorer kan du skicka en registreringskod direkt till dem.

Om du inte har fått någon inbjudan via e-post ber du Marketo-administratören att bjuda in dig.

>[!PREREQUISITES]
>
>Du måste [ha fått en Marketo-licens för e-posttillägg](/help/marketo/product-docs/marketo-sales-insight/msi-outlook-plugin/issue-a-marketo-email-add-in-license.md).

>[!IMPORTANT]
>
>Installationen stöds inte på datorer där Windows-användarmappen innehåller tecken som inte är engelska. Den här mappen genereras automatiskt av Windows under `<System Root>\Users\` baserat på Windows-användarnamnet och kan innehålla icke-engelska tecken om Windows-användarnamnet är ett icke-engelskt namn. Kontakta IT-avdelningen för att kontrollera om du har installationsproblem.

>[!NOTE]
>
>Funktioner för Sales Insight-åtgärder, inklusive Skicka e-post, Lägg till i säljkampanj och Uppgifter, är inte tillgängliga i e-postpluginer för Sales Insight för Gmail och Outlook. För närvarande kan användare bara skicka spårbara e-postmeddelanden med eller utan en Marketo-e-postmall från sin e-postklient när de använder e-postpluginmodulerna för Sales Insight.

## Hämta installationsprogram {#download-installer}

1. Identifiera din [Microsoft Outlook-version](https://support.office.com/en-us/article/what-version-of-outlook-do-i-have-b3a9568c-edb5-42b9-9825-d48d82b2257c){target="_blank"}

1. Klicka på länken om du vill hämta det installationsprogram som är lämpligt för din version av Microsoft Outlook.

   >[!NOTE]
   >
   >För närvarande fungerar länkarna nedan bara i Microsoft Edge, eller genom att högerklicka i Chrome. Vi beklagar eventuella besvär.

   | Outlook-version | 32-bitars Outlook | 64-bitars Outlook |
   |---|---|---|
   | Outlook 2000 | Stöds inte | Ej tillämpligt |
   | Outlook 2003 | [Hämta](https://munchkin.marketo.net/MarketoAddInSetup32.msi) | Ej tillämpligt |
   | Outlook 2007 | [Hämta](https://munchkin.marketo.net/MarketoAddInSetup32.msi) | Ej tillämpligt |
   | Outlook 2010 | [Hämta](https://munchkin.marketo.net/MarketoAddInSetup32.msi) | [Hämta](https://munchkin.marketo.net/MarketoAddInSetup64.msi) |
   | Outlook 2013 | [Hämta](https://munchkin.marketo.net/MarketoAddInSetup32.msi) | [Hämta](https://munchkin.marketo.net/MarketoAddInSetup64.msi) |
   | Outlook 2016 | [Hämta](https://munchkin.marketo.net/MarketoAddInSetup32.msi) | [Hämta](https://munchkin.marketo.net/MarketoAddInSetup64.msi) |
   | Outlook 2019 | [Hämta](https://munchkin.marketo.net/MarketoAddInSetup32.msi) | [Hämta](https://munchkin.marketo.net/MarketoAddInSetup64.msi) |
   | Outlook för Mac | Stöds inte | Stöds inte |
   | Outlook Web App | Stöds inte | Stöds inte |
   | Office 365* | [Hämta](https://munchkin.marketo.net/MarketoAddInSetup32.msi) | [Hämta](https://munchkin.marketo.net/MarketoAddInSetup64.msi) |

   *Office 365-version: endast Windows-klient (i Windows 10, Enterprise eller Pro).

   >[!IMPORTANT]
   >
   >Microsoft har släppt en [ny version av Outlook för Windows](https://techcommunity.microsoft.com/t5/outlook-blog/new-outlook-for-windows-now-available/ba-p/3932068){target="_blank"}. Den nya versionen stöder inte det befintliga MSI Outlook-plugin-programmet. MSI Outlook-pluginprogrammet fortsätter att fungera för Windows-datorer som kör den klassiska versionen av Outlook. [Klicka här](https://techcommunity.microsoft.com/t5/outlook-blog/the-new-outlook-for-windows-for-organization-admins/ba-p/3929169){target="_blank"} om du vill veta mer om nya Outlook för Windows för organisationer.

## Kopiera din registreringskod {#copy-your-registration-code}

1. Kopiera registreringskoden från det inbjudningsmejl du fick.

   ![](assets/image2016-7-22-10-3a45-3a10.png)

1. Stäng Microsoft Outlook.

   ![](assets/ent-key-close-outlook-hand.png)

## Installera {#install}

1. Kör installationsprogrammet.

   ![](assets/image2016-7-25-10-3a23-3a33.png)

   >[!NOTE]
   >
   >Om du får en säkerhetsvarning, oroa dig inte! Klicka bara på **Kör**.

1. Klicka på **Nästa**.

   ![](assets/welcome-to-the-setup-wizard-hand.png)

1. Fyll i **Förnamn**, **Efternamn**, **E-postadress**, kopiera och klistra sedan in **registreringskoden** från e-postmeddelandet i formuläret och klicka på **Nästa**.

   ![](assets/enter-your-information-hands.png)

   >[!TIP]
   >
   >Om installationen misslyckas bör du kontakta din IT-avdelning för att kontrollera att HTTPS-trafik inte blockeras. Installationsprogrammet kräver att HTTPS-trafik är öppen.

1. Klicka på **Nästa** om du vill installera på standardplatsen.

   ![](assets/select-installation-folder-hand.png)

1. Klicka på **Nästa**.

   ![](assets/confirm-installation-hand.png)

   >[!NOTE]
   >
   >Om du får en säkerhetsfråga om en okänd utgivare klickar du på **Ja**.

1. Installationen är klar. Klicka på **Stäng**.

   ![](assets/image2014-9-23-15-3a52-3a11.png)

1. Öppna nu Microsoft Outlook och se Marketo-knapparna.

   ![](assets/image2016-8-24-15-3a47-3a38.png)

   Underbar! Nu är Marketo-knapparna på ett bättre ställe.

Läs mer om hur du använder åtgärderna Marketo Message and Log With Marketo.

>[!MORELIKETHIS]
>
>* [Skicka och spåra ett e-postmeddelande med Marketo-tillägget för e-post för Outlook](/help/marketo/product-docs/marketo-sales-insight/msi-outlook-plugin/send-and-track-an-email-with-the-email-add-in-for-outlook.md){target="_blank"}
>* [Skicka och spåra från Outlook med en Marketo-mall](/help/marketo/product-docs/marketo-sales-insight/msi-outlook-plugin/send-and-track-from-outlook-using-a-marketo-template.md){target="_blank"}
