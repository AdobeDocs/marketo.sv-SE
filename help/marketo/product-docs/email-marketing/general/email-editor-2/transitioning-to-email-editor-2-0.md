---
unique-page-id: 11373011
description: Övergång till e-postredigeraren 2.0 - Marketo Docs - produktdokumentation
title: Övergår till Email Editor 2.0
exl-id: eb9ec8cc-d6e8-4839-a4d9-608d2f264cbb
feature: Email Editor
source-git-commit: 431bd258f9a68bbb9df7acf043085578d3d91b1f
workflow-type: tm+mt
source-wordcount: '631'
ht-degree: 0%

---

# Övergår till Email Editor 2.0 {#transitioning-to-email-editor}

Från och med versionen från juni 19 har alla Marketo-prenumerationer övergått till Email Editor 2.0. [Läs mer](https://nation.marketo.com/docs/DOC-7038) om borttagningen av e-postredigeraren 1.0.

E-post och e-postmallar i din prenumeration ska ha ett versionsnummer. Versionen finns på resurssammanfattningssidan.

![](assets/five-5.png)

Som standard markeras alla dina befintliga e-postmeddelanden och e-postmallar som v1.0 om de skapades antingen före vårutgåvan 16 eller efter utgåvan när e-postredigeraren 2.0 är inaktiverad. När e-postredigeraren 2.0 nu har aktiverats automatiskt ser du följande beteende:

* När du skapar ett nytt e-postmeddelande visas [Väljare för e-postmall](email-template-picker-overview.md) kommer att visas och du kan välja en v2.0-e-postmall.
* När du skapar eller redigerar ett e-postmeddelande med e-postredigeraren 2.0 får du ett mejl som **alltid** markeras som v2.0 (även om du har använt en e-postmall v1.0).

Om din prenumeration har e-post v1.0 innan du går över till e-postredigeraren 2.0 kommer du att uppleva följande beteende baserat på resursens aktuella tillstånd:

**Godkänd** - Om du klickar på Redigera utkast skapas ett v2.0-utkast av det godkända e-postmeddelandet. Om du sedan godkänner utkastet från v2.0 blir det godkända tillståndet för e-postmeddelandet v2.0 och det finns inget sätt att återgå till v1.0.\
**Utkast** - Om du klickar på Redigera utkast markeras utkastet automatiskt som v2.0. I det här läget går det inte att ta bort och återställa till v1.0 eftersom det inte finns någon godkänd version av tillgången.
**Godkänd med utkast** - När du klickar på Redigera utkast markeras det utkastet automatiskt som v2.0. På grund av detta går det inte heller att återställa utkastet till v1.0.

Om din prenumeration har e-postmallar från version 1.0 innan du går över till e-postredigeraren 2.0 fungerar följande:

**Godkänd** - Om du klickar på Redigera utkast skapas ett v2.0-utkast av den befintliga e-postmallen.
**Utkast** - Om du klickar på Redigera utkast markeras utkastet automatiskt som v2.0. I det här läget går det inte att ta bort och återställa till v1.0 eftersom det inte finns någon godkänd version av tillgången.
**Godkänd med utkast** - Om du klickar på Redigera utkast markeras utkastet automatiskt som v2.0. På grund av detta går det inte heller att återställa utkastet till v1.0.

Om du godkänner en e-postmall som tidigare var v1.0 (i något av de ovanstående lägena) visas följande beteende:

För befintliga e-postmeddelanden av version 1.0 som använder mallen (tidigare version 1.0):\
**Godkänt e-postmeddelande v1.0** - Ett v2.0-utkast kommer att skapas för det här e-postmeddelandet, men det nya godkända v2.0-mallen används fortfarande. Den får även eventuella malländringar.\
**Utkast v1.0-e-post** - Utkastet förblir v1.0 tills du klickar på Redigera utkast. Därefter markeras den automatiskt som v2.0 och får eventuella malländringar.\
**Godkänd med e-postutkast v1.0** - Utkastet förblir v1.0 tills du klickar på Redigera utkast. Därefter markeras den automatiskt som v2.0 och får eventuella malländringar.

För befintliga v2.0-e-postmeddelanden som använder mallen (tidigare v1.0):\
**Godkänt v2.0-e-postmeddelande** - Ett v2.0-utkast kommer att skapas för det här e-postmeddelandet, som fortfarande&quot;använder&quot; den nyligen godkända mallen, och kommer att ta emot eventuella malländringar.\
**Utkast v2.0-e-post** - Utkastet ändras inte (v2.0) och du får eventuella malländringar.\
**Godkänd med e-postmeddelande om utkast v2.0** - Utkastet ändras inte (v2.0) och du får eventuella malländringar.

>[!CAUTION]
>
>Om du någonsin godkänner utkastet till v2.0 för en e-postmall v1.0 blir mallen v2.0. Det finns **ingen väg** för att återställa den till v1.0.

Saker att notera

* Godkända e-postmeddelanden är **aldrig** har ändrats.

* Godkända e-postmallar är **aldrig** har ändrats.

* Om några **sällsynt** I vissa fall går det inte att öppna e-post v1.0 i e-postredigeraren 2.0. Om detta inträffar ska du ignorera utkastet och kontakta Marketo Support.

>[!MORELIKETHIS]
>
>* [E-postredigerare 2.0 - översikt](/help/marketo/product-docs/email-marketing/general/email-editor-2/email-editor-v2-0-overview.md)
>* [Syntax för e-postmall](/help/marketo/product-docs/email-marketing/general/email-editor-2/email-template-syntax.md)
