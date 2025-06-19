---
solution: Marketo Engage
product: marketo
title: Spam Assassin
description: TEXT GES HÄR
level: Beginner, Intermediate
feature: Email Designer
hide: true
hidefromtoc: true
source-git-commit: bfa1bc900c2adc263e634a81440b77bef2976d3b
workflow-type: tm+mt
source-wordcount: '183'
ht-degree: 0%

---

# Spam Assassin {#spam-assassin}

Med SpamAssassin i Marketo Engage kan du testa ditt e-postinnehåll och se sannolikheten för att Internet-leverantörer/postlådeleverantörer markerar det som skräppost.

SpamAssassin analyserar ditt innehåll och tilldelar ett poängvärde baserat på olika kriterier. Ju lägre poäng, desto bättre. Det är viktigt att behålla en låg poäng eftersom e-post med hög poäng kan påverka den övergripande leveransförmågan negativt.

## Åtkomst till skräppostrapporten {#access-the-spam-report}

1. Klicka på knappen **Skräppostrapport** på skärmen Simulera.

SCREENSHOT

1. En skräppostrapport genererar.

SCREENSHOT

1. Kontrollera poängen och beskrivningarna för varje objekt.

>[!IMPORTANT]
>
>Om poängen är högre än 5 kan din e-postadress vara blockerad eller markerad som skräppost vid leverans.

1. Om du anser att poängen är för höga redigerar du ditt innehåll i e-post-Designer och kör sedan skräppostrapporten igen tills poängen är där du vill att den ska vara.

SCREENSHOT

>[!NOTE]
>
>Spam score härleds via SpamAssassin, och reglerna ägs inte av Adobe. Mer information om dessa regler finns i [SpamAssassin-dokumentationen](https://spamassassin.apache.org/#_blank). En fullständig lista över fel [visas här](https://spamassassin.apache.org/old/tests_3_0_x.html?utm_source=chatgpt.com).
