---
unique-page-id: 10098379
description: Använd snabbsynkronisering med Microsoft Dynamics för ett nytt anpassat fält - Marketo Docs - produktdokumentation
title: Använd snabbsynkronisering med Microsoft Dynamics för ett nytt anpassat fält
exl-id: c98f1443-c0dd-40e1-919b-f8110088b38a
feature: Microsoft Dynamics
source-git-commit: 431bd258f9a68bbb9df7acf043085578d3d91b1f
workflow-type: tm+mt
source-wordcount: '355'
ht-degree: 0%

---

# Använd snabbsynkronisering med Microsoft Dynamics för ett nytt anpassat fält {#use-quick-sync-with-microsoft-dynamics-for-a-new-custom-field}

Marknadsförare eller säljare vill ha ett nytt fält. Eller så kanske du har glömt en i det ursprungliga fältvalet. Eller så har du ändrat dina behov. I vilket fall som helst kan du använda Snabbsynkronisering för att synkronisera om specifika fält.

I vanliga fall använder du Snabbsynkronisering för att lägga till ett nytt fält och uppdatera värdena. I vissa fall kanske du vill synkronisera ett befintligt fält. Du kan begränsa fältsynkroniseringen baserat på ett uppdaterat eller skapat datumintervall. Se [Avancerade synkroniseringsalternativ](#Advanced_Sync_Options) nedan om du vill ha mer information.

Snabbsynkronisering kan synkronisera null-värden. Om du till exempel använder värdena A och B och ändrar ett B-värde i Dynamics till null synkroniseras null-värdet till Marketo.

## Snabbsynkronisering för alla poster {#quick-sync-for-all-records}

Så här använder du snabbsynkronisering för att synkronisera om nya fält.

1. I Marketo klickar du på **Administratör**.

   ![](assets/image2016-8-19-11-3a14-3a5.png)

1. Klicka **Microsoft Dynamics**.

   ![](assets/image2016-8-19-11-3a15-3a8.png)

1. Om synkroniseringsinformation för fält klickar du på **Redigera**.

   ![](assets/image2016-8-19-11-3a16-3a22.png)

1. Markera fälten som ska snabbsynkroniseras och klicka på **Spara**.

   ![](assets/image2016-8-25-15-3a26-3a11.png)

   >[!NOTE]
   >
   >Du kan välja fält från flera enheter.

1. Du får ett meddelande när synkroniseringen är klar.

   ![](assets/field-sync-update-notification.png)

   >[!CAUTION]
   >
   >Synkroniseringen körs sida vid sida med andra synkroniseringar, och beroende på databasens storlek kan det ta lång tid att slutföra. När ett fält finns i en kö för synkronisering kan du inte avmarkera det.

## Avancerade synkroniseringsalternativ {#advanced-sync-options}

Vad händer om du vill synkronisera ett befintligt fält, men bara vill göra det för en begränsad uppsättning data? Så här gör du.

1. Avmarkera kryssrutan för ett befintligt fält. Klicka **Spara**.

   ![](assets/image2016-8-25-16-3a16-3a32.png)

1. Öppna popup-fönstret igen och markera fältet igen.

   ![](assets/select-field-reselect-hand.png)

1. Klicka **Avancerad synkronisering**.

   ![](assets/image2016-8-25-15-3a52-3a9.png)

1. Välj **Uppdaterat** och välj ett datumintervall med datumväljarna. Klicka **Spara**.

   ![](assets/image2016-8-25-16-3a0-3a3.png)

   Det är bara poster som uppdateras mellan 16 september 2016 och 19 september 2016 som snabbsynkroniseras för fältet.

## Korrigera ej synkroniserade fält {#fixing-out-of-sync-fields}

Om ett Dynamics- och Marketo-fält inte är synkroniserat går det snabbt och enkelt att synkronisera om dem.

1. Avmarkera fältet och klicka på **Spara**.

   ![](assets/image2016-8-25-16-3a16-3a32-1.png)

1. Markera fältet igen och klicka på **Spara**. Det är allt!

   ![](assets/image2016-8-25-16-3a20-3a45.png)

   Det borde fixa det!
