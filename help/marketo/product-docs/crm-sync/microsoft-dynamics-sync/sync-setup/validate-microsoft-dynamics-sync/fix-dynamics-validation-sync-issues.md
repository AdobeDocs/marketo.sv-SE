---
unique-page-id: 10095429
description: Åtgärda problem med synkronisering av Dynamics-validering - Marketo Docs - Produktdokumentation
title: Åtgärda problem med synkronisering av Dynamics-validering
translation-type: tm+mt
source-git-commit: 5c9683c6b00ccbf9e9d606fd4513432c9872ad00
workflow-type: tm+mt
source-wordcount: '409'
ht-degree: 0%

---


# Åtgärda problem med synkronisering av Dynamics-validering {#fix-dynamics-validation-sync-issues}

## Validera resultat för synkroniseringsverktyget {#validate-sync-tool-results}

När du kör Dynamics Validate Sync genereras den här rapporten. Om det finns en ![borttagning](assets/delete.png) bredvid ett steg, se nedan för att identifiera och åtgärda problemet. Kör sedan synkroniseringsvalideringsstegen igen tills resultatet inte visar något annat än bockmarkeringar.

![](assets/image2015-9-22-15-3a58-3a12.png)

## URL:en är giltig {#url-is-valid}

Om du har en ![borttagning](assets/delete.png) här kontrollerar du att URL:en är giltig. Här hittar du Developer Resources och tittar på Organization Service. URL:en kan vara ogiltig av flera orsaker.

1. Logga in i Dynamics. Klicka på ikonen Inställningar och välj **Avancerade inställningar**.

   ![](assets/one.png)

1. Klicka på Inställningar och välj **Anpassningar**.

   ![](assets/two.png)

1. Klicka på **Utvecklarresurser**.

   ![](assets/three.png)

1. URL:en för organisationstjänsten finns under Tjänstslutpunkter.

   ![](assets/four.png)

## Användarnamn och lösenord är giltiga {#username-and-password-are-valid}

Om du har ett ![- här](assets/delete.png) kontrollerar du att ditt Microsoft Dynamics-användarnamn och -lösenord är giltiga.

## Synkroniseringsanvändaren har tilldelats rollen Marketo Sync User {#sync-user-is-assigned-to-the-marketo-sync-user-role}

Om du har en ![](assets/delete.png) - här måste du verifiera att rollen Marketo Sync User (Synkronisera användare) är markerad i Microsoft Dynamics. Se steg 2 i installationsdokumentationen för Microsoft Dynamics.

1. Klicka på ikonen Inställningar i Dynamics och välj **Avancerade inställningar**.

   ![](assets/one.png)

1. Klicka på **Inställningar** och välj **Dokumentskydd**.

   ![](assets/six.png)

1. Klicka på **Användare.**

   ![](assets/image2015-9-24-9-3a47-3a25.png)

1. Klicka på länken för synkroniseringsanvändaren.

   ![](assets/seven.png)

1. Klicka på **Hantera roller**.

   ![](assets/eight.png)

1. Kontrollera att Marketo Sync User-rollen är markerad. Om inte, markerar du den och klickar på **OK.**

   ![](assets/image2015-9-24-9-3a59-3a21.png)

## Marketo-lösningen är korrekt installerad {#marketo-solution-is-properly-installed}

Om du har en ![](assets/delete.png) - här går du till Microsoft Dynamics för att verifiera att Marketo-installationen finns där. Se steg 1 i installationsdokumentationen för Microsoft Dynamics.

1. Klicka på ikonen Inställningar i Dynamics och välj **Avancerade inställningar**.

   ![](assets/one.png)

1. Klicka på **Inställningar **och välj **Lösningar.**

   ![](assets/eleven.png)

1. Kontrollera att lösningen finns med i listan.

   ![](assets/twelve.png)

## Alla steg i lösningen är aktiverade {#all-steps-in-the-solution-are-enabled}

Om du har en ![- här](assets/delete.png) kontrollerar du att ingen av standardstegen har inaktiverats. Alla steg aktiveras automatiskt vid installationen, men de kan inaktiveras under en anpassning.

## Synkroniseringsanvändaren har tilldelats Marketo-lösningen {#sync-user-is-assigned-to-the-marketo-solution}

Om du har en ![- här](assets/delete.png) - kontrollerar du att synkroniseringsanvändaren är tilldelad till standardsidan Marketo i Microsoft Dynamics.

1. Klicka på ikonen Inställningar i Dynamics och välj **Avancerade inställningar**.

   ![](assets/one.png)

1. Klicka på **Settings **och välj **Marketo Config**.

   ![](assets/thirteen.png)

1. Kontrollera att synkroniseringsanvändaren är tilldelad som standard.

   ![](assets/fourteen.png)

## Synkronisera användare matchar användarnamn och lösenord {#sync-user-matches-username-and-password}

Om du har en ![- här](assets/delete.png) - se till att tilldela rätt synkroniseringsanvändare i fältet Marketo-användare i steget Marketo Config-standardinställning i Microsoft Dynamics.

>[!NOTE]
>
>**Relaterade artiklar**
>
>[Verifiera Microsoft Dynamics Sync](../../../../../product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/validate-microsoft-dynamics-sync.md)

