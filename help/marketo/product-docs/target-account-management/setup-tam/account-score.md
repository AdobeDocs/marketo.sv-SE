---
unique-page-id: 11380774
description: Kontopoäng - Marketo Docs - produktdokumentation
title: Kontopoäng
exl-id: 68fb5f41-f715-4a4d-b4da-9db4dc38d67d
source-git-commit: 72e1d29347bd5b77107da1e9c30169cb6490c432
workflow-type: tm+mt
source-wordcount: '356'
ht-degree: 0%

---

# Kontopoäng {#account-score}

Kontobedömning är en viktig del av kontohantering. Det hjälper er att fastställa nivån på engagemanget i era konton.

## Vad är kontobedömning? {#what-is-account-scoring}

Det är en systematisk strategi som är utformad för att hjälpa säljare och marknadsföringsteam att identifiera och prioritera de företag (inklusive potentiella kunder) som mest sannolikt gör ett köp.

I B2B-inköpsprocessernas komplexa värld är det sällan en enskild person fattar ett inköpsbeslut. Det finns ofta olika roller som är involverade, var och en med egna behov. Kontobaserad poängsättning tar hänsyn till detta genom att slå samman poängen från flera leads och tillhandahålla en poäng på kontonivå.

## Vanliga exempel {#common-examples}

<table> 
 <tbody>
  <tr>
   <td><strong>Resultat för kontoengagemang</strong></td> 
   <td>Djup på engagemanget baserat på beteendeaktiviteter som spåras i olika kanaler (t.ex. e-post, webben och annonser) från personer i specifika målkonton.</td>
  </tr>
  <tr>
   <td><strong>Räntepoäng för kontoprodukt</strong></td>
   <td>Personer från målkonton som visar intresse för innehållet från en viss produkt (t.ex. nedladdning av ett faktablad).</td> 
  </tr>
  <tr>
   <td><strong>Resultat för webbengagemang för konto</strong></td>
   <td>Personer från målkonton som besöker webbkanalen. Samma poäng kan skapas för att mäta kanalengagemang från e-post, annonser eller andra kanaler.</td> 
  </tr>
 </tbody>
</table>

## Så här konfigurerar du kontopoäng {#how-to-configure-account-score}

>[!NOTE]
>
>Om du vill beräkna kontopoäng måste du först skapa poängpoäng. Marketo TAM samlar automatiskt in poäng från leads till kontouppgifter. Vi tar till exempel två av de ovanstående exemplen (_Räntepoäng för kontoprodukt_ och _Resultat för webbengagemang för konto_).
>
>Skapa först fält för lead-poäng som hämtar relevant information från varje lead i ett målkonto.\
>Tilldela sedan dessa lead scores till respektive kontopoäng:\
>Räntepoäng för kontoprodukt = SUM (Lead Product Interest Score)\
>Konto Web Engagement Score = SUM (Lead Web Engagement Score)

>[!NOTE]
>
>Användare kan skapa flera poäng för kontointeraktion och tilldela olika personpoäng till olika poäng.

När du har konfigurerat lead-poängen fortsätter du genom att följa stegen nedan.

1. Klicka **Administratör**.

   ![](assets/one-1.png)

1. Klicka **Hantering av målkonto**.

   ![](assets/account-score-2.png)

1. Klicka på Betygsfält **Redigera**.

   ![](assets/account-score-3.png)

   >[!NOTE]
   >
   >Du kan välja upp till **fem** fält för att beräkna kontouppsättningen.

1. Ange namnet på kontouppsättningen och klicka på **Välj personpoäng** och välj bakgrundsmusik.

   ![](assets/four.png)

1. Klicka **+Lägg till** för att lägga till fler bakgrundsmusik.

   ![](assets/five.png)

1. Lägg till alla önskade bakgrundsmusik. Klicka **Spara** när det är klart.

   ![](assets/six.png)
