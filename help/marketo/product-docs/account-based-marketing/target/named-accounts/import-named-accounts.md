---
unique-page-id: 12615800
description: Importera namngivna konton - Marketo Docs - Produktdokumentation
title: Importera namngivna konton
translation-type: tm+mt
source-git-commit: e125f8469239a026aefb703fdb6ba99c32e33565
workflow-type: tm+mt
source-wordcount: '479'
ht-degree: 0%

---


# Importera namngivna konton {#import-named-accounts}

Har du redan en CSV-fil full med potentiella målkonton? Importera dem direkt till ABM!

1. Klicka på listrutan **Nytt** och välj **Importera namngivna konton**.

   ![](assets/inaone.png)

1. Ett nytt fönster öppnas. Klicka på **Bläddra** och markera sedan filen med namngivna konton som du vill importera.

   ![](assets/inatwo.png)

   >[!TIP]
   >
   >Ange [så mycket information](/help/marketo/product-docs/account-based-marketing/target/named-accounts/named-account-overview.md#named-account-attributes) som möjligt i filen. Du kan bara lägga till firmografisk information; ingenting Marketo beräknar (dvs. Pipeline). Om du vill skapa namngivna konton baserat på CRM-konton exporterar du bara kontonamnet och CRM-ID:t från CRM till en CSV-fil, använder alternativet Kontonamn och mappar CRM-ID:t under importprocessen. Om du vill länka ett CRM-konto till ett namngivet konto måste du ange CRM-kontots exakta namn.

1. Välj mellan två borttagningslägen: Kontonamn eller domännamn. I det här exemplet väljer vi Konto. Klicka på listrutan **Lägen** och välj **Efter kontonamn**.

   ![](assets/inathree.png)

   >[!NOTE]
   >
   >Om du väljer **Efter domänläge** måste både namngivna konto- och domänfält inkluderas.

1. Om du vill välja vilken kontolista ditt namngivna konto ska läggas till klickar du på listrutan **Kontolista** och gör ditt val.

   ![](assets/inafour.png)

   >[!NOTE]
   >
   >Du kan också skapa en helt ny kontolista genom att skriva namnet i listrutan.

1. Om du vill skicka ett meddelande om importen klickar du på listrutan **Skicka varning till** och väljer en Marketo-användare. Du _kan inte_ ange en e-postadress manuellt.

   ![](assets/inafive-2.png)

1. Klicka på **Nästa**.

   ![](assets/inasix-2.png)

1. Mappa varje fält genom att dubbelklicka på listrutan **Marketfält** och välja lämpligt fält. Klicka på **Nästa** när du är klar.

   ![](assets/inaseven.png)

   Klart!

   ![](assets/inanine.png)

   >[!NOTE]
   >
   >&quot;Kontrollera importstatus&quot; visar endast de tre senaste aktivitetsdagarna.

Scenarier när du tar bort efter kontonamn:

<table> 
 <tbody> 
  <tr> 
   <td><strong>Importerar post med befintligt namn på konto</strong></td> 
   <td><p>Vi uppdaterar den befintliga posten</p></td> 
  </tr> 
  <tr> 
   <td><strong>Importerar post med nytt namn på konto</strong></td> 
   <td>Vi ska skapa en ny post</td> 
  </tr> 
 </tbody> 
</table>

Scenarier när du tar bort efter domännamn:

<table> 
 <tbody> 
  <tr> 
   <td><strong>Importerar post med ett nytt kontonamn och ett nytt domännamn</strong></td> 
   <td>Vi skapar ett nytt namngivet konto med den angivna informationen</td> 
  </tr> 
  <tr> 
   <td><strong>Importerar post med ett befintligt kontonamn och befintligt domännamn</strong></td> 
   <td>Vi uppdaterar det befintliga namngivna kontot</td> 
  </tr> 
   <tr> 
   <td><strong>Importerar post med ett nytt kontonamn och befintligt domännamn</strong></td> 
   <td>Vi lägger till det nya kontonamnet till det befintliga namngivna kontot som matchar domännamnet och uppdaterar annan information (t.ex. bransch, stat)</td> 
  </tr> 
  <tr> 
   <td><strong>Importerar post med befintligt namn och nytt domännamn</strong></td> 
   <td>Vi lägger till det nya domännamnet till det befintliga namngivna kontot som matchar kontonamnet och uppdaterar annan information (t.ex. bransch, stat)</td> 
  </tr> 
 </tbody> 
</table>

>[!NOTE]
>
>När Marketo lägger till ett namngivet konto uppdaterar vi en regel (bakom kulisserna) som gör att vi kan identifiera personer som ska ingå i det namngivna kontot. Exempel: Om du uppdaterar &quot;IBM&quot; till &quot;IBM, USA&quot; kopplas personer med respektive företagsnamn till det namngivna kontot.

Om Marketo hittar poster som vi ser som dubbletter bearbetar vi bara den första.
