---
solution: Marketo Engage
product: marketo
title: Rapport om skräppost
description: Lär dig hur du använder SpamAssassin för att testa ditt e-postinnehåll och se sannolikheten för att det markeras som skräppost.
level: Beginner, Intermediate
feature: Email Designer
exl-id: 6954850e-2b1a-4bf5-b918-1c54d6926b7e
source-git-commit: 26573c20c411208e5a01aa7ec73a97e7208b35d5
workflow-type: tm+mt
source-wordcount: '228'
ht-degree: 0%

---

# Rapport om skräppost {#email-spam-report}

Med SpamAssassin i Marketo Engage kan du testa ditt e-postinnehåll och se sannolikheten för att Internet-leverantörer/postlådeleverantörer markerar det som skräppost.

SpamAssassin analyserar ditt innehåll och tilldelar ett poängvärde baserat på olika kriterier. Ju lägre poäng, desto bättre. Det är viktigt att behålla en låg poäng eftersom e-post med hög poäng kan påverka den övergripande leveransförmågan negativt.

## Åtkomst till skräppostrapporten {#access-the-spam-report}

1. Klicka på **Simulera innehåll** i ditt e-postmeddelande.

   ![](assets/email-spam-report-1.png){width="600" zoomable="yes"}

   >[!NOTE]
   >
   >Om du inte redan har lagt till en testprofil måste du göra det direkt efter steg 1.

1. Klicka på knappen **Spam-rapport**.

   ![](assets/email-spam-report-2.png)

1. En skräppostrapport genererar.

   ![](assets/email-spam-report-3.png){width="600" zoomable="yes"}

1. Kontrollera poängen och beskrivningarna för varje objekt.

   >[!IMPORTANT]
   >
   >Om poängen är högre än 5 kan e-postmeddelandet blockeras av mottagaren eller markeras som skräppost vid leveransen.

1. Om du anser att poängen är för höga kan du redigera ditt innehåll i e-postmeddelandet i Designer baserat på rapportens resultat och sedan köra **skräppostrapporten** igen.

   ![](assets/email-spam-report-4.png){width="800" zoomable="yes"}

När poängen är som du vill ha dem kan de skickas.

![](assets/email-spam-report-5.png){width="800" zoomable="yes"}

>[!NOTE]
>
>Spam score härleds via SpamAssassin, och **regler ägs inte av Adobe**. Mer information om dessa regler finns i [SpamAssassin-dokumentationen](https://spamassassin.apache.org/#_blank){target="_blank"}. En fullständig lista över fel [visas här](https://spamassassin.apache.org/old/tests_3_0_x.html){target="_blank"}.
