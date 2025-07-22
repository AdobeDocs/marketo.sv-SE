---
unique-page-id: 10099389
description: Marketo Plugin-versioner för  [!DNL Microsoft Dynamics] - Marketo Docs - produktdokumentation
title: Marketo Plugin-versioner för  [!DNL Microsoft Dynamics]
exl-id: c9c25e11-bcf7-49bf-920a-4182af27d278
feature: Microsoft Dynamics
source-git-commit: 0d37fbdb7d08901458c1744dc68893e155176327
workflow-type: tm+mt
source-wordcount: '457'
ht-degree: 0%

---

# Marketo Plugin-versioner för [!DNL Microsoft Dynamics] {#marketo-plugin-releases-for-microsoft-dynamics}

När du först synkroniserar till [!DNL Microsoft Dynamics] hämtar du den senaste versionen av plugin-programmen för Marketo. Marketo uppdaterar regelbundet dessa plugin-program så att du kan gå tillbaka till samma ställe och ladda ned den nya versionen.

[Hämta det senaste plugin-programmet ](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/download-the-marketo-lead-management-solution.md) som motsvarar din [!DNL Dynamics]-version.

![](assets/marketo-plugin-releases-for-microsoft-dynamics-1.png)

## Uppdaterar din [!DNL Dynamics]-lösning {#updating-your-dynamics-solution}

1. Importera den senaste versionen av lösningen till den befintliga versionen av din [!DNL Dynamics] CRM (t.ex. om din [!DNL Dynamics] CRM har version 1.4 och den senaste versionen är 1.5 importerar du _över_ version 1.4).

1. Följande popup-fönster visas. Välj **Uppdatera** och **Behåll anpassningar** och klicka sedan på **Importera**.

![](assets/marketo-plugin-releases-for-microsoft-dynamics-2.png)

## Senaste versioner {#latest-versions}

>[!NOTE]
>
>De här versionerna fungerar för både lokala versioner och onlineversioner av [!DNL Dynamics].

<table> 
 <tbody> 
  <tr> 
   <th style="width:15%">Version</th> 
   <th style="width:20%">Releasedatum</th> 
   <th style="width:65%">Anteckningar</th> 
  </tr>
  <tr> 
   <td>5.0.2.1</td> 
   <td>1/19/24</td> 
   <td>Felkorrigering: Felkorrigerade fel relaterade till den anpassade entitetssynkroniseringen.</td> 
  </tr> 
  <tr> 
   <td>5.0.2.0</td> 
   <td>03/24/23</td> 
   <td>Felkorrigering: Korrigerade fel som förhindrade att kontakter på MS Dynamics slogs samman.</td> 
  </tr> 
  <tr> 
   <td colspan="1">4.2.0.0</td> 
   <td colspan="1">10/16/20</td> 
   <td colspan="1">Stöd för kampanjsynkronisering med MS [!DNL Dynamics] har lagts till.</td> 
  </tr> 
  <tr> 
   <td colspan="1">4.0.0.24</td> 
   <td colspan="1">8/22/18</td> 
   <td colspan="1">Stöd har lagts till för att leda till kontaktprocess för [!DNL Microsoft Dynamics] version 9.x.</td> 
  </tr> 
  <tr> 
   <td colspan="1">4.0.0.23</td> 
   <td colspan="1">6/27/18</td> 
   <td colspan="1">Felkorrigering: Affärsprocessfel vid försök att installera Marketo Solutions för [!DNL Dynamics] 2013.</td> 
  </tr> 
  <tr> 
   <td>4.0.0.24</td> 
   <td>8/22/18</td> 
   <td>Extra stöd för färdiga produkter ger rätt till kontaktprocess för Microsoft Dynamics version 9.x.</td> 
  </tr> 
  <tr> 
   <td colspan="1"><p>4.0.0.21</p></td> 
   <td colspan="1">11/9/16</td> 
   <td colspan="1">Felkorrigering: Plugin-programmet prenumererade inte på händelser som fångar statusändringen för det anpassade objektet. Den här korrigeringen är specifik för [!DNL Dynamics] CRM On Premise 2011. </td> 
  </tr> 
  <tr> 
   <td>4.0.0.22</td> 
   <td>9/29/17</td> 
   <td>Felkorrigering: Intern revision.</td> 
  </tr> 
  <tr> 
   <td><p>4.0.0.21</p></td> 
   <td>11/9/16</td> 
   <td>Felkorrigering: Plugin-programmet prenumererade inte på händelser som fångar statusändringen för det anpassade objektet. Den här korrigeringen är specifik för Dynamics CRM On Premise 2011.</td> 
  </tr> 
  <tr> 
   <td>4.0.0.20</td> 
   <td>7/22/16</td> 
   <td>Felkorrigering: Uppdateringar av kontaktrollen för affärsmöjlighet hämtades inte fullständigt.</td> 
  </tr> 
  <tr> 
   <td>4.0.0.19</td> 
   <td>6/28/16</td> 
   <td>Felkorrigering: En onödig uppdateringstransaktion för kundaffärsmöjlighetsrollen i marknadsföringsloggen noterades när affärsmöjligheten skapades.<p>Felkorrigering: En extra borttagningstransaktion loggades när kundens affärsmöjlighetsroll togs bort.</td> 
  </tr> 
  <tr> 
   <td>4.0.0.18</td> 
   <td>5/31/16</td> 
   <td>Felkorrigering: Uppdateringen och borttagningen av anpassade objekt har gjorts asynkron.</td> 
  </tr> 
  <tr> 
   <td>4.0.0.17</td> 
   <td>4/8/16</td> 
   <td>Felkorrigering: När leadet hade ett synkroniseringsfilter inställt på NO, och affärsmöjligheten och kontakten inte hade något synkroniseringsfilter, genererades inte Skapa logg för kontakten och affärsmöjligheten när leadet kvalificerades.</td> 
  </tr> 
  <tr> 
   <td>4.0.0.16</td> 
   <td>3/29/16</td> 
   <td>Felkorrigering: En tilldelningshändelse loggades när synkroniseringsfiltret stängdes av.</td> 
  </tr> 
  <tr> 
   <td>4.0.0.15</td> 
   <td>3/3/16</td> 
   <td>Felkorrigering: Kunden kunde inte skapa ett lead i CRM eftersom inloggningsanvändaren inte har Marketo Config-behörighet.</td> 
  </tr> 
  <tr> 
   <td colspan="1">4.0.0.14</td> 
   <td colspan="1">1/18/16</td> 
   <td colspan="1">Felkorrigering: Åtkomstbegränsningar för vanliga [!DNL Dynamics]-användare har skapats för att åtgärda säkerhetsproblem.</td> 
  </tr> 
  <tr> 
   <td colspan="1">4.0.0.13</td> 
   <td colspan="1">12/30/15</td> 
   <td>Felkorrigering: Uppdateringar i [!DNL Dynamics] synkroniserades inte till Marketo för steg och bilder.</td> 
  </tr> 
  <tr> 
   <td>4.0.0.12</td> 
   <td>11/12/15</td> 
   <td>Felkorrigering: Leadposter synkroniserades till Marketo när synkroniseringsfiltret var inställt på false.</td> 
  </tr> 
 </tbody> 
</table>

>[!MORELIKETHIS]
>
>[Hämta Marketo Lead Management Solution](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/download-the-marketo-lead-management-solution.md){target="_blank"}
