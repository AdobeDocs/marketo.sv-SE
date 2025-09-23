---
description: Svarsloggning - Marketo Docs - produktdokumentation
title: Svarsloggning
hide: true
hidefromtoc: true
exl-id: a89e8212-83cb-4987-abc9-76c5fd74c152
feature: Sales Insight Actions
source-git-commit: 09a656c3a0d0002edfa1a61b987bff4c1dff33cf
workflow-type: tm+mt
source-wordcount: '237'
ht-degree: 0%

---

# Svarsloggning {#reply-logging}

Sales Insight Actions ger dig möjlighet att automatiskt logga dina potentiella kunders svar på [!DNL Salesforce]. Strukturen som gör att du kan göra detta baseras på vår spårning av e-postsvar. Om vi kan spåra svar från en potentiell kund kan vi logga svaret på [!DNL Salesforce].

## Krav {#requirements}

* E-postmeddelanden måste loggas via API-loggning
* Du måste kunna [spåra ett svar](/help/marketo/product-docs/marketo-sales-insight/actions/send-a-sales-email/email-tracking-overview.md#how-reply-tracking-works)
* Måste vara ansluten till [!DNL Salesforce]
* [!DNL Salesforce] [API-anrop](https://developer.salesforce.com/docs/atlas.en-us.salesforce_app_limits_cheatsheet.meta/salesforce_app_limits_cheatsheet/salesforce_app_limits_platform_api.htm) måste vara tillgängliga

## Aktivera svarsloggning {#enable-reply-logging}

1. Om du vill aktivera svarsloggning går du till inställningssidan för [!DNL Salesforce]. När API-loggningen är utcheckad ser du alternativet att kontrollera _Logga svar_.

   >[!NOTE]
   >
   >Svarsloggning följer samma regler som du har för att logga skickade e-postmeddelanden. Detta inkluderar hur e-postmeddelanden loggas, till Leads och Kontakter, när det finns en dubblettpost och om inga matchande poster hittas.

## Anger svarstyp i [!DNL Salesforce] {#setting-type-to-reply-in-salesforce}

Det är viktigt att du hämtar meningsfulla data från dina [!DNL Salesforce]-rapporter. Om du har möjlighet att fylla i fältet Typ som Svara kan du hämta data genom dina rapporter. Anslut till din `[!DNL Salesforce] admin` för att få den här konfigurationen.

1. Gå till **[!UICONTROL Setup]** > **[!UICONTROL Customize]** > **[!UICONTROL Activities]** > **[!UICONTROL Task Fields]**.
1. Klicka på **[!UICONTROL Type]**.
1. Klicka på [!UICONTROL Task Type Picklist Values] under **[!UICONTROL New]**.
1. Skriv&quot;Svara&quot; i den tomma rutan. Se till att du börjar med versal och klickar på **[!UICONTROL Save]**.

   >[!NOTE]
   >
   >Du behöver inte välja en standard i typväljaren. [!DNL Sales Insight Actions] kommer att se att den här aktivitetstypen är tillgänglig i din [!DNL Salesforce]-instans och fylla i aktivitetsfältet på dina inkommande aktiviteter därefter.
