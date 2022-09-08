---
unique-page-id: 10096681
description: Understanding Webinar Program Status - Marketo Docs - produktdokumentation
title: Om status för webbinarium
exl-id: ef0b1b94-a612-4aa8-9b4a-aa7ef0e2abaa
source-git-commit: 40cfdddac66b7cd90e33bedf11888a7c5e3b38c9
workflow-type: tm+mt
source-wordcount: '432'
ht-degree: 0%

---

# Om status för webbinarium {#understanding-webinar-program-statuses}

>[!IMPORTANT]
>
>Från och med augusti 2022 har ON24 inte längre stöd för nya Marketo-integreringar. Informationen i den här artikeln gäller endast befintliga användare.

Programstatus representerar olika händelsestatusar som en person går igenom som medlem i händelsen. De är kopplade till en kanaltyp. Marketo har en inbyggd kanaltyp som kallas **Webbinarium**. Statuser kan användas i både batch- och utlösarkampanjer.

Människor rör sig linjärt genom programstatusarna och går inte tillbaka i status. En person med statusen **Anmäld** kan inte gå tillbaka till **Registrerad**.

Här är en kort beskrivning av programstatus som är kopplad till webbseminariekanalen.

>[!TIP]
>
>Om du vill uppdatera statusar manuellt klickar du på  **Uppdatera från webbseminarieleverantör** i **Händelseåtgärder** nedrullningsbar meny.

![](assets/image2015-12-17-13-3a52-3a39.png)

**Inte i programmet** - Använd den här statusen för att ta bort personer från händelsen.

**Inbjuden** - Använd den här statusen för att lägga till personer till händelsen.

**Väntar på godkännande** - Använd den här statusen om du vill vänta med att skicka ett bekräftelsemeddelande till dina personer via e-post. Se&quot;Manuellt godkännande av registranter&quot; i [ON24 - Händelseregistreringsuppdateringar](/help/marketo/product-docs/demand-generation/events/create-an-event/create-an-event-with-the-marketo-on24-adapter/on24-event-registration-updates.md) för mer information.

**Väntar** - Använd den här statusen om du vill att vissa personer ska vänta tills fler platser blir tillgängliga.

**Avvisad** - Använd den här statusen för att avvisa registreringen av en person till din händelse.

**Registrerad** - Den här statusen överför personer till ON24 när du använder ON24-integreringen. Personens status uppdateras när ON24 svarar på att personen registrerats korrekt.

**Registreringsfel** - Den här statusen visar att användaren påträffade ett fel när han/hon försökte registrera sig för händelsen.

>[!NOTE]
>
>Om ett registreringsfel inträffar kan du få ytterligare information för den personen genom att titta i kolumnen Statusorsak på fliken Medlemmar i programmet. När felet är åtgärdat kan du manuellt ändra användarens programstatus till Registrerad i Marketo.

**Anmäld** - När webbinariet är avslutat returnerar ON24 en lista över personer som deltog. Den här statusen hämtas automatiskt till Marketo.

**Angivet på begäran** - Personer som deltog i den arkiverade versionen av webbinariet får den här statusen.

**Ingen visning** - När webbinariet har avslutats och när närvarodata har hämtats in från ON24 uppdateras statusen för personer som registrerade sig men inte deltog till Ingen visning. Det kan ta mellan 30 minuter och 3 timmar för ON24 att förbereda den slutliga närvaroinformationen och göra den tillgänglig i Marketo.

>[!NOTE]
>
>För att Marketo ska kunna dra in statusen No Show måste personen ha registrerats *i Marketo*. Vi kan inte hämta No Shows som kommer från On24-dataflödet.

>[!MORELIKETHIS]
>
>[Om Marketo ON24-nätverkskortshändelser](/help/marketo/product-docs/demand-generation/events/create-an-event/create-an-event-with-the-marketo-on24-adapter/understanding-marketo-on24-adapter-events.md)
