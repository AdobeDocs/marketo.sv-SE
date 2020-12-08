---
unique-page-id: 2360362
description: Steg 1 av 3 - Lägg till Marketo-fält i Salesforce (Enterprise/Unlimited) - Marketo Docs - Produktdokumentation
title: Steg 1 av 3 - Lägg till Marketto-fält i Salesforce (Enterprise/Unlimited)
translation-type: tm+mt
source-git-commit: c33b7ab59e612f37d3f64bb954579700dc574068
workflow-type: tm+mt
source-wordcount: '754'
ht-degree: 0%

---


# Steg 1 av 3: Lägg till Marketo-fält i Salesforce (Enterprise/Unlimited) {#step-of-add-marketo-fields-to-salesforce-enterprise-unlimited}

>[!NOTE]
>
>**Förutsättningar**
>
>Du måste ha tillgång till Salesforce API:er för att kunna synkronisera mellan Marketo och Salesforce.

Marketo använder en uppsättning fält för att hämta in viss typ av marknadsföringsrelaterad information. Om du vill ha dessa data i Salesforce följer du instruktionerna nedan.

1. Skapa tre anpassade fält i Salesforce för lead- och kontaktobjekten: Poäng, förvärvsprogram och förvärvstidpunkt.
1. Mappa dessa anpassade fält mellan leads och kontakter så att värdena överförs vid konvertering i Salesforce.
1. Du kan skapa ytterligare fält om det behövs (se tabellen nedan).

Alla dessa anpassade fält är valfria och behöver inte synkronisera Marketo och Salesforce. Vi rekommenderar att du skapar fält för poäng, anskaffningsprogram och anskaffningsdatum.

## Lägg till Marketo-fält i Salesforce {#add-marketo-fields-to-salesforce}

Lägg till tre anpassade fält i lead- och kontaktobjekten i Salesforce som listas ovan. Om du vill lägga till fler fält kan du läsa tabellen med tillgängliga fält i slutet av det här avsnittet.

Utför följande steg för vart och ett av de tre anpassade fälten för att lägga till dem. Börja med bakgrundsmusik.

1. Logga in i Salesforce och klicka på Inställningar.

   ![](assets/image2016-5-23-13-3a15-3a21.png)

1. Klicka på Anpassa på menyn Skapa till vänster och välj Leads. Klicka på Fält.

   ![](assets/image2016-5-23-13-3a20-3a5.png)

1. Klicka på Nytt i avsnittet Anpassade fält och relationer längst ned på sidan.

   ![](assets/image2016-5-26-14-3a41-3a40.png)

1. Välj lämplig fälttyp (för poäng - tal), Acquisition Program - text; Anskaffningsdatum - datum/tid).

   ![](assets/choose-field-type-2-hand.png)

1. Klicka på Nästa.

   ![](assets/image2016-5-26-14-3a51-3a14.png)

1. Ange fältetikett, längd och fältnamn enligt tabellen nedan.

<table> 
 <thead> 
  <tr> 
   <th> 
    <div>
      Fältetikett 
    </div></th> 
   <th> 
    <div>
      Fältnamn 
    </div></th> 
   <th> 
    <div>
      Datatyp 
    </div></th> 
   <th> 
    <div>
      Fältattribut 
    </div></th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td>Poäng</td> 
   <td>mkto71_Lead_Score</td> 
   <td>Nummer</td> 
   <td>Längd 10<br>decimaler 0 </td> 
  </tr> 
  <tr> 
   <td>Anskaffningsdatum</td> 
   <td>mkto71_Acquisition_Date</td> 
   <td>Datum/tid</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>Anskaffningsprogram</td> 
   <td>mkto71_Acquisition_Program</td> 
   <td>Text</td> 
   <td>Längd 255</td> 
  </tr> 
 </tbody> 
</table>

>[!NOTE]
>
>Salesforce lägger till __c i fältnamn när de används för att skapa API-namn.

![](assets/image2016-5-26-14-3a55-3a33.png)

>[!NOTE]
>
>Text- och nummerfält kräver en längd, men inte datum-/tidsfält. En beskrivning är valfri.

1. Klicka på Nästa.

   ![](assets/image2016-5-23-14-3a50-3a5.png)

1. Ange åtkomstinställningarna och klicka på Nästa:

   * Ställ in alla roller till **Visible **och **Read-Only**

   * Avmarkera kryssrutan **Skrivskyddad** för din synkroniseringsanvändares profil:

      * Om du har en användare med profilen för en *systemadministratör* som synkroniseringsanvändare avmarkerar du kryssrutan **Skrivskyddad** för systemadministratörsprofilen (se nedan)
      * Om du har skapat en *anpassad profil* för synkroniseringsanvändaren avmarkerar du kryssrutan **Skrivskyddad** för den anpassade profilen

   ![](assets/image2016-6-30-9-3a25-3a4.png)

1. Välj de sidlayouter som ska visa fältet.

   ![](assets/image2016-5-26-15-3a14-3a45.png)

1. Klicka på Spara och ny för att gå tillbaka och skapa de två andra anpassade fälten. Klicka på Spara när du är klar med alla tre.

   ![](assets/image2016-5-23-15-3a8-3a43.png)

1. Klicka på Anpassa på menyn Skapa till vänster och välj Kontakter. Klicka på Fält.
1. Utför steg 3 till 10 för fälten Poäng, Inköpsdatum och Anskaffningsprogram på kontaktobjektet, precis som för lead-objektet.
1. Du kan också använda ovanstående procedur för ytterligare anpassade fält från den här tabellen.

<table> 
 <thead> 
  <tr> 
   <th> 
    <div>
      Fältetikett 
    </div></th> 
   <th> 
    <div>
      Fältnamn 
    </div></th> 
   <th> 
    <div>
      Datatyp 
    </div></th> 
   <th> 
    <div>
      Fältattribut 
    </div></th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td>ID för förvärvsprogram</td> 
   <td>mkto71_Acquisition_Program_Id</td> 
   <td>Nummer</td> 
   <td>Längd 18<br>decimaler 0 </td> 
  </tr> 
  <tr> 
   <td>Ursprunglig referens</td> 
   <td>mkto71_Original_Referrer</td> 
   <td>Text</td> 
   <td>Längd 255</td> 
  </tr> 
  <tr> 
   <td>Ursprunglig sökmotor</td> 
   <td>mkto71_Original_Search_Engine</td> 
   <td>Text</td> 
   <td>Längd 255</td> 
  </tr> 
  <tr> 
   <td>Ursprunglig sökfras</td> 
   <td>mkto71_Original_Search_Phrase</td> 
   <td>Text</td> 
   <td>Längd 255</td> 
  </tr> 
  <tr> 
   <td>Ursprunglig källinformation</td> 
   <td>mkto71_Original_Source_Info</td> 
   <td>Text</td> 
   <td>Längd 255</td> 
  </tr> 
  <tr> 
   <td>Ursprunglig källtyp</td> 
   <td>mkto71_Original_Source_Type</td> 
   <td>Text</td> 
   <td>Längd 255</td> 
  </tr> 
  <tr> 
   <td>Inaktuell ort</td> 
   <td>mkto71_Insted_City</td> 
   <td>Text</td> 
   <td>Längd 255</td> 
  </tr> 
  <tr> 
   <td>Infört företag</td> 
   <td>mkto71_Insted_Company</td> 
   <td>Text</td> 
   <td>Längd 255</td> 
  </tr> 
  <tr> 
   <td>Infört land</td> 
   <td>mkto71_Insted_Country</td> 
   <td>Text</td> 
   <td>Längd 255</td> 
  </tr> 
  <tr> 
   <td>Ingående metropolitområde</td> 
   <td>mkto71_Insted_Metropolitan_Area</td> 
   <td>Text</td> 
   <td>Längd 255</td> 
  </tr> 
  <tr> 
   <td>Riktnummer för inkommande telefon</td> 
   <td>mkto71_Insted_Phone_Area_Code</td> 
   <td>Text</td> 
   <td>Längd 255</td> 
  </tr> 
  <tr> 
   <td>Infört postnummer</td> 
   <td>mkto71_Insted_Postal_Code</td> 
   <td>Text</td> 
   <td>Längd 255</td> 
  </tr> 
  <tr> 
   <td>Ingångsregion</td> 
   <td>mkto71_Insted_State_Region</td> 
   <td>Text</td> 
   <td>Längd 255</td> 
  </tr> 
 </tbody> 
</table>

## Mappa anpassade fält för konverteringar {#map-custom-fields-for-conversions}

Ett anpassat fält på lead-objektet i Salesforce bör mappas till ett kontaktfält på kontaktobjektet så att data överförs när en konvertering inträffar.

1. Klicka på **Konfigurera** i det övre högra hörnet.

   ![](assets/image2016-5-26-16-3a34-3a0.png)

1. Skriv&quot;Fält&quot; i navigeringssökningen utan att trycka på Retur. Fält visas under olika objekt; Klicka på **Fält** under Leads.

   ![](assets/image2016-5-26-16-3a36-3a32.png)

1. Gå till avsnittet Leadanpassade fält och relationer och klicka på **Mappa lead-fält**.

   ![](assets/image2016-5-26-16-3a39-3a29.png)

1. Klicka på listrutan bredvid fältet som du vill mappa.

   ![](assets/image2016-5-26-16-3a49-3a53.png)

1. Välj motsvarande anpassat kontaktfält.

   ![](assets/image2016-5-26-16-3a56-3a23.png)

1. Upprepa stegen ovan för alla andra fält som du har skapat.
1. Klicka på **Spara** när du är klar.

   Inte så lätt, eller hur?

>[!NOTE]
>
>**Djupdykning**
>
>Här är en länk till en [video om hela proceduren](https://nation.marketo.com/videos/1475) som ska göra den kristallklar!

>[!NOTE]
>
>**Relaterade artiklar**
>
>* [Steg 2 av 3: Skapa en Salesforce-användare för Marketo (Enterprise/Unlimited)](step-2-of-3-create-a-salesforce-user-for-marketo-enterprise-unlimited.md)

>



