---
unique-page-id: 11384433
description: Installation av kontoteam - Marketo Docs - produktdokumentation
title: Kontouppsättningsinställningar
exl-id: a4aee37f-5e39-4296-b720-b1c73c98df9e
feature: Target Account Management
source-git-commit: 431bd258f9a68bbb9df7acf043085578d3d91b1f
workflow-type: tm+mt
source-wordcount: '181'
ht-degree: 0%

---

# Kontouppsättningsinställningar {#account-team-setup}

Ett kontoteam är en grupp intressenter som arbetar tillsammans med ett namngivet konto. Följ de här stegen för att välja vilka CRM-kontoroller som ska läggas till.

1. Klicka på **Admin**.

   ![](assets/one-3.png)

1. Klicka på **Hantering av målkonto**.

   ![](assets/account-team-setup-2.png)

1. Klicka på **Redigera** under medlemmar i kontogruppen.

   ![](assets/3.png)

   >[!NOTE]
   >
   >Som kontoroll ger du den ett namn och matchar det till önskat fält för användarsökning i CRM.

1. Skriv in namnet på din kontoroll och markera fältet **CRM**. Lägg till upp till 10.

   ![](assets/four-2.png)

   >[!NOTE]
   >
   >Du kan inte välja kontoägare. Den väljs som standard från kontonivån i CRM.

1. Klicka på **Spara** när du är klar.

   ![](assets/five-2.png)

   >[!CAUTION]
   >
   >Om du gör en uppdatering kan det ta lite tid innan ändringarna återspeglas i TAM.

   >[!NOTE]
   >
   >* När flera CRM-konton med olika kontoägare sammanfogas till ett namngivet konto väljer Marketo en kontoägare och lägger till andra kontoägare som&quot;Kontomedägare&quot;
   >
   >* Om ett CRM-rollfält senare byter namn eller tas bort kommer Marketo TAM att avbryta synkroniseringen av de uppdaterade värdena tills användaren uppdaterar inställningarna i TAM manuellt
