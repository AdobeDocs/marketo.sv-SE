---
description: Agentinställningar - Marketo Docs - produktdokumentation
title: Agentinställningar
hide: true
hidefromtoc: true
feature: Dynamic Chat
source-git-commit: ea9e02d9ad52991757f137c7c2b549b98f139ba5
workflow-type: tm+mt
source-wordcount: '231'
ht-degree: 0%

---

# Agentinställningar {#agent-settings}

Anslut Outlook- eller Gmail-kalendern på fliken Kalender för användning vid schemaläggning av möten i chattbot.

![](assets/agent-settings-1.png)

När en användares kalender är ansluten till Dynamic Chat läggs de till i kön och deras kalender blir tillgänglig för webbplatsbesökare att schemalägga avtalade tider på.

>[!NOTE]
>
>Du kan ansluta en kalender per användare. Om du vill få möten i flera kalendrar måste du lägga till flera användare och låta dem ansluta sina kalendrar.

Användare kan också anpassa innehållet i den inbjudan som skickas till besökaren när de schemalägger en avtalad tid i användarens kalender. De kan också markera kryssrutan längst ned för att inkludera länken Google Meet eller Microsoft Teams (beroende på vilken kalender som var ansluten).

![](assets/agent-settings-2.png)

>[!TIP]
>
>Använd ikonen för token (klammerparenteser) för att anpassa bekräftelsemeddelanden för mötesbokningar med hjälp av person- eller företagsattribut.

## Behörigheter {#permissions}

När du konfigurerar med Outlook tilldelas Dynamic Chat följande behörigheter:

* Fullständig åtkomst till dina kalendrar
* Logga in dig och läs din profil
* Bevara åtkomst till data som du har gett åtkomst till
* Läs inställningarna för din postlåda

När du konfigurerar med Google tilldelas Dynamic Chat följande behörigheter:

* Skapa, ändra eller ta bort kalendrar
* Uppdatera enskilda kalenderhändelser
* Ändra inställningarna, inklusive vilka som kan se händelserna
* Ändra vem kalendern delas med
* Åtkomst till ditt namn, din e-postadress, språkpreferens och profilbild
