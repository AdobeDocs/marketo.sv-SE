---
unique-page-id: 2953419
description: Använda Rich Text Editor - Marketo Docs - Produktdokumentation
title: Använda RTF-redigeraren
translation-type: tm+mt
source-git-commit: 0f0217a88929661798015b51a26259a973f9f6ea
workflow-type: tm+mt
source-wordcount: '736'
ht-degree: 0%

---


# Använda RTF-redigeraren {#using-the-rich-text-editor}

Textredigeraren (RTE) visas i hela Marketo och är tillgänglig när du vill lägga till eller redigera innehåll. Du kommer att se en version av den på landningssidor, program, e-post, formulär och utdrag. Klicka bara på **Redigera utkast** så öppnas det.

## Redigeringsinställningar {#editor-settings}

Rotblockelementets inställning definierar vilka taggar som omsluter innehållet. Som standard använder e-postrotelementet `<p>`-taggar. Du kan ändra det genom att följa stegen nedan.

>[!TIP]
>
>Även om du kan välja ditt rotblockselement rekommenderar vi alltid att du använder standardinställningarna för att få en så bra användarupplevelse som möjligt.

1. Klicka på **Admin**.

   ![](assets/one.png)

1. Klicka på **E-post**.

   ![](assets/two.png)

1. Klicka på **Redigera inställningar för textredigeraren**.

   ![](assets/three.png)

1. I listrutan **E-post-/fragmentredigerare** väljer du `<div>` eller Ingen och klickar på **Spara**. `<div>` används i det här exemplet.

   ![](assets/four.png)

   Om du har `<div class=“mktEditable”></div>` i en e-postmall visas följande HTML-källbeteende när du öppnar avsnittet och skriver&quot;Text Goes Here&quot; i redigeraren:

<table> 
 <tbody> 
  <tr> 
   <th>&lt;p&gt;</th> 
   <th>&lt;div&gt;</th> 
   <th>Ingen</th> 
  </tr> 
  <tr> 
   <td><p>&lt;div class="“mktEditable”"&gt;<br>&lt;p&gt;Texten visas här&lt;/p&gt;<br>&lt;/div&gt;</p></td> 
   <td><p>&lt;div class="“mktEditable”"&gt;<br>&lt;div&gt;Texten visas här&lt;/div&gt;<br>&lt;/div&gt;</p></td> 
   <td><p>&lt;div class="“mktEditable”"&gt;<br>Texten visas här<br>&lt;/div&gt;</p></td> 
  </tr> 
 </tbody> 
</table>

>[!TIP]
>
>Du kan också ändra startssidredigerarens rotblockselement genom att följa samma steg, men klicka på listrutan **Landing Page Editor** i steg 4 i stället för i e-postredigeraren.

>[!NOTE]
>
>Rotblockelementet är alltid `<p>` för RTF-programtoken.

## Funktioner {#features}

Här är de funktioner du hittar i en RTE.

| Ikon | Namn | Vad det gör |
|---|---|---|
| ![—](assets/image2015-7-9-10-3a23-3a24.png) | Teckensnittsfamilj | Välj din stil - vi har massor! |
| ![—](assets/image2015-7-9-10-3a22-3a11.png) | Teckenstorlek | Hur stor vill du ha den? 25 alternativ, från 8 px till 90 px. |
| ![—](assets/image2015-7-9-10-3a59-3a4.png) | Stilar | Välj Stycke eller ett format med sex rubriker (för landningssidor). |
| ![—](assets/image2015-7-9-10-3a20-3a1.png) | Radavstånd | Välj avståndet mellan raderna. |
| ![—](assets/image2015-7-9-10-3a25-3a52.png) | Textfärg | Svart, röd eller vad du vill. |
| ![—](assets/image2015-7-9-10-3a24-3a38.png) | Bakgrundsfärg | Markera för att betona. |
| ![—](assets/image2015-7-9-10-3a28-3a4.png) | Fet | **Mörkare och tjockare**. |
| ![—](assets/image2015-7-9-10-3a29-3a1.png) | Kursiv | *Vinklad, för betoning eller* citat. |
| ![—](assets/image2015-7-9-10-3a30-3a56.png) | Understruken | Placerar en linje under texten. |
| ![—](assets/image2015-7-9-10-3a31-3a57.png) | Justering | Använd den här listrutan för att utforma text och bilder. Centrera dem, välj vänster- eller högerjustering eller lägg kanten på kanten med fullständig justering. |  | ![—](assets/image2015-7-9-10-3a32-3a47.png) | Lista | Välj punkter eller nummer i listrutan. Punkter är bra med listor och siffror med steg. |
| ![—](assets/image2015-7-9-10-3a38-3a0.png) | Indrag | Välj mer eller mindre indrag. Använd för stycken eller text som du vill sticka ut. |
| ![—](assets/image2015-7-9-10-3a38-3a58.png) | Infoga/redigera länk | Lägg in en länk till en webbplats eller annat innehåll. gör enkelt ändringar i den. |
| ![—](assets/image2015-7-9-10-3a39-3a42.png) | Infoga/redigera bild | En bild säger mer än tusen ord. Släpp in en. Klicka på kameraikonen för att bläddra i Design Studio. Du kan släppa bilder sida vid sida. |
| ![—](assets/image2015-7-9-10-3a40-3a36.png) | Infoga token | Ett kraftfullt verktyg som passar utmärkt för e-postpersonalisering och dataspårning. Var noga med att ange ett standardvärde. |
| ![—](assets/image2015-7-9-10-3a41-3a21.png) | Ångra | Oj då! Gå tillbaka ett steg och försök igen. |
| ![—](assets/image2015-7-9-10-3a42-3a13.png) | Gör om | Om det verkligen är okej, gå tillbaka till originalet. |
| ![—](assets/image2015-7-9-10-3a43-3a29.png) | Tabell | Bygg din egen, som den här. Med en nedrullningsbar meny kan du konfigurera den. |
| ![—](assets/image2015-7-9-10-3a45-3a1.png) | Infoga ankarpunkt | Släpp ankare! |
| ![—](assets/image2015-7-9-10-3a45-3a48.png) | Vågrät linje | Många användningsområden - Perfekt för att dela upp avsnitt. |
| ![—](assets/image2015-10-6-12-3a12-3a17.png) | Redigera HTML | Popup-fönstret för HTML-källkodsredigeraren så att du kan justera koden. |
| ![—](assets/image2015-7-9-10-3a47-3a36.png) | Nedsänkt | Låga hängande bokstäver (som i O`<sub>2</sub>`). |
| ![—](assets/image2015-7-9-10-3a48-3a35.png) | Upphöjd | Du har kraften! (2`<sup>6</sup>`). |
| ![—](assets/image2015-7-9-10-3a49-3a31.png) | Genomstruken | `<s>Put a line through text, like this</s>`. |
| ![—](assets/image2015-7-9-10-3a50-3a11.png) | Specialtecken | Vill du prata om euro? Matematik? Du har 243 val. |
| ![—](assets/image2015-7-9-10-3a52-3a26.png) | Sök och ersätt | Sök efter och ändra saker mycket snabbare än att leta efter varje instans själv. |
| ![—](assets/image2015-7-9-10-3a53-3a37.png) | Radera formatering | Återgå till standard. |
| ![—](assets/image2015-7-9-10-3a55-3a2.png) | Avbryt | Tryck på knappen för att säga &quot;Strunta i det.&quot; |
| ![—](assets/image2015-7-9-10-3a56-3a2.png) | Spara | Tryck på knappen för att säga &quot;OK, I like it.&quot; |

>[!TIP]
>
>Du kan redigera HTML och text på olika skärmar. Var noga med att klicka på **Kopiera från HTML** på fliken **Text** och sedan på **Spara** så att texten matchar HTML-koden.

>[!NOTE]
>
>Du är inte begränsad till teckensnitten i listrutan. Du kan använda en som inte finns med i listan genom att gå till HTML-koden. Alla webbteckensnitt stöds i Marketo, men webbteckensnitt fungerar inte överallt i alla e-postklienter.

## Landningssidor {#landing-pages}

Rotblockelementets inställning definierar vilka taggar som omsluter innehållet. Som standard använder rotblockselementet för landningssidan `<div>`-taggar. Du kan ändra det genom att följa stegen nedan.

>[!TIP]
>
>Även om du kan välja ditt rotblockselement rekommenderar vi alltid att du använder standardinställningarna för att få en så bra användarupplevelse som möjligt.

1. Klicka på **Admin**.

   ![](assets/one.png)

1. Klicka på **E-post**.

   ![](assets/two.png)

1. Klicka på **Redigera inställningar för textredigeraren**.

   ![](assets/three.png)

1. I listrutan **Landing Page Editor** väljer du `<p>` eller Ingen och klickar på **Spara**. `<p>` används i det här exemplet.

   ![](assets/five.png)

   Och det är allt!
