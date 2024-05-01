---
description: Återanropsfunktioner - Marketo Docs - produktdokumentation
title: Återanropsfunktioner
feature: Dynamic Chat
exl-id: 5ae7f6cb-5c57-4257-8a1a-992c9602cfaa
source-git-commit: f355022fb7e6f733bb7485229e395b0fe1a9818f
workflow-type: tm+mt
source-wordcount: '616'
ht-degree: 0%

---

# Återanropsfunktioner {#callback-functions}

Du kan använda Dynamic Chat widget-återanropsfunktioner för att skicka konversationshändelser till andra tredjepartsplattformar.

## Komma igång {#getting-started}

Den här händelsen anger att widgeten Dynamic Chat är klar att användas och utlöses när alla skript som är relaterade till Dynamic Chat läses in på webbsidan.

```javascript
window.addEventListener('adobedx.conversations.ready', () => { 
    // code here will execute when chatbot scripts are loaded in a webpage 
}); 
```

## Konversationshändelser {#conversation-events}

Dessa händelser är relaterade till en konversation som är riktad till en viss sida för en viss besökare.

### Konversationen utlöstes

En konversation (t.ex. en dialogruta) som riktar sig till en webbplatsbesökare är löst och chattbot visas för dem.

```javascript
window.addEventListener('adobedx.conversations.ready', () => { 
    const {addListener, Enum} = window.AdobeDX; 
    addListener(Enum.Events.CONVERSATION_TRIGGERED, (event) => { 
 // code here will execute when the chatbot is loaded for a visitor 
    }); 
});  
```

### Konversationen har aktiverats {#conversation-engaged}

Besökaren var engagerad (t.ex. med sitt första svar) med chattbot.

```javascript
window.addEventListener('adobedx.conversations.ready', () => { 
    const {addListener, Enum} = window.AdobeDX; 
    addListener(Enum.Events.CONVERSATION_ENGAGED, (event) => { 
 // code here will execute when a visitor engages with the chatbot 
     }); 
}); 
```

### Konversationen har slutförts {#conversation-completed}

Besökaren har nått slutet av konversationen.

```javascript
window.addEventListener('adobedx.conversations.ready', () => { 
    const {addListener, Enum} = window.AdobeDX; 
    addListener(Enum.Events.CONVERSATION_COMPLETED, (event) => { 
 // code here will execute when a conversation is completed 
     }); 
}); 
```

### Konversationen har avslutats

Besökaren har avslutat konversationen innan han eller hon är klar.

```javascript
window.addEventListener('adobedx.conversations.ready', () => { 
    const {addListener, Enum} = window.AdobeDX; 
    addListener(Enum.Events.CONVERSATION_CLOSED, (event) => { 
 // code here will execute when a conversation is closed 
    }); 
}); 
```

The `event` parameter är ett objekt med metadata som är relaterade till konversationen. Du kan komma åt dessa metadata via `event.data`.

Här är några viktiga metadatavärden som du kan komma åt:

<table>
<thead>
  <tr>
    <th style="width:75%">Metadata</th>
    <th style="width:25%">Attribut</th>
  </tr>
</thead>
<tbody>
  <tr>
    <td>Konversationsnamn</td>
    <td>payload.name</td>
  </tr>
  <tr>
    <td>Konversations-ID</td>
    <td>payload.id</td>
  </tr>
  <tr>
    <td>Konversationstyp (dialog-/konversationsflöde)</td>
    <td>payload.type</td>
  </tr>
  <tr>
    <td>Användargränssnittstyp (popup/chatbot/inline)</td>
    <td>payload.uiType</td>
  </tr>
  <tr>
    <td>Sessions-ID</td>
    <td>payload.sid</td>
  </tr>
</tbody>
</table>

## Indatahändelser för besökare

Dessa händelser utlöses när en besökare som deltar i en konversation lämnar sin kontaktinformation (t.ex. telefonnummer eller e-postadress). Nedan visas de händelser som hör till den här kategorin.

### Telefonnummer {#phone-number}

Den här händelsen utlöses när en besökare anger sitt telefonnummer under konversationen.

```javascript
window.addEventListener('adobedx.conversations.ready', () => { 
    const {addListener, Enum} = window.AdobeDX; 
    addListener(Enum.Events.CONVERSATION_INPUT_PHONE, (event) => { 
 // code here will execute when a visitor provides their phone number 
    }); 
});  
```

### E-post-ID {#email-id}

Den här händelsen utlöses när en besökare anger sin e-postadress under konversationen.

```javascript
window.addEventListener('adobedx.conversations.ready', () => { 
    const {addListener, Enum} = window.AdobeDX; 
    addListener(Enum.Events.CONVERSATION_INPUT_EMAIL, (event) => { 
 // code here will execute when a visitor provides their email address 
    }); 
}); 
```

The `event` parameter är ett objekt med metadata som är relaterade till konversationen. Du kan komma åt dessa metadata via `event.data`.

Här är några viktiga metadatavärden som du kan komma åt:

<table>
<thead>
  <tr>
    <th style="width:75%">Metadata</th>
    <th style="width:25%">Attribut</th>
  </tr>
</thead>
<tbody>
  <tr>
    <td>Konversationsnamn</td>
    <td>payload.name</td>
  </tr>
  <tr>
    <td>Konversations-ID</td>
    <td>payload.id</td>
  </tr>
  <tr>
    <td>Konversationstyp (dialog-/konversationsflöde)</td>
    <td>payload.type</td>
  </tr>
  <tr>
    <td>Användargränssnittstyp (popup/chatbot/inline)</td>
    <td>payload.uiType</td>
  </tr>
  <tr>
    <td>Sessions-ID</td>
    <td>payload.sid</td>
  </tr>
</tbody>
</table>

## Mötesbokningshändelser {#meeting-booking-events}

Dessa händelser utlöses när en besökare bokar ett möte med din företagsrepresentant.

Nedan visas de händelser som hör till den här kategorin.

### Mötet har bokats {#meeting-booked}

Den här händelsen utlöses när en besökare bokar ett möte i en agentkalender.

```javascript
window.addEventListener('adobedx.conversations.ready', () => { 
    const {addListener, Enum} = window.AdobeDX; 
    addListener(Enum.Events.CONVERSATION_MEETING_BOOKED, (event) => { 
 // code here will execute when a meeting is booked 
    }); 
}); 
```

The `event` parameter är ett objekt med metadata som är relaterade till konversationen. Du kan komma åt dessa metadata via `event.data`.

Här är några viktiga metadatavärden som du kan komma åt:

<table>
<thead>
  <tr>
    <th style="width:75%">Metadata</th>
    <th style="width:25%">Attribut</th>
  </tr>
</thead>
<tbody>
  <tr>
    <td>Konversationsnamn</td>
    <td>payload.name</td>
  </tr>
  <tr>
    <td>Konversations-ID</td>
    <td>payload.id</td>
  </tr>
  <tr>
    <td>Konversationstyp (dialog-/konversationsflöde)</td>
    <td>payload.type</td>
  </tr>
  <tr>
    <td>Användargränssnittstyp (popup/chatbot/inline)</td>
    <td>payload.uiType</td>
  </tr>
  <tr>
    <td>Sessions-ID</td>
    <td>payload.sid</td>
  </tr>
  <tr>
    <td>Agentnamn</td>
    <td>payload.agentName</td>
  </tr>
  <tr>
    <td>Agent-ID</td>
    <td>payload.agentID</td>
  </tr>
  <tr>
    <td>Mötesinformation</td>
    <td>payload.meetingInfo</td>
  </tr>
</tbody>
</table>

## Live Chat Events {#live-chat-events}

Dessa händelser utlöses när en besökare ansluter till en live-agent under deras interaktion med chattbot.

Nedan visas de händelser som hör till den här kategorin.

### Live-chatt begärd {#live-chat-requested}

Den här händelsen utlöses när en besökare väljer alternativet att chatta med en live-agent och en tillgänglig agent håller på att lösas.

```javascript
window.addEventListener('adobedx.conversations.ready', () => { 
    const {addListener, Enum} = window.AdobeDX; 
    addListener(Enum.Events.CONVERSATION_LIVE_CHAT_REQUESTED, (event) => { 
 // code here will execute when a visitor requests a live chat 
    }); 
}); 
```

### Live-chatten har initierats {#live-chat-initiated}

Den här händelsen utlöses när en besökare väljer alternativet att chatta med en live-agent och en agent godkänner chatten.

```javascript
window.addEventListener('adobedx.conversations.ready', () => { 
    const {addListener, Enum} = window.AdobeDX; 
    addListener(Enum.Events.CONVERSATION_LIVE_CHAT_INITIATED, (event) => { 
 // code here will execute after a live agent accepts the chat 
    }); 
}); 
```

### Live-chatt avslutad {#live-chat-ended}

Den här händelsen utlöses när en konversation mellan en besökare och den aktiva agenten avslutas.

```javascript
window.addEventListener('adobedx.conversations.ready', () => { 
    const {addListener, Enum} = window.AdobeDX; 
    addListener(Enum.Events.CONVERSATION_LIVE_CHAT_ENDED, (event) => { 
 // code here will execute when a live chat is ended 
    }); 
}); 
```

### Timeout för live-chatt {#live-chat-timeout}

Den här händelsen utlöses när en live-chattkonversation avbryts på grund av att besökaren slutar svara eller att de har släppts.

```javascript
window.addEventListener('adobedx.conversations.ready', () => { 
    const {addListener, Enum} = window.AdobeDX; 
    addListener(Enum.Events.CONVERSATION_LIVE_CHAT_REQUEST_TIMEOUT, (event) => { 
 // code here will execute when a visitor abandons a live chat 
    }); 
}); 
```

The `event` parameter är ett objekt med metadata som är relaterade till konversationen. Du kan komma åt dessa metadata via `event.data`.

Här är några viktiga metadatavärden som du kan komma åt:

<table>
<thead>
  <tr>
    <th style="width:75%">Metadata</th>
    <th style="width:25%">Attribut</th>
  </tr>
</thead>
<tbody>
  <tr>
    <td>Konversationsnamn</td>
    <td>payload.name</td>
  </tr>
  <tr>
    <td>Konversations-ID</td>
    <td>payload.id</td>
  </tr>
  <tr>
    <td>Konversationstyp (dialog-/konversationsflöde)</td>
    <td>payload.type</td>
  </tr>
  <tr>
    <td>Användargränssnittstyp (popup/chatbot/inline)</td>
    <td>payload.uiType</td>
  </tr>
  <tr>
    <td>Sessions-ID</td>
    <td>payload.sid</td>
  </tr>
  <tr>
    <td>Agentnamn</td>
    <td>payload.agentName</td>
  </tr>
  <tr>
    <td>Agent-ID</td>
    <td>payload.agentID</td>
  </tr>
</tbody>
</table>

Om du vill skicka någon av dessa händelser till en analysplattform som Adobe Analytics eller Google Analytics måste du lägga till deras respektive spårningsanrop i dessa Dynamic Chat-händelser. Det skulle se ut ungefär som exemplet nedan.

```javascript
window.addEventListener('adobedx.conversations.ready', () => { 
    const {addListener, Enum} = window.AdobeDX; 
    addListener(Enum.Events.CONVERSATION_TRIGGERED, (event) => { 
 // Enter Adobe Analytics or Google Analytics function here 
    ga('send', 'event', { 
      eventCategory: Dynamic Chat Conversations', 
      eventAction: 'Conversation Triggered', 
      eventLabel: event.data.payload.id, 
    }); 
    }); 
}); 
```
