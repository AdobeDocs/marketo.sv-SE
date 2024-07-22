---
unique-page-id: 2359422
description: Anpassa ett e-postmeddelande - Marketo Docs - produktdokumentation
title: Anpassa ett e-postmeddelande
exl-id: 1562796e-da47-4305-b950-3bed1d36d339
feature: Getting Started
source-git-commit: 431bd258f9a68bbb9df7acf043085578d3d91b1f
workflow-type: tm+mt
source-wordcount: '321'
ht-degree: 0%

---

# Anpassa ett e-postmeddelande {#personalize-an-email}

## Uppdrag: Gör dina e-postmeddelanden personliga genom att lägga till datatoken {#mission-make-your-emails-personal-by-adding-data-tokens}

>[!PREREQUISITES]
>
>* [Konfigurera och lägg till en person](/help/marketo/getting-started/quick-wins/get-set-up-and-add-a-person.md){target="_blank"}
>* [Skicka en e-postutbrytning](/help/marketo/getting-started/quick-wins/send-an-email.md){target="_blank"}
>* [Drip, Drip, Struktur](/help/marketo/getting-started/quick-wins/drip-drip-nurture.md){target="_blank"}

## Steg 1: Välj ett e-postmeddelande att anpassa {#step-select-an-email-to-personalize}

1. Välj en av de vårdnadstexter som skapades i [föregående snabbvinning](/help/marketo/getting-started/quick-wins/drip-drip-nurture.md){target="_blank"} och klicka på **[!UICONTROL Create draft]**.

   ![](assets/personalize-an-email-1.png)

   >[!NOTE]
   >
   >Detta skapar en kopia av e-postmeddelandet som ett utkast. Kom ihåg att godkänna utkastet för att ändringarna ska börja gälla.

Om du inte har aktiverat en popup-blockerare öppnas e-postredigeraren i ett nytt flik/fönster. Klicka annars **[!UICONTROL Create Draft]** två gånger.

## Steg 2: Gör säljaren till avsändaren {#step-make-the-salesperson-the-sender}

1. Markera fältet **[!UICONTROL From]**, markera och **ta bort** det aktuella namnet.

   ![](assets/personalize-an-email-2.png)

1. Klicka på ikonen **Token** till höger om fältet **[!UICONTROL From]**.

   ![](assets/personalize-an-email-3.png)

1. Sök efter och välj token **`{{lead.Lead Owner First Name}}`**.

   ![](assets/personalize-an-email-4.png)

1. Skriv ditt företagsnamn och ett bindestreck för **Standardvärdet** för att se till att något visas om säljarens förnamn inte är tillgängligt. Klicka på **Infoga**.

   ![](assets/personalize-an-email-5.png)

1. Tryck på blankstegstangenten i fältet **[!UICONTROL From]** och kontrollera att markören blinkar ett blanksteg efter den token du just infogade. Klicka sedan på ikonen **Token** igen.

   ![](assets/personalize-an-email-6.png)

1. Sök efter och välj token **`{{lead.Lead Owner Last Name}}`**.

   ![](assets/personalize-an-email-7.png)

1. Skriv&quot;Sales&quot; för **Default Value** och klicka på **Insert**.

   ![](assets/personalize-an-email-8.png)

## Steg 3: Lägg till leadens namn i e-postmeddelandet {#step-add-the-leads-name-to-the-email}

1. Markera det övre redigerbara avsnittet, klicka på kugghjulsikonen och välj **[!UICONTROL Edit]**.

   ![](assets/personalize-an-email-9.png)

1. Lägg till ett blanksteg efter &quot;Hello&quot; och placera markören framför kommatecknet och klicka sedan på ikonen **Infoga token** .

   ![](assets/personalize-an-email-10.png)

1. Sök efter och välj token **`{{lead.First Name}}`**.

   ![](assets/personalize-an-email-11.png)

1. Ange &quot;Kompis&quot; (eller en etikett som du vill ha) i fältet **[!UICONTROL Default Value]** och klicka på **[!UICONTROL Insert]**.

   ![](assets/personalize-an-email-12.png)

   >[!TIP]
   >
   >Inkludera alltid ett standardvärde för token. Detta garanterar att standardvärdet visas i e-postmeddelandet om en del av den personliga informationen saknas.

1. Klicka på **[!UICONTROL Save]**.

   ![](assets/personalize-an-email-13.png)

1. Under **[!UICONTROL Email Actions]** och välj **[!UICONTROL Approve and Close]**.

   ![](assets/personalize-an-email-14.png)

>[!TIP]
>
>Behöver du en snabb uppdatering av hur du skickar e-postmeddelandet till dig själv? Se [Skicka en e-postutbrytning](/help/marketo/getting-started/quick-wins/send-an-email.md){target="_blank"}.

### Uppdraget är slutfört {#mission-complete}

Grattis, du har personaliserat din e-post!

<br> 

[◄ 6: Drift, Drift, Struktur](/help/marketo/getting-started/quick-wins/drip-drip-nurture.md)

[Uppgift 8: Meddela säljaren ►](/help/marketo/getting-started/quick-wins/alert-the-sales-rep.md)
