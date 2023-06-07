---
description: Fältfrågor - Marketo Docs - produktdokumentation
title: Fältfrågor
source-git-commit: b4773137bf21eccc58a6d975d50748e8ff2a57db
workflow-type: tm+mt
source-wordcount: '160'
ht-degree: 0%

---

# Fältfrågor {#field-prompts}

Med fältuppmaningar kan du lägga till en textsträng i e-postmeddelanden som måste tas bort eller ersättas innan e-postmeddelandet kan skickas. Detta är ett bra sätt att påminna användare om att lägga till ytterligare personalisering.

Skriv ut önskad text om du vill lägga till en fältkommando. Använd ett utropstecken och omge det med klammerparenteser (se nedan).

**Exempel:**

`{{! Introduce yourself}}`

`{{! Insert name of Account Executive}}`

`{{! Add sentence that references their industry and role}}`

<p>Användarna måste ersätta den här texten med sin egen personalisering innan e-postmeddelandet kan skickas.

>[!NOTE]
>
>När du använder uppmaningar med säljkampanjer är det bäst att använda dem med manuella e-poststeg. Med de här stegen tilldelas en användare en påminnelseuppgift att skicka e-postmeddelandet, vilket ger dem möjlighet att ersätta uppmaningarna med anpassad text. Automatiska e-poststeg i Försäljningskampanjer kommer att försöka skicka automatiskt, utan att användaren tillåts att ersätta uppmaningarna. Fråga som inte ersätts kommer att göra att e-postmeddelanden inte kan skickas.
