---
description: Steg 2 av 3 - Skapa en [!DNL Veeva] CRM-användare för Marketo Engage - Marketo Docs - Produktdokumentation
title: Steg 2 av 3 - Skapa en veeva CRM-användare för Marketo Engage
exl-id: 78945192-36b0-4e0b-830a-f37eb0b83484
feature: Veeva CRM
source-git-commit: 0d37fbdb7d08901458c1744dc68893e155176327
workflow-type: tm+mt
source-wordcount: '545'
ht-degree: 1%

---

# Steg 2 av 3: Skapa en [!DNL Veeva] CRM-användare för Marketo Engage {#step-2-of-3-create-a-veeva-crm-user-for-marketo-engage}

>[!NOTE]
>
>Stegen i den här artikeln måste slutföras av en CRM-administratör för [!DNL Veeva].

>[!PREREQUISITES]
>
>[Steg 1 av 3: Lägg till Marketo-fält i [!DNL Salesforce] (Professional)](/help/marketo/product-docs/crm-sync/veeva-crm-sync/setup/step-1-of-3-add-marketo-fields-to-veeva-crm.md){target="_blank"}

I den här artikeln anpassar du fältbehörigheter med en [!DNL Veeva] CRM-sidlayout och skapar en [!DNL Marketo-Veeva] CRM-synkroniseringsanvändare.

## Ange sidlayout {#set-page-layouts}

Om du följer de här stegen kan Marketo synkroniseringsanvändare uppdatera anpassade fält.

1. Klicka på sidlayouten **[!UICONTROL Account]** (personkonto) i navigeringsfältet utan att trycka på Retur och klicka på **[!UICONTROL Page Layout]** under [!UICONTROL Contacts].

   ![](assets/step-2-of-3-create-a-veeva-crm-user-1.png)

1. Klicka på **[!UICONTROL Page Layouts]**.

   ![](assets/step-2-of-3-create-a-veeva-crm-user-2.png)

1. Klicka på **[!UICONTROL HCP - Professional]**.

   ![](assets/step-2-of-3-create-a-veeva-crm-user-3.png)

1. Klicka och dra en ny **[!UICONTROL Section]** till sidlayouten.

1. Ange Marketo för **[!UICONTROL Section Name]** och klicka på **[!UICONTROL OK]**.

   ![](assets/step-2-of-3-create-a-veeva-crm-user-4.png)

1. Klicka och dra fältet **[!UICONTROL Score]** till avsnittet Marketo.

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

1. När du är klar med layouten [!UICONTROL HCP-Professional] klickar du på **[!UICONTROL Save]**.

   ![](assets/step-2-of-3-create-a-veeva-crm-user-6.png)

>[!NOTE]
>
>Upprepa detta för andra [!UICONTROL Account]-sidlayouter.

## Skapa en profil {#create-a-profile}

1. Klicka på **[!UICONTROL Setup]**.

   ![](assets/step-2-of-3-create-a-veeva-crm-user-7.png)

1. Skriv&quot;profiler&quot; i navigeringsfältet och klicka på länken **[!UICONTROL Profiles]**.

   ![](assets/step-2-of-3-create-a-veeva-crm-user-8.png)

1. Klicka på **[!UICONTROL New]**.

   ![](assets/step-2-of-3-create-a-veeva-crm-user-9.png)

1. Välj **[!UICONTROL Standard User]**, ge profilen namnet [!UICONTROL Marketo-Salesforce Sync] och klicka på **[!UICONTROL Save]**.

   ![](assets/step-2-of-3-create-a-veeva-crm-user-10.png)

## Ange profilbehörigheter {#set-profile-permissions}

1. Klicka på **[!UICONTROL Edit]** för att ange säkerhetsbehörigheter.

   ![](assets/step-2-of-3-create-a-veeva-crm-user-11.png)

1. Kontrollera att [!UICONTROL Administrative Permissions] är markerat under avsnittet [!UICONTROL API Enabled].

   ![](assets/step-2-of-3-create-a-veeva-crm-user-12.png)

   >[!TIP]
   >
   >Kontrollera kryssrutan [!UICONTROL Password Never Expires].

1. Kontrollera att [!UICONTROL General User Permissions] och [!UICONTROL Edit Events] är markerade under avsnittet [!UICONTROL Edit Tasks].

   ![](assets/step-2-of-3-create-a-veeva-crm-user-13.png)

1. Under avsnittet [!UICONTROL Standard Object Permissions] kontrollerar du att behörigheterna [!UICONTROL Read], [!UICONTROL Create], [!UICONTROL Edit] och [!UICONTROL Delete] har kontrollerats för [!UICONTROL Accounts] och [!UICONTROL Contacts].

   ![](assets/step-2-of-3-create-a-veeva-crm-user-14.png)

1. Under avsnittet [!UICONTROL Custom Object Permissions] kontrollerar du att [!UICONTROL Read]-behörigheterna har kontrollerats för [!UICONTROL Call], [!UICONTROL Call Key Message] och andra önskade anpassade objekt.

   ![](assets/step-2-of-3-create-a-veeva-crm-user-15.png)

1. När du är klar klickar du på **[!UICONTROL Save]** längst ned på sidan.

   ![](assets/step-2-of-3-create-a-veeva-crm-user-16.png)

## Ange fältbehörigheter {#set-field-permissions}

1. Diskutera med era marknadsförare för att ta reda på vilka anpassade fält som behövs för att synkronisera.

   >[!NOTE]
   >
   >Det här steget förhindrar att fält som du inte behöver visas i Marketo, vilket gör att det blir rörigt och snabbar upp synkroniseringen.

1. Gå till avsnittet [!UICONTROL profile detail] på sidan **[!UICONTROL Field-Level Security]**. Klicka på **[!UICONTROL View]** om du vill redigera tillgängligheten för objekten [!UICONTROL Contact] och [!UICONTROL Account].

   ![](assets/step-2-of-3-create-a-veeva-crm-user-17.png)

   >[!TIP]
   >
   >Du kan konfigurera andra objekt efter organisationens behov.

1. Klicka på **[!UICONTROL Edit]** för varje objekt.

   ![](assets/step-2-of-3-create-a-veeva-crm-user-18.png)

Leta reda på de onödiga fälten och kontrollera att [!UICONTROL Read Access] och [!UICONTROL Edit Access] är **un** markerade. Klicka på **[!UICONTROL Save]** när du är klar.

![](assets/step-2-of-3-create-a-veeva-crm-user-19.png)

>[!NOTE]
>
>Redigera bara tillgängligheten för anpassade fält.

1. När du har inaktiverat alla onödiga fält kontrollerar du [!UICONTROL Read Access] och [!UICONTROL Edit Access] för följande objektfält. Klicka på **[!UICONTROL Save]** när du är klar.

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

Marketo kräver autentiseringsuppgifter för åtkomst till [!DNL Veeva] CRM. Detta görs bäst med en dedikerad användare som skapats med stegen nedan.

>[!NOTE]
>
>Om din organisation inte har några ytterligare [!DNL Veeva] CRM-licenser kan du använda en befintlig Marketing-användare med systemadministratörsprofilen.

1. Ange&quot;användare&quot; i navigeringsfältet och klicka på **[!UICONTROL Users]** under [!UICONTROL Manage Users].

   ![](assets/step-2-of-3-create-a-veeva-crm-user-20.png)

1. Klicka på **[!UICONTROL New User]**.

   ![](assets/step-2-of-3-create-a-veeva-crm-user-21.png)

1. Fyll i de obligatoriska fälten, markera **[!UICONTROL User License]**: **[!UICONTROL Salesforce]**, ange **[!UICONTROL Profile]**: **[!UICONTROL Marketo Sync]** Användare och klicka på **[!UICONTROL Save]**.

   ![](assets/step-2-of-3-create-a-veeva-crm-user-22.png)

>[!TIP]
>
>Kontrollera att den e-postadress du anger är giltig. Du måste logga in som synkroniseringsanvändare för att återställa lösenordet.

Underbar! Nu har du ett konto som Marketo Engage kan använda för att ansluta till [!DNL Veeva] CRM. Låt oss göra det.

>[!MORELIKETHIS]
>
>[Steg 3 av 3: Anslut Marketo och [!DNL Veeva] CRM](/help/marketo/product-docs/crm-sync/veeva-crm-sync/setup/step-3-of-3-connect-marketo-engage-and-veeva-crm.md){target="_blank"}
