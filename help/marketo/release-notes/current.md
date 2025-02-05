---
description: Aktuell versionsinformation – Marketo Docs – Produktdokumentation
title: Aktuell versionsinformation
exl-id: a2eccad5-73ad-48f9-8091-51cee23824e1
feature: Release Information
source-git-commit: 6f2c91d31b1d2ea3f2977aa3c9b1ca40e5459a16
workflow-type: tm+mt
source-wordcount: '551'
ht-degree: 2%

---

# Versionsinformation: januari 2025 {#release-notes-jan-25}

Här nedan hittar du alla funktioner som ingår i versionen från 25 januari. Se om det finns funktioner i Adobe Marketo Engage Edition.

Versionsinformationen för Adobe Dynamic Chat [ finns här](/help/marketo/release-notes/dynamic-chat.md){target="_blank"}.

>[!AVAILABILITY]
>
>Funktioner som anges av en stjärna (![stjärna](assets/yellow-star.png)) är betalda tillägg. Kontakta din Marketo Engage-representant om du vill veta mer.

## Standardfunktioner för lanseringscykel {#standard-release-cycle-features}

Följande funktioner ingår i standardversionscykeln och kommer att släppas den **17 januari 2025**, med en fasad utrullning av återstående funktioner under de följande veckorna. Versionsfunktioner och datum kan komma att ändras. Kontrollera status bredvid varje funktion.

<table style="table-layout:auto"> 
 <tbody> 
  <tr> 
   <th style="width:65%">Funktion</th> 
   <th style="width:10%">Status</th>
   <th style="width:25%">Dokumentation</th>
  </tr>
    <tr> 
   <td><strong>Ny e-post för Designer</strong>: Skapa moderna och effektiva e-postmeddelanden med den nya inbyggda e-postadressen Designer i Marketo Engage. Få tillgång till någon av de färdiga e-postmallarna som är färdiga att användas, eller skapa enkelt en egen. Använd dynamiskt innehåll och få tillgång till bilder från Adobe Experience Manager molntjänster. Använd Content Accelerator Gen-AI-funktionaliteten för att skapa innovativa och högpresterande e-postmeddelanden i stor skala.
   <p><img src="assets/note-icon.png" alt="anteckningsikon"> Obs! Din Marketo Engage-prenumeration måste migreras till <a href="https://experienceleague.adobe.com/en/docs/marketo/using/product-docs/administration/marketo-with-adobe-identity/adobe-identity-management-overview">Adobe Identity Management System (IMS)</a> för att du ska kunna komma åt den nya e-postdesignern. Om du inte har gjort det än och vill begära att det ska gå fort kontaktar du kontoteamet (din kontoansvarige) på Adobe eller <a href="https://nation.marketo.com/t5/support/ct-p/Support">Marketo support</a>. Kontakta Adobe Account Team för att få tillgång till funktionerna för Gen-AI i Content Accelerator.</td>
   <td>Levererat</td>
   <td><a href="/help/marketo/product-docs/email-marketing/email-designer/overview.md">E-posta Designer - översikt</a></td>
  </tr>
  <tr> 
   <td> </td> 
   <td> </td>
   <td> </td>
  </tr>
  <tr> 
   <td><strong>Avregistrera registranter från en händelse i interaktiva webbinarier</strong>: Om du inte vill ha någon registrant i webbinariet av någon anledning kan du avregistrera dem. Arbetsflödet tar bort både registranten från Marketo och Adobe Connect.</td> 
   <td><i>Kommer snart</i></td>
   <td><i>Kommer snart</i></td>
  </tr>
  <tr> 
   <td> </td> 
   <td> </td>
   <td> </td>
  </tr>
  <tr> 
   <td><strong>Inaktivera kampanjer i arkiv</strong>: Inaktivera aktiva utlösarkampanjer och avbryt alla schemalagda batchkörningar av kampanjer i en mapp när den arkiveras. Eftersom det finns en extra behörighetskontroll för att arkivera mappar som innehåller aktiva kampanjer (Aktivera utlösarkampanj och Schemalägg batchkampanj), inaktiveras den här funktionen som standard i den här versionen och kan aktiveras genom att gå till <b>Admin</b> &gt; <b>Treasure Chest</b> i din Marketo Engage-prenumeration.</td> 
   <td><i>Kommer snart</i></td>
   <td><i>Kommer snart</i></td>
  </tr>
 </tbody> 
</table>
<br/>

## Meddelanden {#announcements}

* **Borttagning av sociala funktioner**: Onsdagen den 31 juli 2024 började Marketo Engage ta bort följande sociala funktioner i produkten:

   * Omröstningar
   * Knappen Socialt
   * Värvningserbjudande
   * Videodelning
   * Dragningar

Sedan dess har man inte kunnat skapa, klona eller bädda in någon av dessa sociala funktioner i Marketo Engage. Befintliga sociala tillgångar fortsätter att fungera fram till 31 januari 2025. Den 1 februari 2025 upphör sociala tillgångar att fungera. Sociala funktioner inbäddade i landningssidor måste tas bort. [Läs mer](https://nation.marketo.com/t5/employee-blogs/marketo-engage-social-features-deprecation/ba-p/351977){target="_blank"}

* **Hämta API-uppdatering för programmedlemmar**: Vi har förbättrat API:t [Hämta programmedlemmar](https://experienceleague.adobe.com/en/docs/marketo-developer/marketo/rest/lead-database/program-members#query){target="_blank"} så att det går att hämta programmedlemmens identifierare. Detta gör du genom att lägga till id i listan med fält som anges i parametern fields i API-begäran.

* **Resten av API:t &#39;access_token&#39;-parametern har tagits bort**: Frågeparametern `access_token` som används för att autentisera Marketo REST API-anrop har tagits bort och är inte tillgänglig efter den 30 juni 2025. Alla nya och befintliga integreringar ska autentisera REST API-anrop med rubriken Authorization, [, vilket beskrivs här](https://experienceleague.adobe.com/en/docs/marketo-developer/marketo/rest/authentication){target="_blank"}.

* **SOAP API-borttagning**: Stödet för Marketo SOAP API upphör 31 oktober 2025. Tjänster som använder SOAP API-funktioner ska migreras till [REST API](https://experienceleague.adobe.com/en/docs/marketo-developer/marketo/rest/rest-api){target="_blank"}.
