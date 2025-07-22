---
unique-page-id: 4720125
description: Integrera RTP med Google Universal Analytics - Marketo Docs - produktdokumentation
title: Integrera RTP med Google Universal Analytics
exl-id: e8fc8730-c91d-44ad-8843-aa5b38f1ebd1
feature: Web Personalization
source-git-commit: 0d37fbdb7d08901458c1744dc68893e155176327
workflow-type: tm+mt
source-wordcount: '368'
ht-degree: 0%

---

# Integrera RTP med [!DNL Google Universal Analytics] {#integrate-rtp-with-google-universal-analytics}

## Intro {#intro}

Utnyttja [!DNL Google Universal Analytics] (GUA) med [!DNL Marketo Real-Time Personalization]s (RTP)-data (Firmographic) och personaliseringsdata för att bättre kunna mäta och analysera era onlinemarknadsföringsinsatser.

I det här inlägget beskrivs hur du konfigurerar och integrerar RTP-plattformen [!DNL Marketo Real-Time Personalization] med [!DNL Google Universal Analytics] (GUA)-konton. RTP-data kan läggas in i ditt GUA-konto så att du kan se resultatet för organisationer, branscher, företagsgrafik och RTP-segment som besöker din webbplats.

**[!DNL Google Universal Analytics]**

[!DNL Google Universal Analytics] med RTP:s data ger dig en bättre förståelse för hur B2B-användare interagerar med ditt onlineinnehåll och hjälper dig att mäta och få bättre resultat med dina personaliseringskampanjer. [Läs mer om  [!DNL Google Universal Analytics]](https://support.google.com/analytics/answer/2790010/?hl=en&authuser=1).

>[!NOTE]
>
>**Endast för Google Tag Manager-användare**
>
>Ingen kodning eller specialkonfiguration behöver göras. Se till att du slutför följande checklista:
>
>* RTP-dimensioner skapas i [!DNL Google Universal Analytics]
>* [RTP-taggen är korrekt installerad i Google Tag Manager](https://docs.marketo.com/display/public/DOCS/Implementing+RTP+using+Google+Tag+Manager)
>* [!DNL Google Universal Analytics]-integrering är aktiverad i RTP:s kontoinställningar
>* [[!DNL Google Universal Analytics] taggen är korrekt konfigurerad i Google Tag Manager](https://support.google.com/tagmanager/answer/6107124?hl=en)
>* [Taggen Google Tag Manager är korrekt installerad på webbplatsen](https://developers.google.com/tag-manager/quickstart)

## Ställ in anpassade dimensioner i GUA {#set-up-custom-dimensions-in-gua}

1. I GOOGLE ANALYTICS

   1. Gå till **[!UICONTROL Admin]**
   1. Välj **[!UICONTROL Account].**
   1. Välj **[!UICONTROL Property].**
   1. Välj **[!UICONTROL Custom Definitions]** och **[!UICONTROL Custom Dimensions]**.

      ![](assets/image2014-11-29-11-3a2-3a32.png)

1. Lägg till en ny anpassad dimension. Klicka på **[!UICONTROL +New Custom Dimension]**

   ![](assets/image2014-11-29-11-3a8-3a16.png)

1. Lägg till följande **[!UICONTROL Custom Dimensions]:**

<table> 
 <tbody> 
  <tr> 
   <td><p><strong>Anpassat Dimension-namn</strong></p></td> 
   <td><p><strong>Omfång</strong></p></td> 
   <td><p><strong>Aktiv</strong></p></td> 
  </tr> 
  <tr> 
   <td><p><strong>RTP-organisation</strong></p></td> 
   <td><p>Session</p></td> 
   <td><p align="center">✓</p></td> 
  </tr> 
  <tr> 
   <td><p><strong>RTP-Bransch</strong></p></td> 
   <td><p>Session</p></td> 
   <td><p align="center">✓</p></td> 
  </tr> 
  <tr> 
   <td><p><strong>RTP-kategori</strong></p></td> 
   <td><p>Session</p></td> 
   <td><p align="center">✓</p></td> 
  </tr> 
  <tr> 
   <td><p><strong>RTP-grupp</strong></p></td> 
   <td><p>Session</p></td> 
   <td><p align="center">✓</p></td> 
  </tr> 
 </tbody> 
</table>

>[!NOTE]
>
>**Anpassade Dimension-namn** måste vara exakt som de definieras i tabellen ovan (annars visas inte anpassade RTP-instrumentpaneler och rapporter i GUA korrekt)

1. Lägg till **[!UICONTROL Name]**. Välj scopet som **[!UICONTROL Session]**. Klicka på **[!UICONTROL Create]**.

   ![](assets/image2014-11-29-11-3a12-3a51.png)

Din lista över anpassade Dimension bör se ut så här.

![](assets/image2014-11-29-11-36-50-version-2.png)

När du har aktiverat Anpassade dimensioner i GUA går du till RTP-plattformen för att aktivera de här dimensionerna i RTP.

## Aktivera GUA-integreringen i ditt RTP-konto {#activate-the-gua-integration-in-your-rtp-account}

1. Gå till **[!UICONTROL Account Settings]i RTP-plattformen.**

   ![](assets/image2014-11-29-11-3a27-3a7.png)

1. Klicka på **[!UICONTROL Account Settings]** under **[!UICONTROL Domain]**.
1. Klicka på **[!UICONTROL Analytics]** under **[!UICONTROL Google Universal Analytics]**.
1. Vrid **[!UICONTROL On]** på relevanta anpassade dimensioner och händelser för att lägga till dessa data från RTP till [!DNL Google Universal Analytics].
1. Ange **[!UICONTROL Index number]** för dimensionen justerad mot indexnumret i GUA.
1. Klicka på **[!UICONTROL Save]**.

![](assets/image2014-11-29-11-31-23-version-2.png)

>[!NOTE]
>
>Indexnumret för den anpassade Dimension finns i GUA under Anpassade dimensioner.
>
>Exempel: RTP-Industry Index Number är lika med 1, RTP-Organization Index Number är lika med 2.

## Ta bort gamla instrumentpaneler i Google Analytics {#remove-old-dashboards-in-google-analytics}

1. I Google Analytics. Gå till **[!UICONTROL Reporting].**
1. Klicka på **[!UICONTROL Dashboards].**
1. Välj en **[!UICONTROL Dashboard]** (RTP B2B- eller RTP-prestanda)
1. Klicka på **[!UICONTROL Delete Dashboard]**.

![](assets/image2014-11-29-11-3a42-3a55.png)
