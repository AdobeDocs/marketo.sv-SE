---
description: Steg 2 av 3 - Skapa en veeva CRM-användare för Marketo Engage - Marketo Docs - Produktdokumentation
title: Steg 2 av 3 - Skapa en veeva CRM-användare för Marketo Engage
exl-id: 78945192-36b0-4e0b-830a-f37eb0b83484
feature: Veeva CRM
source-git-commit: 0087a5e88b8bd9601875f68a2e7cadeebdb5d682
workflow-type: tm+mt
source-wordcount: '592'
ht-degree: 1%

---

# Steg 2 av 3: Skapa en Veeva CRM-användare för Marketo Engage {#step-2-of-3-create-a-veeva-crm-user-for-marketo-engage}

>[!NOTE]
>
>Stegen i den här artikeln måste slutföras av en Veeva CRM-administratör.

>[!PREREQUISITES]
>
>[Steg 1 av 3: Lägg till Marketo-fält i Salesforce (Professional)](/help/marketo/product-docs/crm-sync/veeva-crm-sync/setup/step-1-of-3-add-marketo-fields-to-veeva-crm.md){target="_blank"}

I den här artikeln ska du anpassa fältbehörigheter med en veeva CRM-sidlayout och skapa en Marketo-veeva CRM-synkroniseringsanvändare.

## Ange sidlayout {#set-page-layouts}

Om du följer de här stegen kan Marketo synkroniseringsanvändare uppdatera anpassade fält.

1. Klicka på sidlayouten Konto (personkonto) i navigeringsfältet utan att trycka på Retur och klicka på **[!UICONTROL Page Layout]** under Kontakter.

   ![](assets/step-2-of-3-create-a-veeva-crm-user-1.png)

1. Klicka på **[!UICONTROL Page Layouts]**.

   ![](assets/step-2-of-3-create-a-veeva-crm-user-2.png)

1. Klicka på **[!UICONTROL HCP - Professional]**.

   ![](assets/step-2-of-3-create-a-veeva-crm-user-3.png)

1. Klicka och dra en ny **[!UICONTROL Section]** till sidlayouten.

1. Ange&quot;Marketo&quot; som avsnittsnamn och klicka på **[!UICONTROL OK]**.

   ![](assets/step-2-of-3-create-a-veeva-crm-user-4.png)

1. Klicka och dra bakgrundsmusiken till Marketo-delen.

   ![](assets/step-2-of-3-create-a-veeva-crm-user-5.png)

1. Upprepa ovanstående steg för följande fält:

   * Inaktuell ort
   * Berört företag
   * Berört land
   * Ingående metropolitområde
   * Riktnummer för inkommande telefon
   * Infört postnummer
   * Ingångsregion

   >[!NOTE]
   >
   >Dessa fält måste finnas i sidlayouten så att Marketo kan läsa/skriva till dem.

   >[!TIP]
   >
   >Skapa två kolumner för fälten genom att dra nedåt till höger på sidan. Du kan flytta fält från den ena sidan till den andra om du vill balansera kolumnlängden.

1. När du är klar med HCP-Professional-layouten klickar du på **[!UICONTROL Save]**.

   ![](assets/step-2-of-3-create-a-veeva-crm-user-6.png)

   >[!NOTE]
   >
   >Upprepa detta för andra sidlayouter för konton.

## Skapa en profil {#create-a-profile}

1. Klicka på **[!UICONTROL Setup]**.

   ![](assets/step-2-of-3-create-a-veeva-crm-user-7.png)

1. Skriv&quot;profiler&quot; i navigeringsfältet och klicka på **[!UICONTROL Profiles]** länk.

   ![](assets/step-2-of-3-create-a-veeva-crm-user-8.png)

1. Klicka på **[!UICONTROL New]**.

   ![](assets/step-2-of-3-create-a-veeva-crm-user-9.png)

1. Välj standardanvändare, ge profilen namnet&quot;Marketo-Salesforce-synkronisering&quot; och klicka på **[!UICONTROL Save]**.

   ![](assets/step-2-of-3-create-a-veeva-crm-user-10.png)

## Ange profilbehörigheter {#set-profile-permissions}

1. Klicka **[!UICONTROL Edit]** för att ange säkerhetsbehörigheter.

   ![](assets/step-2-of-3-create-a-veeva-crm-user-11.png)

1. Under Administrativa behörigheter ser du till att **[!UICONTROL API Enabled]** är markerat.

   ![](assets/step-2-of-3-create-a-veeva-crm-user-12.png)

   >[!TIP]
   >
   >Markera rutan Lösenordet upphör aldrig att gälla.

1. Under avsnittet Allmänna användarbehörigheter ser du till att **[!UICONTROL Edit Events]** och **[!UICONTROL Edit Tasks]** är markerade.

   ![](assets/step-2-of-3-create-a-veeva-crm-user-13.png)

1. Under avsnittet Standardobjektbehörigheter ser du till att **[!UICONTROL Read]**, **[!UICONTROL Create]**, **[!UICONTROL Edit]** och **[!UICONTROL Delete]** behörigheter kontrolleras för konton och kontakter.

   ![](assets/step-2-of-3-create-a-veeva-crm-user-14.png)

1. Kontrollera att Läs-behörigheterna är ikryssade under avsnittet Anpassade objektbehörigheter **[!UICONTROL Call]**, **[!UICONTROL Call Key Message]** och andra anpassade objekt.

   ![](assets/step-2-of-3-create-a-veeva-crm-user-15.png)

1. När du är klar klickar du **[!UICONTROL Save]** längst ned på sidan.

   ![](assets/step-2-of-3-create-a-veeva-crm-user-16.png)

## Ange fältbehörigheter {#set-field-permissions}

1. Diskutera med era marknadsförare för att ta reda på vilka anpassade fält som behövs för att synkronisera.

   >[!NOTE]
   >
   >Det här steget förhindrar att fält som du inte behöver visas i Marketo, vilket gör att det blir rörigt och snabbar upp synkroniseringen.

1. Gå till profildetaljsidan [!UICONTROL Field-Level Security] -avsnitt. Klicka **[!UICONTROL View]** om du vill redigera tillgängligheten för objekten Kontakt och Konto.

   ![](assets/step-2-of-3-create-a-veeva-crm-user-17.png)

   >[!TIP]
   >
   >Du kan konfigurera andra objekt efter organisationens behov.

1. För varje objekt klickar du **[!UICONTROL Edit]**.

   ![](assets/step-2-of-3-create-a-veeva-crm-user-18.png)

1. Leta reda på de onödiga fälten och se till att Läs- och Redigera-åtkomst är _avmarkerad_. Klicka **[!UICONTROL Save]** när det är klart.

   ![](assets/step-2-of-3-create-a-veeva-crm-user-19.png)

   >[!NOTE]
   >
   >Redigera bara tillgängligheten för anpassade fält.

1. När du är klar med inaktiveringen av alla onödiga fält kontrollerar du Läs åtkomst och Redigera åtkomst för följande objektfält. Klicka **[!UICONTROL Save]** när det är klart.

<table>
 <tbody>
  <tr>
   <th>Objekt
   <th>Fält
  </tr>
  <tr>
   <td>Konto</td>
   <td>Typfält</td>
  </tr>
  <tr>
   <td>Händelse</td>
   <td>Alla fält</td>
  </tr>
  <tr>
   <td>Uppgift</td>
   <td>Alla fält</td>
  </tr>
 </tbody>
</table>

## Skapa synkroniserad användare {#create-sync-user}

Marketo kräver autentiseringsuppgifter för att få åtkomst till Veeva CRM. Detta görs bäst med en dedikerad användare som skapats med stegen nedan.

>[!NOTE]
>
>Om din organisation inte har några ytterligare veva CRM-licenser kan du använda en befintlig Marketing-användare med systemadministratörsprofilen.

1. Ange&quot;användare&quot; i navigeringsfältet och klicka på **[!UICONTROL Users]** under Hantera användare.

   ![](assets/step-2-of-3-create-a-veeva-crm-user-20.png)

1. Klicka på **[!UICONTROL New User]**.

   ![](assets/step-2-of-3-create-a-veeva-crm-user-21.png)

1. Fyll i de obligatoriska fälten, välj användarlicens: Salesforce, ange profilen: Marketo Sync User och klicka på **[!UICONTROL Save]**.

   ![](assets/step-2-of-3-create-a-veeva-crm-user-22.png)

>[!TIP]
>
>Kontrollera att den e-postadress du anger är giltig. Du måste logga in som synkroniseringsanvändare för att återställa lösenordet.

Underbar! Nu har du ett konto som Marketo Engage kan använda för att ansluta till Veeva CRM. Låt oss göra det.

>[!MORELIKETHIS]
>
>[Steg 3 av 3: Anslut Marketo och Veeva CRM](/help/marketo/product-docs/crm-sync/veeva-crm-sync/setup/step-3-of-3-connect-marketo-engage-and-veeva-crm.md){target="_blank"}
