---
unique-page-id: 11378812
description: Upptäck konton - Marketo Docs - produktdokumentation
title: Identifiera konton
exl-id: 90da4ae0-0a12-48bd-8bae-a7431d2cf4f4
feature: Target Account Management
source-git-commit: dd4c8472ec3f453462bd8046daf70c89c587724a
workflow-type: tm+mt
source-wordcount: '558'
ht-degree: 0%

---

# Identifiera konton {#discover-accounts}

Använd alternativet Discover för att identifiera potentiella målkonton.

## Identifiera CRM-konton {#discover-crm-accounts}

Identifiera potentiella målkonton från CRM.

>[!NOTE]
>
>När du har anslutit CRM till Marketo TAM visar **Identifiera CRM-konton** alla CRM-konton och relevant information som hjälper dig att välja rätt namngivna konton. Marketo lägger till ytterligare information utöver vad som tas emot från CRM.

**Personer** (i Identifiera CRM-konton och Identifiera Marketo-företag): Innehåller både kontakter och leads. Leads kan identifieras med Marketo [lead-to-account-matchning](/help/marketo/product-docs/target-account-management/target/named-accounts/lead-to-account-matching.md).

**Potentiella personer** (I Identifiera CRM-konton och Identifiera Marketo-företag): Visar hur många leads Marketo hittade som eventuellt kan tillhöra ett CRM-konto.

**Anpassat CRM-fält** (endast i Identifiera CRM-konton): Detta hjälper dig att justera din försäljnings- och marknadsföringsorganisation för att välja rätt målkonton. När du har [mappat det anpassade CRM-fältet](/help/marketo/product-docs/target-account-management/setup-tam/create-a-custom-field-for-crm-discovery.md) med Marketo TAM visar vi mappade data som hjälper dig att identifiera målkonton.

1. Klicka på listrutan **Nytt** i Namngivna konton och välj **Identifiera CRM-konton**.

   ![](assets/disc-crm-one.png)

1. Ett nytt fönster/en ny flik öppnas. Markera de CRM-konton som du vill lägga till i dina namngivna konton och klicka på **Nästa**.

   ![](assets/disc-crm-two.png)

1. Förhandsgranskningsskärmen bekräftar hur många markeringar du har gjort. Klicka på **Skapa**.

   ![](assets/disc-three.png)

   Det är allt som finns till det!

   ![](assets/disc-four.png)

## Upptäck Marketo Companies {#discover-marketo-companies}

Identifiera rätt företag för målinriktning.

>[!NOTE]
>
>I Upptäck Marketo Companies ser du Marketo-företag som inte kommer från din CRM.

1. Klicka på listrutan **Nytt** i Namngivna konton och välj **Upptäck Marketo-företag**.

   ![](assets/one-1.png)

1. Ett nytt fönster/en ny flik öppnas. Markera de företag som du vill lägga till i dina namngivna konton och klicka på **Nästa**.

   ![](assets/disc-comp-two.png)

   >[!NOTE]
   >
   >I Upptäck Marketo Companies och Discover CRM arbetar Marketo automatiskt:
   >
   >* Söker efter personer från din Marketo-databas som har det företaget angivet i sin lista. Om du ser flera värden för vissa attribut (t.ex. Bransch) beror det på att Marketo hittade olika värden för de enskilda personerna. Attributet med flest träffar
   >
   >I **Identifiera endast CRM**, Marketo automatiskt:
   >
   >* Synkroniserar och associerar CRM-kontakter med det namngivna kontot
   >
   >I **Upptäck endast Marketo Companies**, Marketo automatiskt:
   >
   >* Filtrerar ut de flesta Internetleverantörer och offentliga domäner (t.ex. yahoo.com, gmail.com) som företagsnamn
   >
   >* Tar bort CRM-konton. Om du har &quot;Acme&quot; i en post och &quot;Acme Inc&quot; (eller något av följande suffix: Co, Corp, Corporation, GmbH, Inc, Incorporated, LLC, LLP, LP, Ltd, PA, PC, PLC, PLLC), sammanfogar vi dem i TAM som &quot;Acme&quot;

1. Klicka på nedåtpilen under kolumnen Namngivet konto för att visa listrutan.

   ![](assets/disc-comp-three.png)

   >[!CAUTION]
   >
   >Framöver kommer alla nya personer från dessa utvalda företag automatiskt att tilldelas sina respektive namngivna konton. Kontrollera dessa företag och se till att de har tilldelats rätt namngivet konto.

1. Om du vill välja ett befintligt konto klickar du på listrutan **Namngivet konto**, väljer önskat konto och klickar sedan på **Nästa**.

   ![](assets/disc-comp-four.png)

   Du kan också skapa ett nytt namngivet konto genom att skriva det önskade namnet direkt i listrutan. Klicka utanför rutan när du är klar..

   ![](assets/disc-comp-five.png)

   ...så ser du ditt nya namngivna konto. Då klickar du bara på **Nästa**, som i steg 4.

   ![](assets/disc-comp-six.png)

1. Klicka på **Skapa**.

   ![](assets/disc-comp-seven.png)

   Snyggt jobbat!

   ![](assets/disc-co-six.png)

>[!NOTE]
>
>Om det finns en felmatchning mellan de CRM-konton du har valt och det som finns i Identifiera CRM-stödraster beror det troligen på ett eller flera av följande:
>
>* Har olika CRM-konton med liknande namn som har tagits bort
>* Nästa schemalagda synkronisering har inte utförts än

>[!MORELIKETHIS]
>
>[Lead till kontomatchning](/help/marketo/product-docs/target-account-management/target/named-accounts/lead-to-account-matching.md)
