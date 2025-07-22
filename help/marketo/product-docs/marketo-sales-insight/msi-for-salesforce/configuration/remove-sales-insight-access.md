---
description: Ta bort Sales Insight Access - Marketo Docs - produktdokumentation
title: Ta bort åtkomst till Sales Insight
exl-id: 3cda112a-524e-469b-a222-c0192b2f5301
feature: Marketo Sales Insights
source-git-commit: 0d37fbdb7d08901458c1744dc68893e155176327
workflow-type: tm+mt
source-wordcount: '329'
ht-degree: 1%

---

# Ta bort [!DNL Sales Insight]-åtkomst {#remove-sales-insight-access}

Följ de här stegen för att ta bort åtkomsten till [!DNL Sales Insight]-funktionerna i [!DNL Salesforce]. Gäller för [!DNL Salesforce] Classic och Lightning.

## Översikt {#overview}

Behörighet till de objekt som nämns nedan, apex-klasser och visualforce-sidor krävs för att få åtkomst till alla [!DNL Sales Insight]-funktioner. Om du tar bort dessa tas åtkomsten till [!DNL Sales Insight] bort.

**Objektinställningar**

<table> 
 <tbody> 
 <tr> 
   <td>BestBetsCache</td> 
   <td>Läs, skapa, redigera, ta bort, visa alla, ändra alla</td> 
  </tr> 
  <tr> 
   <td>[!DNL Best Bets] Visa detaljer</td> 
   <td>Läs, skapa, redigera, ta bort, visa alla, ändra alla</td> 
  </tr> 
  <tr> 
   <td>[!DNL Best Bets] Vyer</td> 
   <td>Läs, skapa, redigera, ta bort, visa alla, ändra alla</td> 
  </tr> 
  <tr> 
   <td>EmailActivityCache</td> 
   <td>Läs, skapa, redigera, ta bort, visa alla, ändra alla</td> 
  </tr> 
  <tr> 
   <td>GetMethodArgus</td> 
   <td>Läs, skapa, redigera, ta bort, visa alla, ändra alla</td> 
  </tr> 
  <tr> 
   <td>GroupWebActivityCache</td> 
   <td>Läs, skapa, redigera, ta bort, visa alla, ändra alla</td> 
  </tr> 
  <tr> 
   <td>IntressantMomentsCache</td> 
   <td>Läs, skapa, redigera, ta bort, visa alla, ändra alla</td> 
  </tr> 
  <tr> 
   <td>[!DNL Marketo Sales Insight] Konfig</td> 
   <td>Läs, skapa, redigera, ta bort, visa alla, ändra alla</td> 
  </tr> 
  <tr> 
   <td>ScoringCache</td> 
   <td>Läs, skapa, redigera, ta bort, visa alla, ändra alla</td> 
  </tr> 
  <tr> 
   <td>Värden</td> 
   <td>Läs, skapa, redigera, ta bort, visa alla, ändra alla</td> 
  </tr> 
  <tr> 
   <td>WebActivityCache</td> 
   <td>Läs, skapa, redigera, ta bort, visa alla, ändra alla</td> 
  </tr> 
 </tbody> 
</table>

* Apex-klassåtkomst: 159 Apex-klasser som börjar med &quot;mkto_si&quot;
* Visualforce-sidåtkomst: 64 Visualforce-sidor som börjar med &quot;mkto_si&quot;
* Definitioner av anpassade inställningar: mkto_si.Marketo Settings &amp; mkto_si.User Preferences

## Tar bort åtkomst till [!DNL Sales Insight] {#removing-access-to-sales-insight}

1. Logga in på ditt [!DNL Salesforce]-konto.

1. Klicka på **[!UICONTROL Setup]**.

   ![](assets/remove-sales-insight-access-1.png)

1. Klicka på [!UICONTROL Administrator] under **[!UICONTROL Manage Users]** och sedan på **[!UICONTROL Profiles]**.

1. Klicka på den profil som du vill uppdatera och sedan **[!UICONTROL Edit]**.

1. Bläddra ned till [!UICONTROL Custom Tab Settings] under [!UICONTROL Tab Settings].

1. Välj alternativet [!UICONTROL Tab Hidden] i listrutan för [!DNL Marketo Sales Insight] Config- och MSI [!DNL Marketo Sales]-utkorg.

   ![](assets/remove-sales-insight-access-2.png)

   ![](assets/remove-sales-insight-access-3.png)

1. Bläddra ned till [!UICONTROL Custom Object Permissions].

1. Ta bort&quot;Läs, Skapa, Redigera, Ta bort&quot;-åtkomst från följande objekt:

   * BestBetsCache
   * [!DNL Best Bets] Visa detaljer
   * [!DNL Best Bets] vyer
   * EmailActivityCache
   * GetMethodArgus
   * GroupWebActivityCache
   * IntressantMomentsCache
   * Konfiguration för [!DNL Marketo Sales Insight]
   * ScoringCache
   * Värden
   * WebActivityCache

1. Bläddra ned till avsnittet [!UICONTROL Enabled Apex Class Access]. Klicka på **[!UICONTROL Edit]**.

1. I avsnittet [!UICONTROL Enabled Apex Classes] väljer du alla klasser som börjar med mkto_si. Detta bör innehålla upp till 159 klasser.

1. Klicka på **[!UICONTROL Remove]** och sedan på **[!UICONTROL Save]**.

   ![](assets/remove-sales-insight-access-4.png)

1. Bläddra ned till avsnittet [!UICONTROL Enabled Visualforce Page Access]. Klicka på **[!UICONTROL Edit]**.

1. I avsnittet [!UICONTROL Enabled Visualforce Pages] markerar du alla sidor som börjar med mkto_si. Detta bör innehålla upp till 64 sidor.

1. Klicka på **[!UICONTROL Remove]** och sedan på **[!UICONTROL Save]**.

   ![](assets/remove-sales-insight-access-5.png)

1. Bläddra ned till avsnittet [!UICONTROL Enabled Custom Setting Definitions Access]. Klicka på **[!UICONTROL Edit]**.

1. Välj&quot;Marketo Sales Insight.mkto_si.Marketo Settings&quot; och&quot;Marketo Sales Insight.mkto_si.User Preferences&quot;.

1. Klicka på **[!UICONTROL Remove]** och sedan på **[!UICONTROL Save]**.

   ![](assets/remove-sales-insight-access-6.png)

Nu räcker det! Du har tagit bort [!DNL Sales Insight]-åtkomst. Upprepa samma steg för alla andra profiler som du vill ta bort åtkomst till.
