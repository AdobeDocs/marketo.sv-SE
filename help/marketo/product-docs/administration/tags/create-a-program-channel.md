---
unique-page-id: 2950682
description: Skapa en programkanal - Marketo Docs - produktdokumentation
title: Skapa en programkanal
exl-id: 7b4e15db-c221-45a9-9588-99eb2510cde7
source-git-commit: 48c2d1deea84ee747ecc2453e770ad33dd49f578
workflow-type: tm+mt
source-wordcount: '428'
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

1. Gå till **Administratör** område.

   ![](assets/create-a-program-channel-1.png)

1. Klicka **Taggar**.

   ![](assets/create-a-program-channel-2.png)

   >[!NOTE]
   >
   >Varför taggar? En kanal är ett sätt att beskriva ett program, precis som andra taggar. Kanalen har bara specialfunktioner.

1. Klicka på **+** signera bredvid **Kanal** för att utöka och se befintliga kanaler.

   ![](assets/create-a-program-channel-3.png)

1. Under **Nytt**, klicka **Ny kanal**.

   ![](assets/create-a-program-channel-4.png)

   >[!NOTE]
   >
   >**Exempel**
   >
   >Kanal: Billboard
   >
   >* Använd för: Standard
   >* Progression: Medlem, engagerad (om du är osäker, så fungerar dessa bra)
   >* Slutfört: Engagerad

   >
   >Kanal: Part
   >
   >* Använd för: Händelse
   >* Progression: Inbjuden, Registrerad, Inget bildspel och Deltar
   >* Slutfört: Anmäld

   >
   >Kolla in Progressions of existing channel för att få en uppfattning om hur de används.

1. Låt oss följa exemplet med partikanalen. Ge ditt nya namn **Kanal** och välj den programtyp som ska användas.

   ![](assets/create-a-program-channel-5.png)

   >[!NOTE]
   >
   >Gäller för vad? Det finns flera typer av program. Matcha kanalen till rätt typ. Om du är osäker, välj **Standard**.

   >[!NOTE]
   >
   >När du använder Händelse med webbinarium kommer systemmappningar att låsas (vilket krävs av webbinarieintegreringar) och kan inte redigeras.

1. Ange de två första statusnamnen för programmet och klicka sedan på **Lägg till steg**.

   ![](assets/create-a-program-channel-6.png)

1. Ange ett annat program **Status** och **Steg** nummer och klicka sedan på **Lägg till steg**.

   ![](assets/create-a-program-channel-7.png)

   >[!TIP]
   >
   >The **Steg** talet används för sortering av programstatus. Tänk på att det inte går att gå bakåt i dessa steg. De kan bara ändra status till ett högre eller lika värde. Använd lika värden när statusvärdena ska växla fram och tillbaka i stället för en progression.

1. Ange det sista programmet **Status** och **Steg** tal.

   ![](assets/create-a-program-channel-8.png)

   >[!NOTE]
   >
   >När du använder typen Händelse måste du mappa systemet för statusvärdena Registrerad, Väntelistat och Attended. Dessa statusvärden kan därför inte döljas.

1. Välj **Status för mobilinloggning** for **Registrerad**.

   ![](assets/create-a-program-channel-9.png)

1. Välj **Status för mobilinloggning** for **Anmäld**.

   ![](assets/create-a-program-channel-10.png)

   >[!NOTE]
   >
   >**Status för mobilinloggning**** **alternativ är bara tillgängliga om kanalen används för händelseprogram.

   >[!NOTE]
   >
   >Endast personer med **Status för mobilinloggning** av **Registrerad** och **Anmäld** visas i [Appar för mobilincheckning](/help/marketo/product-docs/core-marketo-concepts/mobile-apps/event-check-in/event-check-in-overview.md).

   >[!TIP]
   >
   >Om en ny person skapas i appen för mobilincheckning ställs den in på Registrerad i händelseprogrammet. Om en person checkas in i händelsen i appen ställs den in på Bifogad i händelseprogrammet.

1. Välj **Lyckades** programstatus, klicka sedan på **Skapa**.

   ![](assets/create-a-program-channel-11.png)

   Snyggt gjort! När du skapar ett nytt program av den typen är den nya kanalen ett av alternativen.
