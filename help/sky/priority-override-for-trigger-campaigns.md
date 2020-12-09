---
title: priority-override-for-trigger-campaign
description: Åsidosättning av prioritet för utlösarkampanjer
translation-type: tm+mt
source-git-commit: e149133a5383faaef5e9c9b7775ae36e633ed7b1
workflow-type: tm+mt
source-wordcount: '301'
ht-degree: 0%

---


# Åsidosättning av prioritet för utlösarkampanjer

<br> 

Administratörer kan åsidosätta Marketos fasta prioritet för utlösarkampanjer för att ange prioriteringar som bättre överensstämmer med affärsmålen.

>[!NOTE]
>
>Den här funktionen är bara tillgänglig för utlösarkampanjer och för användare som har beviljats behörigheten Redigera utlösarkampanjprioritet.

>[!CAUTION]
>
>Vi rekommenderar starkt att du använder den här funktionen för en begränsad uppsättning affärskritiska kampanjer (25 är det rekommenderade maxvärdet). Om du använder funktionen löst i en stor uppsättning kan det påverka kampanjkörningen negativt.

## Åsidosätt prioritet

1. Klicka på **[!UICONTROL Schedule]** fliken i utlösarkampanjen och klicka sedan på **[!UICONTROL Override Priority]**.

   ![Bild ett](/help/sky/assets/smart-campaigns/priority-override-for-trigger-campaigns/priority-override-for-trigger-campaigns-1.png)

1. Välj en ny prioritetsnivå i listrutan. Klicka **[!UICONTROL Confirm]**.

   ![Bild två](/help/sky/assets/smart-campaigns/priority-override-for-trigger-campaigns/priority-override-for-trigger-campaigns-2.png)

   ![Bild tre](/help/sky/assets/smart-campaigns/priority-override-for-trigger-campaigns/priority-override-for-trigger-campaigns-3.png)

>[!NOTE]
>
>* Du kan visa kampanjens standardprioritet i [!UICONTROL Campaign Queue] listan under [!UICONTROL Marketing Activities]. Vi rekommenderar att du ställer in kampanjprioriteten på en nivå som är högre än standardnivån för att öka exekveringsfrekvensen.
>* Prioriteten för användarinställningen gäller endast nya personer som är kvalificerade för kampanjen. Personer som redan är i kö påverkas inte.


## Återställ prioritet

1. Om du vill återställa kampanjprioriteten till systemstandardvärdet går du till fliken **[!UICONTROL Schedule]** i utlösarkampanjen och klickar på **[!UICONTROL Reset Priority]**.

   ![Bild fyra](/help/sky/assets/smart-campaigns/priority-override-for-trigger-campaigns/priority-override-for-trigger-campaigns-4.png)

1. Bekräfta genom **[!UICONTROL Reset]** att klicka.

   ![Bild fem](/help/sky/assets/smart-campaigns/priority-override-for-trigger-campaigns/priority-override-for-trigger-campaigns-5.png)

>[!NOTE]
>
>Prioritetsåsidosättningar och -återställningar sparas i granskningsspåret. Du kan visa [granskningsspåret](https://docs.marketo.com/x/GZ2t) genom [!UICONTROL Admin] området Klassisk.

## Åsidosätt åtkomst med Bevilja prioritet

>[!CAUTION]
>
>Endast administratörer eller användare med administratörsansvar bör ha åtkomst till åsidosättande av kampanjprioritet.

1. Klicka i [!UICONTROL Admin] området **[!UICONTROL Users & Roles]**.

   ![Bild sex](/help/sky/assets/smart-campaigns/priority-override-for-trigger-campaigns/priority-override-for-trigger-campaigns-6.png)

1. Klicka på **[!UICONTROL Roles]** fliken, markera den användare som du vill ge åtkomst till och klicka sedan på **[!UICONTROL Edit Role]**.

   ![Bild sju](/help/sky/assets/smart-campaigns/priority-override-for-trigger-campaigns/priority-override-for-trigger-campaigns-7.png)

1. Under [!UICONTROL Access Marketing Activities], kolla **[!UICONTROL Edit Trigger Campaign Priority]**. Klicka **[!UICONTROL Save]**.

   ![Bild åtta](/help/sky/assets/smart-campaigns/priority-override-for-trigger-campaigns/priority-override-for-trigger-campaigns-8.png)

## Visa kampanjprioritet i Marketo Classic

Du kan visa kampanjprioritet i [!DNL Classic] upplevelsen genom att klicka på **[!UICONTROL Schedule]** fliken i en utlösarkampanj.

![Bild nio](/help/sky/assets/smart-campaigns/priority-override-for-trigger-campaigns/priority-override-for-trigger-campaigns-9.png)

>[!NOTE]
>
>Prioriteten i upplevelsen är bara att visa [!DNL Classic] . Det går bara att ändra eller återställa kampanjens prioritet via Marketo Sky.
