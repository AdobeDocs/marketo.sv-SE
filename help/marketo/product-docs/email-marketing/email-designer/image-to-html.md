---
title: GenStudio Integration för Marketo Engage
description: Lär dig använda GenStudio i Marketo Engage.
solution: Marketo Engage
product: marketo
level: Beginner, Intermediate
feature: Email Designer
hide: true
hidefromtoc: true
source-git-commit: 6f1b4b6478e95d6d8aa332622daf2f29dd794bfe
workflow-type: tm+mt
source-wordcount: '1326'
ht-degree: 0%

---

# Konvertera bilder till HTML-mallar {#image-to-html}

## Översikt {#overview}

Konverteraren av bilder till HTML snabbar upp e-postproduktionen avsevärt genom att konvertera statiska bilder till fullt anpassningsbara, modulära mallar för e-postinnehåll från HTML. Med det här kodfria verktyget kan du omvandla visuell design från grafiska designers eller designverktyg till responsiva, redigerbara e-postmallar som kan återanvändas gång på gång.

Genom att utnyttja generativ AI-teknik analyserar konverteraren bild till HTML layout, typografi, färger och visuella element i bilden och genererar ren, modulär HTML-kod som bevarar designtroheten samtidigt som den säkerställer fullständig redigerbarhet och kompatibilitet med Email Designer.

>[!PREREQUISITES]
>
>* Du måste först godkänna villkoren för [Core Gen-AI och de kompletterande villkoren](https://www.adobe.com/legal/terms/enterprise-licensing/genai-ww.html){target="_blank"} för att kunna använda Gen-AI-funktionen i e-postprogrammet för Designer. Kontakta Adobe Account Team (din kontoansvarige) för mer information.
>* Du måste ha behörighet för _Åtkomstnamn_ och _Åtkomst till e-postmall_ aktiverad [&#x200B; i din Marketo-roll](https://experienceleague.adobe.com/sv/docs/marketo/using/product-docs/administration/users-and-roles/managing-user-roles-and-permissions#edit-a-role).

## Konvertera en bild {#convert-an-image}

Följ stegen nedan om du vill konvertera en bild till en helt anpassningsbar e-postmall från HTML.

>[!NOTE]
>
>För bästa resultat bör du använda bilder med hög kvalitet med tydliga visuella element och läsbar text. Bilderna bör helst vara 600-800 pixlar breda för att matcha e-postens standardmått.

1. I _Design Studio_ klickar du på **E-postmallar** och sedan på **E-postmallar (ny)**.

   ![](assets/image-to-html-1.png)

1. Klicka på **[!UICONTROL Convert image to template]**.

   ![](assets/image-to-html-2.png)

1. Ange ett _mallnamn_ och en valfri beskrivning. Du kan också välja vilken varumärkesstil du vill använda. Överför eller dra och släpp den önskade bilden.

   ![](assets/image-to-html-3.png)

   DEEPTHI KAN JAG DELETE DEN HÄR BILDTAGGEN...

   >[!CAUTION]
   >
   >När du överför en bild för konvertering tas **allt innehåll som för närvarande läggs till i e-postmeddelandet bort och ersätts** med den genererade mallen. Om du har befintligt innehåll i ditt e-postmeddelande måste du spara det innan du fortsätter med bildkonverteringen.

   DEEPTHI can I DELETE THIS CAUTION TAGG^^^

1. Bläddra nedåt och markera kryssrutan _Överföringsfilen innehåller inte.._. Klicka på **Konvertera**.

   ![](assets/image-to-html-4.png)

   >[!NOTE]
   >
   >Genereringsprocessen kan ta upp till fem minuter beroende på hur komplex och stor din bilddesign är. AI-bearbetningen sker i bakgrunden, så du kan navigera bort från den här skärmen och arbeta med andra åtgärder medan konverteringen pågår. Du kan behöva uppdatera biblioteksskärmen för _e-postmallen_ för att se statusändringen.

1. När konverteringen är klar sparas mallen automatiskt som ett utkast. Markera den.

   ![](assets/image-to-html-5.png)

1. Den konverterade mallen öppnas i e-post-Designer med fullständiga redigeringsfunktioner. Nu kan du:

   * Redigera textinnehåll och tillämpa personalisering
   * Ändra bilder och lägga till länkar
   * Justera färger, teckensnitt och format
   * Lägga till, ta bort eller ordna om innehållskomponenter
   * Utnyttja alla e-post-Designer-funktioner på samma sätt som andra mallar

   ![](assets/image-to-html-6.png){width="800" zoomable="yes"}

1. Ni kan göra vilka justeringar som helst för att förfina mallen och matcha varumärkesriktlinjerna.

1. När du är nöjd med mallen klickar du på **[!UICONTROL Save & close]** och sedan på **Publicera**.

Mallen är nu tillgänglig i biblioteket _E-postmallar_ och kan användas när du skapar e-postmeddelanden.

## Vanliga användningsfall {#use-cases}

Bilden till HTML-konverteraren är perfekt för:

* **Plattformsmigrering**: Migrerar från en annan e-postmarknadsföringsplattform? Konvertera dina befintliga e-postdesigner till HTML-mallar som är redo för Marketo Engage utan att behöva bygga om från grunden
* **Konvertering av designmodeller**: Omvandla designmodeller från verktyg som Photoshop, Figma eller andra designprogram till funktionella e-postmallar
* **Skapa mallar snabbt**: Generera e-postmallar snabbt för tidskänsliga kampanjer utan att vänta på utvecklarresurser
* **Skapa mallbibliotek**: Skapa ett omfattande bibliotek med varumärkeskonsekventa mallar som icke-tekniska teammedlemmar kan anpassa och distribuera

## Bästa praxis {#best-practices}

**Innan du börjar**

* **Spara befintligt innehåll**: Om du konverterar en bild till HTML ersätts allt befintligt innehåll i e-postmeddelandet. Spara alltid ditt aktuella arbete innan du använder den här funktionen.
* **Planera ditt arbetsflöde**: Använd konverteraren för bilden till HTML i början av e-postprocessen eller kontrollera att du är redo att ersätta allt aktuellt innehåll.

**Bildförberedelse**

* **Upplösning**: Använd högupplösta bilder för bättre textigenkänning och elementidentifiering.
* **Klarhet**: Kontrollera att texten är tydligt läsbar och att visuella element är väldefinierade.
* **Bredd**: Designa bilder med standardbredder för e-post (600-800px) så att de matchar vanliga krav för e-postklient.
* **Filformat**: Använd JPEG- eller PNG-format - undvik komprimerade bilder eller bilder med låg kvalitet.
* **Fullständig design**: Inkludera den fullständiga e-postdesignen i en enda bild, från sidhuvud till sidfot.

**Designöverväganden**

* **Enkla layouter**: Enkla, välstrukturerade layouter konverteras exaktare än mycket komplexa designer.
* **Standardelement**: Använd vanliga designmönster för e-post (sidhuvud, brödavsnitt, CTA:er, sidfot).
* **Textläsbarhet**: Kontrollera att texten och bakgrunden har tillräckligt hög kontrast.
* **Webbsäkra teckensnitt**: Designer som använder vanliga webbsäkra teckensnitt har bättre återgivning.
* **Undvik överlappande element**: Håll designelementen tydligt separerade för bättre strukturegenkänning.

**Efter konvertering**

* **Granska utkastet**: När konverteringen är klar sparas mallen automatiskt som ett utkast. Granska noggrant den genererade HTML:n.
* **Testa noggrant**: Testa e-postmeddelandet på olika e-postklienter och enheter. Utnyttja integrationen [Litmus](/help/marketo/product-docs/email-marketing/email-designer/test-email-rendering.md) om du vill få snabbare resultat.
* **Förfina manuellt**: Gör ändringar efter behov med e-postfunktionen Designer som ger fullständig redigering.
* **Varumärkesjustering**: Verifiera att färger, teckensnitt och format matchar varumärkesriktlinjerna.
* **Personalization**: Lägg till dynamiskt innehåll och personaliseringstoken efter behov.
* **Tillgänglighet**: Granska och förbättra tillgänglighetsfunktionerna om det behövs.

## Begränsningar och överväganden {#limitations}

Tänk på följande begränsningar när du använder Image to HTML-konverteraren.

* **AI-tolkning**: AI genererar HTML baserat på en visuell tolkning av din bild. Komplexa eller ovanliga designer kan kräva manuella justeringar efter konverteringen.

* **Textprecision**: Även om AI försöker identifiera och återge text korrekt måste du alltid verifiera textinnehållet och göra nödvändiga korrigeringar.

* **Dynamiskt innehåll**: Vid konverteringen skapas statisk HTML baserat på din bild. Ni måste lägga till personalisering, dynamiskt innehåll och spårning manuellt efter konverteringen.

* **Komplexa layouter**: Mycket komplexa designer med komplicerade lager, ovanliga former eller element som inte är standard kanske inte konverteras perfekt. Enklare design ger i allmänhet bättre resultat.

* **Bearbetningstid**: Konverteringsprocessen kan ta upp till fem minuter beroende på hur komplex och stor bilden är. AI-bearbetningen sker i bakgrunden, vilket gör att du kan arbeta med andra uppgifter utan att behöva hålla skärmen öppen. Mallen sparas automatiskt som ett utkast när konverteringen är klar.

>[!NOTE]
>
>Konverteraren för bilder till HTML är utformad för att ge en bra startpunkt för e-postgenerering. Den genererade HTML bör granskas och förfinas med e-post-Designer för att säkerställa att den uppfyller dina krav.

## Frågor och svar {#faq}

+++Vad händer med mitt befintliga e-postinnehåll när jag använder bilden till HTML-konverteraren?

Allt befintligt innehåll i e-postmeddelandet tas bort och ersätts med den nya mallen när du överför en bild för konvertering. Spara viktigt innehåll innan du använder den här funktionen. Det är bäst att använda konverteraren för bild till HTML i början av e-postprocessen.

+++

+++Vilka filformat stöds?

Konverteraren för bild till HTML stöder bildformaten JPEG (.jpg, .jpeg) och PNG (.png).

+++

+++Hur lång tid tar konverteringsprocessen?

Konverteringen kan ta upp till fem minuter, beroende på hur komplex och stor bilddesignen är. AI-bearbetningen sker i bakgrunden, så du kan navigera bort och arbeta med andra åtgärder. Du behöver inte hålla skärmen öppen. När konverteringen är klar sparas filen automatiskt som ett utkast som du kan granska och redigera.

+++

+++Kan jag redigera den genererade mallen?

Ja! Den genererade HTML-mallen öppnas i e-post-Designer med fullständiga redigeringsfunktioner. Du kan ändra alla aspekter av mallen, inklusive text, bilder, format, layout och struktur.

+++

+++Vad händer om konverteringen inte matchar min design exakt?

AI gör sitt bästa för att tolka din design på ett korrekt sätt, men det kan behövas vissa manuella finjusteringar. Använd e-post-Designer för att justera eventuella element som behöver finjusteras.

+++

+++Kan jag använda den här funktionen för landningssidor eller andra innehållstyper?

Konverteraren av bilder till HTML är för närvarande särskilt framtagen för e-postmallar. För andra innehållstyper använder du standardalternativen för design och import som finns i e-post-Designer.

+++

+++Kan jag återanvända konverterade mallar för flera e-postkampanjer?

Ja! Mallar som skapas med bilden till HTML-konverteraren sparas automatiskt i ditt _e-postmallsbibliotek_. Du kan komma åt och återanvända dem i alla e-postmeddelanden som kommer framåt.

+++
