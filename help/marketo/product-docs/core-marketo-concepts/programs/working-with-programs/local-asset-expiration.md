---
description: Förfallotid för lokala tillgångar - Marketo Docs - produktdokumentation
title: Förfallotid för lokal resurs
exl-id: 603e3eee-0531-4139-a8f5-279831ad011f
feature: Programs
source-git-commit: 431bd258f9a68bbb9df7acf043085578d3d91b1f
workflow-type: tm+mt
source-wordcount: '239'
ht-degree: 0%

---

# Förfallotid för lokal resurs {#local-asset-expiration}

Ange ett förfallodatum/tid för att avpublicera landningssidor, inaktivera utlösarkampanjer eller stoppa återkommande batchkampanjer.

## Bevilja förfallotillstånd för planerad tillgång {#grant-schedule-asset-expiration-permission}

Innan du kan schemalägga förfallodatum för en mediefil måste din Marketo-roll ha rätt behörighet aktiverad.

>[!NOTE]
>
>**Administratörsbehörigheter krävs**

1. Klicka på **[!UICONTROL Users & Roles]** i området [!UICONTROL Admin].

   ![](assets/local-asset-expiration-1.png)

1. Klicka på fliken **[!UICONTROL Roles]**, markera den användare som du vill ge åtkomst till och klicka sedan på **[!UICONTROL Edit Role]**.

   ![](assets/local-asset-expiration-2.png)

1. Under [!UICONTROL Access Marketing Activities] väljer du **[!UICONTROL Schedule Local Asset Expiration]** och klickar på **[!UICONTROL Save]**.

   ![](assets/local-asset-expiration-3.png)

## Ange ett förfallodatum {#set-an-expiration-date}

1. Högerklicka på önskat program och välj **[!UICONTROL Set Local Asset Expiration]**.

   ![](assets/local-asset-expiration-4.png)

1. Kontrollera de mediefiler du vill ange ett förfallodatum för och klicka sedan på **[!UICONTROL Set Expiration]**.

   ![](assets/local-asset-expiration-5.png)

1. Välj ett förfallodatum.

   ![](assets/local-asset-expiration-6.png)

1. Ställ in en tid. Du måste schemalägga en tid på minst 15 minuter (glöm inte att ange AM/PM). Klicka på **[!UICONTROL Confirm]** när du är klar.

   ![](assets/local-asset-expiration-7.png)

>[!NOTE]
>
>* Om du vill redigera ett befintligt förfallodatum kontrollerar du bara resurserna och klickar på **[!UICONTROL Set Expiration]**.
>* När en resurs har gått ut visas den inte längre i rutnätet Förfallodatum. Rutnätet visar bara publicerade landningssidor, aktiva utlösarkampanjer och återkommande batchkampanjer.
>* Schemalagda förfallodatum tas bort om resursen flyttas till ett annat program.

## Ta bort ett förfallodatum {#remove-an-expiration-date}

1. Om du vill ta bort ett förfallodatum kontrollerar du resurserna och klickar på **[!UICONTROL Remove Expiration]**.

   ![](assets/local-asset-expiration-8.png)

1. Granska de resurser som påverkas och klicka sedan på **[!UICONTROL Confirm]**.

   ![](assets/local-asset-expiration-9.png)

>[!NOTE]
>
>Det går inte att ta bort förfallodatum som är mindre än 15 minuter framåt. Om du vill ta bort förfallodatumet måste du vänta tills resursen har gått ut och sedan godkänna eller aktivera den igen.
