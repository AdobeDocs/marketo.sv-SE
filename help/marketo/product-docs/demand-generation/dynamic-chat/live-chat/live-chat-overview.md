---
description: Live Chat Overview - Marketo Docs - produktdokumentation
title: Översikt över live-chatt
feature: Dynamic Chat
exl-id: 44e8b249-b534-4cec-a612-daa184acd266
source-git-commit: 82ff48a227f7f05d49d0189cc48df48c34190622
workflow-type: tm+mt
source-wordcount: '550'
ht-degree: 0%

---

# Översikt över live-chatt {#live-chat-overview}

Med live-chatt kan besökare på webbplatsen delta i chattsamtal i realtid med säljarna.

## Lägg till chattagenter live {#add-live-chat-agents}

Om du vill komma igång med live-chatt måste du lägga till dina live-chattagenter som [användare i Adobe Admin Console](/help/marketo/product-docs/demand-generation/dynamic-chat/setup-and-configuration/add-or-remove-chat-users.md#add-a-chat-user){target="_blank"} and give them the [Live Chat permission](/help/marketo/product-docs/demand-generation/dynamic-chat/setup-and-configuration/permissions.md){target="_blank"}. När detta är klart kan du lägga till en [live chattkort](#using-the-live-chat-card) till en ny eller befintlig dialogruta.

När besökare begär att få chatta med en agent via din dialogruta har agenterna flera [meddelandealternativ](/help/marketo/product-docs/demand-generation/dynamic-chat/live-chat/agent-inbox.md#live-chat-notifications){target="_blank"}. When they click on the notification, they'll be taken to their [Agent Inbox](/help/marketo/product-docs/demand-generation/dynamic-chat/live-chat/agent-inbox.md){target="_blank"} där de kan börja chatta med besökaren.

>[!NOTE]
>
>Agentavataren använder profilbilden från agentens Adobe-kontoprofil. Följ för att uppdatera bilden [dessa steg](https://helpx.adobe.com/manage-account/using/edit-adobe-account-personal-profile.html){target="_blank"}.

## Använda chattkortet {#using-the-live-chat-card}

Använd chattkortet i [Stream Designer](/help/marketo/product-docs/demand-generation/dynamic-chat/automated-chat/stream-designer.md){target="_blank"} när ni vill att besökarna ska chatta med en handläggare.

![](assets/live-chat-overview-1.png)

>[!IMPORTANT]
>
>Chattkortet måste alltid vara det sista kortet i grenen. Om kortet placeras i en slumpmässig position i grenen kan det överraska besökaren genom att plötsligt ansluta dem till en agent.

### Bästa praxis {#best-practices}

* Använd ett frågekort före live-chattkortet och fråga besökaren om de vill ansluta.
* När besökaren har gått med på att ansluta använder du informationskortet för att samla in en del av deras information, t.ex. för-/efternamn, e-postadress, befattning osv. (du bör begära minst förnamn och e-postadress).

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
   <td>Alla anpassade regler rullas igenom när man överväger var besökaren ska dirigeras. Om besökaren inte är berättigad till någon anpassad regel får de <a href="/help/marketo/product-docs/demand-generation/dynamic-chat/setup-and-configuration/agent-management.md#live-chat-fallback" target="_blank">live-chattmeddelande</a>.</td>
  </tr> 
  <tr> 
   <td><b>Team</b></td>
   <td>Välj ett specifikt team som ska få chatten. Om du väljer det här alternativet tilldelas det runt en robat i teamet.</td>
  </tr>
 </tbody> 
</table>

## Live Chat-meddelanden {#live-chat-notifications}

För att kunna ta emot webbläsarmeddelanden för live-chatt måste alla live-chattagenter aktivera webbläsarmeddelanden för Dynamic Chat när de uppmanas till det.

### Aktivera meddelanden {#enabling-notifications}

Live-chattagenter ser en banderoll högst upp på skärmen när de loggar in som visar&quot;Aktivera webbläsarmeddelanden för att ta emot live-chattmeddelanden&quot;. Klicka **Aktivera**.

![](assets/live-chat-overview-4.png)

Live-chattagenterna uppmanas sedan av webbläsaren att visa meddelanden. Klicka **Tillåt**.

![](assets/live-chat-overview-5.png)

Om agenter inte får webbläsarmeddelanden även efter att de har tillåtit det i webbläsaren, kan de behöva aktivera meddelanden för webbläsaren i operativsystemets meddelandeinställningar:

[Steg för Mac](https://support.apple.com/guide/mac-help/change-notifications-settings-mh40583/mac){target="_blank"}

[Steg för Windows](https://support.microsoft.com/en-us/windows/change-notification-settings-in-windows-8942c744-6198-fe56-4639-34320cf9444e){target="_blank"}

### När en live-chatt dirigeras till en agent {#when-a-live-chat-is-routed-to-an-agent}

När en live-chatt dirigeras till en agent ser de en blå banderoll högst upp på skärmen och ber dem att godkänna.

![](assets/live-chat-overview-3.png)

>[!TIP]
>
>Du kan också konfigurera webbläsarmeddelanden, som meddelar dig om du inte är inloggad på Dynamic Chat.
>
>* Aktivera webbläsarmeddelanden i [Google Chrome](https://support.google.com/chrome/answer/3220216?hl=en&amp;co=GENIE.Platform%3DDesktop){target="_blank"}
>* Aktivera webbläsarmeddelanden i [Mozilla Firefox](https://support.mozilla.org/en-US/kb/push-notifications-firefox){target="_blank"}

### Saker att notera {#things-to-note}

* Agenter har 45 sekunder på sig att svara innan meddelandet&quot;Godkänn chatt&quot; går ut
* Det finns för närvarande en gräns på 10 chatt per agent

>[!MORELIKETHIS]
>
>[Agent Inbox](/help/marketo/product-docs/demand-generation/dynamic-chat/live-chat/agent-inbox.md){target="_blank"}
