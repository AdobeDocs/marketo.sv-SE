---
description: Versionsinformation - oktober 2022 - Marketo Docs - produktdokumentation
title: Versionsinformation - oktober 2022
exl-id: 1494b8b9-049c-4969-ab95-a4be41d886b0
feature: Release Information
source-git-commit: 26573c20c411208e5a01aa7ec73a97e7208b35d5
workflow-type: tm+mt
source-wordcount: '603'
ht-degree: 5%

---

# Versionsinformation: oktober 2022 {#release-notes-oct-22}

Här nedan hittar du alla funktioner som ingår i versionen från 22 oktober. Se om det finns funktioner i Adobe Marketo Engage Edition.

>[!AVAILABILITY]
>
>Funktioner som anges av en stjärna (![stjärna](assets/yellow-star.png)) är betalda tillägg. Kontakta Marketo Engage om du vill veta mer.

## Standardfunktioner för lanseringscykel {#standard-release-cycle-features}

Följande funktioner ingår i standardversionscykeln och kommer att släppas den **14 oktober 2022**, med en fasad utrullning av återstående funktioner under de följande veckorna. Versionsfunktioner och datum kan komma att ändras. Kontrollera status för respektive funktion nedan.

### Marknadsföringsdatamiljö {#marketing-data-environment}

</br>

* **Synkronisering av anpassade fält för programmedlem**: Möjlighet att dubbelriktat synkronisera utökningsbara fält som har hämtats för en programmedlem (t.ex. deltagarinställningar under händelseregistrering som mat, sessioner, spår osv.) med fält för kampanjmedlem i Salesforce.

<table>
  <tr>
   <td><b>Status</b></td>
   <td><b>Dokumentationsuppdateringar</b></td>
  </tr>
  <tr>
   <td>Levererat</td>
   <td><a href="/help/marketo/product-docs/core-marketo-concepts/programs/working-with-programs/program-member-custom-field-sync.md">Synkronisering av anpassat fält för programmedlem</a></td>
  </tr>
  </tbody>
</table>

* **Adobe Privacy Service-integrering**: Harmonisera med Privacy Service för att automatisera kompatibiliteten med dataintegritetsregler för alla Experience Cloud-produkter. För närvarande är den här tjänsten endast tillgänglig för Marketo Engage-kunder som har anslutit sig till Adobe Identity Management System.

<table>
  <tr>
   <td><b>Status</b></td>
   <td><b>Dokumentationsuppdateringar</b></td>
  </tr>
  <tr>
   <td>Levererat</td>
   <td><a href="/help/marketo/product-docs/administration/marketo-with-adobe-identity/adobe-identity-management-overview.md">Adobe Identity Management</a></td>
  </tr>
  </tbody>
</table>

### Nästa generations upplevelser {#modern-ux}

</br>

* **Uppdaterade Screens i nästa generations upplevelse**: Vi levererar nya, uppdaterade skärmar i nästa generations upplevelser som erbjuder uppdaterade design- och användarvänlighetsförbättringar som är tillgängliga via växlingsfunktion:

   * Information om landningssidmall
   * E-postmallslista

<table>
  <tr>
   <td><b>Status</b></td>
   <td><b>Dokumentationsuppdateringar</b></td>
  </tr>
  <tr>
   <td>Levererat</td>
   <td><a href="/help/marketo/product-docs/marketo-engage-modern-ux/toggle-switch.md">Växla av/på</a></td>
  </tr>
  </tbody>
</table>

* **Förbättrad användning per flik i Information om e-postmall**: I den nya versionen visas ytterligare information om resurser som använder e-postmallen, inklusive Resursstatus, Senast ändrad och Senast ändrad av. Du kan också söka efter, sortera och filtrera listan som används av resurser.

<table>
  <tr>
   <td><b>Status</b></td>
   <td><b>Dokumentationsuppdateringar</b></td>
  </tr>
  <tr>
   <td>Levererat</td>
   <td>n/a</td>
  </tr>
  </tbody>
</table>

* **Rapportera resursfiltermoduler**: Ny design för rapportkonfigurationsmoduler som visar ett nytt resursträd på konfigurationsmenyn och ett filter för Skapad och ändrad den.

<table>
  <tr>
   <td><b>Status</b></td>
   <td><b>Dokumentationsuppdateringar</b></td>
  </tr>
  <tr>
   <td>Levererat</td>
   <td>n/a</td>
  </tr>
  </tbody>
</table>

### API-förbättringar {#api-enhancements}

</br>

* **Masslead-import: Salesperson-association**: Paritet med lead REST API för att kunna associera leads med säljare under bulklead-importprocessen, vilket minskar komplexiteten och antalet API-anrop som krävs.

<table>
  <tr>
   <td><b>Status</b></td>
   <td><b>Dokumentationsuppdateringar</b></td>
  </tr>
  <tr>
   <td>Levererat</td>
   <td><a href="https://developer.adobe.com/marketo-apis/api/mapi/#tag/Bulk-Import-Leads">Import av massutr</a></td>
  </tr>
  </tbody>
</table>

### Försäljningsinsikter {#sales-insight}

</br>

![(stjärna)](assets/yellow-star.png)

* **Sales Insight Integration with Dynamic Chat**: Insights Dashboard innehåller nu Dynamic Chat-aktiviteter i det smarta rutnätet tillsammans med en sammanfattning och detaljerade kort varje vecka.

<table>
  <tr>
   <td><b>Status</b></td>
   <td><b>Dokumentationsuppdateringar</b></td>
  </tr>
  <tr>
   <td>Levererat</td>
   <td><a href="/help/marketo/product-docs/marketo-sales-insight/msi-for-salesforce/features/dynamic-chat-integration.md">Dynamic Chat Integration</a></td>
  </tr>
  </tbody>
</table>

## Agile Release-funktioner

Följande funktioner följer ett Agile-format och släpps på olika datum före eller efter standardreleasedatum. Kontrollera status för respektive funktion nedan.

* **Dialogrutorna Ordna automatiskt strömmar för Dynamic Chat**: Förbättra arbetsytan i din fullmatade dialog genom att ordna allt på arbetsytan i ett rent och lättläst format med en knapptryckning genom att ordna automatiskt.

<table>
  <tr>
   <td><b>Status</b></td>
   <td><b>Dokumentationsuppdateringar</b></td>
  </tr>
  <tr>
   <td>Levererat</td>
   <td><a href="/help/marketo/product-docs/demand-generation/dynamic-chat/automated-chat/stream-designer.md#stream-designer-icons">Strömma Designer-ikoner</a></td>
  </tr>
  </tbody>
</table>

* **Möteslänkar för Dynamic Chat**: Möjlighet att automatiskt inkludera en Teams- eller Meet-länk för Google och Outlook i varje kalenderinbjudan som skickas till besökare.

<table>
  <tr>
   <td><b>Status</b></td>
   <td><b>Dokumentationsuppdateringar</b></td>
  </tr>
  <tr>
   <td>Levererat</td>
   <td><a href="/help/marketo/product-docs/demand-generation/dynamic-chat/setup-and-configuration/agent-settings.md">Kalender</a></td>
  </tr>
  </tbody>
</table>

* **Stöd för ytterligare datatyper för Dynamic Chat**: Tre nya datatyper (boolesk, heltal, flyttal) gör att du kan utnyttja fler befintliga Marketo Engage-fält i Dynamic Chat för saker som målanpassning baserat på poängen eller fråga besökarna ja/nej-frågor.

<table>
  <tr>
   <td><b>Status</b></td>
   <td><b>Dokumentationsuppdateringar</b></td>
  </tr>
  <tr>
   <td>Levererat</td>
   <td>n/a</td>
  </tr>
  </tbody>
</table>

## Meddelanden {#announcements}

* **Forms 1.0**: Borttagningen av Forms 1.0 slutförs i oktober-versionen. Forms 1.0-mediefiler kan inte längre skicka data till Marketo Engage och returnerar fel vid försök.

* **Forms utan skript**: Forms fungerar inte längre när JavaScript är inaktiverat i webbläsaren. Formulärinlämning kräver att Javascript är aktiverat.
