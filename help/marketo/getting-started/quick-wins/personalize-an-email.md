---
unique-page-id: 2359422
description: Anpassa ett e-postmeddelande - Marketo Docs - produktdokumentation
title: Anpassa ett e-postmeddelande
exl-id: 1562796e-da47-4305-b950-3bed1d36d339
source-git-commit: 8aa2f3069c0168f57ac00dfc7270484a9045584c
workflow-type: tm+mt
source-wordcount: '341'
ht-degree: 0%

---

# Anpassa ett e-postmeddelande {#personalize-an-email}

## Uppdrag: Gör dina e-postmeddelanden personliga genom att lägga till datatoken {#mission-make-your-emails-personal-by-adding-data-tokens}

>[!PREREQUISITES]
>
>* [Konfigurera och lägga till en person](/help/marketo/getting-started/quick-wins/get-set-up-and-add-a-person.md){target=&quot;_blank&quot;}
>* [Skicka ett e-postutdrag](/help/marketo/getting-started/quick-wins/send-an-email.md){target=&quot;_blank&quot;}
>* [Drip, Drift, Struktur](/help/marketo/getting-started/quick-wins/drip-drip-nurture.md){target=&quot;_blank&quot;}


## Steg 1: Välj en e-postadress att anpassa {#step-select-an-email-to-personalize}

1. Välj en av de e-postmeddelanden som har skapats i dialogrutan [föregående snabbvinst](/help/marketo/getting-started/quick-wins/drip-drip-nurture.md){target=&quot;_blank&quot;} och klicka på **Skapa utkast**.

   ![](assets/personalize-an-email-1.png)

   >[!NOTE]
   >
   >Detta skapar en kopia av e-postmeddelandet som ett utkast. Kom ihåg att godkänna utkastet för att ändringarna ska börja gälla.

Om du inte har aktiverat en popup-blockerare öppnas e-postredigeraren i ett nytt flik/fönster. I annat fall klickar du på **Skapa utkast** två gånger.

## Steg 2: Gör säljaren till avsändaren {#step-make-the-salesperson-the-sender}

1. Välj **Från** fält, markera och **delete** det aktuella namnet.

   ![](assets/personalize-an-email-2.png)

1. Klicka på **Token** ikonen till höger om **Från** fält.

   ![](assets/personalize-an-email-3.png)

1. Sök och välj **`{{lead.Lead Owner First Name}}`** token.

   ![](assets/personalize-an-email-4.png)

1. Ange ditt företagsnamn och ett tankstreck för **Standardvärde** för att säkerställa att något visas om säljarens förnamn inte är tillgängligt. Klicka **Infoga**.

   ![](assets/personalize-an-email-5.png)

1. Tryck på blankstegstangenten i **Från** ska du se till att markören blinkar ett blanksteg efter den variabel du just infogade. Klicka sedan på **Token** ikonen igen.

   ![](assets/personalize-an-email-6.png)

1. Sök och välj **`{{lead.Lead Owner Last Name}}`** token.

   ![](assets/personalize-an-email-7.png)

1. Skriv&quot;Försäljning&quot; för **Standardvärde** och klicka **Infoga**.

   ![](assets/personalize-an-email-8.png)

## Steg 3: Lägg till leadens namn i e-postmeddelandet {#step-add-the-leads-name-to-the-email}

1. Markera det övre redigerbara avsnittet, klicka på kugghjulsikonen och välj **Redigera**.

   ![](assets/personalize-an-email-9.png)

1. Lägg till ett blanksteg efter &quot;Hello&quot; och placera markören framför kommatecknet och klicka sedan på **Infoga token** ikon.

   ![](assets/personalize-an-email-10.png)

1. Sök och välj **`{{lead.First Name}}`** token.

   ![](assets/personalize-an-email-11.png)

1. Ange &quot;Kompis&quot; (eller någon annan etikett du vill ha) i dialogrutan **Standardvärde** fält och klicka **Infoga**.

   ![](assets/personalize-an-email-12.png)

   >[!TIP]
   >
   >Inkludera alltid ett standardvärde för token; Detta garanterar att standardvärdet visas i e-postmeddelandet om en del av den personliga informationen saknas.

1. Klicka **Spara**.

   ![](assets/personalize-an-email-13.png)

1. Under **E-poståtgärder** och markera **Godkänn och stäng**.

   ![](assets/personalize-an-email-14.png)

>[!TIP]
>
>Behöver du en snabb uppdatering av hur du skickar e-postmeddelandet till dig själv? Se [Skicka ett e-postutdrag](/help/marketo/getting-started/quick-wins/send-an-email.md){target=&quot;_blank&quot;}.

### Uppdraget är slutfört {#mission-complete}

Grattis, du har personaliserat din e-post!

<br> 

[◄ 6: Drip, Drift, Struktur](/help/marketo/getting-started/quick-wins/drip-drip-nurture.md)

[Uppdrag 8: Meddela säljaren ►](/help/marketo/getting-started/quick-wins/alert-the-sales-rep.md)
