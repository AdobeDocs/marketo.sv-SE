---
description: Aktuell versionsinformation - Marketo Docs - produktdokumentation
title: Aktuell versionsinformation
exl-id: a2eccad5-73ad-48f9-8091-51cee23824e1
source-git-commit: 4794c44db57b41f6d9358f7e6cc24a41dda68550
workflow-type: tm+mt
source-wordcount: '582'
ht-degree: 0%

---

# Versionsinformation: Oktober 2022 {#release-notes-oct-22}

Här nedan hittar du alla funktioner som ingår i versionen från 22 oktober. Se om det finns funktioner i din Adobe Marketo Engage-utgåva.

>[!AVAILABILITY]
>
>Funktioner som anges av en stjärna (![stjärna](assets/yellow-star.png)) är betalda tillägg. Kontakta din Marketo Engage-representant om du vill veta mer.

Följande funktioner kommer att lanseras den **14 oktober 2022**, med en stegvis utrullning av återstående funktioner under de följande veckorna (om inget annat anges). Versionsfunktionerna och de exakta datumen kan komma att ändras.

## Flerkanalsmarknadsföring {#cross-channel-orchestration}

* **Ordna dialogströmmar automatiskt för dynamiskt chatt**: Förbättra arbetsytan i den fullmatade dialogen genom att ordna allt på arbetsytan i ett rent och lättläst format med en knapptryckning genom att ordna automatiskt.

* **Stöd för ytterligare datatyper för Dynamic Chat**: Tre nya datatyper (boolesk, heltal, flytande) gör att du kan utnyttja fler befintliga fält i Dynamic Chat för t.ex. målgruppsanpassning baserat på poängen eller fråga besökarna ja/nej-frågor.

* **Möteslänkar för dynamisk chatt**: Möjlighet att automatiskt inkludera en Teams- eller Meet-länk för Google och Outlook i varje kalenderinbjudan som skickas till besökarna.

* **Schemalagda mötesmeddelanden för dynamiskt chatt**: Säljare får automatiska e-postmeddelanden om schemalagda möten samt all relevant information om besökarens chatbot-interaktion.

* **Roller och behörigheter för dynamisk chatt**: Administratörer kan använda detaljerade behörigheter för att styra programmets synlighet och användning och skapa anpassade användarroller.

   * Fullständig åtkomst - användarna kan utnyttja funktionen fullt ut (t.ex. publicera dialogrutor, ändra färgschema etc.)
   * Skrivskyddad åtkomst - användare kan se information men inte göra ändringar (se t.ex. Målkriterier eller Direktuppspelning, men inte ändra)
   * Begränsad åtkomst - användarna kan inte se eller komma åt avsnitten Konfiguration eller Integrering

## Nästa generations upplevelser {#next-generation-experience}

* **Uppdaterade skärmar i nästa generation**: Vi levererar nya, uppdaterade skärmar i nästa generation av upplevelser som erbjuder uppdaterade design- och användarvänlighetsförbättringar som är tillgängliga via växlingsfunktion:

   * Information om landningssidmall
   * E-postmallslista

* **Förbättrad användning per flik i Information om e-postmall**: I den nya versionen visas ytterligare information om resurser som använder e-postmallen, inklusive Resursstatus, Senast ändrad och Senast ändrad av. Du kan också söka efter, sortera och filtrera listan som används av resurser.

* **Rapportera resursfiltermoduler**: Ny design för rapportkonfigurationsmoduler som visar ett nytt resursträd på konfigurationsmenyn och ett filter för Skapat och Ändrat den.

## Marknadsföringsdatamiljö {#marketing-data-environment}

* **Integrering med Adobe Privacy Service**: Harmonisera med Privacy Service för att automatisera efterlevnaden av datasekretesregler i olika Experience Cloud-produkter. För närvarande är den här tjänsten endast tillgänglig för Marketo Engage som har anslutit sig till [Adobe Identity Management](/help/marketo/product-docs/administration/marketo-with-adobe-identity/adobe-identity-management-overview.md){target=&quot;_blank&quot;} System.

* **Synkronisering av anpassade fält för programmedlem**: Möjlighet att dubbelriktat synkronisera utökningsbara fält som tagits emot för en programmedlem (t.ex. deltagarinställningar under händelseregistrering som mat, sessioner, spår osv.)

## API-förbättringar {#api-enhancements}

* **Import av massutr: Säljarassociation**: Paritet med Lead REST API för att kunna koppla leads till säljare under bulkimporten, vilket minskar komplexiteten och antalet API-anrop som krävs.

## Försäljningsinsikter {#sales-insight}

![(stjärna)](assets/yellow-star.png)

* **[Sales Insight Integration with Dynamic Chat](/help/marketo/product-docs/marketo-sales-insight/msi-for-salesforce/features/dynamic-chat-integration.md){target=&quot;_blank&quot;}**: Insikter Dashboard innehåller nu Dynamic Chat-aktiviteter i det smarta rutnätet tillsammans med en sammanfattning och detaljerade kort varje vecka.

## Meddelanden {#announcements}

* **Forms 1.0**: Borttagningen av Forms 1.0 slutförs i oktober-versionen. Forms 1.0-mediefiler kan inte längre skicka data till Marketo Engage och returnerar fel vid försök.

* **Forms utan skript**: Forms fungerar inte längre när Javascript är inaktiverat i webbläsaren. Formulärinlämning kräver att Javascript är aktiverat.
