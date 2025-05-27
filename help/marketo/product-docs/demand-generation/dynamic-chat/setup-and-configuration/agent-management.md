---
description: Agenthantering - Marketo Docs - produktdokumentation
title: Agenthantering
feature: Dynamic Chat
exl-id: 151d8cf2-a5b7-43c4-8418-cc22252108b2
source-git-commit: 42e2a23c1c451c61fd62237fd1305924b51437b2
workflow-type: tm+mt
source-wordcount: '284'
ht-degree: 0%

---

# Agenthantering {#agent-management}

I Agenthantering kan du visa en lista med agenter i din Dynamic Chat-instans, hantera team och ange dina reservregler.

![](assets/agent-management-1.png)

## Agenter {#agents}

På den här fliken visas alla agenter i din Dynamic Chat-instans och den innehåller information om deras namn, e-postadress, status för live-chatt med mera.

![](assets/agent-management-2.png){width="800" zoomable="yes"}

>[!NOTE]
>
>Ser du inte en agent som du _just_ har lagt till? Det kan ta upp till två timmar innan de visas här när de har lagts till i Adobe Admin Console.

## Team {#teams}

Administratörer kan skapa team med agenter för att underlätta dirigering till specifika grupper av säljare.

>[!AVAILABILITY]
>
>Åtkomst till team kräver en Dynamic Chat Prime-prenumeration. Kontakta Adobe Account Team (din kontoansvarige) för mer information.

![](assets/agent-management-3.png)

### Skapa ett team {#create-a-team}

1. Klicka på **+ Skapa team**.

   ![](assets/agent-management-4.png)

1. Ge teamet ett namn.

   ![](assets/agent-management-5.png)

1. Klicka på listrutan **Lägg till agenter** och välj önskade agenter.

   ![](assets/agent-management-6.png)

1. Klicka på **Skapa**.

   ![](assets/agent-management-7.png)

## Reservregler {#fallback-rules}

### Mötesreserv {#meeting-fallback}

Välj ett standardmeddelande (systemmeddelande) eller skriv ett anpassat meddelande så att besökarna kan se när mötesbokningen är otillgänglig.

![](assets/agent-management-8.png)

### Live Chatt Fallback {#live-chat-fallback}

Välj ett standardmeddelande (systemmeddelande) eller skriv ett anpassat meddelande så att besökarna kan se när Live-chatten är otillgänglig.

![](assets/agent-management-9.png)

>[!NOTE]
>
>* Om du markerar kryssrutan _Inkludera mötesbokningsalternativ_ får chattbesökaren möjlighet att boka ett möte när inga agenter är tillgängliga för live-chatt.
>
>* **För anpassade regler/team som ett Live-chattkort**: Vid sökning efter agenter, om de inte är tillgängliga eller inte kan ansluta, återgår det till Round Robin för att försöka med &quot;Tillgängliga agenter&quot; (alla som är tillgängliga vid den tidpunkten oavsett vilken routningslogik/regel som placerades i strömmen).

>[!TIP]
>
>När du skapar ett anpassat meddelande kan du formatera teckensnittet, använda länkar och till och med infoga känslolägesikoner! `:)`
