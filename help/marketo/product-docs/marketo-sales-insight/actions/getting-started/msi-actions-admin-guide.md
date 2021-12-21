---
description: MSI Actions Admin Guide - Marketo Docs - produktdokumentation
title: Administratörshandbok för MSI-åtgärder
hide: true
hidefromtoc: true
source-git-commit: 9ee07611ffae25fea4bffa3124927083bf187ddd
workflow-type: tm+mt
source-wordcount: '509'
ht-degree: 0%

---

# Administratörshandbok för MSI-åtgärder {#msi-actions-admin-guide}

>[!PREREQUISITES]
>
>* Bekräfta med din Customer Success Manager att MSI-åtgärder har aktiverats för ditt Marketo-konto (om du inte har någon CSM, vänligen [kontakta supporten](https://nation.marketo.com/t5/support/ct-p/Support)).
>* Din Marketo/Salesforce-synkronisering måste vara konfigurerad.


<table>
 <tr>
  <th>Persona</th>
  <th>Steg</th>
 </tr>
 <tr>
  <td>Marketo Admin</td>
  <td>Ställ in Marketo-försäljningskonto</td>
 </tr>
 <tr>
  <td>Marketo Admin eller <br/>Salesforce-administratör</td>
  <td>Anslut Marketo-försäljningskonto till Salesforce</td>
 </tr>
 <tr>
  <td>Marketo Admin</td>
  <td>Anslut Marketo-försäljningskonto till Marketo</td>
 </tr>
 <tr>
  <td>Marketo Admin</td>
  <td>Initiera datasynkronisering från Marketo till Marketo försäljningskonto</td>
 </tr>
 <tr>
  <td>Marketo Admin</td>
  <td>Bjud in användare till MSI-Actions</td>
 </tr>
 <tr>
  <td>Salesforce-administratör</td>
  <td>Installera/uppgradera MSI-paket i Salesforce</td>
 </tr>
 <tr>
  <td>Salesforce-administratör</td>
  <td>Konfigurera MSI-åtgärder i Salesforce</td>
 </tr>
</table>

## Ställ in Marketo försäljningskonto {#set-up-marketo-sales-account}

1. I Marketo klickar du på **Administratör**.

PICC

1. Klicka **Försäljningsinsikter** sedan **Åtgärdskonfiguration**. Välj i en lista över Marketo-administratörer som du vill bjuda in och klicka på **Skicka inbjudan**.

PICC

Användaren får ett e-postmeddelande med steg för att få åtkomst till kontot.

>[!NOTE]
>
>Ytterligare användare läggs inte till via Marketo utan läggs i stället till via sidan Användarhantering för försäljningskonto. [Klicka här](/help/marketo/product-docs/marketo-sales-connect/admin/invite-users.md) om du vill veta mer om hur du lägger till fler användare.

## Anslut Marketo-försäljningskonto till Salesforce {#connect-marketo-sales-account-to-salesforce}

1. Klicka på kugghjulsikonen på ditt Marketo-konto och välj **Inställningar**.

PICC

1. Under Administratörsinställningar klickar du på **Salesforce**.

PICC

1. Klicka på fliken Anslutningar och anpassningar **Anslut**.

PICC

1. Klicka **OK**.

PICC

Om du redan är inloggad i Salesforce är du ansluten. Om du inte gör det blir du ombedd att logga in.

## Anslut Marketo till ditt konto för säljappar {#connect-marketo-to-your-sales-apps-account}

1. Klicka på kugghjulsikonen på ditt Marketo-konto och välj **Inställningar**.

PICC

1. Under Administratörsinställningar klickar du på **Marketo**.

PICC

1. Klicka **koppla**. Ditt konto ansluts då.

>[!NOTE]
>
>Om det inte ansluter kopierar du inloggningsuppgifterna från fliken Åtgärder i Marketo Sales Insight och klistrar in dem på fliken Konfigurera.

## Initiera datasynkronisering {#initiate-data-sync}

1. I Marketo klickar du på Admin.

PICC

1. Klicka på Sales Insight och sedan på Actions Config.

PICC

1. Klicka på Synkroniseringskortet för åtgärdsfält **Synkronisera**.

PICC

1. En förhandsgranskning av fälten som ska synkroniseras visas. Klicka **Starta synkronisering**.

PICC

Personposter som finns i Marketo och Salesforce synkroniseras med ditt Marketo Sales Apps-konto.

## Bjud in enskilda användare till MSI-åtgärder {#invite-individual-users-to-msi-actions}

1. Klicka på kugghjulsikonen på ditt Marketo-konto och välj **Inställningar**.

PICC

1. Under Administratörsinställningar väljer du **Användarhantering**.

PICC

1. Klicka **Åtgärder** och markera **Bjud in användare**.

PICC

1. Ange e-postadress(er) och klicka på **Bjud in**.

>[!NOTE]
>
>Som standard läggs alla nya medlemmar till i gruppen Alla.

Du får ett bekräftelsemeddelande.

## Bjud in användare via CSV till MSI-åtgärder {#invite-users-via-csv-to-msi-actions}

1. Klicka på kugghjulsikonen på ditt Marketo-konto och välj **Inställningar**.

PICC

1. Under Administratörsinställningar väljer du **Användarhantering**.

PICC

1. Klicka **Åtgärder** och markera **Bjud in användare via CSV**.

PICC

1. Bläddra efter CSV-filen på datorn, markera den och klicka på **Nästa**.

PICC

1. Bekräfta att fälten är korrekt mappade och klicka på **Bjud in**.

PICC

Du får ett bekräftelsemeddelande när inbjudningarna har skickats.

>[!NOTE]
>
>När detta är klart kan du antingen uppgradera ditt befintliga MSI-paket eller installera ett nytt och gå vidare till [konfigurera MSI-åtgärder i Salesforce](/help/marketo/product-docs/marketo-sales-insight/actions/salesforce-configuration/msi-actions-configuration-in-salesforce.md).
