---
unique-page-id: 2949711
description: Installera Marketo Email-tillägget för Outlook med en registreringskod - Marketo Docs - Produktdokumentation
title: Installera Marketo-e-posttillägget för Outlook med en registreringskod
translation-type: tm+mt
source-git-commit: 567a18fde3335076cc24d2302096c791fa4084f0
workflow-type: tm+mt
source-wordcount: '427'
ht-degree: 0%

---


# Installera Marketo-e-posttillägget för Outlook med en registreringskod {#install-the-marketo-email-add-in-for-outlook-with-a-registration-code}

Om användarna har tillgång till administratörsinställningarna på sina bärbara datorer kan du skicka en registreringskod direkt till dem.

Om du inte har fått någon inbjudan via e-post ber du Marketo-administratören att bjuda in dig.

>[!PREREQUISITES]
>
>Du måste vara [utfärdad en Marketo Email-tilläggslicens](/help/marketo/product-docs/marketo-sales-insight/msi-outlook-plugin/issue-a-marketo-email-add-in-license.md).

>[!NOTE]
>
>Från och med 10/1/20 har den senaste versionen av Outlook-plugin inte längre stöd för offlineläge. Detta börjar gälla efter installation/uppgradering på eller efter 10/1.

## Hämta installationsprogrammet {#download-installer}

1. Identifiera din [Microsoft Outlook-version](https://support.office.com/en-us/article/what-version-of-outlook-do-i-have-b3a9568c-edb5-42b9-9825-d48d82b2257c)

1. Klicka på länken om du vill hämta det installationsprogram som passar din version av Microsoft Outlook.

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

   *Office 365-version: Endast Windows-klient (i Windows 10, Enterprise eller Pro).

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

1. Installationen är nu klar, klicka på **Stäng**.

   ![](assets/image2014-9-23-15-3a52-3a11.png)

1. Öppna nu Microsoft Outlook och se Marketo-knapparna.

   ![](assets/image2016-8-24-15-3a47-3a38.png)

   Underbar! Nu är Marketo-knapparna på en bättre plats.

Läs mer om hur du använder åtgärderna Marketo Message och Log With Marketo.

>[!MORELIKETHIS]
>
>* [Skicka och spåra ett e-postmeddelande med tillägget Marketo Email för Outlook](/help/marketo/product-docs/marketo-sales-insight/msi-outlook-plugin/send-and-track-an-email-with-the-email-add-in-for-outlook.md)
>* [Skicka och spåra från Outlook med en Marketo-mall](/help/marketo/product-docs/marketo-sales-insight/msi-outlook-plugin/send-and-track-from-outlook-using-a-marketo-template.md)

