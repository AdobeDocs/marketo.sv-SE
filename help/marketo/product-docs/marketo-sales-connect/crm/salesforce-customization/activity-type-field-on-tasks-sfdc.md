---
unique-page-id: 14352476
description: Fält för aktivitetstyp på uppgifter (SFDC) - Marketo Docs - produktdokumentation
title: Fält för aktivitetstyp på uppgifter (SFDC)
exl-id: b291e641-d3af-4667-a01c-cd491cd87add
feature: Marketo Sales Connect
source-git-commit: 09a656c3a0d0002edfa1a61b987bff4c1dff33cf
workflow-type: tm+mt
source-wordcount: '245'
ht-degree: 1%

---

# Fält för aktivitetstyp på uppgifter (SFDC) {#activity-type-field-on-tasks-sfdc}

Med hjälp av [!DNL Sales Connect] kan du logga e-post och samtal som en aktivitet i [!DNL Salesforce]. En viktig del av att ha värdefulla data i [!DNL Salesforce] är att fältet [!UICONTROL Type] fyller i rätt värde.

>[!NOTE]
>
>Loggning av e-postmeddelanden via BCC kommer inte att användas i listan Uppgiftstyp, utan fyller i textfältet automatiskt som e-post eftersom de levereras till [!DNL Salesforce] via din BCC-adress.

## Krav {#requirements}

* Anslutning med [!DNL Salesforce]
* Inget standardtypvärde har valts i listrutan Aktivitetstyp
* Samtal, svar och e-post måste alla finnas i listrutan Aktivitetstyp (skiftlägesfrågor)
* Inga arbetsflöden eller utlösare som utför åtgärder på värdet i typfältet

## Inställningar {#setup}

Kontrollera först att du har rätt plocklistevärden på plats. Du behöver hjälp av din [!DNL Salesforce]-administratör för att kunna göra ändringar i din lista.

1. Navigera till [Salesforce.com](https://salesforce.com) och klicka på Konfigurera i det övre högra hörnet.
1. Klicka på **[!UICONTROL Customize]**.
1. Klicka på **[!UICONTROL Activities]**.
1. Klicka på **[!UICONTROL Task Fields]**.
1. Klicka på **[!UICONTROL Type]**.
1. Du finns nu i listan över uppgiftstyper. Kontrollera att du inte har valt &#39;Standard&#39;.
1. Kontrollera att det finns ett [!UICONTROL Type]-värde för [!UICONTROL Email], [!UICONTROL Call] och [!UICONTROL Reply].

Nu när detta är på plats börjar du se textfältet fylla i motsvarande värde för loggade e-postmeddelanden, samtal och svar. Dessa värden fylls _inte_ i på påminnelseaktiviteter för Sales Connect.

>[!NOTE]
>
>Om du inte ser Svara som ett värde lägger du till det genom att klicka på **[!UICONTROL New]**. Svara är inte ett standardvärde i [!DNL Salesforce].
