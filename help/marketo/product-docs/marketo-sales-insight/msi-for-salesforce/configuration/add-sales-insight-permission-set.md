---
description: Lägg till behörighetsuppsättning för Sales Insight - Marketo Docs - produktdokumentation
title: Lägg till behörighetsuppsättning för försäljningsinsikter
hide: true
hidefromtoc: true
source-git-commit: 2ac0ef0b715eb2acd03fe2c5ad4cfee8daeef4f6
workflow-type: tm+mt
source-wordcount: '386'
ht-degree: 0%

---

# Lägg till behörighetsuppsättning för försäljningsinsikter {#add-sales-insight-permission-set}

Följ de här stegen för att lägga till åtkomst till Sales Insight-funktioner i Salesforce. Gäller för Salesforce Classic och Lightning

>[!PREREQUISITES]
>
>[Uppdatera ditt Sales Insight Salesforce-paket](/help/marketo/product-docs/marketo-sales-insight/msi-for-salesforce/upgrading/upgrading-your-msi-package.md){target=&quot;_blank&quot;} till version 1.8000 eller senare om du vill använda den här funktionen.

>[!IMPORTANT]
>
>Om du tidigare har gett Sales Insight tillgång till alla profiler och/eller implementerat Sales Insight för alla användare, måste du [ta bort åtkomst på profilnivå](/help/marketo/product-docs/marketo-sales-insight/msi-for-salesforce/configuration/remove-sales-insight-access.md){target=&quot;_blank&quot;} om du vill använda den här behörighetsgruppen.

## Översikt {#overview}

&quot;Marketo App&quot;-behörighet ingår i Salesforce-paketet Sales Insight. Den ger åtkomst till nedanstående objekt, API-klasser och visualforce-sidor. Dessa krävs för att få tillgång till alla funktioner i Sales Insight.

**Objektinställningar**

<table> 
 <tbody> 
 <tr> 
   <td>BestBetsCache</td> 
   <td>Läs, skapa, redigera, ta bort, visa alla, ändra alla</td> 
  </tr> 
  <tr> 
   <td>Visningsdetaljer för bästa val</td> 
   <td>Läs, skapa, redigera, ta bort, visa alla, ändra alla</td> 
  </tr> 
  <tr> 
   <td>Vyer för bästa val</td> 
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
   <td>Marketo Sales Insight Config</td> 
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

* Åtkomst till Apex-klass: 159 Apex-klasser som är med &quot;mkto_si&quot;
* Visualforce-sidåtkomst: 64 Visualforce-sidor som är med &quot;mkto_si&quot;
* Definitioner av anpassade inställningar: mkto_si.Marketo Settings &amp; mkto_si.User Preferences

## Lägga till Marketo App-behörighetsuppsättning till användare {#adding-marketo-app-permission-set-to-users}

1. Logga in på ditt Salesforce-konto.

PICC

1. Klicka **Inställningar**.

PICC

1. Under Administratör klickar du för att ta bort **Hantera användare** sedan **Användare**.

PICC

1. Under Alla användare väljer du den användare som du vill ge åtkomst till och klickar sedan på **Tilldelningar för behörighetsuppsättning**.

PICC

1. Klicka **Redigera uppdrag**.

PICC

1. Välj **Marketo App Access** från de tillgängliga behörighetsgrupperna, och **Lägg till**. Klicka **Spara**.

PICC

1. När du rullar nedåt på sidan Användarinformation visas Marketo App Access under Tilldelningar av behörighetsuppsättningar.

PICC

>[!NOTE]
>
>Användare som inte har tillgång till Sales Insight ser det här meddelandet: &quot;Du har inte behörighet att komma åt den här fliken.&quot;

Nu räcker det! Du har lagt till Sales Insight-åtkomst. Upprepa samma steg för alla andra profiler som du vill lägga till åtkomst för.
