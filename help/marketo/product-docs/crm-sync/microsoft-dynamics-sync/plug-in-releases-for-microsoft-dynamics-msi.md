---
unique-page-id: 10099102
description: Plugin-versioner för Microsoft Dynamics MSI - Marketo Docs - produktdokumentation
title: Plugin-versioner för Microsoft Dynamics MSI
exl-id: 830f7dc3-07fd-429b-b0fd-290ffdda88e6
feature: Microsoft Dynamics
source-git-commit: 431bd258f9a68bbb9df7acf043085578d3d91b1f
workflow-type: tm+mt
source-wordcount: '316'
ht-degree: 6%

---

# Plugin-versioner för Microsoft Dynamics MSI {#plug-in-releases-for-microsoft-dynamics-msi}

När du först synkroniserar till Microsoft Dynamics hämtar och installerar du den senaste versionen av plugin-programmen för Marketo Sales Insight (MSI). Marketo uppdaterar regelbundet dessa plugin-program så att du kan gå tillbaka till samma ställe och ladda ned den nya versionen.

Om du använder Marketo inbyggda CRM-synkroniseringslösning för Dynamics, ska du [ladda ned det senaste plugin-programmet](/help/marketo/product-docs/marketo-sales-insight/msi-for-microsoft-dynamics/installing/download-the-marketo-sales-insight-solution-for-microsoft-dynamics.md){target="_blank"} corresponding to your Dynamics release. For those who have a custom sync and have purchased Marketo Sales Insight, the [package is here](https://mktg-cdn.marketo.com/community/MarketoSalesInsight_NonNative.zip){target="_blank"}.

>[!NOTE]
>
>Dessa versioner fungerar både lokalt och online för Dynamics.

## Uppgradera din MSI-lösning {#upgrading-your-msi-solution}

1. Importera den senaste versionen av lösningen _över den befintliga versionen_ i Dynamics CRM genom att trycka på **Importera** i Dynamics.

   ![](assets/plug-in-releases-for-microsoft-dynamics-msi-1.png)

>[!NOTE]
>
>Exempel: om din Dynamics CRM har version 2.0.0.20 och den senaste versionen är 2.0.0.21, ska du importera _över_ version 2.0.0.20.

1. Klicka **Nästa**.

   ![](assets/plug-in-releases-for-microsoft-dynamics-msi-2.png)

1. Välj **Steg för uppgradering** och **Underhåll anpassningar** och sedan klicka **Importera**.

   ![](assets/plug-in-releases-for-microsoft-dynamics-msi-3.png)

1. Klicka **Nästa**.

   ![](assets/plug-in-releases-for-microsoft-dynamics-msi-4.png)

1. Efter en lyckad import ser du två MSI-lösningar: MarketoSalesInsight och MarketoSalesInsight_Upgrade. Välj den äldre lösningen och klicka på Tillämpa uppgradering av lösning.

   ![](assets/plug-in-releases-for-microsoft-dynamics-msi-5.png)

Och det är allt! Efter uppgraderingen visas bara en MSI-lösning.

## Versionsuppdateringar {#version-updates}

<table> 
 <colgroup> 
  <col> 
  <col> 
  <col> 
 </colgroup> 
 <tbody> 
  <tr> 
   <th colspan="1">Releasedatum</th> 
   <th colspan="1">Version</th> 
   <th colspan="1">Anteckningar</th> 
  </tr> 
  <tr> 
   <td colspan="1">02/03/22</td> 
   <td colspan="1">2.0.0.27</td> 
   <td colspan="1">Kontolayout för insikter: Intressanta ögonblick, bakgrundsmusik, webbaktiviteter, e-postaktiviteter</td> 
  </tr>
  <tr> 
   <td colspan="1">01/05/22</td> 
   <td colspan="1">2.0.0.26</td> 
   <td colspan="1">Adobes poäng för e-post</td> 
  </tr>
  <tr> 
   <td colspan="1">10/28/21</td> 
   <td colspan="1">2.0.0.25</td> 
   <td colspan="1">Mätvärden för produktanvändning, ny global instrumentpanel (webbaktivitet, e-post, bästa val)</td> 
  </tr>
  <tr> 
   <td colspan="1">02/10/21</td> 
   <td colspan="1">2.0.0.22</td> 
   <td colspan="1">Ta bort automatisk granskning aktiverad och dokumentera ändringar i MSI-lösningen</td> 
  </tr>
  <tr> 
   <td colspan="1">10/01/20</td> 
   <td colspan="1">2.0.0.21</td> 
   <td colspan="1">Felkorrigering: Tilldela åtkomst till MSI API-konfigurationsfält för användare med rollen Sales Insight</td> 
  </tr> 
  <tr> 
   <td colspan="1">07/20/20</td> 
   <td colspan="1">2.0.0.20</td> 
   <td colspan="1">Felkorrigering: Lägg till ett valideringsmeddelande för osynkroniserade poster</td> 
  </tr> 
  <tr> 
   <td colspan="1">06/12/20</td> 
   <td colspan="1">2.0.0.19</td> 
   <td colspan="1">Felkorrigering: Så här döljer du MSI-hemligt lösenord i MSD API-konfiguration</td> 
  </tr> 
  <tr> 
   <td colspan="1">05/26/20</td> 
   <td colspan="1">2.0.0.18</td> 
   <td colspan="1">Felkorrigering: Så här ändrar du MSI-roll-ID-validering för att visa MSI-knappar</td> 
  </tr> 
  <tr> 
   <td colspan="1">05/21/20</td> 
   <td colspan="1">2.0.0.17</td> 
   <td colspan="1">Felkorrigering: Visa ägarfält och göra fält icke-obligatoriska</td> 
  </tr> 
  <tr> 
   <td colspan="1">04/28/20</td> 
   <td colspan="1">2.0.0.16</td> 
   <td colspan="1">Felkorrigering: Tar bort länkberoende för inställning av platskarta för MSD CRM</td> 
  </tr> 
 </tbody> 
</table>
