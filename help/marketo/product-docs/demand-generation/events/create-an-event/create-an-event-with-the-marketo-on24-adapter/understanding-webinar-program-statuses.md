---
unique-page-id: 10096681
description: Understanding Webinar Program Status - Marketo Docs - produktdokumentation
title: Om status för webbinarium
exl-id: ef0b1b94-a612-4aa8-9b4a-aa7ef0e2abaa
feature: Events
source-git-commit: 431bd258f9a68bbb9df7acf043085578d3d91b1f
workflow-type: tm+mt
source-wordcount: '414'
ht-degree: 0%

---

# Om status för webbinarium {#understanding-webinar-program-statuses}

Programstatus representerar olika händelsestatusar som en person går igenom som medlem i händelsen. De är kopplade till en kanaltyp. Marketo har en inbyggd kanaltyp som kallas **webbinarium**. Statuser kan användas i både batch- och utlösarkampanjer.

Människor rör sig linjärt genom programstatusarna och går inte tillbaka i status. En person med statusen **Attended** kan till exempel inte gå tillbaka till **Registered**.

Här är en kort beskrivning av programstatus som är kopplad till webbseminariekanalen.

>[!TIP]
>
>Om du vill uppdatera status manuellt klickar du på **Uppdatera från webbinariet-providern** i listrutan **Händelseåtgärder**.

![](assets/image2015-12-17-13-3a52-3a39.png)

**Inte i programmet** - Använd den här statusen för att ta bort personer från händelsen.

**Inbjuden** - Använd den här statusen för att lägga till personer i händelsen.

**Väntar på godkännande** - Använd den här statusen för att vänta med att skicka ett bekräftelsemeddelande via e-post till dina personer. Mer information finns i&quot;Manuellt Approving Registrants&quot; i [ON24 Event Registration Updates](/help/marketo/product-docs/demand-generation/events/create-an-event/create-an-event-with-the-marketo-on24-adapter/on24-event-registration-updates.md){target="_blank"}.

**Vänta i listan** - Använd den här statusen om du vill att vissa personer ska vänta tills ytterligare platser blir tillgängliga.

**Avvisad** - Använd den här statusen för att avvisa registreringen av en person till din händelse.

**Registrerad** - Den här statusen överför personer till ON24 när du använder ON24-integreringen. Personens status uppdateras när ON24 svarar på att personen registrerats korrekt.

**Registreringsfel** - Den här statusen visar att användaren påträffade ett fel när han/hon försökte registrera sig för händelsen.

>[!NOTE]
>
>Om ett registreringsfel inträffar kan du få ytterligare information för den personen genom att titta i kolumnen Statusorsak på fliken Medlemmar i programmet. När felet är åtgärdat kan du manuellt ändra användarens programstatus till Registrerad i Marketo.

**Attended** - On24 returnerar en lista med personer som deltog när webbinariet avslutades. Den här statusen hämtas automatiskt till Marketo.

**Anmäld på begäran** - Personer som deltog i den arkiverade versionen av webbinariet får den här statusen.

**Ingen visning** - När webbinariet avslutas och när närvarodata hämtas från ON24 uppdateras statusen för personer som har registrerat sig men inte deltagit till ingen visning. Det kan ta mellan 30 minuter och 3 timmar för ON24 att förbereda den slutliga närvaroinformationen och göra den tillgänglig i Marketo.

>[!NOTE]
>
>För att Marketo ska kunna dra in statusen No Show måste personerna ha registrerats *i Marketo*. Vi kan inte hämta No Shows som kommer från On24-dataflödet.

>[!MORELIKETHIS]
>
>[Om Marketo ON24-nätverkskortshändelser](/help/marketo/product-docs/demand-generation/events/create-an-event/create-an-event-with-the-marketo-on24-adapter/understanding-marketo-on24-adapter-events.md){target="_blank"}
