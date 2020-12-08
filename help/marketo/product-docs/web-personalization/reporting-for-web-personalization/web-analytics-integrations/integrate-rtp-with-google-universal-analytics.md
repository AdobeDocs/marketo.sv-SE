---
unique-page-id: 4720125
description: Integrera RTP med Google Universal Analytics - Marketo Docs - produktdokumentation
title: Integrera RTP med Google Universal Analytics
translation-type: tm+mt
source-git-commit: 47b2fee7d146c3dc558d4bbb10070683f4cdfd3d
workflow-type: tm+mt
source-wordcount: '432'
ht-degree: 0%

---


# Integrera RTP med Google Universal Analytics {#integrate-rtp-with-google-universal-analytics}

## Intro {#intro}

Utnyttja Google Universal Analytics (GUA) med Marketo Real-Time Personalization&#39;s (RTP) firmographic and personalization data för att bättre mäta och analysera era webbmarknadsföringssatsningar.

I det här inlägget beskrivs hur du konfigurerar och integrerar plattformen Marketo Real-Time Personalization (RTP) med Google Universal Analytics-konton (GUA). RTP-data kan läggas in i ditt GUA-konto så att du kan se resultatet för organisationer, branscher, företagsgrafik och RTP-segment som besöker din webbplats.

**Google Universal Analytics**

Google Universal Analytics med RTP:s data ger er en bättre förståelse för hur B2B-användare interagerar med ert onlineinnehåll och hjälper er att mäta och få bättre resultat av era personaliseringskampanjer. [Läs mer om Google Universal Analytics](https://support.google.com/analytics/answer/2790010/?hl=en&amp;authuser=1).

>[!NOTE]
>
>**`For Google Tag Manager Users Only`**
>
>Ingen kodning eller specialkonfiguration behöver göras. Se till att du slutför följande checklista:
>
>* `RTP dimensions are created in Google Universal Analytics`
>* [RTP-taggen har installerats korrekt i Google Tag Manager](https://docs.marketo.com/display/public/DOCS/Implementing+RTP+using+Google+Tag+Manager)
>* `Google Universal Analytics Integration is enabled in the RTP's Account Settings`
>* [Google Universal Analytics-taggen är korrekt konfigurerad i Google Tag Manager](https://support.google.com/tagmanager/answer/6107124?hl=en)
>* [Google Tag Manager-taggen är korrekt installerad på webbplatsen](https://developers.google.com/tag-manager/quickstart)

>



## Konfigurera anpassade Dimensioner i GUA {#set-up-custom-dimensions-in-gua}

1. I Google Analytics

   1. Gå till **Admin**
   1. Välj **konto.**
   1. Markera **egenskapen.**
   1. Välj **Anpassade definitioner **och **Anpassade Dimensioner.**

      ![](assets/image2014-11-29-11-3a2-3a32.png)

1. Lägg till en ny anpassad dimension. Klicka **+Ny anpassad Dimension**

   ![](assets/image2014-11-29-11-3a8-3a16.png)

1. Lägg till följande **anpassade Dimensioner:**

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
>**Namnen på anpassade Dimensioner** måste vara exakt som de definieras i tabellen ovan (annars visas inte anpassade RTP-instrumentpaneler och rapporter i GUA korrekt)

1. Lägg till **Name. **Välj scope som **session.** Klicka på **Skapa.**

   ![](assets/image2014-11-29-11-3a12-3a51.png)

Listan Anpassad Dimension bör se ut så här.

![](assets/image2014-11-29-11-36-50-version-2.png)

När du har aktiverat anpassade Dimensioner i GUA går du till RTP-plattformen för att aktivera de här dimensionerna i RTP.

## Aktivera GUA-integreringen i ditt RTP-konto {#activate-the-gua-integration-in-your-rtp-account}

1. Gå till **Kontoinställningar på RTP-plattformen.**

   ![](assets/image2014-11-29-11-3a27-3a7.png)

1. Klicka på **Domän under** Kontoinställningar **.**
1. Under **Analytics, **klicka på **Google Universal Analytics**.
1. Aktivera **berörda anpassade Dimensioner och händelser för** att lägga till dessa data från RTP till Google Universal Analytics.
1. Ange **indexnumret** för dimensionen justerad mot indexnumret i GUA.
1. Klicka på **Spara**.

![](assets/image2014-11-29-11-31-23-version-2.png)

>[!NOTE]
>
>Indexnumret för den anpassade Dimensionen finns i GUA under Anpassade Dimensioner.
>
>Exempel: RTP-Industry Index Number är lika med 1, RTP-Organization Index Number är lika med 2.

## Ta bort gamla instrumentpaneler i Google Analytics {#remove-old-dashboards-in-google-analytics}

1. I Google Analytics. Gå till **Rapportering.**
1. Klicka på **Kontrollpaneler.**
1. Välj en **Dashboard **(RTP B2B- eller RTP-prestanda)
1. Klicka på **Ta bort instrumentpanel**.

![](assets/image2014-11-29-11-3a42-3a55.png)

