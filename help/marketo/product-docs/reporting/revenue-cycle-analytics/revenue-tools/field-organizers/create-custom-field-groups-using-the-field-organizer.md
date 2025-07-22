---
unique-page-id: 10094404
description: Skapa anpassade fältgrupper med fältorganiseraren - Marketo Docs - produktdokumentation
title: Skapa anpassade fältgrupper med fältorganiseraren
exl-id: 0425a446-2c92-4a2a-85c4-e05c22118035
feature: Reporting, Revenue Cycle Analytics
source-git-commit: 0d37fbdb7d08901458c1744dc68893e155176327
workflow-type: tm+mt
source-wordcount: '951'
ht-degree: 1%

---

# Skapa anpassade fältgrupper med fältorganiseraren {#create-custom-field-groups-using-the-field-organizer}

Innan du kan aktivera anpassade fältgrupper för rapportering i området för modellresultatanalys (Leads) i intäktscykelutforskaren måste du kategorisera standardfält eller anpassade fält i grupper för rapportering via Fältorganiseraren i Marketo Lead Management. Detta gäller endast lead- och företagsattribut.
När du väljer ett standardfält eller ett anpassat fält i listrutan Fält i dialogrutan Sorteraren i nytt fält mappas den Marketo Lead Management-datatyp som är associerad med det fält som du vill gruppera med en av tre tillgängliga redigerare i Sorteraren: sträng, heltal eller datum.

| Marketo Lead Management-datatyp | Datatyp för redigeraren i fältorganiseraren |
|---|---|
| Sträng | Sträng |
| E-post | Sträng |
| Heltal | Heltal |
| Text | Sträng |
| URL | Sträng |
| Referens | Stöds inte |
| Valuta | Heltal |
| DateTime | Datum |
| Boolean | Stöds inte |
| Tel. | Sträng |
| Datum | Datum |
| Float | Heltal |
| Beräknat | Stöds inte |

I följande tre avsnitt beskrivs hur du skapar en anpassad fältgrupp för en sträng, ett heltal eller en datumtyp.

## Skapa anpassad fältgrupp - Strängredigeraren {#create-custom-field-group-string-editor}

1. Klicka på **[!UICONTROL Lead Database]**.

   ![](assets/one.png)

1. Klicka på **[!UICONTROL New]** och välj **[!UICONTROL New Field Organizer]**.

   ![](assets/two.png)

1. Klicka på **[!UICONTROL Field]** och välj ett standardfält eller ett anpassat fält med en datatyp som mappar till strängredigeraren (se tabellen i föregående avsnitt). [!UICONTROL Country] används här.

   ![](assets/three.png)

1. Klicka på **[!UICONTROL Create]**.

   ![](assets/four.png)

   Den nya anpassade gruppen visas i Lead Database-trädet som fältnamn > Fältnamnsgrupp (exempel: Land > Landgrupp).

   ![](assets/4.5.png)

1. Klicka på pennikonen för att anpassa namnet. Du kan till exempel ändra namnet&quot;Landgrupp&quot; till&quot;Kontinent&quot;. Skriv det nya namnet och klicka utanför rutan för att spara automatiskt.

   ![](assets/five.png)

1. Som standard placeras alla datavärden i undergruppen [!UICONTROL Other]. Om du vill kategorisera datavärdena klickar du på **[!UICONTROL Add Group]** för att skapa en undergrupp och ge den ett namn.

   >[!NOTE]
   >
   >Du kan lägga till upp till tio undergrupper för att kategorisera datavärdena. Varje undergrupp som skapas tilldelas ett ID-nummer.

   I det här exemplet har grupper skapats för de flesta kontinenter.

   ![](assets/six.png)

   >[!NOTE]
   >
   >Om du vill ta bort en undergrupp klickar du bara på det röda X:et bredvid undergruppens namn. Om det finns datavärden i gruppen flyttas datavärdena till standardgruppen [!UICONTROL Other].

1. Markera ett eller flera datavärden på arbetsytan och dra och släpp datavärdena i lämplig undergrupp.

   ![](assets/seven.png)

   >[!NOTE]
   >
   >Om du vill ta bort ett datavärde från en undergrupp tilldelar du om datavärdet till standardgruppen Annan.

1. Använd filteralternativet i det övre vänstra hörnet direkt ovanför arbetsytan för att markera och visa datavärdena i en eller flera undergrupper. Datavärdena som baseras på filtermarkeringen visas på arbetsytan.

   ![](assets/eight.png)

   >[!NOTE]
   >
   >När grupperna har definierats kan du aktivera den anpassade fältgruppen för rapportering i Model Performance Analysis (Leads) via fliken Revenue Cycle Analytics i Marketo Lead Management.

## Skapa anpassad fältgrupp - heltalsredigerare {#create-custom-field-group-integer-editor}

1. Klicka på **[!UICONTROL Lead Database]**.

   ![](assets/one.png)

1. Klicka på **[!UICONTROL New]** och välj **[!UICONTROL New Field Organizer]**.

   ![](assets/two.png)

1. Klicka på **[!UICONTROL Field]** och välj ett standardfält eller ett anpassat fält med en datatyp som mappar till strängredigeraren (se tabellen i föregående avsnitt). [!UICONTROL Annual Revenue] används här.

   ![](assets/nine.png)

1. Klicka på **[!UICONTROL Create]**.

   ![](assets/9.5.png)

   Den nya anpassade gruppen visas i trädet Lead Database som representeras av Field Name > Field Name Group (Field Name Group) (Exempel: Annual Revenue > Annual Revenue Group).

   ![](assets/9.6.png)

1. Klicka på det anpassade gruppnamnet som är standard ovanför heltalsredigeraren för att anpassa namnet. Du kan till exempel byta namn på Årlig intäktsgrupp till Årlig intäkt efter storlek. Klicka på **[!UICONTROL Save]**.

   ![](assets/eleven.png)

   Med heltalsredigeraren kan du skapa flera undergrupper för att definiera varje undergrupp efter storlek. I det här exemplet kommer tre grupper att skapas för små, Medium och Enterprise.

1. Om du vill lägga till din första grupp anger du ett namn i fältet **[!UICONTROL Group Name]** (exempel: Liten) och anger ett maxvärde i fältet **[!UICONTROL Group Range]** (exempel: 20000). Klicka på **[!UICONTROL Add Group]**.

   ![](assets/twelve.png)

   En tom grupppost visas under den grupp som du just angav. I exemplet nedan visas en post för små, Medium och Enterprise-företag.

   >[!NOTE]
   >
   >Du kan lägga till upp till tio undergrupper för att kategorisera datavärdena. Varje gruppintervallpost bygger på föregående post. Om du lämnar den sista gruppintervallposten tom för den sista anpassade undergruppen som du skapar, kommer inget maximalt datavärde att anges.

1. Klicka på fliken Sammanfattning för att spara och granska inställningarna.

   ![](assets/thirteen.png)

   >[!NOTE]
   >
   >Om du vill ta bort en undergrupp klickar du på det röda X:et bredvid undergruppens namn.

1. Granska dina inställningar på sidan Sammanfattning.

   ![](assets/13.5.png)

   >[!NOTE]
   >
   >När grupperna har definierats kan du aktivera den anpassade fältgruppen för rapportering i Model Performance Analysis (Leads) via fliken Revenue Cycle Analytics i Marketo Lead Management.

## Skapa anpassad fältgrupp - datumredigerare {#create-custom-field-group-date-editor}

1. Klicka på **[!UICONTROL Lead Database]**.

   ![](assets/one.png)

1. Klicka på **[!UICONTROL New]** och välj **[!UICONTROL New Field Organizer]**.

   ![](assets/two.png)

1. Klicka på **[!UICONTROL Field]** och välj ett standardfält eller ett anpassat fält med en datatyp som mappar till strängredigeraren (se tabellen i föregående avsnitt). [!UICONTROL Acquisition Date] används här.

   ![](assets/fourteen.png)

1. Klicka på **[!UICONTROL Create]**.

   ![](assets/14.5.png)

   Den nya anpassade gruppen visas i trädet Lead Database som representeras av Field Name > Field Name Group (Field Name Group) (Exempel: Acquisition Date > Acquisition Date Group).

   ![](assets/14.6.png)

1. Klicka på det anpassade gruppnamnet som är standard ovanför datumredigeraren för att anpassa namnet. Du kan till exempel ändra namnet&quot;Inköpsdatumgrupp&quot; till&quot;Inköpsdatumkategorier&quot;. Klicka på **[!UICONTROL Save]**.

   ![](assets/fifteen.png)

   Med datumredigeraren kan du skapa flera undergrupper och definiera varje undergrupp efter datum. I det här exemplet skapas tre grupper: Q1-15 Leads, Q2-15 Leads och Q3-15 Leads.

1. Om du vill lägga till din första grupp anger du ett namn i fältet **[!UICONTROL Group Name]** (exempel: Q1-15 Leads) och ett datum i datumfältet som representerar det datum då leadet förvärvades den eller tidigare (exempel: 3/31/2015 för den sista dagen i Q1-15). Klicka på **[!UICONTROL Add Group]**.

   ![](assets/sixteen.png)

   >[!NOTE]
   >
   >Du kan lägga till upp till tio undergrupper för att kategorisera datavärdena. Varje [!UICONTROL Group Range]-post bygger på den föregående posten. Om du lämnar den sista [!UICONTROL Group Range]-posten tom för den sista anpassade undergruppen som du skapar, kommer inget slutdatumvärde att anges.

   I exemplet nedan visas en post för Q1 2015 som leder genom Q3.

   ![](assets/16.5.png)

   Och det är allt! Bra jobbat.
