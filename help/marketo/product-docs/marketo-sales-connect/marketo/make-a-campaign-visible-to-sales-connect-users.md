---
unique-page-id: 14745655
description: Gör en kampanj synlig för användare av Sales Connect - Marketo Docs - produktdokumentation
title: Gör en kampanj synlig för användare av Sales Connect
exl-id: 1fde53e3-2764-4e4b-897f-635b78534133
feature: Marketo Sales Connect
source-git-commit: 09a656c3a0d0002edfa1a61b987bff4c1dff33cf
workflow-type: tm+mt
source-wordcount: '96'
ht-degree: 0%

---

# Gör en kampanj synlig för [!DNL Sales Connect] användare {#make-a-campaign-visible-to-sales-connect-users}

Kampanjer kan bara delas om de är synliga. Så här gör du.

1. Välj (eller skapa) den kampanj du vill dela.

   ![](assets/make-a-marketing-campaign-visible-msc-1.png)

1. Klicka på fliken **[!UICONTROL Smart List]**.

   ![](assets/make-a-marketing-campaign-visible-msc-2.png)

1. Lägg till [!UICONTROL Campaign is Requested]-utlösaren.

   ![](assets/make-a-marketing-campaign-visible-msc-3.png)

1. Välj [!UICONTROL is] **[!UICONTROL Web Service API]** som källa.

   ![](assets/make-a-marketing-campaign-visible-msc-4.png)

1. Klicka på fliken **[!UICONTROL Flow]**.

   ![](assets/make-a-marketing-campaign-visible-msc-5.png)

1. Lägg till flödesåtgärden [!UICONTROL Interesting Moment].

   ![](assets/make-a-marketing-campaign-visible-msc-6.png)

1. För [!UICONTROL Type] väljer du **[!UICONTROL Web]**.

   ![](assets/make-a-marketing-campaign-visible-msc-7.png)

1. Skriv ett meddelande till ditt säljteam i rutan [!UICONTROL Description]. I det här exemplet använder vi tokens för att ange formuläret som fylldes i.

   ![](assets/make-a-marketing-campaign-visible-msc-8.png)

1. Klicka på fliken **[!UICONTROL Schedule]** och **[!UICONTROL Activate]** kampanjen.

   ![](assets/make-a-marketing-campaign-visible-msc-9.png)
