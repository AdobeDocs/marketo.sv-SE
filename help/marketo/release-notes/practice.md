---
description: Practice Release Notes - Marketo Docs - produktdokumentation
title: Versionsinformation
hide: true
hidefromtoc: true
exl-id: e1004c31-8b8c-4bc7-845f-4e06644a3273
source-git-commit: d6d8674ef3357cef1b388a43baade1c57ed98e3e
workflow-type: tm+mt
source-wordcount: '602'
ht-degree: 1%

---

# Versionsinformation: Oktober 2022 {#release-notes-oct-22}

Här nedan hittar du alla funktioner som ingår i versionen från 22 oktober. Se om det finns funktioner i din Adobe Marketo Engage-utgåva.

>[!AVAILABILITY]
>
>Funktioner som anges av en stjärna (![stjärna](assets/yellow-star.png)) är betalda tillägg. Kontakta din Marketo Engage-representant om du vill veta mer.

Följande funktioner kommer att lanseras den **14 oktober 2022**, med en stegvis utrullning av återstående funktioner under de följande veckorna (om inget annat anges). Versionsfunktionerna och de exakta datumen kan komma att ändras.

## Flerkanalsmarknadsföring {#cross-channel-orchestration}

_**Dynamiskt chatt**_

* **Ordna dialogströmmar automatiskt för dynamiskt chatt**: Förbättra arbetsytan i den fullmatade dialogen genom att ordna allt på arbetsytan i ett rent och lättläst format med en knapptryckning genom att ordna automatiskt.

* **Stöd för ytterligare datatyper för Dynamic Chat**: Tre nya datatyper (boolesk, heltal, flytande) gör att du kan utnyttja fler befintliga fält i Dynamic Chat för t.ex. målgruppsanpassning baserat på poängen eller fråga besökarna ja/nej-frågor.

* **Möteslänkar för dynamisk chatt**: Möjlighet att automatiskt inkludera en Teams- eller Meet-länk för Google och Outlook i varje kalenderinbjudan som skickas till besökarna.

* **Schemalagda mötesmeddelanden för dynamiskt chatt**: Säljare får automatiska e-postmeddelanden om schemalagda möten samt all relevant information om besökarens chatbot-interaktion.

* **Roller och behörigheter för dynamisk chatt**: Administratörer kan använda detaljerade behörigheter för att styra programmets synlighet och användning och skapa anpassade användarroller.

   * Fullständig åtkomst - användarna kan utnyttja funktionen fullt ut (t.ex. publicera dialogrutor, ändra färgschema etc.)
   * Skrivskyddad åtkomst - användare kan se information men inte göra ändringar (se t.ex. Målkriterier eller Direktuppspelning, men inte ändra)
   * Begränsad åtkomst - användarna kan inte se eller komma åt avsnitten Konfiguration eller Integrering

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

## Nästa generations upplevelser {#next-generation-experience}

* **Uppdaterade skärmar i nästa generation**: Vi levererar nya, uppdaterade skärmar i nästa generation av upplevelser som erbjuder uppdaterade design- och användarvänlighetsförbättringar som är tillgängliga via växlingsfunktion:

   * Information om landningssidmall
   * E-postmallslista

<table> 
  <tr> 
   <td><b>Status</b></td>
   <td><b>Dokumentationsuppdateringar</b></td>
  </tr>
  <tr> 
   <td>Levererat</td>
   <td><a href="/help/marketo/product-docs/marketo-engage-next-generation-experience/toggle-switch.md">Växla av/på</a></td>
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

* **Rapportera resursfiltermoduler**: Ny design för rapportkonfigurationsmoduler som visar ett nytt resursträd på konfigurationsmenyn och ett filter för Skapat och Ändrat den.

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

## Marknadsföringsdatamiljö {#marketing-data-environment}

* **Integrering med Adobe Privacy Service**: Harmonisera med Privacy Service för att automatisera efterlevnaden av datasekretesregler i olika Experience Cloud-produkter. För närvarande är den här tjänsten endast tillgänglig för Marketo Engage som har anslutit sig till Adobe Identity Management System.

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

## API-förbättringar {#api-enhancements}

* **Import av massutr: Säljarassociation**: Paritet med Lead REST API för att kunna koppla leads till säljare under bulkimporten, vilket minskar komplexiteten och antalet API-anrop som krävs.

<table> 
  <tr> 
   <td><b>Status</b></td>
   <td><b>Dokumentationsuppdateringar</b></td>
  </tr>
  <tr> 
   <td>Levererat</td>
   <td><a href="https://developers.marketo.com/rest-api/bulk-import/bulk-lead-import/">Import av massutr</a></td>
  </tr>
  </tbody>
</table>

## Försäljningsinsikter {#sales-insight}

![(stjärna)](assets/yellow-star.png)

* **Sales Insight Integration with Dynamic Chat**: Insikter Dashboard innehåller nu Dynamic Chat-aktiviteter i det smarta rutnätet tillsammans med en sammanfattning och detaljerade kort varje vecka.

<table> 
  <tr> 
   <td><b>Status</b></td>
   <td><b>Dokumentationsuppdateringar</b></td>
  </tr>
  <tr> 
   <td>Levererat</td>
   <td><a href="/help/marketo/product-docs/marketo-sales-insight/msi-for-salesforce/features/dynamic-chat-integration.md">Dynamisk chattintegrering</a></td>
  </tr>
  </tbody>
</table>

## Meddelanden {#announcements}

* **Forms 1.0**: Borttagningen av Forms 1.0 slutförs i oktober-versionen. Forms 1.0-mediefiler kan inte längre skicka data till Marketo Engage och returnerar fel vid försök.

* **Forms utan skript**: Forms fungerar inte längre när Javascript är inaktiverat i webbläsaren. Formulärinlämning kräver att Javascript är aktiverat.