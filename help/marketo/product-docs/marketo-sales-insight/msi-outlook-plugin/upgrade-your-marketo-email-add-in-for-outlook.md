---
unique-page-id: 2949279
description: Uppgradera ditt Marketo-e-posttillägg för Outlook - Marketo Docs - Produktdokumentation
title: Uppgradera ditt Marketo-e-posttillägg för Outlook
exl-id: 079f1142-8062-448c-aa07-59ecd89a718f
source-git-commit: 72e1d29347bd5b77107da1e9c30169cb6490c432
workflow-type: tm+mt
source-wordcount: '405'
ht-degree: 5%

---

# Uppgradera ditt Marketo-e-posttillägg för Outlook {#upgrade-your-marketo-email-add-in-for-outlook}

När det finns en ny version av Marketo-tillägget för e-post för Outlook följer du dessa anvisningar för att uppgradera.

>[!NOTE]
>
>Från och med 10/1/20 har den senaste versionen av Outlook-plugin inte längre stöd för offlineläge. Detta börjar gälla efter installation/uppgradering på eller efter 10/1.

## Hämta installationsprogram {#download-installer}

Hämta det installationsprogram som är lämpligt för din version av Microsoft Outlook.

<table> 
 <colgroup> 
  <col> 
  <col> 
  <col> 
  <col> 
  <col> 
 </colgroup> 
 <tbody> 
  <tr> 
   <th><br></th> 
   <th colspan="2">Installation av inbjudan till en användare</th> 
   <th colspan="2">Installation av företagsnyckel</th> 
  </tr> 
  <tr> 
   <td><strong>Outlook-version</strong></td> 
   <td><strong>32-bitars</strong></td> 
   <td><strong>64-bitars</strong></td> 
   <td><strong>32-bitars</strong></td> 
   <td><strong>64-bitars</strong></td> 
  </tr> 
  <tr> 
   <td>Outlook 2000</td> 
   <td>Stöds inte</td> 
   <td>Ej tillämpligt</td> 
   <td>Stöds inte</td> 
   <td>Ej tillämpligt</td> 
  </tr> 
  <tr> 
   <td>Outlook 2003</td> 
   <td><a href="https://munchkin.marketo.net/MarketoAddInSetup32.msi" rel="nofollow">Ladda ned</a></td> 
   <td>Ej tillämpligt</td> 
   <td>Stöds inte</td> 
   <td>Ej tillämpligt</td> 
  </tr> 
  <tr> 
   <td>Outlook 2007</td> 
   <td><a href="https://munchkin.marketo.net/MarketoAddInSetup32.msi" rel="nofollow">Ladda ned</a></td> 
   <td>Ej tillämpligt</td> 
   <td>Stöds inte</td> 
   <td>Ej tillämpligt</td> 
  </tr> 
  <tr> 
   <td>Outlook 2010</td> 
   <td><a href="https://munchkin.marketo.net/MarketoAddInSetup32.msi" rel="nofollow">Ladda ned</a></td> 
   <td><a href="https://munchkin.marketo.net/MarketoAddInSetup64.msi" rel="nofollow">Ladda ned</a></td> 
   <td><a href="https://munchkin.marketo.net/MarketoAddInSetup32.msi" rel="nofollow">Ladda ned</a></td> 
   <td><a href="https://munchkin.marketo.net/MarketoAddInSetup64.msi" rel="nofollow">Ladda ned</a></td> 
  </tr> 
  <tr> 
   <td>Outlook 2013</td> 
   <td><a href="https://munchkin.marketo.net/MarketoAddInSetup32.msi" rel="nofollow">Ladda ned</a></td> 
   <td><a href="https://munchkin.marketo.net/MarketoAddInSetup64.msi" rel="nofollow">Ladda ned</a></td> 
   <td><a href="https://munchkin.marketo.net/MarketoAddInSetup32.msi" rel="nofollow">Ladda ned</a></td> 
   <td><a href="https://munchkin.marketo.net/MarketoAddInSetup64.msi" rel="nofollow">Ladda ned</a></td> 
  </tr> 
  <tr> 
   <td>Outlook 2016</td> 
   <td><a href="https://munchkin.marketo.net/MarketoAddInSetup32.msi" rel="nofollow">Ladda ned</a></td> 
   <td><a href="https://munchkin.marketo.net/MarketoAddInSetup64.msi" rel="nofollow">Ladda ned</a></td> 
   <td><a href="https://munchkin.marketo.net/MarketoAddInSetup32.msi" rel="nofollow">Ladda ned</a></td> 
   <td><a href="https://munchkin.marketo.net/MarketoAddInSetup64.msi" rel="nofollow">Ladda ned</a></td> 
  </tr> 
  <tr> 
   <td colspan="1">Outlook 2019</td> 
   <td colspan="1"><a href="https://munchkin.marketo.net/MarketoAddInSetup32.msi" rel="nofollow">Ladda ned</a></td> 
   <td colspan="1"><a href="https://munchkin.marketo.net/MarketoAddInSetup64.msi" rel="nofollow">Ladda ned</a></td> 
   <td colspan="1"><a href="https://munchkin.marketo.net/MarketoAddInSetup32.msi" rel="nofollow">Ladda ned</a></td> 
   <td colspan="1"><a href="https://munchkin.marketo.net/MarketoAddInSetup64.msi" rel="nofollow">Ladda ned</a></td> 
  </tr> 
  <tr> 
   <td>Outlook för Mac</td> 
   <td>Stöds inte</td> 
   <td>Stöds inte</td> 
   <td>Stöds inte</td> 
   <td>Stöds inte</td> 
  </tr> 
  <tr> 
   <td colspan="1">Outlook Web App</td> 
   <td colspan="1">Stöds inte</td> 
   <td colspan="1">Stöds inte</td> 
   <td colspan="1">Stöds inte</td> 
   <td colspan="1">Stöds inte</td> 
  </tr> 
  <tr> 
   <td colspan="1">Office 365*</td> 
   <td colspan="1"><a href="https://munchkin.marketo.net/MarketoAddInSetup32.msi" rel="nofollow">Ladda ned</a></td> 
   <td colspan="1"><a href="https://munchkin.marketo.net/MarketoAddInSetup64.msi" rel="nofollow">Ladda ned</a></td> 
   <td colspan="1"><a href="https://munchkin.marketo.net/MarketoAddInSetup32.msi" rel="nofollow">Ladda ned</a></td> 
   <td colspan="1"><a href="https://munchkin.marketo.net/MarketoAddInSetup64.msi" rel="nofollow">Ladda ned</a></td> 
  </tr> 
 </tbody> 
</table>

&#42;Office 365-version: Endast Windows-klient (i Windows 10, Enterprise eller Pro).

## Uppgradera {#upgrade}

1. Identifiera [Microsoft Outlook-version](https://support.microsoft.com/en-us/office/what-version-of-outlook-do-i-have-b3a9568c-edb5-42b9-9825-d48d82b2257c?ui=en-us&amp;rs=en-us&amp;ad=us).

1. Välj version i listan ovan.

1. Kör installationsprogrammet.

   ![](assets/image2014-9-23-16-3a53-3a56.png)

1. Klicka **Nästa**.

   ![](assets/image2014-9-23-16-3a54-3a8.png)

   >[!NOTE]
   >
   >I vissa fall saknas uppgifterna. Kopiera den från registreringsmeddelandet och stäng sedan Outlook.

1. Stäng Microsoft Outlook.

   ![](assets/ent-key-close-outlook-hand.png)

1. Du kommer att lägga märke till att all information är förifylld. Klicka bara **Nästa**.

   ![](assets/image2014-9-23-16-3a54-3a40.png)

   >[!TIP]
   >
   >Om installationen misslyckas bör du samarbeta med din IT-avdelning för att säkerställa att HTTPS-trafik inte blockeras. Installationsprogrammet kräver att HTTPS-trafik är öppen.

1. Klicka **Nästa** för att installera på standardplatsen.

   ![](assets/image2014-9-23-16-3a54-3a55.png)

1. Klicka **Nästa**.

   ![](assets/image2014-9-23-16-3a55-3a20.png)

1. Installationen har slutförts. Klicka **Stäng**.

   ![](assets/image2014-9-23-16-3a55-3a34.png)

1. Öppna nu Microsoft Outlook för att se den senaste versionen av Marketo-knapparna.

   ![](assets/image2016-8-24-15-3a47-3a38.png)

>[!MORELIKETHIS]
>
>* [Skicka och spåra ett e-postmeddelande med Marketo e-posttillägg för Outlook](/help/marketo/product-docs/marketo-sales-insight/msi-outlook-plugin/send-and-track-an-email-with-the-email-add-in-for-outlook.md)
>* [Skicka och spåra från Outlook med en Marketo-mall](/help/marketo/product-docs/marketo-sales-insight/msi-outlook-plugin/send-and-track-from-outlook-using-a-marketo-template.md)

