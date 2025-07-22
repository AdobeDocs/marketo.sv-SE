---
description: Lägg till Sales Insight-åtkomst till profiler - Marketo Docs - produktdokumentation
title: Lägg till åtkomst till profiler för Sales Insight
exl-id: 269f9093-f530-4e3b-aac7-e317976cf0f0
feature: Marketo Sales Insights
source-git-commit: 0d37fbdb7d08901458c1744dc68893e155176327
workflow-type: tm+mt
source-wordcount: '363'
ht-degree: 0%

---

# Lägg till [!DNL Sales Insight]-åtkomst till profiler {#add-sales-insight-access-to-profiles}

Så här skapar du en profil med åtkomst till [!DNL Sales Insight] samtidigt som du tar bort åtkomst för dina andra profiler. Detta gäller användare som redan har installerat [[!DNL Sales Insight] AppExchange-paketet](/help/marketo/product-docs/marketo-sales-insight/msi-for-salesforce/installation/install-marketo-sales-insight-package-in-salesforce-appexchange.md){target="_blank"}.

>[!IMPORTANT]
>
>Om du tidigare har gett [!DNL Sales Insight] åtkomst till alla profiler måste du [ta bort profilnivååtkomst](/help/marketo/product-docs/marketo-sales-insight/msi-for-salesforce/configuration/remove-sales-insight-access.md){target="_blank"} för att kunna använda den här behörighetsgruppen.

## Skapa en ny profil för [!DNL Sales Insight] {#create-a-new-profile-for-sales-insight}

Om du har en dedikerad profil för dina [!DNL Sales Insight]-användare kan du hoppa över det här steget.

1. Gå till sidan Inställningar i [!DNL Salesforce].

1. Sök efter profiler i Snabbsökning och välj alternativet **[!UICONTROL Profile]**.

1. Klicka på knappen **[!UICONTROL New Profile]** överst på sidan.

1. Välj en profil att klona och ge den ett namn (t.ex. Sales Insight User).

1. Klicka på **[!UICONTROL Save]** när du är klar.

## Lägg till [!DNL Sales Insight] behörigheter {#add-sales-insight-permissions}

1. Gå tillbaka till din profillista.

1. Klicka på länken **[!UICONTROL Edit]** för den nya profilen som du nyss skapade (eller för någon annan befintlig profil som du vill ge [!DNL Sales Insight] åtkomst till).

1. På redigeringssidan måste du ändra några inställningar.

   **För profiler som har behörighet till[!DNL Sales Insight]**:

   * Ändra Marketo-flikarna till Standard på i flikinställningarna
   * I Anpassade objektbehörigheter markerar du Läs, Skapa, Redigera och Ta bort på konfigurationen [!DNL Marketo Sales Insight] (om användaren ska ha tillgång till konfigurationsinställningarna, som vanligtvis används för administratörer)

   **För profiler som inte har behörighet till[!DNL Sales Insight]**:

   * Ändra Marketo-flikarna till Dold flik i Tabbinställningar
   * Avmarkera Läs, Skapa, Redigera och Ta bort på konfigurationen [!DNL Marketo Sales Insight] i Anpassade objektbehörigheter

1. Klicka på **[!UICONTROL Save]** när du är klar.

## Skapa layout för [!DNL Sales Insight] {#create-layout-for-sales-insight}

1. Gå till sidan Inställningar och klicka sedan på **[!UICONTROL App Setup]** > **[!UICONTROL Customize]** > **[!UICONTROL Leads]** > **[!UICONTROL Page Layouts]**. Klicka sedan på knappen **[!UICONTROL New]**.

1. Klona layouten och ge layouten ett passande namn (t.ex. Sales Insight Layout).

1. Klicka på **[!UICONTROL Save]** när du är klar.

1. Upprepa dessa steg för sidlayouterna [!UICONTROL Contacts], [!UICONTROL Opportunities] och [!UICONTROL Accounts].

## Tilldela profil till layout {#assign-profile-to-layout}

1. Gå tillbaka till avsnittet Sidlayouter och klicka på knappen **[!UICONTROL Page Layout Assignment]**.

1. Välj **[!UICONTROL Edit Assignment]**.

1. Välj din [!DNL Sales Insight]-profil i listan och välj sedan din [!DNL Sales insight]-layout i listrutan [!UICONTROL Select Page Layout].

1. Klicka på **[!UICONTROL Save]** när du är klar.

1. Upprepa dessa steg för sidlayouterna [!UICONTROL Contacts], [!UICONTROL Opportunities] och [!UICONTROL Accounts].

## Andra ändringar {#other-changes}

Här är några andra platser där [!DNL Sales Insight] objekt kan visas. Du måste ta bort dem direkt eftersom du inte kan använda profiler för att begränsa deras åtkomst:

* Ta bort [!DNL Sales Insight]-knappar från söklayouter för [!UICONTROL Contacts], [!UICONTROL Leads] och [!UICONTROL Accounts]
* Ta bort [!DNL Sales Insight] kolumner från kontakt- och leadlistor
