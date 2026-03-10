---
description: Lär dig hur du lägger till Marketo-fält i Veeva CRM innan du ansluter. Skapa bakgrundsmusiken och valfria marknadsföringsfält för kontaktobjekt i Veeva.
title: Steg 1 av 3 - Lägg till Marketo-fält i [!DNL Veeva] CRM
exl-id: a9a59e76-a7a4-4391-8169-922bd6acfb6d
feature: Veeva CRM
source-git-commit: 2b29f05a27f847184e0968442012d443e9e0597d
workflow-type: tm+mt
source-wordcount: '496'
ht-degree: 1%

---

# Steg 1 av 3: Lägg till Marketo-fält i [!DNL Veeva] CRM {#step-1-of-3-add-marketo-fields-to-veeva-crm}

>[!PREREQUISITES]
>
>CRM-instansen [!DNL Veeva] måste ha åtkomst till Salesforce API:er för att kunna synkronisera data mellan Marketo Engage och [!DNL Veeva] CRM.

Marketo Engage använder en uppsättning fält för att samla in viss typ av marknadsföringsrelaterad information. Om du vill ha dessa data i [!DNL Veeva] CRM följer du instruktionerna nedan.

1. Skapa ett anpassat fält i [!DNL Veeva] CRM för kontaktobjekten: Poäng
1. Du kan skapa ytterligare fält om du vill (se tabellen nedan).

Alla dessa anpassade fält är valfria och behöver inte synkronisera Marketo Engage och [!DNL Veeva] CRM.

## Lägg till Marketo-fält i [!DNL Veeva] CRM {#add-marketo-fields-to-veeva-crm}

Lägg till ett anpassat fält på lead- och kontaktobjekten i [!DNL Veeva] CRM som listas ovan. Om du vill lägga till fler fält kan du läsa tabellen med tillgängliga fält i slutet av det här avsnittet.

Utför följande steg för fältet Poäng för att lägga till det.

1. Logga in på [!DNL Veeva] CRM och klicka på **[!UICONTROL Setup]**.

   ![](assets/step-1-of-3-add-marketo-fields-1.png)

1. Klicka på **[!UICONTROL Objects and Fields]** och välj **[!UICONTROL Object Manager]**.

   ![](assets/step-1-of-3-add-marketo-fields-2.png)

1. Sök efter &quot;Kontakt&quot; i sökfältet.

   ![](assets/step-1-of-3-add-marketo-fields-3.png)

1. Klicka på objektet **[!UICONTROL Contact]**.

1. Välj **[!UICONTROL Fields and Relationships]**.

1. Klicka på **[!UICONTROL New]**.

   ![](assets/step-1-of-3-add-marketo-fields-4.png)

1. Välj lämplig fälttyp (för Poäng - tal).

   ![](assets/step-1-of-3-add-marketo-fields-5.png)

1. Klicka på **[!UICONTROL Next]**.

   ![](assets/step-1-of-3-add-marketo-fields-6.png)

1. Ange **[!UICONTROL Field Label]**, **[!UICONTROL Length]** och **[!UICONTROL Field Name]** för fältet, vilket visas i tabellen nedan.

<table>
 <tbody>
  <tr>
   <th>Fältetikett
   <th>Fältnamn
   <th>Datatyp
   <th>Fältattribut
  </tr>
  <tr>
   <td>Poäng</td>
   <td>mkto71_Lead_Score</td>
   <td>Nummer</td>
   <td>Längd 10<br/>
Decimaler 0</td>
  </tr>
 </tbody>
</table>

>[!NOTE]
>
>[!DNL Veeva] CRM lägger till __c i fältnamn när de används för att skapa API-namn.

![](assets/step-1-of-3-add-marketo-fields-7.png)

>[!NOTE]
>
>Text- och nummerfält kräver en längd, men inte datum-/tidsfält. En beskrivning är valfri.

1. Klicka på **[!UICONTROL Next]**.

   ![](assets/step-1-of-3-add-marketo-fields-8.png)

1. Ange åtkomstinställningarna och klicka på **[!UICONTROL Next]**.

1. Ange alla roller till **[!UICONTROL Visible]** och **[!UICONTROL Read-Only]**.

1. Avmarkera kryssrutan **[!UICONTROL Read-Only]** för din synkroniseringsanvändares profil:

* Om du har en användare med en systemadministratörsprofil som synkroniseringsanvändare avmarkerar du kryssrutan [!UICONTROL Read-Only] för systemadministratörsprofilen (se nedan).
* Om du har skapat en anpassad profil för synkroniseringsanvändaren avmarkerar du kryssrutan [!UICONTROL Read-Only] för den anpassade profilen.

  ![](assets/step-1-of-3-add-marketo-fields-9.png)

1. Välj de sidlayouter som ska visa fältet.

1. Klicka på **[!UICONTROL Save & New]** om du vill gå tillbaka och skapa de två andra anpassade fälten.

1. Klicka på **[!UICONTROL Save]** när du är klar med alla tre.

   ![](assets/step-1-of-3-add-marketo-fields-10.png)

>[!NOTE]
>
>Genom att lägga till fältet i kontaktobjektet läggs de även till i personkontoobjektet.

VALFRITT: Använd ovanstående procedur för ytterligare anpassade fält från tabellen nedan.

<table>
 <tbody>
  <tr>
   <th>Fältetikett
   <th>Fältnamn
   <th>Datatyp
   <th>Fältattribut
  </tr>
  <tr>
   <td>Inaktuell ort</td>
   <td>mkto71_Insted_City</td>
   <td>Text</td>
   <td>Längd 255</td>
  </tr>
  <tr>
   <td>Berört företag</td>
   <td>mkto71_Insted_Company</td>
   <td>Text</td>
   <td>Längd 255</td>
  </tr>
  <tr>
   <td>Berört land</td>
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

>[!NOTE]
>
>Värden i fält som automatiskt tilldelats av Marketo är inte omedelbart tillgängliga i [!DNL Veeva] CRM när det nya fältet har skapats. Marketo synkroniserar data till [!DNL Veeva] CRM vid nästa uppdatering till posten i något av systemen (d.v.s. en synkroniserad uppdatering av något av fälten mellan Marketo och [!DNL Veeva] CRM).
