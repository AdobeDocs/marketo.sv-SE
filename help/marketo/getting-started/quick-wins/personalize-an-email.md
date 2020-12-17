---
unique-page-id: 2359422
description: Anpassa ett e-postmeddelande - Marketo Docs - Produktdokumentation
title: Anpassa ett e-postmeddelande
translation-type: tm+mt
source-git-commit: d7d6aee63144c472e02fe0221c4a164183d04dd4
workflow-type: tm+mt
source-wordcount: '335'
ht-degree: 0%

---


# Anpassa ett e-postmeddelande {#personalize-an-email}

## Uppdrag: Gör dina e-postmeddelanden personliga genom att lägga till datatoken {#mission-make-your-emails-personal-by-adding-data-tokens}

>[!PREREQUISITES]
>
>* [Konfigurera och lägga till en person](/help/marketo/getting-started/quick-wins/get-set-up-and-add-a-person.md)
>* [Skicka ett e-postutdrag](/help/marketo/getting-started/quick-wins/send-an-email.md)
>* [Drip, Drift, Struktur](/help/marketo/getting-started/quick-wins/drip-drip-nurture.md)


## Steg 1: Välj en e-postadress att anpassa {#step-select-an-email-to-personalize}

1. Välj en av de vårdnadstexter som skapades i [föregående snabbwin](/help/marketo/getting-started/quick-wins/drip-drip-nurture.md) och klicka på **Redigera utkast**.

   ![](assets/one-4.png)

   >[!NOTE]
   >
   >Detta skapar en kopia av e-postmeddelandet som ett utkast. Du måste godkänna utkastet för att ändringarna ska börja gälla.

Om du inte har aktiverat en popup-blockerare öppnas e-postredigeraren i ett nytt flik/fönster. Annars klickar du **Redigera utkast** två gånger.

## Steg 2: Gör säljaren till avsändaren {#step-make-the-salesperson-the-sender}

1. Markera fältet **Från**, markera och **ta bort** det aktuella namnet.

   ![](assets/two-5.png)

1. Klicka på ikonen **Token** till höger om fältet **Från**.

   ![](assets/three-4.png)

1. Sök efter och välj **`{{lead.Lead Owner First Name}}`**-token.

   ![](assets/four-3.png)

1. Skriv ditt företagsnamn och ett bindestreck för **Standardvärdet** för att se till att något visas om säljarens förnamn inte är tillgängligt. Klicka på **Infoga**.

   ![](assets/five-4.png)

1. Tryck på blankstegstangenten i fältet **Från** och se till att markören blinkar ett blanksteg efter den variabel du just infogade. Klicka sedan på ikonen **Token** igen.

   ![](assets/six-4.png)

1. Sök efter och välj **`{{lead.Lead Owner Last Name}}`**-token.

   ![](assets/seven-5.png)

1. Skriv &quot;Sales&quot; för **Standardvärde** och klicka på **Infoga**.

   ![](assets/eight-3.png)

## Steg 3: Lägg till leadens namn i e-postmeddelandet {#step-add-the-leads-name-to-the-email}

1. Markera den övre redigerbara delen, klicka på kugghjulsikonen och välj **Redigera**.

   ![](assets/nine-2.png)

1. Lägg till ett blanksteg efter &quot;Hello&quot; och placera markören framför kommatecknet och klicka sedan på ikonen **Infoga token**.

   ![](assets/ten-4.png)

1. Sök efter och välj **`{{lead.First Name}}`**-token.

   ![](assets/eleven-4.png)

1. Ange &quot;Kompis&quot; (eller en etikett du vill ha) i fältet **Standardvärde** och klicka på **Infoga**.

   ![](assets/twelve-3.png)

   >[!TIP]
   >
   >Inkludera alltid ett standardvärde för token; Detta garanterar att standardvärdet visas i e-postmeddelandet om en del av den personliga informationen saknas.

1. Klicka på **Spara**.

   ![](assets/thirteen-3.png)

1. Stäng fliken/fönstret för e-postredigeraren.

   ![](assets/fourteen-3.png)

1. Under **E-poståtgärder** väljer du **Godkänn utkast**.

   ![](assets/fifteen-3.png)

>[!TIP]
>
>Behöver du en snabb uppdatering av hur du skickar e-postmeddelandet till dig själv? Se [Skicka en e-poststund](/help/marketo/getting-started/quick-wins/send-an-email.md).

### Uppdraget är klart {#mission-complete}

Grattis, du har personaliserat din e-post!

<br> 

[◄ 6: Drip, Drift, Struktur](/help/marketo/getting-started/quick-wins/drip-drip-nurture.md)

[Uppdrag 8: Meddela säljaren ►](/help/marketo/getting-started/quick-wins/alert-the-sales-rep.md)
