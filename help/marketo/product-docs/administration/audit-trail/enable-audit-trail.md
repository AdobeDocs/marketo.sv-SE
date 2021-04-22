---
unique-page-id: 11382122
description: Aktivera granskningsspår - Marketo Docs - produktdokumentation
title: Aktivera granskningsspår
exl-id: 3ab2d7b2-1be1-4b3f-a9cc-d3edfa963679
translation-type: tm+mt
source-git-commit: 72e1d29347bd5b77107da1e9c30169cb6490c432
workflow-type: tm+mt
source-wordcount: '245'
ht-degree: 0%

---

# Aktivera granskningsspår {#enable-audit-trail}

Granskningsspårning är tillgängligt för alla kunder och styrs av två administratörsbehörigheter.

>[!NOTE]
>
>Som standard har alla systemadministratörsroller båda behörigheterna aktiverade.

## Aktivera granskningsspår för en roll {#enable-audit-trail-for-a-role}

1. Klicka på **Admin**.

   ![](assets/one-2.png)

1. Välj **Användare och roller** och klicka på **Roller**.

   ![](assets/two-2.png)

1. Markera rollen som du vill aktivera granskningsspår för och klicka på **Redigera roll**.

   ![](assets/three-1.png)

   >[!NOTE]
   >
   >Du kan också skapa en ny roll och ge den åtkomst till granskningsspår här.

1. Expandera behörigheten **Åtkomstadministratör**. Välj **Åtkomst till granskningsspår** och/eller **Åtkomst till inloggningshistorik**, beroende på dina behov. Klicka på **Spara**.

   ![](assets/four-1.png)

   >[!NOTE]
   >
   >**Definition**
   >
   >**Åtkomst till granskningsspår:** Ger användare åtkomst till både resursgranskningsspår och administratörsgranskningsspår.
   >
   >**Åtkomst till inloggningshistorik:** Ger användare åtkomst till  [användarens inloggningshistorik](/help/marketo/product-docs/administration/audit-trail/user-login-history.md).

## Tilldela roll för granskningsspår till en användare {#assign-audit-trail-role-to-a-user}

>[!PREREQUISITES]
>
>[Skapa ](/help/marketo/product-docs/administration/users-and-roles/create-delete-edit-and-change-a-user-role.md#create-a-role) eller  [](#enable-audit-trail) aktivera befintlig roll och ge den behörigheten Granskningsspår.

1. I **Användare och roller** klickar du på **Användare**.

   ![](assets/five-1.png)

1. Markera den användare som du vill ge granskningsspår åtkomst till och klicka på **Redigera användare**.

   ![](assets/six-1.png)

   >[!NOTE]
   >
   >Den här processen gäller även när du skapar en ny användare.

1. Välj de granskningsspårsroller du har skapat. I det här exemplet skapade vi&quot;Granskningsspår - Tillgångar och administratör&quot; och&quot;Granskningsspår - Med inloggningshistorik&quot;.

   ![](assets/seven-1.png)

   >[!CAUTION]
   >
   >Om du har aktiverat arbetsytor markerar du rollens kryssruta, som markerar alla arbetsytor. Om du avmarkerar en enskild arbetsyta döljs granskningsspåret. Det innebär att du ser granskningsversionsdata för alla arbetsytor. Du kan dölja arbetsytor när [filtrera](/help/marketo/product-docs/administration/audit-trail/filtering-in-audit-trail.md).

1. Klicka på **Spara**.

   ![](assets/eight-1.png)
