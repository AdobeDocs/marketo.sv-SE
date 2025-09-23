---
unique-page-id: 2949711
description: Installera Marketo-tillägget för e-post för  [!DNL Outlook]  med en registreringskod - Marketo Docs - Produktdokumentation
title: Installera Marketo e-posttillägg för  [!DNL Outlook] med en registreringskod
exl-id: d7a877c2-f71e-44da-b323-04f6cdb44eb0
feature: Marketo Sales Insights
source-git-commit: 09a656c3a0d0002edfa1a61b987bff4c1dff33cf
workflow-type: tm+mt
source-wordcount: '522'
ht-degree: 2%

---

# Installera Marketo e-posttillägg för [!DNL Outlook] med en registreringskod {#install-the-marketo-email-add-in-for-outlook-with-a-registration-code}

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

1. Identifiera din [Microsoft Outlook-version](https://support.office.com/en-us/article/what-version-of-outlook-do-i-have-b3a9568c-edb5-42b9-9825-d48d82b2257c){target="_blank"}.

1. I tabellen nedan klickar du på länken för att hämta rätt ZIP-fil för din version av Microsoft Outlook.

1. Zippa upp filen för att få tillgång till den nödvändiga MSI-filen och fortsätt med installationen.

   >[!NOTE]
   >
   >För närvarande fungerar länkarna nedan bara i [!DNL Microsoft Edge] eller genom att högerklicka i [!DNL Chrome]. Vi beklagar eventuella besvär.

<table><thead>
  <tr>
    <th>Outlook-version</th>
    <th>32-bitars Outlook</th>
    <th>64-bitars Outlook</th>
  </tr></thead>
<tbody>
  <tr>
    <td>Outlook 2000</td>
    <td>Stöds inte</td>
    <td>Ej tillämpligt</td>
  </tr>
  <tr>
    <td>Outlook 2003</td>
    <td><a href="https://munchkin.marketo.net/MarketoAddInSetup32.zip">Ladda ned</a></td>
    <td>Ej tillämpligt</td>
  </tr>
  <tr>
    <td>Outlook 2007</td>
    <td><a href="https://munchkin.marketo.net/MarketoAddInSetup32.zip">Ladda ned</a></td>
    <td>Ej tillämpligt</td>
  </tr>
  <tr>
    <td>Outlook 2010</td>
    <td><a href="https://munchkin.marketo.net/MarketoAddInSetup32.zip">Ladda ned</a></td>
    <td><a href="https://munchkin.marketo.net/MarketoAddInSetup64.zip">Ladda ned</a></td>
  </tr>
  <tr>
    <td>Outlook 2013</td>
    <td><a href="https://munchkin.marketo.net/MarketoAddInSetup32.zip">Ladda ned</a></td>
    <td><a href="https://munchkin.marketo.net/MarketoAddInSetup64.zip">Ladda ned</a></td>
  </tr>
  <tr>
    <td>Outlook 2016</td>
    <td><a href="https://munchkin.marketo.net/MarketoAddInSetup32.zip">Ladda ned</a></td>
    <td><a href="https://munchkin.marketo.net/MarketoAddInSetup64.zip">Ladda ned</a></td>
  </tr>
  <tr>
    <td>Outlook 2019</td>
    <td><a href="https://munchkin.marketo.net/MarketoAddInSetup32.zip">Ladda ned</a></td>
    <td><a href="https://munchkin.marketo.net/MarketoAddInSetup64.zip">Ladda ned</a></td>
  </tr>
  <tr>
    <td>Outlook för Mac</td>
    <td>Stöds inte</td>
    <td>Stöds inte</td>
  </tr>
  <tr>
    <td>Outlook Web App</td>
    <td>Stöds inte</td>
    <td>Stöds inte</td>
  </tr>
  <tr>
    <td>Office 365*</td>
    <td><a href="https://munchkin.marketo.net/MarketoAddInSetup32.zip">Ladda ned</a></td>
    <td><a href="https://munchkin.marketo.net/MarketoAddInSetup64.zip">Ladda ned</a></td>
  </tr>
</tbody></table>

*[!DNL Office] 365 version: [!DNL Windows] endast klient (på [!DNL Windows] 10, [!DNL Enterprise] eller [!DNL Pro]).

>[!IMPORTANT]
>
>Microsoft har släppt en [ny version av Outlook för Windows](https://techcommunity.microsoft.com/t5/outlook-blog/new-outlook-for-windows-now-available/ba-p/3932068){target="_blank"}. Den nya versionen stöder inte det befintliga MSI Outlook-plugin-programmet. MSI Outlook-pluginprogrammet fortsätter att fungera för Windows-datorer som kör den klassiska versionen av Outlook. [Klicka här](https://techcommunity.microsoft.com/t5/outlook-blog/the-new-outlook-for-windows-for-organization-admins/ba-p/3929169){target="_blank"} om du vill veta mer om nya Outlook för Windows för organisationer.

## Kopiera din registreringskod {#copy-your-registration-code}

1. Kopiera registreringskoden från det inbjudningsmejl du fick.

   ![](assets/image2016-7-22-10-3a45-3a10.png)

1. Stäng [!DNL Microsoft Outlook].

   ![](assets/ent-key-close-outlook-hand.png)

## Installera {#install}

1. Kör installationsprogrammet.

   ![](assets/image2016-7-25-10-3a23-3a33.png)

   >[!NOTE]
   >
   >Om du får en säkerhetsvarning, oroa dig inte! Klicka bara på **Kör**.

1. Klicka på **[!UICONTROL Next]**.

   ![](assets/welcome-to-the-setup-wizard-hand.png)

1. Fyll i **[!UICONTROL First Name]**, **[!UICONTROL Last Name]**, **[!UICONTROL Email Address]**, kopiera och klistra in **[!UICONTROL Registration code]** från e-postmeddelandet i formuläret och klicka på **[!UICONTROL Next]**.

   ![](assets/enter-your-information-hands.png)

   >[!TIP]
   >
   >Om installationen misslyckas bör du kontakta din IT-avdelning för att kontrollera att HTTPS-trafik inte blockeras. Installationsprogrammet kräver att HTTPS-trafik är öppen.

1. Klicka på **[!UICONTROL Next]** om du vill installera på standardplatsen.

   ![](assets/select-installation-folder-hand.png)

1. Klicka på **[!UICONTROL Next]**.

   ![](assets/confirm-installation-hand.png)

   >[!NOTE]
   >
   >Om du får en säkerhetsfråga om en okänd utgivare klickar du på **[!UICONTROL Yes]**.

1. Installationen är nu klar, klicka på **[!UICONTROL Close]**.

   ![](assets/image2014-9-23-15-3a52-3a11.png)

1. Öppna [!DNL Microsoft Outlook] och se Marketo-knapparna.

   ![](assets/image2016-8-24-15-3a47-3a38.png)

   Underbar! Nu är Marketo-knapparna på ett bättre ställe.

Läs mer om hur du använder åtgärderna Marketo Message and Log With Marketo.

>[!MORELIKETHIS]
>
>* [Skicka och spåra ett e-postmeddelande med Marketo-tillägget för e-post för Outlook](/help/marketo/product-docs/marketo-sales-insight/msi-outlook-plugin/send-and-track-an-email-with-the-email-add-in-for-outlook.md){target="_blank"}
>* [Skicka och spåra från Outlook med en Marketo-mall](/help/marketo/product-docs/marketo-sales-insight/msi-outlook-plugin/send-and-track-from-outlook-using-a-marketo-template.md){target="_blank"}
