---
solution: Marketo Engage
product: marketo
title: Testa e-poståtergivning med Litmus
description: Marketo Engage-användare kan integrera sitt Litmus-konto för att smidigt testa innehåll som skickas i olika e-postklienter.
level: Beginner, Intermediate
feature: Email Designer
exl-id: ccef36af-362a-4ac0-9030-492e9d7f10b5
source-git-commit: 3a71e0f0da0f6201ccda73a0c8bd5b94864308c0
workflow-type: tm+mt
source-wordcount: '370'
ht-degree: 0%

---

# Testa e-poståtergivning med Litmus {#test-email-rendering-with-litmus}

Utnyttja ditt [Litmus](https://www.litmus.com/email-testing)-konto i Marketo Engage för att omedelbart se hur din e-post återges i vanliga e-postklienter.

>[!AVAILABILITY]
>
>Den här funktionen är tillgänglig för alla Marketo Engage-användare som har ett aktivt Litmus-konto.

## Litmus Enterprise Users {#litmus-enterprise}

Följande steg gäller för användare av [Litmus Enterprise-planen](https://www.litmus.com/pricing/enterprise){target="_blank"}.

1. På skärmen _Redigera e-postinnehåll_ klickar du på knappen **Simulera innehåll** .

   ![](assets/test-email-rendering-with-litmus-1.png)

1. Välj testmottagare och klicka på knappen **Återge e-post** .

   ![](assets/test-email-rendering-with-litmus-2.png){width="800" zoomable="yes"}

1. Om du inte redan har det **ansluter du ditt Litmus-konto**. Om du redan har gjort det går du vidare till steg 6.

   ![](assets/test-email-rendering-with-litmus-3.png){width="800" zoomable="yes"}

1. Ange dina inloggningsuppgifter och klicka på **Logga in**.

   >[!IMPORTANT]
   >
   >När du ansluter ditt Litmus-konto till Marketo Engage godkänner du att testmeddelanden skickas till Litmus. När du har skickat testmeddelandena hanteras dessa inte längre av Adobe. Litmus-principen för datalagring gäller därför för dessa e-postmeddelanden, inklusive personaliseringsdata som kan inkluderas i dem.

1. Klicka på **Anslut** för att slutföra integreringen.

   ![](assets/test-email-rendering-with-litmus-4.png)

1. Klicka på knappen **Kör test** om du vill generera förhandsgranskningar via e-post.

1. Se hur materialet ser ut i vanliga e-postklienter för datorer, mobiler och webben. Klicka på så många miniatyrbilder du vill förhandsgranska.

   ![](assets/test-email-rendering-with-litmus-5.png){width="800" zoomable="yes"}

   >[!NOTE]
   >
   >Lär dig hur du [anpassar din standardlista för e-postklienter](https://help.litmus.com/article/227-change-your-default-email-clients-list).

1. När du har testat klart klickar du på bakåtpilen uppe till vänster för att återgå till skärmen _Simulera innehåll_.

   ![](assets/test-email-rendering-with-litmus-6.png)

**VALFRITT STEG**: Om du bestämmer dig för att göra ändringar i e-postmeddelandet måste du klicka på **Återge e-post** för att visa dem. Se även till att klicka på knappen **Testa igen** längst upp till höger på skärmen _Förhandsvisa e-post_.

![](assets/test-email-rendering-with-litmus-7.png)

## Litmus Core-användare {#litmus-core}

Följande steg gäller för användare av [Litmus Core-planen](https://www.litmus.com/pricing/){target="_blank"}.

1. Hämta testets e-postadress i ditt Litmus-konto genom att klicka på knappen **Kopiera testadress** på skärmen _Testa_.

   ![](assets/test-email-rendering-with-litmus-8.png){width="800" zoomable="yes"}

1. I Marketo Engage går du till skärmen _Redigera e-postinnehåll_ för det önskade e-postmeddelandet och klickar på knappen **Simulera innehåll** .

   ![](assets/test-email-rendering-with-litmus-9.png){width="600" zoomable="yes"}

1. Markera testmottagarna och klicka på knappen **Skicka korrektur** .

   ![](assets/test-email-rendering-with-litmus-10.png){width="800" zoomable="yes"}

1. Ange den litermus-e-postadress du kopierade i steg 1 och klicka på **Skicka korrektur** igen.

   ![](assets/test-email-rendering-with-litmus-11.png)

1. Granska e-postmeddelandet i ditt Litmus-konto (i mappen för den e-postadress som du kopierade från Litmus).

   ![](assets/test-email-rendering-with-litmus-12.png){width="800" zoomable="yes"}
