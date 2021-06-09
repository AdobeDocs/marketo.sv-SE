---
description: Konfigurera Sales Insight för ditt team - Marketo Docs - produktdokumentation
title: Konfigurera Sales Insight för ditt team
exl-id: 269f9093-f530-4e3b-aac7-e317976cf0f0
source-git-commit: ecceb1a3aff3a2088379f8f4f2ac33e566f90e21
workflow-type: tm+mt
source-wordcount: '416'
ht-degree: 0%

---

# Konfigurera Sales Insight för ditt team {#setting-up-sales-insight-for-your-team}

Så här skapar du en profil med tillgång till Sales Insight och tar bort åtkomsten till dina andra profiler. Detta är till för användare som redan har installerat [Sales Insight AppExchange-paketet](/help/marketo/product-docs/marketo-sales-insight/msi-for-salesforce/installation/install-marketo-sales-insight-package-in-salesforce-appexchange.md).

## Skapa en ny profil för Sales Insight {#create-a-new-profile-for-sales-insight}

Om du har en dedikerad profil för dina Sales Insight-användare kan du hoppa över det här steget.

1. Gå till sidan Inställningar i Salesforce.

1. Sök efter profiler i Snabbsökning och välj alternativet **Profil**.

1. Klicka på knappen **Ny profil** överst på sidan.

1. Välj en profil att klona och ge den ett namn (t.ex.: Sales Insight User).

1. Klicka på **Spara** när du är klar.

## Lägg till försäljningsinsiderbehörigheter {#add-sales-insight-permissions}

1. Gå tillbaka till din profillista.

1. Klicka på länken **Redigera** för den nya profilen som du just skapade (eller för någon annan befintlig profil som du vill ge Sales Insight åtkomst till).

1. På redigeringssidan måste du ändra några inställningar.

   **För profiler som har åtkomst till Sales Insight**:

   * Ändra Marketo-flikarna till Standard på i flikinställningarna
   * I Anpassade objektbehörigheter markerar du Läs, Skapa, Redigera och Ta bort på Marketo Sales Insight Config (om användaren ska ha tillgång till konfigurationsinställningarna, som vanligtvis används för administratörer)

   **För profiler som inte tillåts åtkomst till Sales Insight**:

   * Ändra Marketo-flikarna till Dold flik i Tabbinställningar
   * Avmarkera Läs, Skapa, Redigera och Ta bort i konfigurationen för Marketo Sales Insight i Anpassade objektbehörigheter


1. Klicka på **Spara** när du är klar.

## Skapa layout för Sales Insight {#create-layout-for-sales-insight}

1. Gå till sidan Inställningar och klicka sedan på **Appinställningar** > **Anpassa** > **Leads** > **Sidlayouter**. Klicka sedan på knappen **Nytt**.

1. Klona layouten och ge layouten ett passande namn (t.ex.: Sales Insight Layout).

1. Klicka på **Spara** när du är klar.

1. Upprepa dessa steg för sidlayouterna Kontakter, Affärsmöjligheter och Konton.

## Tilldela profil till layout {#assign-profile-to-layout}

1. Gå tillbaka till avsnittet Sidlayouter och klicka på knappen **Sidlayoutuppdrag**.

1. Välj **Redigera uppdrag**.

1. Välj din Sales Insight-profil i listan och välj sedan din layout för säljinsikter i listrutan Välj sidlayout.

1. Klicka på **Spara** när du är klar.

1. Upprepa dessa steg för sidlayouterna Kontakter, Affärsmöjligheter och Konton.

## Andra ändringar {#other-changes}

Här är några andra ställen där Sales Insight-artiklar kan visas. Du måste ta bort dem direkt eftersom du inte kan använda profiler för att begränsa deras åtkomst:

* Ta bort Säljannonser från söklayouter för kontakter, leads och konton
* Ta bort kolumner för försäljningsinsikter från kontaktlistor och leadlistor
