---
unique-page-id: 2950682
description: Skapa en programkanal - Marketo Docs - Produktdokumentation
title: Skapa en programkanal
translation-type: tm+mt
source-git-commit: 00887ea53e395bea3a11fd28e0ac98b085ef6ed8
workflow-type: tm+mt
source-wordcount: '440'
ht-degree: 0%

---


# Skapa en programkanal {#create-a-program-channel}

Ett program är ett specifikt marknadsföringsinitiativ. Kanalen är avsedd att fungera som leveransmekanism, som webbinarium, sponsring eller online-annons.

>[!NOTE]
>
>**Administratörsbehörigheter krävs**

>[!NOTE]
>
>**Djupdykning**
>
>Läs mer om [program](http://docs.marketo.com/display/docs/programs), det viktigaste elementet i Marketo.

1. Klicka på **Taggar** under avsnittet **Admin**.

   ![](assets/image2014-9-24-12-3a57-3a27.png)

   >[!NOTE]
   >
   >Varför taggar? En kanal är ett sätt att beskriva ett program, precis som andra taggar. Kanalen har bara specialfunktioner.

1. Klicka på **+** -tecknet bredvid **Kanal** för att expandera och visa befintliga kanaler.

   ![](assets/image2014-9-24-12-3a58-3a33.png)

1. Klicka på **Ny kanal under** Ny **.**.

   ![](assets/image2014-9-24-12-3a58-3a53.png)

   >[!NOTE]
   >
   >**Exempel**
   >
   >
   >Kanal: Billboard
   >
   >    
   >    
   >    * Använd för: Standard
   >    * Progression: Medlem, engagerad (om du är osäker, så fungerar dessa bra)
   >    * Slutfört: Engagerad

   >    
   >    
   >Kanal: Part
   >
   >    
   >    
   >    * Använd för: Händelse
   >    * Progression: Inbjuden, Registrerad, Inget bildspel och Deltar
   >    * Slutfört: Anmäld

   >    
   >    
   >Kolla in Progressions of existing channel för att få en uppfattning om hur de används.

1. Låt oss följa exemplet med partikanalen. Namnge din nya **kanal** och välj den programtyp som den ska användas för.

   ![](assets/image2014-9-24-13-3a0-3a17.png)

   >[!NOTE]
   >
   >Gäller för vad? Det finns flera typer av program. Matcha kanalen till rätt typ. Om du är osäker väljer du **Standard**.

   >[!NOTE]
   >
   >När du använder Händelse med webbinarium kommer systemmappningar att låsas (vilket krävs av webbinarieintegreringar) och kan inte redigeras.

   Ange de två första programstatusnamnen och klicka sedan på Lägg till steg.
   ![](assets/image2014-9-24-15-3a37-3a0.png)

1. Ange en annan **programstatus** och ett **stegnummer** och klicka sedan på **Lägg till steg**.

   ![](assets/image2014-9-24-15-3a37-3a30.png)

   >[!TIP]
   >
   >Stegnumret **används** för att sortera programstatus. Tänk på att det inte går att gå bakåt i dessa steg. De kan bara ändra status till ett högre eller lika värde. Använd lika värden när statusvärdena ska växla fram och tillbaka i stället för en progression.

1. Ange den sista **programstatusen** och **stegnumret** .

   ![](assets/image2014-9-24-15-3a39-3a15.png)

   >[!NOTE]
   >
   >När du använder typen Händelse måste du mappa systemet för statusvärdena Registrerad, Väntelistat och Attended. Dessa statusvärden kan därför inte döljas.

1. Välj **Mobile-incheckningsstatus** för **registrerad**.

   ![](assets/image2014-9-24-15-3a39-3a43.png)

1. Välj **Mobile-incheckningsstatus** för **Bifogad**.

   ![](assets/image2014-9-24-15-3a40-3a21.png)

   >[!NOTE]
   >
   >**Status** för Mobile-incheckning** **alternativ är bara tillgängliga om kanalen används för händelseprogram.

   >[!NOTE]
   >
   >**Påminnelse**
   >
   >
   >Endast personer med **Mobile Check-in-status**** **för **Registrerad** och **bifogad** kommer att visas i [Mobile Check-in-apparna](http://docs.marketo.com/display/docs/events).

   >[!TIP]
   >
   >Om en ny person skapas i appen för mobilincheckning ställs den in på Registrerad i händelseprogrammet. Om en person checkas in i händelsen i appen ställs den in på Bifogad i händelseprogrammet.

1. Välj **Slutfört** -programstatus och klicka sedan på **Skapa**.

   ![](assets/image2014-9-24-15-3a42-3a54.png)

   Snyggt gjort! När du skapar ett nytt program av den typen är den nya kanalen ett av alternativen.

