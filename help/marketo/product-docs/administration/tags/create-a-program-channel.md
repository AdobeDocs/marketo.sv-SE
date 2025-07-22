---
unique-page-id: 2950682
description: Skapa en programkanal - Marketo Docs - produktdokumentation
title: Skapa en programkanal
exl-id: 7b4e15db-c221-45a9-9588-99eb2510cde7
feature: Tags
source-git-commit: 0d37fbdb7d08901458c1744dc68893e155176327
workflow-type: tm+mt
source-wordcount: '387'
ht-degree: 0%

---

# Skapa en programkanal {#create-a-program-channel}

Ett program är ett specifikt marknadsföringsinitiativ. Kanalen är avsedd att fungera som leveransmekanism, som webbinarium, sponsring eller online-annons.

>[!NOTE]
>
>**Administratörsbehörigheter krävs**

>[!NOTE]
>
>Läs mer om [program](/help/marketo/product-docs/core-marketo-concepts/programs/creating-programs/understanding-programs.md), det viktigaste elementet i Marketo.

1. Gå till området **[!UICONTROL Admin]**.

   ![](assets/create-a-program-channel-1.png)

1. Klicka på **[!UICONTROL Tags]**.

   ![](assets/create-a-program-channel-2.png)

   >[!NOTE]
   >
   >Varför taggar? En kanal är ett sätt att beskriva ett program, precis som andra taggar. Kanalen har bara specialfunktioner.

1. Klicka på **+** bredvid [!UICONTROL Channel] för att expandera och visa befintliga kanaler.

   ![](assets/create-a-program-channel-3.png)

1. Klicka på **[!UICONTROL New]** under **[!UICONTROL New Channel]**.

   ![](assets/create-a-program-channel-4.png)

   >[!NOTE]
   >
   >**Exempel**
   >
   >Kanal: Billboard
   >
   >* Använd på: Standard
   >* Progression: Medlem, engagerad (om du är osäker, så fungerar dessa bra)
   >* Slutfört: Engagerat
   >
   >Kanal: Fest
   >
   >* Använd på: händelse
   >* Progression: Inbjuden, Registrerad, Ingen visning och Bifogad
   >* Slutförd: Deltagad
   >
   >Kolla in Progressions of existing channel för att få en uppfattning om hur de används.

1. Låt oss följa exemplet med partikanalen. Namnge din nya **[!UICONTROL Channel]** och välj den programtyp som den ska användas för.

   ![](assets/create-a-program-channel-5.png)

   >[!NOTE]
   >
   >Gäller för vad? Det finns flera typer av program. Matcha kanalen till rätt typ. Välj **[!UICONTROL Default]** om du är osäker.

   >[!NOTE]
   >
   >När [!UICONTROL Event with Webinar] används kommer systemmappningar att låsas (vilket krävs av webbinära integreringar) och kan inte redigeras.

1. Ange de två första statusnamnen för programmet och klicka sedan på **[!UICONTROL Add Step]**.

   ![](assets/create-a-program-channel-6.png)

1. Ange ett annat program, **[!UICONTROL Status]** och **[!UICONTROL Step]**, och klicka sedan på **[!UICONTROL Add Step]**.

   ![](assets/create-a-program-channel-7.png)

   >[!TIP]
   >
   >Numret **[!UICONTROL Step]** används för att sortera programstatus. Tänk på att det inte går att gå bakåt i dessa steg. De kan bara ändra status till ett högre eller lika värde. Använd lika värden när statusvärdena ska växla fram och tillbaka i stället för en progression.

1. Ange det sista programmet **[!UICONTROL Status]** och **[!UICONTROL Step]**-numret.

   ![](assets/create-a-program-channel-8.png)

   >[!NOTE]
   >
   >Systemmappning krävs för statusvärdena Registrerad, Väntelistat och Attended när typen [!UICONTROL Event] används. Dessa statusvärden kan därför inte döljas.

1. Välj **[!UICONTROL Mobile Check-in Status]** för **[!UICONTROL Registered]**.

   ![](assets/create-a-program-channel-9.png)

1. Välj **[!UICONTROL Mobile Check-in Status]** för **[!UICONTROL Attended]**.

   ![](assets/create-a-program-channel-10.png)

   >[!NOTE]
   >
   >**[!UICONTROL Mobile Check-in Status]** alternativ är bara tillgängliga om kanalen är för händelseprogram.

   >[!NOTE]
   >
   >Endast personer med **[!UICONTROL Mobile Check-in Status]** av **[!UICONTROL Registered]** och **[!UICONTROL Attended]** visas i [apparna för mobilincheckning](/help/marketo/product-docs/core-marketo-concepts/mobile-apps/event-check-in/event-check-in-overview.md).

   >[!TIP]
   >
   >Om en ny person skapas i appen för mobilincheckning ställs den in på [!UICONTROL Registered] i händelseprogrammet. Om en person checkas in i händelsen i appen ställs den in på [!UICONTROL Attended] i händelseprogrammet.

1. Välj programstatus för **[!UICONTROL Success]** och klicka sedan på **[!UICONTROL Create]**.

   ![](assets/create-a-program-channel-11.png)

   Snyggt gjort! När du skapar ett nytt program av den typen är den nya kanalen ett av alternativen.
