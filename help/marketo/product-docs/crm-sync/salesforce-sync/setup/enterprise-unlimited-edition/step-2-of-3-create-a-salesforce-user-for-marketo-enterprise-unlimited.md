---
unique-page-id: 2360364
description: Steg 2 av 3 - Skapa en Salesforce-användare för Marketo (Enterprise/Unlimited) - Marketo Docs - Produktdokumentation
title: Steg 2 av 3 - Skapa en Salesforce-användare för Marketo (Enterprise/Unlimited)
exl-id: 871f335c-7b1e-47e1-8320-a18fbf21a970
feature: Salesforce Integration
source-git-commit: 989804463f44afbf35ab11c0f23c37b0d328e652
workflow-type: tm+mt
source-wordcount: '393'
ht-degree: 0%

---

# Steg 2 av 3: Skapa en Salesforce-användare för Marketo (Enterprise/Unlimited) {#step-of-create-a-salesforce-user-for-marketo-enterprise-unlimited}

>[!NOTE]
>
>Dessa steg måste utföras av en Salesforce-administratör

>[!PREREQUISITES]
>
>[Steg 1 av 3: Lägg till Marketo-fält i Salesforce (Enterprise/Unlimited)](/help/marketo/product-docs/crm-sync/salesforce-sync/setup/enterprise-unlimited-edition/step-1-of-3-add-marketo-fields-to-salesforce-enterprise-unlimited.md){target="_blank"}

I den här artikeln ska du ange användarbehörigheter i Salesforce-profilen och skapa ett Marketo-Salesforce-integrationskonto.

## Skapa en profil {#create-a-profile}

1. Klicka på **[!UICONTROL Setup]**.

   ![](assets/image2015-6-11-16-3a15-3a27.png)

1. Skriv&quot;profiler&quot; i navigeringsfältet och klicka på länken **[!UICONTROL Profiles]**.

   ![](assets/sfdc-profiles-hands.png)

1. Klicka på **[!UICONTROL New]**.

   ![](assets/image2014-12-9-9-3a19-3a15.png)

1. Välj **[!UICONTROL Standard User]**, ge profilen namnet&quot;Marketo-Salesforce Sync&quot; och klicka på **[!UICONTROL Save]**.

   ![](assets/image2014-12-9-9-3a19-3a22.png)

## Ange profilbehörigheter {#set-profile-permissions}

1. Klicka på **[!UICONTROL Edit]** för att ange säkerhetsbehörigheter.

   ![](assets/image2014-12-9-9-3a19-3a30.png)

1. Kontrollera att följande rutor är markerade under avsnittet **[!UICONTROL Administrative Permissions]**:

   * API aktiverat
   * Redigera HTML-mallar
   * Hantera offentliga dokument
   * Hantera offentliga mallar

   ![](assets/image2014-12-9-9-3a19-3a38.png)

   >[!TIP]
   >
   >Kontrollera kryssrutan **[!UICONTROL Password Never Expires]**.

1. Kontrollera att följande rutor är markerade under avsnittet Allmänna användarbehörigheter:

   * Konvertera leads
   * Redigera händelser
   * Redigera uppgifter

   ![](assets/image2014-12-9-9-3a19-3a47.png)

1. Under avsnittet Standardbehörigheter för objekt kontrollerar du att behörigheterna Läs, Skapa, Redigera och Ta bort är ikryssade:

   * Konton
   * Kampanjer
   * Kontakter
   * Leads
   * Möjligheter

   >[!NOTE]
   >
   >Bevilja behörigheter till kampanjerna om du tänker använda kampanjsynkronisering.

   ![](assets/image2014-12-9-9-3a19-3a57.png)

1. När du är klar klickar du på **[!UICONTROL Save]** längst ned på sidan.

   ![](assets/image2014-12-9-9-3a20-3a5.png)

## Ange fältbehörigheter {#set-field-permissions}

1. Diskutera med era marknadsförare för att ta reda på vilka anpassade fält som behövs för att synkronisera.

   >[!NOTE]
   >
   >Det här steget förhindrar att fält som du inte behöver visas i Marketo, vilket gör att det blir rörigt och snabbar upp synkroniseringen.

1. Gå till avsnittet **[!UICONTROL Field-Level Security]** på profilinformationssidan. Klicka på **[!UICONTROL View]** om du vill redigera tillgängligheten för objekten:

   * Lead
   * Kontakt
   * Konto
   * Möjligheter

   >[!TIP]
   >
   >Du kan konfigurera andra objekt efter organisationens behov.

   ![](assets/image2014-12-9-9-3a20-3a14.png)

1. Klicka på **[!UICONTROL Edit]** för varje objekt.

   ![](assets/sfdc-sync-field-edit1.png)

1. Leta reda på de fält som inte behövs, kontrollera att **[!UICONTROL Read Access]** och **[!UICONTROL Edit Access]** inte är markerade. Klicka på **[!UICONTROL Save]** när du är klar.

   >[!NOTE]
   >
   >Redigera bara tillgängligheten för anpassade fält.

   ![](assets/sfdc-sync-field-edit2.png)

1. När du har inaktiverat alla onödiga fält måste du kontrollera **[!UICONTROL Read Access and Edit Access]** efter följande objektfält. Klicka på **[!UICONTROL Save]** när du är klar.

<table> 
 <tbody> 
  <tr> 
   <th>Objekt</th> 
   <th>Fält</th> 
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

![](assets/sfdc-check-the-boxes.png)

## Skapa Marketo-Salesforce Sync-konto {#create-marketo-salesforce-sync-account}

>[!TIP]
>
>Skapa ett dedikerat Salesforce-konto (t.ex. `marketo@yourcompany.com`) för att skilja mellan Marketo och andra Salesforce-användare.

1. Skriv Hantera användare i navigeringsfältet och klicka sedan på **[!UICONTROL Users]**. Klicka på **[!UICONTROL New User]**.

   ![](assets/sfdc-new-users.png)

1. Fyll i obligatoriska fält. Markera sedan **[!UICONTROL User License: Salesforce]** och den profil som du skapade tidigare. Klicka på **[!UICONTROL Save]** när du är klar.

   ![](assets/image2014-12-9-9-3a20-3a56.png)

Steg 2 av 3 är slutförd.

>[!NOTE]
>
>[Steg 3 av 3: Anslut Marketo och Salesforce (Enterprise/Unlimited)](/help/marketo/product-docs/crm-sync/salesforce-sync/setup/enterprise-unlimited-edition/step-3-of-3-connect-marketo-and-salesforce-enterprise-unlimited.md){target="_blank"}
