---
description: Synkronisering av anpassade fält för programmedlem - Marketo Docs - produktdokumentation
title: Synkronisering av anpassat fält för programmedlem
exl-id: 7facfc79-a411-4ad9-b847-2002763af5bb
feature: Programs
source-git-commit: e49860ae611f2f77789bb491aeccbee46a911a2c
workflow-type: tm+mt
source-wordcount: '348'
ht-degree: 0%

---

# Synkronisering av anpassat fält för programmedlem {#program-member-custom-field-sync}

>[!PREREQUISITES]
>
>* Skapar [anpassade programmedlemsfält](/help/marketo/product-docs/core-marketo-concepts/programs/working-with-programs/program-member-custom-fields.md){target="_blank"}
>* [Synkronisera en Salesforce-kampanj med ett program](/help/marketo/product-docs/core-marketo-concepts/programs/working-with-programs/sync-an-sfdc-campaign-with-a-program.md){target="_blank"}

>[!NOTE]
>
>Objektet Program Member kan ha upp till 20 anpassade fält. Dessa fält är tillgängliga för alla program.

## Mappa Salesforce-fält till anpassade programmedlemsfält {#map-salesforce-fields-to-program-member-custom-fields}

1. Klicka på **[!UICONTROL Admin]** i Marketo.

   ![](assets/program-member-custom-field-sync-1.png)

1. Klicka på **[!DNL Salesforce]** och sedan på **[!UICONTROL Edit]** bredvid Synkronisering av anpassade fält för programmedlem.

   ![](assets/program-member-custom-field-sync-2.png)

1. Använd sökrutan för att hitta de Salesforce-fält som du vill mappa. I det här exemplet använder vi Do Not Call.

   ![](assets/program-member-custom-field-sync-3.png)

1. Klicka på listrutan.

   ![](assets/program-member-custom-field-sync-4.png)

1. Välj önskat anpassat fält för Marketo-programmedlem som ska mappas.

   ![](assets/program-member-custom-field-sync-5.png)

   >[!NOTE]
   >
   >I listrutan visas endast anpassade fält för programmedlemmar som matchar datatypen för Salesforce-fältet.

1. Om du vill ha ytterligare fältkopplingar avmarkerar du sökrutan och upprepar steg 3 till 5.

1. Klicka på **[!UICONTROL Save]** när du är klar.

   ![](assets/program-member-custom-field-sync-6.png)

   >[!IMPORTANT]
   >
   >Ändringar av programmedlemsdata i mappade fält synkroniseras mellan Marketo och Salesforce framåt.

   >[!NOTE]
   >
   >Om du byter namn på eller ändrar datatypen för ett fält i Salesforce tar vi bort alla mappningar av det fältet med det anpassade fältet för programmedlem. Men du kan mappa om det med det nya fältet efter granskning.

## Ta bort mappning av Salesforce-fält från anpassade programmedlemsfält {#unmap-salesforce-fields-from-program-member-custom-fields}

Om du vill frigöra ett fält för att ersätta det, eller bara göra en allmän ändring, måste du först ta bort mappningen. Så här gör du.

1. Klicka på **[!UICONTROL Admin]** i Marketo.

   ![](assets/program-member-custom-field-sync-7.png)

1. Klicka på **[!DNL Salesforce]** och sedan på **[!UICONTROL Edit]** bredvid Synkronisering av anpassade fält för programmedlem.

   ![](assets/program-member-custom-field-sync-8.png)

1. Använd sökrutan för att hitta de fält som du vill ta bort mappningen för. I det här exemplet använder vi Do Not Call.

   ![](assets/program-member-custom-field-sync-9.png)

   >[!TIP]
   >
   >Du kan markera kryssrutan **[!UICONTROL Mapped]** om du bara vill visa mappade fält.

1. Ta bort mappningen genom att klicka på **X** bredvid fältet.

   ![](assets/program-member-custom-field-sync-10.png)

1. Mappningen har tagits bort. Klicka på **[!UICONTROL Save]**.

   ![](assets/program-member-custom-field-sync-11.png)

## Datatypsmappning {#data-type-mapping}

<table>
  <colgroup>
    <col/>
    <col/>
  </colgroup>
  <tbody>
    <tr>
      <th>SFDC-datatyp</th>
      <th>Datatyp för anpassat fält för programmedlem</th>
    </tr>
    <tr>
      <td>Text</td>
      <td>Sträng</td>
    </tr>
    <tr>
      <td>Picklist</td>
      <td>Sträng</td>
    </tr>
    <tr>
      <td>Flervalslista</td>
      <td>Sträng</td>
    </tr>
    <tr>
      <td>Tel.</td>
      <td>Sträng</td>
    </tr>
    <tr>
      <td>E-post</td>
      <td>Sträng</td>
    </tr>
    <tr>
      <td>Antal (m)</td>
      <td>Heltal</td>
    </tr>
    <tr>
      <td>Number(m,n)</td>
      <td>Float</td>
    </tr>
    <tr>
      <td>Kryssruta</td>
      <td>Boolean</td>
    </tr>
    <tr>
      <td>URL</td>
      <td>URL</td>
    </tr>
    <tr>
      <td>Datum</td>
      <td>Datum</td>
    </tr>
    <tr>
      <td>Datetime</td>
      <td>Datetime</td>
    </tr>
    <tr>
      <td>Uppslag (referens)</td>
      <td>Sträng</td>
    </tr>
    <tr>
      <td>Base64</td>
      <td>Sträng</td>
    </tr>
  </tbody>
</table>

>[!MORELIKETHIS]
>
>* [Ändra programmedlemsdata](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/program-flow-actions/change-program-member-data.md){target="_blank"}
>* [Visa data i programmedlemsrutnätet](/help/marketo/product-docs/core-marketo-concepts/programs/working-with-programs/manage-and-view-members.md){target="_blank"}
>* [SFDC-synkronisering - kampanjsynkronisering](/help/marketo/product-docs/crm-sync/salesforce-sync/sfdc-sync-details/sfdc-sync-campaign-sync.md){target="_blank"}
