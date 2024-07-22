---
unique-page-id: 10095429
description: Åtgärda problem med synkronisering av Dynamics-validering - Marketo Docs - produktdokumentation
title: Åtgärda problem med synkronisering av Dynamics-validering
exl-id: 1a300249-65b7-49b1-bf50-82236916298f
feature: Microsoft Dynamics
source-git-commit: 431bd258f9a68bbb9df7acf043085578d3d91b1f
workflow-type: tm+mt
source-wordcount: '487'
ht-degree: 0%

---

# Åtgärda problem med synkronisering av Dynamics-validering {#fix-dynamics-validation-sync-issues}

## Validera resultat för synkroniseringsverktyget {#validate-sync-tool-results}

När du kör Dynamics Validate Sync genereras en rapport. Om det finns en ![x](assets/delete.png) bredvid ett steg, se alternativen nedan för att identifiera och åtgärda problemet. Kör sedan synkroniseringsvalideringsstegen igen tills resultatet visar ingenting annat än gröna bockar.

![](assets/image2015-9-22-15-3a58-3a12.png)

## URL:en är giltig {#url-is-valid}

Om du har en ![x](assets/delete.png) här kontrollerar du att URL:en är giltig. Här hittar du Developer Resources och tittar på Organization Service. URL:en kan vara ogiltig av flera orsaker.

1. Logga in i Dynamics. Klicka på ikonen Inställningar och välj **Avancerade inställningar**.

   ![](assets/one.png)

1. Klicka på Inställningar och välj **Anpassningar**.

   ![](assets/two.png)

1. Klicka på **Utvecklarresurser**.

   ![](assets/three.png)

1. URL:en för organisationstjänsten finns under Tjänstslutpunkter.

   ![](assets/four.png)

## Användarnamn och lösenord är giltiga {#username-and-password-are-valid}

Om du har en ![x](assets/delete.png) här kontrollerar du att dina Microsoft Dynamics-autentiseringsuppgifter är giltiga. För webb-API S2S-autentisering måste användarnamnet i Marketo matcha [e-postadressen](https://docs.microsoft.com/en-us/power-platform/admin/manage-application-users#view-or-edit-the-details-of-an-application-user) för programanvändaren i CRM. För andra typer bör det matcha användarnamnet för Synkronisera användare.

## Synkroniseringsanvändaren har tilldelats användarrollen Marketo Sync {#sync-user-is-assigned-to-the-marketo-sync-user-role}

Om du har en ![x](assets/delete.png) här kan det vara en av de tre frågorna nedan.

**Alternativ ett - Verifiera att användarrollen Marketo Sync är markerad i Microsoft Dynamics**:

1. Klicka på inställningsikonen i Dynamics och välj **Avancerade inställningar**.

   ![](assets/one.png)

1. Klicka på **Inställningar** och välj **Säkerhet**.

   ![](assets/six.png)

1. Klicka på **Användare.**

   ![](assets/image2015-9-24-9-3a47-3a25.png)

1. Klicka på länken för synkroniseringsanvändaren.

   ![](assets/seven.png)

1. Klicka på **Hantera roller**.

   ![](assets/eight.png)

1. Kontrollera att Marketo Sync User-rollen är markerad. Om inte, kontrollera den och klicka på **OK.**

   ![](assets/image2015-9-24-9-3a59-3a21.png)

**Alternativ två - Bekräfta godkännande av beviljande**:

1. Granska [Bevilja samtycke för klient-ID och appregistrering](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/grant-consent-for-client-id-and-app-registration.md) för att bekräfta att appen har administratörsgodkännande för att anropa API:er.

**Alternativ tre - Synkronisera användare**:

1. Kontrollera att Synkronisera användare har lagts till i Marketo Config.

## Marketo-lösningen är korrekt installerad {#marketo-solution-is-properly-installed}

Om du har en ![x](assets/delete.png) här går du till Microsoft Dynamics för att verifiera att Marketo-installationen finns där. Se steg 1 i installationsdokumentationen för Microsoft Dynamics.

1. Klicka på inställningsikonen i Dynamics och välj **Avancerade inställningar**.

   ![](assets/one.png)

1. Klicka på **Inställningar** och välj **Lösningar.**

   ![](assets/eleven.png)

1. Kontrollera att lösningen finns med i listan.

   ![](assets/twelve.png)

## Alla steg i lösningen är aktiverade {#all-steps-in-the-solution-are-enabled}

Om du har ![x](assets/delete.png) här kontrollerar du att inga av standardstegen har inaktiverats. Alla steg aktiveras automatiskt vid installationen, men de kan inaktiveras under en anpassning.

## Synkroniseringsanvändaren har tilldelats Marketo-lösningen {#sync-user-is-assigned-to-the-marketo-solution}

Om du har ![x](assets/delete.png) här kontrollerar du att Synkronisera-användaren är tilldelad till Marketo-standardsidan i Microsoft Dynamics.

1. Klicka på inställningsikonen i Dynamics och välj **Avancerade inställningar**.

   ![](assets/one.png)

1. Klicka på **Inställningar** och välj **Marketo Config**.

   ![](assets/thirteen.png)

1. Kontrollera att synkroniseringsanvändaren är tilldelad som standard.

   ![](assets/fourteen.png)

## Synkronisera användare matchar användarnamn och lösenord {#sync-user-matches-username-and-password}

Om du har en ![x](assets/delete.png) här ska du tilldela rätt synkroniseringsanvändare i fältet Marketo-användare i konfigurationssteget för Marketo i Microsoft Dynamics.

>[!MORELIKETHIS]
>
>[Verifiera Microsoft Dynamics Sync](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/validate-microsoft-dynamics-sync.md)
