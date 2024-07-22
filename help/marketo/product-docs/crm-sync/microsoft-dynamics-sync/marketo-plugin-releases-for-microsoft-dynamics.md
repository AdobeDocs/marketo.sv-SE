---
unique-page-id: 10099389
description: Marketo Plugin Releases for Microsoft Dynamics - Marketo Docs - Produktdokumentation
title: Marketo Plugin Releases for Microsoft Dynamics
exl-id: c9c25e11-bcf7-49bf-920a-4182af27d278
feature: Microsoft Dynamics
source-git-commit: f1fd9564abe4702c3a124442ee26027d4d22f23d
workflow-type: tm+mt
source-wordcount: '474'
ht-degree: 0%

---

# Marketo Plugin Releases for Microsoft Dynamics {#marketo-plugin-releases-for-microsoft-dynamics}

När du först synkroniserar till Microsoft Dynamics hämtar du den senaste versionen av plugin-programmen för Marketo. Marketo uppdaterar regelbundet dessa plugin-program så att du kan gå tillbaka till samma ställe och ladda ned den nya versionen.

[Hämta det senaste plugin-programmet](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/download-the-marketo-lead-management-solution.md){target="_blank"} som motsvarar din Dynamics-release.

![](assets/marketo-plugin-releases-for-microsoft-dynamics-1.png)

## Uppdaterar Dynamics-lösningen {#updating-your-dynamics-solution}

1. Importera den senaste versionen av lösningen till den befintliga versionen av Dynamics CRM (t.ex. om Dynamics CRM har version 1.4 och den senaste versionen är 1.5 importerar du _över_ version 1.4).

1. Följande popup-fönster visas. Välj **Uppdatera** och **Behåll anpassningar** och klicka sedan på **Importera**.

![](assets/marketo-plugin-releases-for-microsoft-dynamics-2.png)

## Senaste versioner {#latest-versions}

>[!NOTE]
>
>Dessa versioner fungerar både lokalt och online för Dynamics.

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
   <td>5.0.1.8</td> 
   <td>03/27/23</td> 
   <td>Felkorrigering: Förhindrar att plugin-programmet skriver över andra anpassningar av gränssnittselementen i MS Dynamics.
   <p>
   Felkorrigering: Återgjorda navigeringsrutor som saknas i 5.0.1.1.</td> 
  </tr> 
  <tr> 
   <td>5.0.1.1</td> 
   <td>02/04/21</td> 
   <td>Stöd för synkronisering av flervalsalternativuppsättningsfält (den här funktionen är endast tillgänglig för V9.X och senare).</td> 
  </tr> 
  <tr> 
   <td>4.2.0.0</td> 
   <td>10/16/20</td> 
   <td>Stöd för kampanjsynkronisering med MS Dynamics har lagts till.</td> 
  </tr> 
  <tr> 
   <td>4.0.0.24</td> 
   <td>8/22/18</td> 
   <td>Stöd för körklara lösningar berättigar till kontaktprocess för Microsoft Dynamics version 9.x.</td> 
  </tr> 
  <tr> 
   <td>4.0.0.23</td> 
   <td>6/27/18</td> 
   <td>Felkorrigering: Affärsprocessfel vid försök att installera Marketo Solutions för Dynamics 2013.</td> 
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
   <td>4.0.0.14</td> 
   <td>1/18/16</td> 
   <td>Felkorrigering: Åtkomstbegränsningar för normala Dynamics-användare har skapats för att åtgärda säkerhetsproblem.</td> 
  </tr> 
  <tr> 
   <td>4.0.0.13</td> 
   <td>12/30/15</td> 
   <td>Felkorrigering: Uppdateringar i Dynamics synkroniserades inte till Marketo för steg och bilder.</td> 
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
