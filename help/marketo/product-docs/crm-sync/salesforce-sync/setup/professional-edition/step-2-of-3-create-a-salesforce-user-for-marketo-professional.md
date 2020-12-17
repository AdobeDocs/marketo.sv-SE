---
unique-page-id: 3571797
description: Steg 2 av 3 - Skapa en Salesforce-användare för Marketo (Professional) - Marketo Docs - Produktdokumentation
title: Steg 2 av 3 - Skapa en Salesforce-användare för Marketo (Professional)
translation-type: tm+mt
source-git-commit: e149133a5383faaef5e9c9b7775ae36e633ed7b1
workflow-type: tm+mt
source-wordcount: '426'
ht-degree: 0%

---


# Steg 2 av 3: Skapa en Salesforce-användare för Marketo (Professional) {#step-of-create-a-salesforce-user-for-marketo-professional}

>[!NOTE]
>
>De här stegen måste utföras av en Salesforce-administratör

>[!PREREQUISITES]
>
>* [Steg 1 av 3: Lägg till Marketo-fält i Salesforce (Professional)](step-1-of-3-add-marketo-fields-to-salesforce-professional.md)

>



I den här artikeln ska du anpassa fältbehörigheter med en Salesforce-sidlayout och skapa en Marketo-Salesforce-synkroniseringsanvändare.

## Ange sidlayout {#set-page-layouts}

Salesforce Professional anger tillgänglighet på fältnivå med sidlayouter, i motsats till Salesforce Enterprise/Unlimited&#39;s Profiles. Med de här stegen kan Marketto synkronisera användaren för att uppdatera anpassade fält.

1. Skriv **sidlayouter** i navigeringsfältet utan att trycka på **Enter** och klicka på **Sidlayout** under **Leads**.

   ![](assets/image2016-2-26-12-3a58-3a32.png)

1. Klicka på **Redigera** bredvid Leadlayout.

   ![](assets/image2016-2-26-13-3a2-3a46.png)

1. Klicka och dra ett nytt **avsnitt** till sidlayouten.

   ![](assets/image2014-12-9-12-3a56-3a40.png)

1. Ange Marketo för **Avsnittsnamn** och klicka på **OK**.

   ![](assets/image2014-12-9-12-3a56-3a52.png)

1. Klicka och dra fältet **Anskaffningsdatum** till avsnittet **Marketo**.

   ![](assets/image2014-12-9-12-3a57-3a0.png)

1. Upprepa ovanstående steg för följande fält:

   * Anskaffningsprogram
   * ID för förvärvsprogram
   * Avanmäl dig via e-post
   * Inaktuell ort
   * Infört företag
   * Infört land
   * Ingående metropolitområde
   * Riktnummer för inkommande telefon
   * Infört postnummer
   * Ingångsregion
   * Leadpoäng
   * Ursprunglig referens
   * Ursprunglig sökmotor
   * Ursprunglig sökfras
   * Ursprunglig källinformation
   * Ursprunglig källtyp

   >[!NOTE]
   >
   >Dessa fält måste finnas i sidlayouten så att Marketo kan läsa/skriva till dem.

   >[!TIP]
   >
   >Skapa två kolumner för fälten genom att dra nedåt till höger på sidan. Du kan flytta fält från den ena sidan till den andra om du vill balansera kolumnlängden.

1. Klicka på **Spara** när du är klar med att lägga till fält.

   ![](assets/image2014-12-9-12-3a57-3a10.png)

1. Upprepa alla ovanstående steg för Salesforce **Kontaktsidlayout**.

   ![](assets/image2016-2-26-13-3a10-3a1.png)

1. Kom ihåg att klicka på **Spara** när du är klar med **Kontaktsidans layout**.

   ![](assets/image2014-12-9-12-3a57-3a30.png)

   >[!NOTE]
   >
   >**Påminnelse**
   >
   >
   >Kontrollera att fältet **Heldagshändelse** har lagts till i **händelsesidlayouten**.

## Skapa synkroniseringsanvändare {#create-sync-user}

Marketo kräver inloggningsuppgifter för att få åtkomst till Salesforce. Detta görs bäst med en dedikerad användare som skapats med stegen nedan.

>[!NOTE]
>
>Om din organisation inte har några ytterligare Salesforce-licenser kan du använda en befintlig **marknadsföringsanvändare** med profilen **Systemadministratör**.

1. Ange &quot;användare&quot; i navigeringsfältet och klicka på **Användare** under **Hantera användare**.

   ![](assets/image2014-12-9-12-3a57-3a42.png)

1. Klicka på **Ny användare**.

   ![](assets/image2014-12-9-12-3a58-3a1.png)

1. Fyll i de obligatoriska fälten och välj **Användarlicens: Salesforce**, ange **profilen: Systemadministratör**, kontrollera **Marknadsförare** och klicka på **Spara**.

   ![](assets/image2014-12-9-12-3a58-3a11.png)

   >[!TIP]
   >
   >Kontrollera att den e-postadress du anger är giltig. Du måste logga in som synkroniseringsanvändare för att återställa lösenordet.

Underbar! Nu har du ett konto som Marketo kan använda för att ansluta till Salesforce. Låt oss göra det.

>[!NOTE]
>
>**Relaterade artiklar**
>
>* [Steg 3 av 3: Connect Marketo och Salesforce (Professional)](step-3-of-3-connect-marketo-and-salesforce-professional.md)

>



