---
description: Åsidosättning av prioritet för utlösarkampanjer - Marketo Docs - produktdokumentation
title: Åsidosättning av prioritet för utlösarkampanjer
exl-id: cf9b4d27-0e4c-40cf-accd-4f4a102160cc
feature: Smart Campaigns
source-git-commit: 431bd258f9a68bbb9df7acf043085578d3d91b1f
workflow-type: tm+mt
source-wordcount: '220'
ht-degree: 1%

---

# Åsidosättning av prioritet för utlösarkampanjer {#priority-override-for-trigger-campaigns}

Administratörer kan åsidosätta Marketo fastställda prioritet för utlösarkampanjer för att ange prioriteringar som bättre motsvarar affärsmålen.

>[!NOTE]
>
>Den här funktionen är endast tillgänglig för utlösarkampanjer och för användare som har tilldelats [Behörighet för att redigera utlösarkampanjprioritet](#grant-priority-override-access).

>[!CAUTION]
>
>Vi rekommenderar starkt att du använder den här funktionen för en begränsad uppsättning affärskritiska kampanjer (25 är det rekommenderade maxvärdet). Om du använder funktionen löst i en stor uppsättning kan det påverka kampanjkörningen negativt.

## Åsidosätt åtkomst med Bevilja prioritet {#grant-priority-override-access}

>[!NOTE]
>
>Endast administratörer eller användare med administratörsansvar bör ha åtkomst till åsidosättande av kampanjprioritet.

1. I [!UICONTROL Admin] område, klicka **[!UICONTROL Users & Roles]**.

   ![](assets/priority-override-for-trigger-campaigns-1.png)

1. Klicka på **[!UICONTROL Roles]** väljer du den användare som du vill ge åtkomst till och klickar sedan på **[!UICONTROL Edit Role]**.

   ![](assets/priority-override-for-trigger-campaigns-2.png)

1. Under [!UICONTROL Access Marketing Activities] väljer du **[!UICONTROL Edit Trigger Campaign Priority]**. Klicka på **[!UICONTROL Save]**.

   ![](assets/priority-override-for-trigger-campaigns-3.png)

## Åsidosätt prioritet {#override-priority}

1. Hitta era utlösarkampanjer. Högerklicka på den och välj **[!UICONTROL Override Campaign Priority]**.

   ![](assets/priority-override-for-trigger-campaigns-4.png)

1. Klicka på **[!UICONTROL Override Campaign Priority]** för att aktivera. Välj en ny prioritetsnivå och klicka på **[!UICONTROL Confirm]**.

   ![](assets/priority-override-for-trigger-campaigns-5.png)

   Den nya prioritetsnivån visas på fliken Schema.

   ![](assets/priority-override-for-trigger-campaigns-6.png)

>[!NOTE]
>
>* Du kan visa kampanjens standardprioritet i [!UICONTROL Campaign Queue] under [!UICONTROL Marketing Activities]. Vi rekommenderar att du ställer in kampanjprioriteten på en nivå som är högre än standardnivån för att öka exekveringsfrekvensen.
>* Prioriteten för användarinställningen gäller endast nya personer som är kvalificerade för kampanjen. Personer som redan är i kö påverkas inte.
>* Prioritetsåsidosättningar hämtas i [Granskningsspår](/help/marketo/product-docs/administration/audit-trail/audit-trail-overview.md).
