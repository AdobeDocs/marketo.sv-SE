---
unique-page-id: 2953419
description: Använda RTF-redigeraren - Marketo Docs - produktdokumentation
title: Använda RTF-redigeraren
exl-id: 9b2d6d41-f947-4859-aad9-a10c15eb013a
feature: Email Editor
source-git-commit: 26573c20c411208e5a01aa7ec73a97e7208b35d5
workflow-type: tm+mt
source-wordcount: '659'
ht-degree: 1%

---

# Använda RTF-redigeraren {#using-the-rich-text-editor}

Textredigeraren (RTE) visas i hela Marketo och är tillgänglig när du vill lägga till eller redigera innehåll. Du kommer att se en version av den på landningssidor, program, e-post, formulär och utdrag. Klicka bara på **[!UICONTROL Edit Draft]** så öppnas den så att du kan ta del av den.

## Inställningar för Redigeraren {#editor-settings}

Rotblockelementets inställning definierar vilka taggar som omsluter innehållet. Som standard använder e-postrotelementet `<p>`-taggar. Du kan ändra det genom att följa stegen nedan.

>[!TIP]
>
>Även om du kan välja ditt rotblockselement rekommenderar vi alltid att du använder standardinställningarna för att få en så bra användarupplevelse som möjligt.

1. Klicka på **[!UICONTROL Admin]**.

   ![](assets/one.png)

1. Klicka på **[!UICONTROL Email]**.

   ![](assets/two.png)

1. Klicka på **[!UICONTROL Edit Text Editor Settings]**.

   ![](assets/three.png)

1. I listrutan **[!UICONTROL Email]/[!UICONTROL Snippet Editor]** väljer du `<div>` eller [!UICONTROL None] och klickar på **[!UICONTROL Save]**. `<div>` används i detta exempel.

   ![](assets/four.png)

   Om du har `<div class=“mktEditable”></div>` i en e-postmall visas följande HTML Source-beteende när du öppnar avsnittet och skriver&quot;Text Goes Here&quot; i redigeraren:

<table>
 <tbody>
  <tr>
   <th>&lt;p&gt;</th>
   <th>&lt;div&gt;</th>
   <th>Ingen</th>
  </tr>
  <tr>
   <td><p>&lt;div class="mktEditable"&gt;<br>&lt;p&gt;Text Goes Here&lt;/p&gt;<br>&lt;/div&gt;</p></td>
   <td><p>&lt;div class="mktEditable"&gt;<br>&lt;div&gt;Text Goes Here&lt;/div&gt;<br>&lt;/div&gt;</p></td>
   <td><p>&lt;div class="mktEditable"&gt;<br>Text Goes Here<br>&lt;/div&gt;</p></td>
  </tr>
 </tbody>
</table>

>[!TIP]
>
>Du kan också ändra startssidredigerarens rotblockselement genom att följa samma steg, men klicka på listrutan **[!UICONTROL Landing Page Editor]** i steg 4 i stället för [!UICONTROL Email] / [!UICONTROL Snippet Editor].

>[!NOTE]
>
>Rotblockelementet är alltid `<p>` för RTF-programtoken.

## Funktioner {#features}

Här är de funktioner du hittar i en RTE.

| Ikon | Namn | Vad det gör |
|---|---|---|
| ![—](assets/image2015-7-9-10-3a23-3a24.png) | [!UICONTROL Font Family] | Välj din stil - vi har massor! |
| ![—](assets/image2015-7-9-10-3a22-3a11.png) | [!UICONTROL Font Size] | Hur stor vill du ha den? 25 alternativ, från 8 px till 90 px. |
| ![—](assets/image2015-7-9-10-3a59-3a4.png) | [!UICONTROL Styles] | Välj Stycke eller ett format med sex rubriker (för landningssidor). |
| ![—](assets/image2015-7-9-10-3a20-3a1.png) | [!UICONTROL Line Spacing] | Välj avståndet mellan raderna. |
| ![—](assets/image2015-7-9-10-3a25-3a52.png) | [!UICONTROL Text Color] | Svart, röd eller vad du vill. |
| ![—](assets/image2015-7-9-10-3a24-3a38.png) | [!UICONTROL Background Color] | Markera för att framhäva. |
| ![—](assets/image2015-7-9-10-3a28-3a4.png) | [!UICONTROL Bold] | **Mörkare och tjockare**. |
| ![—](assets/image2015-7-9-10-3a29-3a1.png) | [!UICONTROL Italic] | *Vinklad, för betoning eller citat* s. |
| ![—](assets/image2015-7-9-10-3a30-3a56.png) | [!UICONTROL Underline] | Placerar en linje under texten. |
| ![—](assets/image2015-7-9-10-3a31-3a57.png) | [!UICONTROL Alignment] | Använd den här listrutan för att utforma text och bilder. Centrera dem, välj vänster- eller högerjustering eller lägg kanten på kanten med fullständig justering. |  | ![—](assets/image2015-7-9-10-3a32-3a47.png) | Lista | Välj punkter eller nummer i listrutan. Punkter är bra med listor och siffror med steg. |
| ![—](assets/image2015-7-9-10-3a38-3a0.png) | [!UICONTROL Indent] | Välj mer eller mindre indrag. Använd för stycken eller text som du vill sticka ut. |
| ![—](assets/image2015-7-9-10-3a38-3a58.png) | [!UICONTROL Insert/Edit Link] | Lägg in en länk till en webbplats eller annat innehåll och gör enkelt ändringar i den. |
| ![—](assets/image2015-7-9-10-3a39-3a42.png) | [!UICONTROL Insert/Edit Image] | En bild säger mer än tusen ord. Släpp in en. Klicka på kameraikonen för att bläddra i Design Studio. Du kan släppa bilder sida vid sida. |
| ![—](assets/image2015-7-9-10-3a40-3a36.png) | [!UICONTROL Insert Token] | Ett kraftfullt verktyg som passar utmärkt för e-postpersonalisering och dataspårning. Var noga med att ange ett standardvärde. |
| ![—](assets/image2015-7-9-10-3a41-3a21.png) | [!UICONTROL Undo] | Oj då! Gå tillbaka ett steg och försök igen. |
| ![—](assets/image2015-7-9-10-3a42-3a13.png) | [!UICONTROL Redo] | Om det verkligen är okej, gå tillbaka till originalet. |
| ![—](assets/image2015-7-9-10-3a43-3a29.png) | [!UICONTROL Table] | Bygg din egen, som den här. Med en nedrullningsbar meny kan du konfigurera den. |
| ![—](assets/image2015-7-9-10-3a45-3a1.png) | [!UICONTROL Insert Anchor] | Släpp ankare! |
| ![—](assets/image2015-7-9-10-3a45-3a48.png) | [!UICONTROL Horizontal Line] | Många användningsområden - Perfekt för att dela upp avsnitt. |
| ![—](assets/image2015-10-6-12-3a12-3a17.png) | [!UICONTROL Edit HTML] | Uppgraderar HTML Source Editor så att du kan redigera koden. |
| ![—](assets/image2015-7-9-10-3a47-3a36.png) | [!UICONTROL Subscript] | Låga hängande bokstäver (som i O`<sub>2</sub>`). |
| ![—](assets/image2015-7-9-10-3a48-3a35.png) | [!UICONTROL Superscript] | Du har kraften! (2`<sup>6</sup>`). |
| ![—](assets/image2015-7-9-10-3a49-3a31.png) | [!UICONTROL Strikethrough] | `<s>Put a line through text, like this</s>`. |
| ![—](assets/image2015-7-9-10-3a50-3a11.png) | [!UICONTROL Special Character] | Vill du prata om euro? Matematik? Du har 243 val. |
| ![—](assets/image2015-7-9-10-3a52-3a26.png) | [!UICONTROL Find and Replace] | Sök efter och ändra saker mycket snabbare än att leta efter varje instans själv. |
| ![—](assets/image2015-7-9-10-3a53-3a37.png) | [!UICONTROL Clear Formatting] | Återgå till standard. |
| ![—](assets/image2015-7-9-10-3a55-3a2.png) | [!UICONTROL Cancel] | Tryck på knappen för att säga &quot;Strunta i det.&quot; |
| ![—](assets/image2015-7-9-10-3a56-3a2.png) | [!UICONTROL Save] | Tryck på knappen för att säga &quot;OK, I like it.&quot; |

>[!TIP]
>
>Du redigerar din HTML och text på olika skärmar. Klicka på **[!UICONTROL Copy from HTML]** på fliken **[!UICONTROL Text]** och sedan på **[!UICONTROL Save]** så att texten matchar din HTML.

>[!NOTE]
>
>Du är inte begränsad till teckensnitten i listrutan. Du kan använda en som inte finns med i listan genom att gå till HTML-koden. Alla webbteckensnitt stöds i Marketo, men webbteckensnitt fungerar inte överallt i alla e-postklienter.

## Landningssidor {#landing-pages}

Rotblockelementets inställning definierar vilka taggar som omsluter innehållet. Som standard använder rotblockselementet för landningssidan `<div>` taggar. Du kan ändra det genom att följa stegen nedan.

>[!TIP]
>
>Även om du kan välja ditt rotblockselement rekommenderar vi alltid att du använder standardinställningarna för att få en så bra användarupplevelse som möjligt.

1. Klicka på **[!UICONTROL Admin]**.

   ![](assets/one.png)

1. Klicka på **[!UICONTROL Email]**.

   ![](assets/two.png)

1. Klicka på **[!UICONTROL Edit Text Editor Settings]**.

   ![](assets/three.png)

1. I listrutan **[!UICONTROL Landing Page Editor]** väljer du `<p>` eller [!UICONTROL None] och klickar på **[!UICONTROL Save]**. `<p>` används i detta exempel.

   ![](assets/five.png)

   Och det är allt!
