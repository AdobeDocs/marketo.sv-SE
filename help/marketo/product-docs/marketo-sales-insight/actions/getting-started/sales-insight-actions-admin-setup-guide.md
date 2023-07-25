---
description: Sales Insight Actions Admin Setup Guide - Marketo Docs - produktdokumentation
title: Handbok för administration av Sales Insight Actions
exl-id: 339d518d-445b-4634-ab81-92c9d5541927
feature: Sales Insight Actions
source-git-commit: 02b2e39580c5eac63de4b4b7fdaf2a835fdd4ba5
workflow-type: tm+mt
source-wordcount: '660'
ht-degree: 0%

---

# Handbok för administration av Sales Insight Actions {#sales-insight-actions-admin-setup-guide}

>[!NOTE]
>
>Marketo Sales Insight Actions är ett webbaserat program som integreras med Salesforce-användargränssnittet via [Marketo Sales Insight-paket](/help/marketo/product-docs/marketo-sales-insight/msi-for-salesforce/installation/install-marketo-sales-insight-package-in-salesforce-appexchange.md){target="_blank"}. Det kallas ibland&quot;Marketo Sales&quot; eller&quot;Actions&quot;.

>[!PREREQUISITES]
>
>* Bekräfta med kontoteamet (din kontohanterare) på Adobe att MSI-åtgärder har aktiverats för ditt Marketo Engage-konto (om du inte har någon kontohanterare kontaktar du [Marketo Support](https://nation.marketo.com/t5/support/ct-p/Support){target="_blank"}).
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

   ![](assets/msi-actions-admin-guide-1.png)

   >[!NOTE]
   >
   >Om du inte ser ett klient-ID och klienthemlighet på integreringsinformationskortet aktiverar du åtgärdsinstansen genom att bjuda in den första användaren, så visas klient-ID och klienthemlighet.

1. Klicka **Försäljningsinsikter** sedan **Åtgärdskonfiguration**. Välj i en lista över Marketo-administratörer som du vill bjuda in och klicka på **Skicka inbjudan**.

   ![](assets/msi-actions-admin-guide-2.png)

Användaren får ett e-postmeddelande med steg för att få åtkomst till kontot.

>[!NOTE]
>
>Ytterligare användare läggs inte till via Marketo utan läggs i stället till via sidan Användarhantering för försäljningskonto. [Klicka här](/help/marketo/product-docs/marketo-sales-connect/admin/invite-users.md){target="_blank"} om du vill veta mer om hur du lägger till fler användare.

## Anslut Marketo-försäljningskonto till Salesforce {#connect-marketo-sales-account-to-salesforce}

1. Klicka på kugghjulsikonen på ditt Marketo-konto och välj **Inställningar**.

   ![](assets/msi-actions-admin-guide-3.png)

1. Under Administratörsinställningar klickar du på **Salesforce**.

   ![](assets/msi-actions-admin-guide-4.png)

1. Klicka på fliken Anslutningar och anpassningar **Anslut**.

   ![](assets/msi-actions-admin-guide-5.png)

1. Klicka **OK**.

   ![](assets/msi-actions-admin-guide-6.png)

Om du redan är inloggad i Salesforce är du ansluten. Annars blir du ombedd att logga in.

## Anslut Marketo till ditt konto för säljappar {#connect-marketo-to-your-sales-apps-account}

1. Klicka på kugghjulsikonen på ditt Marketo-konto och välj **Inställningar**.

   ![](assets/msi-actions-admin-guide-7.png)

1. Under Administratörsinställningar klickar du på **Marketo**.

   ![](assets/msi-actions-admin-guide-8.png)

1. Klicka **koppla**. Ditt konto ansluts då.

   ![](assets/msi-actions-admin-guide-9.png)

>[!NOTE]
>
>Om det inte ansluter kopierar du inloggningsuppgifterna från fliken Åtgärder i Marketo Sales Insight och klistrar in dem på fliken Konfigurera.

## Initiera datasynkronisering {#initiate-data-sync}

Synkroniseringen av datafält för Sales Insight Actions gör att systemet kan hämta personinformation från din Marketo Engage-databas till din Sales Insight Actions-databas, hålla persondata uppdaterade och se till att aktiviteter loggas till rätt poster i Marketo och Salesforce.

>[!CAUTION]
>
>När du har initierat datasynkronisering bör du **not** ta bort den ursprungliga användaren från din instans av Sales Insight Actions. Det här är användaren som den första inbjudan skickades till.

1. I Marketo klickar du på **Administratör**.

   ![](assets/msi-actions-admin-guide-10.png)

1. Klicka **Försäljningsinsikter**.

   ![](assets/msi-actions-admin-guide-11.png)

1. Klicka på **Åtgärdskonfiguration** -fliken. Klicka på Synkroniseringskortet för åtgärdsfält **Synkronisera**.

   ![](assets/msi-actions-admin-guide-12.png)

1. En förhandsgranskning av fälten som ska synkroniseras visas. Klicka **Starta synkronisering**.

   ![](assets/msi-actions-admin-guide-13.png)

Personposter som finns i Marketo och Salesforce synkroniseras med ditt Marketo Sales Apps-konto.

>[!NOTE]
>
>Läs mer om hur människor och aktivitetsdata synkroniseras mellan Sales Insight Actions, Marketo och Salesforce. [klicka här](/help/marketo/product-docs/marketo-sales-insight/actions/admin/sync-sales-action-data-with-marketo-and-salesforce.md){target="_blank"}.

## Bjud in enskilda användare till MSI-åtgärder {#invite-individual-users-to-msi-actions}

1. Klicka på kugghjulsikonen på ditt Marketo-konto och välj **Inställningar**.

   ![](assets/msi-actions-admin-guide-14.png)

1. Under Administratörsinställningar väljer du **Användarhantering**.

   ![](assets/msi-actions-admin-guide-15.png)

1. Klicka **Åtgärder** och markera **Bjud in användare**.

   ![](assets/msi-actions-admin-guide-16.png)

1. Ange e-postadress(er) och klicka på **Bjud in**.

   ![](assets/msi-actions-admin-guide-17.png)

>[!NOTE]
>
>Som standard läggs alla nya medlemmar till i gruppen Alla.

Du får ett bekräftelsemeddelande.

## Bjud in användare via CSV till MSI-åtgärder {#invite-users-via-csv-to-msi-actions}

1. Klicka på kugghjulsikonen på ditt Marketo-konto och välj **Inställningar**.

   ![](assets/msi-actions-admin-guide-18.png)

1. Under Administratörsinställningar väljer du **Användarhantering**.

   ![](assets/msi-actions-admin-guide-19.png)

1. Klicka **Åtgärder** och markera **Bjud in användare via CSV**.

   ![](assets/msi-actions-admin-guide-20.png)

1. Bläddra efter CSV-filen på datorn, markera den och klicka på **Nästa**.

   ![](assets/msi-actions-admin-guide-21.png)

1. Bekräfta att fälten är korrekt mappade och klicka på **Bjud in**.

   ![](assets/msi-actions-admin-guide-22.png)

Du får ett bekräftelsemeddelande när inbjudningarna har skickats.

>[!NOTE]
>
>När detta är klart kan du antingen uppgradera ditt befintliga MSI-paket eller installera ett nytt och gå vidare till [konfigurera MSI-åtgärder i Salesforce](/help/marketo/product-docs/marketo-sales-insight/actions/crm/salesforce-package-configuration/sales-insight-actions-configuration-in-salesforce.md){target="_blank"}.
