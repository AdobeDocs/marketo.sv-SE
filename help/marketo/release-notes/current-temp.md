---
description: Aktuell versionsinformation – Marketo Docs – Produktdokumentation
title: Aktuell versionsinformation
hide: true
hidefromtoc: true
feature: Release Information
source-git-commit: 7ec3687c0c16738805394377b2080295c2f18032
workflow-type: tm+mt
source-wordcount: '304'
ht-degree: 2%

---

# Versionsinformation: maj 2025 {#release-notes-may-25}

Här nedan hittar du alla funktioner som ingår i versionen från maj 25. Se om det finns funktioner i Adobe Marketo Engage Edition.

Versionsinformationen för Adobe Dynamic Chat [finns här](/help/marketo/release-notes/dynamic-chat.md){target="_blank"}.

>[!AVAILABILITY]
>
>Funktioner som anges av en stjärna (![stjärna](assets/yellow-star.png)) är betalda tillägg. Kontakta Marketo Engage om du vill veta mer.

## Standardfunktioner för lanseringscykel {#standard-release-cycle-features}

Följande funktioner ingår i standardversionscykeln och kommer att släppas den **23 maj 2025**, med en fasad utrullning av återstående funktioner under de följande veckorna. Versionsfunktioner och datum kan komma att ändras. Kontrollera status bredvid varje funktion.

<table style="table-layout:auto"> 
 <tbody>
  <tr> 
   <td><strong>Utlösartoken för attribut</strong>: Utökad lista över utlösartokens som kan användas med data från aktivitetsattribut i fält för smarta kampanjer.</td> 
   <td><i>Kommer snart</i></td>
   <td><i>Kommer snart</i></td>
  </tr>
 </tbody> 
</table>
<br/>

## Meddelanden {#announcements}

* **Ny analysfunktion - offentlig Beta**: [Avancerad BI-analys](/help/marketo/product-docs/reporting/advanced-bi-analytics/overview.md){target="_blank"} (kallades tidigare Intäktsutforskaren och avancerad Report Builder) började distribueras till alla nuvarande användare av intäktscykelutforskaren i mitten av april. Det nya verktyget erbjuder ett flexibelt gränssnitt för rapportering och visualisering av data från Marketo Engage, med detaljerad information om utveckling, prestanda och mycket annat. Den har bättre interaktivitet och visualisering, snabbare prestanda och en smidigare och mer intuitiv användarupplevelse.

För att få tillgång till den här funktionen måste du ha köpt tillägget Avancerad BI Analytics. Kontakta Adobe Account Team (din kontoansvarige) för mer information.

* **Resten av API:t &#39;access_token&#39;-parametern har tagits bort**: Frågeparametern `access_token` som används för att autentisera Marketo REST API-anrop har tagits bort och är inte tillgänglig efter den 30 juni 2025. Alla nya och befintliga integreringar ska autentisera REST API-anrop med rubriken Authorization, [, vilket beskrivs här](https://experienceleague.adobe.com/en/docs/marketo-developer/marketo/rest/authentication){target="_blank"}.

* **Borttagning av SOAP API**: Stödet för Marketo SOAP API upphör 31 oktober 2025. Tjänster som använder SOAP API-funktioner bör migreras till [REST API](https://experienceleague.adobe.com/en/docs/marketo-developer/marketo/rest/rest-api){target="_blank"}.
