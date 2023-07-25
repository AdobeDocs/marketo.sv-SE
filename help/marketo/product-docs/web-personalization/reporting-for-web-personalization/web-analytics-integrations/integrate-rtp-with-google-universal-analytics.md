---
unique-page-id: 4720125
description: Integrera RTP med Google Universal Analytics - Marketo Docs - produktdokumentation
title: Integrera RTP med Google Universal Analytics
exl-id: e8fc8730-c91d-44ad-8843-aa5b38f1ebd1
feature: Web Personalization
source-git-commit: 431bd258f9a68bbb9df7acf043085578d3d91b1f
workflow-type: tm+mt
source-wordcount: '456'
ht-degree: 0%

---

# Integrera RTP med Google Universal Analytics {#integrate-rtp-with-google-universal-analytics}

## Intro {#intro}

Utnyttja Google Universal Analytics (GUA) med Marketo Real-Time Personalization&#39;s (RTP) firmographic and personalization data för att bättre mäta och analysera era onlinemarknadsföringsinsatser.

I det här inlägget beskrivs hur du konfigurerar och integrerar Marketo Real-Time Personalization (RTP)-plattformen med Google Universal Analytics-konton (GUA). RTP-data kan läggas in i ditt GUA-konto så att du kan se resultatet för organisationer, branscher, företagsgrafik och RTP-segment som besöker din webbplats.

**Google Universal Analytics**

Google Universal Analytics med RTP:s data ger er en bättre förståelse för hur B2B-användare interagerar med ert onlineinnehåll och hjälper er att mäta och få bättre resultat av era personaliseringskampanjer. [Läs mer om Google Universal Analytics](https://support.google.com/analytics/answer/2790010/?hl=en&amp;authuser=1).

>[!NOTE]
>
>**Endast för Google Tag Manager-användare**
>
>Ingen kodning eller specialkonfiguration behöver göras. Se till att du slutför följande checklista:
>
>* RTP-dimensioner skapas i Google Universal Analytics
>* [RTP-taggen är korrekt installerad i Google Tag Manager](https://docs.marketo.com/display/public/DOCS/Implementing+RTP+using+Google+Tag+Manager)
>* Integrering med Google Universal Analytics är aktiverat i RTP:s kontoinställningar
>* [Taggen Google Universal Analytics är korrekt konfigurerad i Google Tag Manager](https://support.google.com/tagmanager/answer/6107124?hl=en)
>* [Taggen Google Tag Manager är korrekt installerad på webbplatsen](https://developers.google.com/tag-manager/quickstart)

## Konfigurera anpassade Dimensioner i GUA {#set-up-custom-dimensions-in-gua}

1. I Google Analytics

   1. Gå till **Administratör**
   1. Välj **Konto.**
   1. Välj **Egenskap.**
   1. Välj **Anpassade definitioner** och **Anpassade Dimensioner**.
      ![](assets/image2014-11-29-11-3a2-3a32.png)

1. Lägg till en ny anpassad dimension. Klicka **+Ny anpassad Dimension**

   ![](assets/image2014-11-29-11-3a8-3a16.png)

1. Lägg till följande **Anpassade Dimensioner:**

<table> 
 <tbody> 
  <tr> 
   <td><p><strong>Namn på anpassad Dimension</strong></p></td> 
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
>**Namn på anpassad Dimension** måste vara exakt enligt definitionen i tabellen ovan (annars visas inte anpassade RTP-instrumentpaneler och rapporter i GUA korrekt)

1. Lägg till **Namn**. Markera omfånget som **Session**. Klicka **Skapa**.

   ![](assets/image2014-11-29-11-3a12-3a51.png)

Listan Anpassad Dimension bör se ut så här.

![](assets/image2014-11-29-11-36-50-version-2.png)

När du har aktiverat anpassade Dimensioner i GUA går du till RTP-plattformen för att aktivera de här dimensionerna i RTP.

## Aktivera GUA-integreringen i ditt RTP-konto {#activate-the-gua-integration-in-your-rtp-account}

1. På RTP-plattformen går du till **Kontoinställningar.**

   ![](assets/image2014-11-29-11-3a27-3a7.png)

1. Under **Kontoinställningar**, klicka **Domän**.
1. Under **Analyser**, klicka **Google Universal Analytics**.
1. Sväng **På** de anpassade Dimensioner och händelser som behövs för att lägga till dessa data från RTP i Google Universal Analytics.
1. Ange **Indexnummer** för dimensionen justerad mot indexnumret i GUA.
1. Klicka **Spara**.

![](assets/image2014-11-29-11-31-23-version-2.png)

>[!NOTE]
>
>Indexnumret för den anpassade Dimensionen finns i GUA under Anpassade Dimensioner.
>
>Exempel: RTP-Industry Index Number är lika med 1, RTP-Organization Index Number är lika med 2.

## Ta bort gamla instrumentpaneler i Google Analytics {#remove-old-dashboards-in-google-analytics}

1. I Google Analytics. Gå till **Rapportering.**
1. Klicka på **Instrumentpaneler.**
1. Välj en **Kontrollpanel** (RTP B2B- eller RTP-prestanda)
1. Klicka **Ta bort instrumentpanel**.

![](assets/image2014-11-29-11-3a42-3a55.png)
