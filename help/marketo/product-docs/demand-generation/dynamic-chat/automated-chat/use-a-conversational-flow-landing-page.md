---
description: Använd en startsida för konversationsflöde - Marketo Docs - produktdokumentation
title: Använda en startsida för konversationsflöde
hide: true
hidefromtoc: true
feature: Dynamic Chat
source-git-commit: 5ef17e8c3988706a4d95332312ffb035f35bb269
workflow-type: tm+mt
source-wordcount: '226'
ht-degree: 0%

---

# Använda en startsida för konversationsflöde{#use-a-conversational-flow-landing-page}

Genom att bädda in ett konversationsflöde i Dynamic Chat direkt på en landningssida i Marketo Engage kan besökare schemalägga ett möte via Dynamic Chat utan att behöva fylla i ett formulär eller interagera med en chattbot.

>[!PREREQUISITES]
>
>Skapa en enkel [Konversationsflöde](/help/marketo/product-docs/demand-generation/dynamic-chat/automated-chat/create-a-conversational-flow.md) som bara innehåller **Mötesbokning** kort.

## Guidade landningssidor {#guided-landing-pages}

Bädda in följande kod i mallen för guidad landningssida: `<div class="mktoConversation" id="exampleConversation" mktoName= "Example Conversation"></div>`.

Öppna mallen för guidad landningssida i redigeraren och välj platshållaren för konversationsflöde.

Klicka på listrutan Konversationsflöde och välj den CF som du skapade i steg 1.

Behåll alltid leveranstyp som **Textbunden**. Klicka **Infoga**.

Det konversationsflöde du just angav visas som ett element till höger.

SCREENSHOT

>[!NOTE]
>
>För närvarande visas inte konversationsflödet i huvudförhandsvisningsfönstret.

## Landningssidor i fri form {#free-form-landing-pages}

Text


ANMÄRKNINGAR FRÅN STEVE-MÖTET

guidad lp, nytt div-id för mall, välj konverteringsflöde

frihandstlp, ikonen för att ta över - caveat: add note - När du placerar cf i redigeraren visas inte en förhandsgranskning (ingen platshållare heller) - &quot;du kommer inte att se en förhandsgranskning&quot; - på sidofältet ser de att cf finns på sidan - guidad lp listar det som ett element - använd &quot;just nu&quot; när du förklarar - funktionen blir tillgänglig en vecka på 22 och
