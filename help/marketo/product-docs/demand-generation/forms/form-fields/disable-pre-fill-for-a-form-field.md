---
unique-page-id: 2359675
description: Inaktivera förifyllning för ett formulärfält - Marketo Docs - produktdokumentation
title: Inaktivera förifyllning för ett formulärfält
exl-id: c600e0ce-1b94-4f7b-b75d-f550a2904799
feature: Forms
source-git-commit: 0d37fbdb7d08901458c1744dc68893e155176327
workflow-type: tm+mt
source-wordcount: '158'
ht-degree: 1%

---

# Inaktivera förifyllning för ett formulärfält {#disable-pre-fill-for-a-form-field}

När en webbbesökare är känd (kodad) kommer Marketo-formulär att förifylla fält med deras information som standard. Så här gör du om du vill stänga av det här.

>[!NOTE]
>
>**Formulärförifyllning** är aktiverat som standard. Inställningarna för förifyllning på landningssidnivå och förifyllning på administratörsnivå trumpar inställningen för formulärnivå:
>
>Form > Landing Page > Admin

## Inaktivera förifyllning {#how-to-disable-pre-fill}

1. Gå till **[!UICONTROL Marketing Activities]**.

   ![](assets/login-marketing-activities-7.png)

1. Markera formuläret och klicka på **[!UICONTROL Edit Form]**.

   ![](assets/image2014-9-15-14-3a26-3a46.png)

   >[!CAUTION]
   >
   >Förifyll formulär fungerar inte när du bäddar in ett formulär på dina egna sidor. Det fungerar bara på Marketo landningssidor.

1. Markera ett av fälten och ange **[!UICONTROL Form Pre-fill]** till **[!UICONTROL Disabled]**.

   ![](assets/image2014-9-15-14-3a26-3a54.png)

   >[!TIP]
   >
   >Du kan även inaktivera förifyllnad av formulär på landningssidnivå eller på adminnivå.

1. Klicka på **[!UICONTROL Finish]**.

   ![](assets/image2014-9-15-14-3a27-3a1.png)

1. Klicka på **[!UICONTROL Approve and Close]**.

   ![](assets/image2014-9-15-14-3a27-3a6.png)

## Känsliga fält {#sensitive-fields}

När du [markerar ett fält som känsligt](/help/marketo/product-docs/administration/field-management/mark-a-field-as-sensitive.md) och förhindrar att dess värden fylls i i formulär i förväg, visas detta i alternativet Förifyll.

![](assets/disable-pre-fill.png)
