---
unique-page-id: 2359422
description: Anpassa ett e-postmeddelande - Marketo Docs - Produktdokumentation
title: Anpassa ett e-postmeddelande
translation-type: tm+mt
source-git-commit: 5c9683c6b00ccbf9e9d606fd4513432c9872ad00
workflow-type: tm+mt
source-wordcount: '390'
ht-degree: 0%

---


# Anpassa ett e-postmeddelande {#personalize-an-email}

## Uppdrag: Gör dina e-postmeddelanden personliga genom att lägga till datatoken {#mission-make-your-emails-personal-by-adding-data-tokens}

>[!NOTE]
>
>**FYI**
>
>Marketo standardiserar nu språk för alla prenumerationer, så du kan se lead/leads i din prenumeration och person/personer på docs.marketo.com. Dessa termer betyder samma sak. det påverkar inte artikelinstruktionerna. Det finns andra förändringar också. [Läs mer](http://docs.marketo.com/display/DOCS/Updates+to+Marketo+Terminology).

>[!NOTE]
>
>**Förutsättningar**
>
>* [Konfigurera och lägga till en person](get-set-up-and-add-a-person.md)
>* [Skicka ett e-postutdrag](send-an-email.md)
>* [Drip, Drift, Struktur](drip-drip-nurture.md)


## Steg 1: Välj en e-postadress att anpassa {#step-select-an-email-to-personalize}

1. Välj en av de vårdnadstexter som skapades i den [tidigare snabbvinningen](drip-drip-nurture.md) och klicka på **Redigera utkast**.

   ![](assets/one-4.png)

   >[!NOTE]
   >
   >Detta skapar en kopia av e-postmeddelandet som ett utkast. Du måste godkänna utkastet för att ändringarna ska börja gälla.

   **Redigera utkast**

Om du inte har aktiverat en popup-blockerare öppnas e-postredigeraren i ett nytt flik/fönster. Klicka annars två gånger.

## Steg 2: Gör säljaren till avsändaren {#step-make-the-salesperson-the-sender}

1. Markera fältet **Från** , markera och **ta bort** det aktuella namnet.

   ![](assets/two-5.png)

1. Klicka på ikonen **Token** till höger om fältet **Från** .

   ![](assets/three-4.png)

1. Sök efter och välj **`{{lead.Lead Owner First Name}}`** token.

   ![](assets/four-3.png)

1. Skriv ditt företagsnamn och ett tankstreck för **standardvärdet** för att se till att något visas om säljarens förnamn inte är tillgängligt. Klicka på **Infoga**.

   ![](assets/five-4.png)

1. Tryck på blankstegstangenten i fältet **Från** och se till att markören blinkar ett blanksteg efter den variabel du just infogade. Klicka sedan på **tokenikonen** igen.

   ![](assets/six-4.png)

1. Sök efter och välj **`{{lead.Lead Owner Last Name}}`** token.

   ![](assets/seven-5.png)

1. Skriv&quot;Försäljning&quot; som **standardvärde** och klicka på **Infoga**.

   ![](assets/eight-3.png)

## Steg 3: Lägg till leadens namn i e-postmeddelandet {#step-add-the-leads-name-to-the-email}

1. Markera den övre redigerbara delen, klicka på kugghjulsikonen och välj **Redigera**.

   ![](assets/nine-2.png)

1. Lägg till ett blanksteg efter &quot;Hello&quot; och placera markören framför kommatecknet och klicka sedan på ikonen **Infoga token** .

   ![](assets/ten-4.png)

1. Sök efter och välj **`{{lead.First Name}}`** token.

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
>Behöver du en snabb uppdatering av hur du skickar e-postmeddelandet till dig själv? Se [Skicka en e-poststund](send-an-email.md).

### Se en video {#watch-a-video}

`<iframe width="630" height="470" src="//play.vidyard.com/iRnqxMyJg6VKyuPeuxmHFb.html?v=3.1.1" frameborder="0" allowfullscreen></iframe>`

### Uppdraget är slutfört {#mission-complete}

Grattis, du har personaliserat din e-post!

<br> 

[◄ 6: Drip, Drip,](drip-drip-nurture.md) Naturvårdsuppdrag [8: Meddela säljaren ►](alert-the-sales-rep.md)