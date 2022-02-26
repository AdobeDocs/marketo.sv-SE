---
description: Förfallotid för lokala tillgångar - Marketo Docs - produktdokumentation
title: Förfallotid för lokal resurs
hide: true
hidefromtoc: true
source-git-commit: 8baa8bc8ed897314945964deed5f867866a79f8c
workflow-type: tm+mt
source-wordcount: '237'
ht-degree: 0%

---

# Förfallotid för lokal resurs {#local-asset-expiration}

Ange ett förfallodatum/tid för att avpublicera landningssidor, inaktivera utlösarkampanjer eller stoppa återkommande batchkampanjer.

## Bevilja förfallotillstånd för planerad tillgång {#grant-schedule-asset-expiration-permission}

Innan du kan schemalägga förfallodatum för en mediefil måste din Marketo-roll ha rätt behörighet aktiverad.

>[!NOTE]
>
>**Administratörsbehörigheter krävs**

1. I [!UICONTROL Admin] område, klicka **[!UICONTROL Users & Roles]**.

   ![](assets/local-asset-expiration-1.png)

1. Klicka på **[!UICONTROL Roles]** väljer du den användare som du vill ge åtkomst till och klickar sedan på **[!UICONTROL Edit Role]**.

   ![](assets/local-asset-expiration-2.png)

1. Under [!UICONTROL Access Marketing Activities], markera **[!UICONTROL Schedule Local Asset Expiration]** och klicka **[!UICONTROL Save]**.

   ![](assets/local-asset-expiration-3.png)

## Ange ett förfallodatum {#set-an-expiration-date}

1. Högerklicka på önskat program och välj **[!UICONTROL Set Local Asset Expiration]**.

   ![](assets/local-asset-expiration-4.png)

1. Markera de mediefiler du vill ange ett förfallodatum för och klicka sedan på **[!UICONTROL Set Expiration]**.

   ![](assets/local-asset-expiration-5.png)

1. Välj ett förfallodatum.

   ![](assets/local-asset-expiration-6.png)

1. Ställ in en tid. Du måste schemalägga en tid på minst 20 minuter i framtiden (glöm inte att ange AM/PM). Klicka **[!UICONTROL Confirm]** när det är klart.

   ![](assets/local-asset-expiration-7.png)

>[!NOTE]
>
>* Om du vill redigera ett befintligt förfallodatum kontrollerar du bara tillgångarna och klickar på **[!UICONTROL Set Expiration]**.
>* När en resurs har gått ut visas den inte längre i rutnätet Förfallodatum. Rutnätet visar bara publicerade landningssidor, aktiva utlösarkampanjer och återkommande batchkampanjer.
>* Schemalagda förfallodatum tas bort om resursen flyttas till ett annat program.


## Ta bort ett förfallodatum {#remove-an-expiration-date}

1. Om du vill ta bort ett förfallodatum kontrollerar du tillgången/tillgångarna och klickar på **[!UICONTROL Remove Expiration]**.

   ![](assets/local-asset-expiration-8.png)

1. Granska de resurser som påverkas och klicka sedan på **[!UICONTROL Confirm]**.

   ![](assets/local-asset-expiration-9.png)

>[!NOTE]
>
>Det går inte att ta bort förfallodatum som är mindre än 15 minuter framåt. Om du vill ta bort förfallodatumet måste du vänta tills resursen har gått ut och sedan godkänna eller aktivera den igen.
