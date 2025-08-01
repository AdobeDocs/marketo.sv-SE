---
unique-page-id: 12615800
description: Importera [!UICONTROL Named Accounts] - Marketo Docs - produktdokumentation
title: Importera [!UICONTROL Named Accounts]
exl-id: 3f40e567-9256-4efd-beea-4e818770759f
feature: Target Account Management
source-git-commit: 26573c20c411208e5a01aa7ec73a97e7208b35d5
workflow-type: tm+mt
source-wordcount: '440'
ht-degree: 0%

---

# Importera [!UICONTROL Named Accounts] {#import-named-accounts}

Har du redan en CSV-fil full med potentiella målkonton? Importera dem direkt till TAM!

1. Klicka på listrutan **[!UICONTROL New]** och välj **[!UICONTROL Import Named Accounts]**.

   ![](assets/inaone.png)

1. Ett nytt fönster öppnas. Klicka på **[!UICONTROL Browse]** och markera sedan filen med namngivna konton som du vill importera.

   ![](assets/inatwo.png)

   >[!TIP]
   >
   >Ange [så mycket information](/help/marketo/product-docs/target-account-management/target/named-accounts/named-account-overview.md#named-account-attributes) som möjligt i filen. Du kan bara lägga till firmografisk information. Det finns inga Marketo-beräkningar (dvs. Pipeline). Om du vill skapa namngivna konton baserat på CRM-konton exporterar du bara kontonamnet och CRM-ID:t från CRM till en CSV-fil, använder alternativet Kontonamn och mappar CRM-ID:t under importprocessen. Om du vill länka ett CRM-konto till ett namngivet konto måste du ange CRM-kontots exakta namn.

1. Välj mellan två borttagningslägen: Kontonamn eller Domännamn. I det här exemplet väljer vi Konto. Klicka på listrutan **[!UICONTROL Modes]** och välj **[!UICONTROL By Account Name]**.

   ![](assets/inathree.png)

   >[!NOTE]
   >
   >Om du väljer **[!UICONTROL By Domain Name]** måste både namngivna konto- och domänfält inkluderas.

1. Om du vill välja vilken kontolista ditt namngivna konto ska läggas till i klickar du på listrutan **[!UICONTROL Account List]** och gör ditt val.

   ![](assets/inafour.png)

   >[!NOTE]
   >
   >Du kan också skapa ett helt nytt [!UICONTROL Account List] genom att skriva namnet i listrutan.

1. Om du vill skicka ett meddelande om importen klickar du på listrutan **[!UICONTROL Send Alert To]** och väljer en Marketo-användare. Du _kan inte_ ange en e-postadress manuellt.

   ![](assets/inafive-2.png)

1. Klicka på **[!UICONTROL Next]**.

   ![](assets/inasix-2.png)

1. Mappa varje fält genom att dubbelklicka på listrutan **[!UICONTROL Marketo Field]** och välja rätt fält. Klicka på **[!UICONTROL Next]** när du är klar.

   ![](assets/inaseven.png)

   Klart!

   ![](assets/inanine.png)

   >[!NOTE]
   >
   >&quot;Kontrollera importstatus&quot; visar endast de tre senaste aktivitetsdagarna.

Scenarier när du tar bort [!UICONTROL by Account Name]:

<table>
 <tbody>
  <tr>
   <td><strong>Importerar post med befintligt <span class="uicontrol">namn på konto</span></strong></td>
   <td><p>Vi uppdaterar den befintliga posten</p></td>
  </tr>
  <tr>
   <td><strong>Importerar post med nytt namn för <span class="uicontrol">namngivet konto</span></strong></td>
   <td>Vi ska skapa en ny post</td>
  </tr>
 </tbody>
</table>

Scenarier när du tar bort [!UICONTROL by Domain Name]:

<table>
 <tbody>
  <tr>
   <td><strong>Importerar post med ett nytt kontonamn och ett nytt domännamn</strong></td>
   <td>Vi skapar ett nytt <span class="uicontrol">namngivet konto</span> med den angivna informationen</td>
  </tr>
  <tr>
   <td><strong>Importerar post med ett befintligt kontonamn och befintligt domännamn</strong></td>
   <td>Vi uppdaterar det befintliga <span class="uicontrol">namngivna kontot</span></td>
  </tr>
   <tr>
   <td><strong>Importerar post med ett nytt kontonamn och befintligt domännamn</strong></td>
   <td>Vi lägger till det nya kontonamnet till det befintliga <span class="uicontrol">namngivna kontot</span> som matchar domännamnet och uppdaterar annan information (t.ex. bransch, stat)</td>
  </tr>
  <tr>
   <td><strong>Importerar post med befintligt <span class="uicontrol">namn på konto</span> och nytt domännamn</strong></td>
   <td>Vi lägger till det nya domännamnet till det befintliga <span class="uicontrol">namngivna kontot</span> som matchar kontonamnet och uppdaterar annan information (t.ex. bransch, stat)</td>
  </tr>
 </tbody>
</table>

>[!NOTE]
>
>När Marketo lägger till ett namngivet konto uppdaterar vi en regel (bakom kulisserna) som gör att vi kan identifiera personer som ska vara en del av [!UICONTROL Named Account]. Exempel: Om du uppdaterar &quot;IBM&quot; till &quot;IBM, USA&quot; kopplas personer med något av företagsnamnen till [!UICONTROL Named Account].

Om Marketo hittar poster som vi ser som dubbletter bearbetar vi bara den första.
