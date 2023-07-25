---
unique-page-id: 3571797
description: Steg 2 av 3 - Skapa en Salesforce-användare för Marketo (Professional) - Marketo Docs - Produktdokumentation
title: Steg 2 av 3 - Skapa en Salesforce-användare för Marketo (Professional)
exl-id: 7eb4bf89-b6e4-45e0-adee-e2976cb01dd3
feature: Salesforce Integration
source-git-commit: 431bd258f9a68bbb9df7acf043085578d3d91b1f
workflow-type: tm+mt
source-wordcount: '423'
ht-degree: 1%

---

# Steg 2 av 3: Skapa en Salesforce-användare för Marketo (Professional) {#step-of-create-a-salesforce-user-for-marketo-professional}

>[!NOTE]
>
>De här stegen måste utföras av en Salesforce-administratör

>[!PREREQUISITES]
>
>[Steg 1 av 3: Lägg till Marketo-fält i Salesforce (Professional)](/help/marketo/product-docs/crm-sync/salesforce-sync/setup/professional-edition/step-1-of-3-add-marketo-fields-to-salesforce-professional.md)

I den här artikeln ska du anpassa fältbehörigheter med en Salesforce-sidlayout och skapa en Marketo-Salesforce-synkroniseringsanvändare.

## Ange sidlayout {#set-page-layouts}

Salesforce Professional anger tillgänglighet på fältnivå med sidlayouter, i motsats till Salesforce Enterprise/Unlimited&#39;s Profiles. Om du följer de här stegen kan Marketo synkroniseringsanvändare uppdatera anpassade fält.

1. Typ **sidlayout** i navigeringsfältet utan att trycka på **Retur** och klicka **Sidlayout** under **Leads**.

   ![](assets/image2016-2-26-12-3a58-3a32.png)

1. Klicka **Redigera** bredvid Leadlayout.

   ![](assets/image2016-2-26-13-3a2-3a46.png)

1. Klicka och dra en ny **Avsnitt** till sidlayouten.

   ![](assets/image2014-12-9-12-3a56-3a40.png)

1. Ange&quot;Marketo&quot; för **Avsnittsnamn** och klicka **OK**.

   ![](assets/image2014-12-9-12-3a56-3a52.png)

1. Klicka och dra fältet **Anskaffningsdatum** till **Marketo** -avsnitt.

   ![](assets/image2014-12-9-12-3a57-3a0.png)

1. Upprepa ovanstående steg för följande fält:

   * Anskaffningsprogram
   * ID för förvärvsprogram
   * Avanmäl dig via e-post
   * Inaktuell ort
   * Berört företag
   * Berört land
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

1. Klicka **Spara** när fält har lagts till.

   ![](assets/image2014-12-9-12-3a57-3a10.png)

1. Upprepa alla ovanstående steg för Salesforce **Kontaktsidlayout**.

   ![](assets/image2016-2-26-13-3a10-3a1.png)

1. Kom ihåg att klicka **Spara** när du är klar med **Kontaktsidlayout**.

   ![](assets/image2014-12-9-12-3a57-3a30.png)

   >[!NOTE]
   >
   >Se till att **Heldagshändelse** fältet har lagts till i **Händelsesidlayout**.

## Skapa synkroniserad användare {#create-sync-user}

Marketo kräver inloggningsuppgifter för att få åtkomst till Salesforce. Detta görs bäst med en dedikerad användare som skapats med stegen nedan.

>[!NOTE]
>
>Om din organisation inte har några ytterligare Salesforce-licenser kan du använda en befintlig **Marknadsförare** med **Systemadministratör** profil.

1. Ange&quot;användare&quot; i navigeringsfältet och klicka på **Användare** under **Hantera användare**.

   ![](assets/image2014-12-9-12-3a57-3a42.png)

1. Klicka **Ny användare**.

   ![](assets/image2014-12-9-12-3a58-3a1.png)

1. Fyll i de obligatoriska fälten, välj **Användarlicens: Salesforce**, ange **Profil: Systemadministratör**, kontrollera **Marknadsförare** och klicka **Spara**.

   ![](assets/image2014-12-9-12-3a58-3a11.png)

   >[!TIP]
   >
   >Kontrollera att den e-postadress du anger är giltig. Du måste logga in som synkroniseringsanvändare för att återställa lösenordet.

Underbar! Nu har du ett konto som Marketo kan använda för att ansluta till Salesforce. Låt oss göra det.

>[!MORELIKETHIS]
>
>[Steg 3 av 3: Connect Marketo och Salesforce (Professional)](/help/marketo/product-docs/crm-sync/salesforce-sync/setup/professional-edition/step-3-of-3-connect-marketo-and-salesforce-professional.md)
