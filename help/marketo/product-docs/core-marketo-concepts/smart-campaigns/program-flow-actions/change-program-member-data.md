---
description: Lär dig hur du ändrar programmedlemsdata i ett flödessteg. Uppdatera medlemsstatus eller anpassade fält för personer i ett program.
title: Ändra medlemsuppgifter för program
exl-id: 2ed8468e-0dbb-48c1-be60-7b51e92f9095
feature: Smart Campaigns
source-git-commit: 3efcb529cd3e35027f35e51dfd91f95e94af9d61
workflow-type: tm+mt
source-wordcount: '146'
ht-degree: 0%

---

# Ändra medlemsuppgifter för program {#change-program-member-data}

Du kan använda Marketo för att uppdatera ett fälts värde med hjälp av åtgärden Ändra datavärde.

>[!NOTE]
>
>Du kan också blockera ett fält så att det inte uppdateras. Mer information finns i Blockera uppdateringar till ett fält.

1. Gå till flödessteget **[!UICONTROL Change Program Member Data]** på fliken Flöde i Smart Campaign och välj önskat program.

   ![](assets/change-program-member-data-1.png)

1. Sök efter och markera det attribut som du vill ändra värdet för.

   ![](assets/change-program-member-data-2.png)

1. Ange det attributvärde som du vill använda.

   ![](assets/change-program-member-data-3.png)

>[!NOTE]
>
>Du kan också använda variabler i [!UICONTROL New Value].

Kör nu bara Smart Campaign, så är du klar!

>[!TIP]
>
>Om du vill rensa fälten i stället för att uppdatera dem kan du ange&quot;NULL&quot; (inga citattecken, versaler) som [!UICONTROL New Value].

>[!MORELIKETHIS]
>
>* [Använd token i flödessteg](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/flow-actions/use-tokens-in-flow-steps.md){target="_blank"}
>* [Lägg till data i ett fält](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/flow-actions/append-data-to-a-field.md){target="_blank"}
