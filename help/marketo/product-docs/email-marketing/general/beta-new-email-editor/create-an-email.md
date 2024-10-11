---
description: Skapa ett e-postmeddelande - Marketo Docs - produktdokumentation
title: Skapa ett e-postmeddelande
hide: true
hidefromtoc: true
feature: Email Editor
source-git-commit: 2d69e52883d141e3976c6d4fc1de6038675af602
workflow-type: tm+mt
source-wordcount: '1063'
ht-degree: 0%

---

# Skapa ett e-postmeddelande {#create-an-email}

Introduktionstext här.

>[!IMPORTANT]
>
>Den här artikeln är endast avsedd för medlemmar av den nya e-postredigeraren i Marketo Engage som har en sluten betaversion. Sprid inte information.

1. Logga in på Marketo Engage via [Adobe Experience Cloud](https://experiencecloud.adobe.com/){target="_blank"}.

1. I Min Marketo väljer du **Design Studio**.

   ![](assets/create-an-email-1.png)

1. Välj **E-post (ny redigerare)** i trädet.

   ![](assets/create-an-email-2.png)

1. Klicka på knappen **Skapa e-post** .

   ![](assets/create-an-email-3.png)

1. Ange ett e-postnamn och en ämnesrad. Klicka på **Skapa**.

   ![](assets/create-an-email-4.png)

Så där ja. Nu är det dags att designa e-postmeddelanden.

## Välj innehållstyp {#choose-your-content-type}

1. Klicka på **+ Lägg till e-postinnehåll** i det e-postmeddelande du just skapade.

   SCREENSHOT

1. Sidan Skapa din e-post visas. Du kan välja mellan några alternativ:

* [Designa från grunden](#design-from-scratch) med e-postredigeraren

* [Importera din egen HTML](#import-html) via en HTML- eller zip-fil

* [Välj en befintlig mall](#choose-a-template) (ett av våra exempel eller ett du redan har sparat)

### Designa från grunden {#design-from-scratch}

När du börjar från början i e-postredigeraren använder du alternativen nedan för att definiera ditt innehåll.

1. Välj **Designa från grunden** på mallstartsidan.

Lägg till struktur och innehåll i e-postmeddelandet.

Lägg till bilder.

Anpassa innehållet.

Granska och uppdatera länkar.

### Importera HTML {#import-html}

Du kan importera befintligt HTML-innehåll för att utforma e-postmallar. Innehållet kan vara

* En HTML-fil med en infogad formatmall

* En ZIP-fil som innehåller en HTML-fil, formatmallen (.css) och bilder

>[!NOTE]
>
>ZIP-filstrukturen har inga begränsningar. Referenserna måste dock vara relativa och passa in i trädstrukturen i ZIP-mappen.

1. Välj **Importera HTML** på mallsidan.

   SCREENSHOT

1. Dra och släpp HTML- eller ZIP-filen och klicka på **Importera**.

   SCREENSHOT

>[!NOTE]
>
>När HTML-innehållet har överförts är ditt innehåll i kompatibilitetsläge. I det här läget kan du bara anpassa texten, lägga till länkar eller inkludera resurser i innehållet.

Du kan göra önskade ändringar av det importerade innehållet med hjälp av [e-postredigeringsverktygen](#add-structure-and-content).

### Välj en mall {#choose-a-template}

Det finns två typer av mallar att välja mellan.

* Exempelmallar: Marketo Engage har fyra färdiga e-postmallar.

* Sparade mallar: Det här är mallar som du har skapat från grunden med hjälp av menyn Mallar eller ett e-postmeddelande som du har skapat och valt att spara som en mall.

>[!BEGINTABS]

>[!TAB Exempelmallar]

Välj en av våra färdiga mallar för att snabbt komma igång med e-postdesignen.

1. Välj **Exempelmallar** på sidan Skapa din e-post.

   SCREENSHOT

1. Välj önskad mall.

   SCREENSHOT

1. En förhandsgranskning visas. Bekräfta ditt val genom att klicka på **Använd den här mallen**.

   SCREENSHOT

>[!TAB Sparade mallar]

Välj någon av de mallar du skapat tidigare.

1. Välj Sparade mallar på sidan Skapa din e-post.

   SCREENSHOT

1. Välj önskad mall.

   SCREENSHOT

1. En förhandsgranskning visas. Bekräfta ditt val genom att klicka på **Använd den här mallen**.

   SCREENSHOT

>[!ENDTABS]

## Lägga till struktur och innehåll {#add-structure-and-content}

1. Om du vill börja skapa eller ändra innehåll drar och släpper du ett objekt från Strukturer på arbetsytan. Redigera inställningarna i rutan till höger.

   >[!TIP]
   >
   >Markera n:n-kolumnkomponenten för att definiera hur många kolumner du vill ha (mellan tre och 10). Du kan också definiera bredden på varje kolumn genom att flytta pilarna under kolumnen.

   SCREENSHOT

   >[!NOTE]
   >
   >Varje kolumnstorlek får inte vara mindre än 10 % av strukturkomponentens totala bredd. Endast tomma kolumner kan tas bort.

1. I avsnittet Innehåll drar du över önskade objekt och släpper dem i en eller flera strukturkomponenter.

   SCREENSHOT

1. Varje komponent kan anpassas via flikarna Inställningar eller Format. Ändra teckensnitt, textstil, marginal med mera.

SCREENSHOT

### Lägg till Assets {#add-assets}

I resursväljaren kan du välja resurser som lagras direkt i Assets-biblioteket. Dubbelklicka på den mapp som innehåller dina resurser. Dra och släpp dem i en strukturkomponent.

Infoga anpassningsfält för att anpassa innehållet utifrån profilattribut, målgruppsmedlemskap, sammanhangsbaserade attribut med mera.

Klicka på Aktivera villkorsinnehåll för att lägga till dynamiskt innehåll och anpassa innehållet till målprofilerna baserat på villkorliga regler.

Klicka på fliken Länkar i den vänstra rutan för att visa alla URL:er för innehållet som ska spåras. Du kan ändra deras spårningstyp eller etikett och lägga till taggar om det behövs.

Om det behövs kan du anpassa e-postmeddelandet ytterligare genom att klicka på Växla till kodredigerare på den avancerade menyn. På så sätt kan du redigera e-postkällkoden, till exempel för att lägga till spårningstaggar eller anpassade HTML-taggar.

FÖRSIKTIGHET
Du kan inte återgå till den visuella designern för det här e-postmeddelandet efter att du har växlat till kodredigeraren.

När innehållet är klart klickar du på knappen Simulera innehåll för att kontrollera återgivningen. Du kan välja skrivbordsvy eller mobilvy.

När du är klar klickar du på Spara





## Kontrollera aviseringar {#check-alerts}

När du utformar ditt innehåll visas varningar i gränssnittet (längst upp till höger på skärmen) när nyckelinställningar saknas.

Det finns två typer av varningar:

**Varningar**

Varningar hänvisar till rekommendationer och bästa praxis, som:

* **Avanmälningslänken finns inte i e-postmeddelandet**: Även om det är ett krav att avbryta prenumerationen är det bäst att lägga till dem i e-postmeddelandet.

>[!NOTE]
>
>Du behöver inte lägga till ett alternativ för att avbryta prenumerationen för [operativa e-postmeddelanden](/help/marketo/product-docs/email-marketing/general/functions-in-the-editor/make-an-email-operational.md) (ej marknadsföring).

* **Textversionen av HTML är tom**: Du måste definiera en textversion av e-postbrödtexten för när HTML-innehåll inte kan visas.

* **En tom länk finns i e-postbrödtexten**: Kontrollera att alla länkar i e-postmeddelandet är korrekta.

* **E-poststorleken har överskridit gränsen på 100 kB**: Kontrollera att e-postens storlek inte överskrider 100 kB för optimal leverans.

**Fel**

Fel förhindrar att du skickar eller testar e-postmeddelandet tills de har lösts:

* **Ämnesraden saknas**: En ämnesrad för e-post krävs.

* **E-postversionen av meddelandet är tom**: Det här felet inträffar när e-postinnehållet inte har konfigurerats.

## Testa din e-post

När meddelandeinnehållet har definierats kan du använda testprofiler för att förhandsgranska det, skicka korrektur och styra hur det återges i vanliga dator-, mobil- och webbaserade klienter. Om du har infogat anpassat innehåll kan du kontrollera hur det visas i meddelandet med hjälp av testprofilsdata.

Om du vill förhandsgranska ditt e-postinnehåll klickar du på **Simulera innehåll** och lägger sedan till en testprofil för att kontrollera meddelandet med testprofildata.

SCREENSHOT

## Referera till ett e-postmeddelande {#reference-an-email}

När du har skapat ett e-postmeddelande i den nya redigeraren kan du referera till det i Smarta kampanjer eller Smarta listor på samma sätt som du gör med andra e-postmeddelanden.

* Referera den i en smart lista genom att [följa de vanliga stegen](/help/marketo/product-docs/core-marketo-concepts/smart-lists-and-static-lists/creating-a-smart-list/create-a-smart-list.md).

* Referera det i en smart kampanj genom att [följa de vanliga stegen](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/creating-a-smart-campaign/create-a-new-smart-campaign.md).

>[!NOTE]
>
>Det går bara att referera till sparade e-postmeddelanden. Den nya e-postredigeraren har ingen&quot;godkänd&quot; status.
