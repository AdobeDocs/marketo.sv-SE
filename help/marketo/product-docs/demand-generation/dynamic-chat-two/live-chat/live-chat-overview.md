---
description: Live Chat Overview - Marketo Docs - produktdokumentation
title: Översikt över live-chatt
hide: true
hidefromtoc: true
feature: Dynamic Chat
source-git-commit: 89c7cfb987196ebb83bada4a6ba44c760ab83ee4
workflow-type: tm+mt
source-wordcount: '238'
ht-degree: 0%

---

# Översikt över live-chatt {#live-chat-overview}

Använd chattkortet i [strömdesigner](/help/marketo/product-docs/demand-generation/dynamic-chat-two/automated-chat/stream-designer.md){target="_blank"} när ni vill att besökarna ska chatta med en handläggare.

## Använda chattkortet {#using-the-live-chat-card}

![](assets/live-chat-overview-1.png)

>[!IMPORTANT]
>
>Chattkortet måste alltid vara det sista kortet i grenen. Om kortet placeras i en slumpmässig position i grenen kan det överraska besökaren genom att plötsligt ansluta dem till en agent.

**Bästa praxis**

* Använd ett frågekort före live-chattkortet och fråga besökaren om de vill ansluta.
* När besökaren har gått med på att ansluta kan du använda informationskortet för att hämta viss information, som för-/efternamn, e-postadress, jobbtitel osv. (det rekommenderas att minst begära förnamn och e-postadress)

## Alternativ för chattkort live {#live-chat-card-options}

Om du klickar på live-chattkortet i strömmen kan du välja hur besökaren ska dirigeras. Välj bland grundrobat, en agent, anpassade regler eller ett team.

![](assets/live-chat-overview-2.png)

<table> 
 <tbody> 
  <tr> 
   <td><b>Round Robin</b></td>
   <td>Chatt tilldelas agenter i sekventiell ordning.</td>
  </tr> 
  <tr> 
   <td><b>Agent</b></td>
   <td>Välj en specifik agent som ska ta emot chatten.</td>
  </tr>
    <tr> 
   <td><b>Anpassade regler</b></td>
   <td>Alla anpassade regler rullas igenom när man överväger var besökaren ska dirigeras. Om besökaren inte uppfyller något av villkoren, FALLBACK RULE??</td>
  </tr> 
  <tr> 
   <td><b>Team</b></td>
   <td>Välj ett specifikt team som ska få chatten. Om du väljer det här alternativet tilldelas det runt en robat i teamet.</td>
  </tr>
 </tbody> 
</table>

>[!MORELIKETHIS]
>
>* [Agent Inbox](/help/marketo/product-docs/demand-generation/dynamic-chat-two/live-chat/agent-inbox.md){target="_blank"}
>* [Meddelanden](/help/marketo/product-docs/demand-generation/dynamic-chat-two/live-chat/notifications.md){target="_blank"}
