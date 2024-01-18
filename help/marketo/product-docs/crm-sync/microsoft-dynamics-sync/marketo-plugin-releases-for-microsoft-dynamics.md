---
unique-page-id: 10099389
description: Marketo Plugin Releases for Microsoft Dynamics - Marketo Docs - Produktdokumentation
title: Marketo Plugin Releases for Microsoft Dynamics
exl-id: c9c25e11-bcf7-49bf-920a-4182af27d278
feature: Microsoft Dynamics
source-git-commit: e99fa6d25bcf3c4a03234ce48dd17dd7c396c430
workflow-type: tm+mt
source-wordcount: '464'
ht-degree: 0%

---

# Marketo Plugin Releases for Microsoft Dynamics {#marketo-plugin-releases-for-microsoft-dynamics}

När du först synkroniserar till Microsoft Dynamics hämtar du den senaste versionen av plugin-programmen för Marketo. Marketo uppdaterar regelbundet dessa plugin-program så att du kan gå tillbaka till samma ställe och ladda ned den nya versionen.

[Ladda ned det senaste plugin-programmet](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/download-the-marketo-lead-management-solution.md){target="_blank"} motsvarar din Dynamics-release.

![](assets/marketo-plugin-releases-for-microsoft-dynamics-1.png)

## Uppdaterar Dynamics-lösningen {#updating-your-dynamics-solution}

1. Importera den senaste versionen av lösningen till den befintliga versionen av Dynamics CRM (t.ex. om Dynamics CRM har version 1.4 och den senaste versionen är 1.5) importerar du _över_ version 1.4).

1. Följande popup-fönster visas. Välj **Uppdatera** och **Underhåll anpassningar** och sedan klicka **Importera**.

![](assets/marketo-plugin-releases-for-microsoft-dynamics-2.png)

## Senaste versioner {#latest-versions}

>[!NOTE]
>
>Dessa versioner fungerar både lokalt och online för Dynamics.

<table> 
 <tbody> 
  <tr> 
   <th colspan="1">Version</th> 
   <th colspan="1">Releasedatum</th> 
   <th>Anteckningar</th> 
  </tr>
  <tr> 
   <td colspan="1">5.0.2.1</td> 
   <td colspan="1">10/13/23</td> 
   <td colspan="1">Felkorrigering: Felkorrigerade fel relaterade till den anpassade entitetssynkroniseringen.</td> 
  </tr> 
  <tr> 
   <td colspan="1">5.0.2.0</td> 
   <td colspan="1">03/24/23</td> 
   <td colspan="1">Felkorrigering: Korrigerade fel som förhindrade att kontakter på MS Dynamics slogs samman.</td> 
  </tr> 
  <tr> 
   <td colspan="1">5.0.1.8</td> 
   <td colspan="1">03/27/23</td> 
   <td colspan="1">Felkorrigering: Förhindrar att plugin-programmet skriver över andra anpassningar av gränssnittselementen i MS Dynamics.</td> 
  </tr> 
  <tr> 
   <td colspan="1">5.0.1.1</td> 
   <td colspan="1">02/04/21</td> 
   <td colspan="1">Stöd för synkronisering av flervalsalternativuppsättningsfält (den här funktionen är endast tillgänglig för V9.X och senare).</td> 
  </tr> 
  <tr> 
   <td colspan="1">4.2.0.0</td> 
   <td colspan="1">10/16/20</td> 
   <td colspan="1">Stöd för kampanjsynkronisering med MS Dynamics har lagts till.</td> 
  </tr> 
  <tr> 
   <td colspan="1">4.0.0.24</td> 
   <td colspan="1">8/22/18</td> 
   <td colspan="1">Stöd för körklara lösningar berättigar till kontaktprocess för Microsoft Dynamics version 9.x.</td> 
  </tr> 
  <tr> 
   <td colspan="1">4.0.0.23</td> 
   <td colspan="1">6/27/18</td> 
   <td colspan="1">Felkorrigering: Affärsprocessfel vid försök att installera Marketo Solutions för Dynamics 2013.</td> 
  </tr> 
  <tr> 
   <td colspan="1">4.0.0.22</td> 
   <td colspan="1">9/29/17</td> 
   <td colspan="1">Felkorrigering: Intern revision.</td> 
  </tr> 
  <tr> 
   <td colspan="1"><p>4.0.0.21</p></td> 
   <td colspan="1">11/9/16</td> 
   <td colspan="1">Felkorrigering: Plugin-programmet prenumererade inte på händelser som fångar statusändringen för det anpassade objektet. Den här korrigeringen är specifik för Dynamics CRM On Premise 2011.</td> 
  </tr> 
  <tr> 
   <td colspan="1">4.0.0.20</td> 
   <td colspan="1">7/22/16</td> 
   <td colspan="1">Felkorrigering: Uppdateringar av kontaktrollen för affärsmöjlighet hämtades inte fullständigt.</td> 
  </tr> 
  <tr> 
   <td colspan="1">4.0.0.19</td> 
   <td colspan="1">6/28/16</td> 
   <td colspan="1">Felkorrigering: En onödig uppdateringstransaktion för kundaffärsmöjlighetsrollen i marknadsföringsloggen noterades när affärsmöjligheten skapades.<p>Felkorrigering: En extra borttagningstransaktion loggades när kundens affärsmöjlighetsroll togs bort.</td> 
  </tr> 
  <tr> 
   <td colspan="1">4.0.0.18</td> 
   <td colspan="1">5/31/16</td> 
   <td colspan="1">Felkorrigering: Uppdateringen och borttagningen av anpassade objekt har gjorts asynkron.</td> 
  </tr> 
  <tr> 
   <td colspan="1">4.0.0.17</td> 
   <td colspan="1">4/8/16</td> 
   <td colspan="1">Felkorrigering: När leadet hade ett synkroniseringsfilter inställt på NO, och affärsmöjligheten och kontakten inte hade något synkroniseringsfilter, genererades inte Skapa logg för kontakten och affärsmöjligheten när leadet kvalificerades.</td> 
  </tr> 
  <tr> 
   <td colspan="1">4.0.0.16</td> 
   <td colspan="1">3/29/16</td> 
   <td>Felkorrigering: En tilldelningshändelse loggades när synkroniseringsfiltret stängdes av.</td> 
  </tr> 
  <tr> 
   <td colspan="1">4.0.0.15</td> 
   <td colspan="1">3/3/16</td> 
   <td colspan="1">Felkorrigering: Kunden kunde inte skapa ett lead i CRM eftersom inloggningsanvändaren inte har Marketo Config-behörighet.</td> 
  </tr> 
  <tr> 
   <td colspan="1">4.0.0.14</td> 
   <td colspan="1">1/18/16</td> 
   <td colspan="1">Felkorrigering: Åtkomstbegränsningar för normala Dynamics-användare har skapats för att åtgärda säkerhetsproblem.</td> 
  </tr> 
  <tr> 
   <td colspan="1">4.0.0.13</td> 
   <td colspan="1">12/30/15</td> 
   <td>Felkorrigering: Uppdateringar i Dynamics synkroniserades inte till Marketo för steg och bilder.</td> 
  </tr> 
  <tr> 
   <td colspan="1">4.0.0.12</td> 
   <td colspan="1">11/12/15</td> 
   <td colspan="1">Felkorrigering: Leadposter synkroniserades till Marketo när synkroniseringsfiltret var inställt på false.</td> 
  </tr> 
 </tbody> 
</table>

>[!MORELIKETHIS]
>
>[Ladda ned Marketo Lead Management Solution](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/download-the-marketo-lead-management-solution.md){target="_blank"}
