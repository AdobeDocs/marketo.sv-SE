---
unique-page-id: 11382122
description: Aktivera granskningsspår - Marketo Docs - produktdokumentation
title: Aktivera granskningsspår
exl-id: 3ab2d7b2-1be1-4b3f-a9cc-d3edfa963679
feature: Audit Trail
source-git-commit: 431bd258f9a68bbb9df7acf043085578d3d91b1f
workflow-type: tm+mt
source-wordcount: '212'
ht-degree: 1%

---

# Aktivera granskningsspår {#enable-audit-trail}

Granskningsspårning är tillgängligt för alla kunder och styrs av två administratörsbehörigheter.

>[!NOTE]
>
>Som standard har alla systemadministratörsroller båda behörigheterna aktiverade.

## Aktivera granskningsspår för en roll {#enable-audit-trail-for-a-role}

1. Klicka på **[!UICONTROL Admin]**.

   ![](assets/enable-audit-trail-1.png)

1. Välj **[!UICONTROL Users & Roles]** och klicka **[!UICONTROL Roles]**.

   ![](assets/enable-audit-trail-2.png)

1. Markera rollen som du vill aktivera granskningsspår för och klicka på **[!UICONTROL Edit Role]**.

   ![](assets/enable-audit-trail-3.png)

   >[!NOTE]
   >
   >Du kan också skapa en ny roll och ge den åtkomst till granskningsspår här.

1. Expandera **[!UICONTROL Access Admin]** behörighet. Välj **[!UICONTROL Access Audit Trail]** och/eller **[!UICONTROL Access Login History]**, beroende på dina behov. Klicka på **[!UICONTROL Save]**.

   ![](assets/enable-audit-trail-4.png)

   >[!NOTE]
   >
   >**Definition**
   >
   >**[!UICONTROL Access Audit Trail]**: Ger användarna åtkomst till båda [!UICONTROL Asset Audit Trail] och [!UICONTROL Admin Audit Trail].
   >
   >**[!UICONTROL Access Login History]**: Ger användare åtkomst till [Historik för användarinloggning](/help/marketo/product-docs/administration/audit-trail/user-login-history.md).

## Tilldela roll för granskningsspår till en användare {#assign-audit-trail-role-to-a-user}

>[!PREREQUISITES]
>
>[Skapa](/help/marketo/product-docs/administration/users-and-roles/create-delete-edit-and-change-a-user-role.md#create-a-role) eller [enable](#enable-audit-trail) en befintlig roll som ger den behörighet för granskningsspår.

1. I **[!UICONTROL Users & Roles]**, klicka **[!UICONTROL Users]**.

   ![](assets/enable-audit-trail-5.png)

1. Välj den användare som du vill ge granskningsspår åtkomst till och klicka på **[!UICONTROL Edit User]**.

   ![](assets/enable-audit-trail-6.png)

   >[!NOTE]
   >
   >Den här processen gäller även när du skapar en ny användare.

1. Välj de granskningsspårsroller du har skapat. I det här exemplet skapade vi&quot;Granskningsspår - Tillgångar och administratör&quot; och&quot;Granskningsspår - Med inloggningshistorik&quot;.

   ![](assets/enable-audit-trail-7.png)

   >[!CAUTION]
   >
   >Om du har aktiverat arbetsytor markerar du rollens kryssruta, som markerar alla arbetsytor. Om du avmarkerar en enskild arbetsyta döljs granskningsspåret. Det innebär att du ser granskningsversionsdata för alla arbetsytor. Du kan dölja arbetsytor när [filtrering](/help/marketo/product-docs/administration/audit-trail/filtering-in-audit-trail.md).

1. Klicka på **[!UICONTROL Save]**.

   ![](assets/enable-audit-trail-8.png)
