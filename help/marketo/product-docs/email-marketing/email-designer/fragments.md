---
title: Fragment
description: Lär dig hur du skapar och använder visuella innehållsfragment som återanvändbara komponenter för e-post och e-postmallar.
hide: true
hidefromtoc: true
exl-id: abc065a0-cd2f-4f0f-a5f2-228b833b99a8
source-git-commit: aefdb7360ca4c687d05f4695afc618815b08c336
workflow-type: tm+mt
source-wordcount: '2311'
ht-degree: 0%

---

# Fragment

Ett fragment är en återanvändbar komponent som kan refereras i ett eller flera e-postmallar och e-postmallar. Det är vanligtvis ett innehållsblock (text, bild eller båda) som kan skapas och snabbt infogas i projektet. Med den här funktionen kan du skapa flera anpassade innehållsblock i förväg för att sammanställa e-postinnehåll för en förbättrad designprocess. Vanliga användningsområden är t.ex. innehållsblock för sidhuvud/sidfot för e-post, banners för inbjudningar till evenemang, säsongsmeddelanden med mera.

Så här använder du fragment på bästa sätt i dina arbetsflöden:

* _Skapa fragment_ - Skapa visuella fragment, antingen från grunden eller genom att spara innehåll som ett fragment från den visuella innehållsredigeraren.
* _Återanvänd fragment_ - Använd dem så många gånger som behövs i ditt innehåll.

## Visuella fragment {#visual-fragments}

Visuella fragment är fördefinierade visuella block som byggts (med den visuella innehållsredigeraren) och som du kan återanvända i flera e-postmallar eller e-postmallar.

## Få åtkomst till och hantera fragment {#access-and-manage-fragments}

Gå till Design Studio om du vill få tillgång till visuella fragment. Klicka på **[!UICONTROL Fragments (New)]** i trädet till vänster.

![Åtkomst till fragment](assets/fragments-1.png){width="600" zoomable="yes"}

Som standard sorteras tabellen efter kolumnen _[!UICONTROL Modified]_. Klicka på andra kolumnrubriker om du vill ändra vad tabellen sorteras efter. Klicka igen om du vill växla mellan stigande och fallande.

### Fragmentstatus {#fragment-status}

Fragmentstatusen avgör om den är tillgänglig för användning i en e-post- eller e-postmall och vilka ändringar du kan göra i den.

<table>
<tbody>
  <tr>
    <td><b>Utkast</b></td>
    <td>När du skapar ett fragment är det i utkaststatus. Det förblir ett utkast tills du publicerar det för användning i en e-postmall eller e-postmall.
    <p>Tillgängliga åtgärder:
    <li>Redigera all information</li>
    <li>Redigera i visuell designer</li>
    <li>Publish</li>
    <li>Duplicera</li>
    <li>Ta bort</li>
  </td>
  <tr>
    <td><b>Publicerad</b></td>
    <td>När du publicerar ett fragment blir det tillgängligt för användning i en e-postmall eller e-postmall. Publicerat fragmentinnehåll kan inte ändras i den visuella designern.
    <p>Tillgängliga åtgärder:
    <li>Redigera beskrivning</li>
    <li>Lägg till i ett e-postmeddelande eller en mall</li>
    <li>Skapa utkastversion</li>
    <li>Duplicera</li>
    <li>Radera (om den inte används)</li>
    </td>
  </tr>
  <tr>
    <td><b>Publicerat med utkast</b></td>
    <td>När du skapar ett utkast från ett publicerat fragment förblir den publicerade versionen tillgänglig för användning i en e-postmall eller e-postmall, och utkastinnehållet kan ändras i den visuella designern. Om du publicerar utkastet till version ersätter det den aktuella publicerade versionen och innehållet uppdateras i <i>alla</i> e-postmallarna och e-postmallarna som det används i. 
    <p>Tillgängliga åtgärder:
    <li>Redigera beskrivning</li>
    <li>Lägg till i ett e-postmeddelande eller en mall</li>
    <li>Redigera utkast i visuell designer</li>
    <li>Publish draft version</li>
    <li>Duplicera</li>
    <li>Radera (om den inte används)</li>
    </td>
  </tr>
</tbody></table>

### Filtrera fragmentlistan {#filter-the-fragments-list}

Använd sökfältet för att hitta ett fragment efter namn. Klicka på ikonen _Filter_ ( ![Visa eller dölj filterikon](assets/icon-filter.svg) ) för att visa tillgängliga filteralternativ och välja önskade inställningar.

![Filtrera de visade fragmenten](assets/fragments-list-filtered.png){width="700" zoomable="yes"}

### Anpassa kolumnvisningen {#customize-the-column-display}

Anpassa de kolumner som du vill visa i tabellen genom att klicka på ikonen _Anpassa tabell_ ( ![Anpassa tabell-ikon](assets/icon-column-settings.svg) ) längst upp till höger.

Markera de kolumner du vill använda i dialogrutan och klicka på **[!UICONTROL Apply]**.

SCREENSHOT

## Skapa fragment {#create-fragments}

Skapa ett nytt visuellt fragment genom att klicka på **[!UICONTROL Create fragment]** överst till höger.

1. I dialogrutan _[!UICONTROL Create fragment]_anger du ett **[!UICONTROL Name]**och ett valfritt **[!UICONTROL Description]**.

   Fragmentkrav:

   * Namn - högst 100 tecken, måste vara unikt, skiftlägeskänsligt
   * Beskrivning - max 300 tecken
   * Alpha, numeriska tecken och specialtecken är ok
   * Reserverade tecken är **_inte tillåtna_**: `\ / : * ? " < > |`

SCREENSHOT

1. Klicka på **[!UICONTROL Create]**.

   Den visuella designern öppnas med en tom arbetsyta.

1. Använd verktygen för innehållsdesign för att skapa det visuella fragmentinnehållet:

   * [Lägga till struktur och innehåll](#add-structure-and-content)
   * [Lägg till Assets](#add-assets)
   * [Navigera mellan lager, inställningar och format](#navigate-the-layers-settings-and-styles)
   * [Anpassa innehåll](#personalize-content)
   * [Redigera länkad URL-spårning](#edit-linked-url-tracking)

1. Klicka på **[!UICONTROL Save]** när du vill spara utkastet.

1. När du är redo att göra fragmentet tillgängligt för användning i en e-post- eller e-postmall klickar du på **[!UICONTROL Publish]**.

### Lägga till struktur och innehåll {#add-structure-and-content}

{{$include /help/marketo/_includes/content-design-components.md}}

### Lägga till resurser

{{$include /help/_includes/content-design-assets.md}}

### Navigera mellan lager, inställningar och format

{{$include /help/_includes/content-design-navigation.md}}

### Anpassa innehåll

{{$include /help/_includes/content-design-personalization.md}}

### Redigera länkad URL-spårning

{{$include /help/_includes/content-design-links.md}}

## Visa fragmentinformation {#view-fragment-details}

Klicka på namnet på ett fragment på listsidan för att öppna fragmentinformationssidan. Du kan välja att redigera fragmentet, byta namn på fragmentet eller uppdatera fragmentbeskrivningen. Gör uppdateringar och klicka utanför namn- eller beskrivningsfältet för att spara ändringarna automatiskt.

>[!NOTE]
>
>Om ett publicerat fragment används av en e-post- eller e-postmall kan du inte ändra dess namn eller redigera innehållet. Du kan skapa ett utkast om du vill göra ändringar i fragmentet.

![Visa information om ett publicerat fragment](assets/fragment-details-published.png){width="600" zoomable="yes"}

Klicka på **[!UICONTROL Edit fragment]** för att öppna fragmentet i den visuella innehållsredigeraren.

Avsluta vyn när som helst genom att klicka på pilen _Bakåt_ längst upp till vänster, som återgår till listsidan _Fragment_ .

## Visa fragment som används av referenser {#view-fragment-used-by-references}

Klicka på fliken **[!UICONTROL Used By]** på sidan med fragmentinformation för att visa information om var fragmentet används i Marketo Engage.

>[!IMPORTANT]
>
>Ett fragment som används av en e-post- eller e-postmall kan inte tas bort.

Referenser visas enligt kategori: _E-post_ eller _E-postmall_. E-postmeddelanden i Journey Optimizer B2B edition är inbäddade och redigerade inom kontoresor, så den överordnade resan för det e-postmeddelande som använder fragmentet visas i referenser. &lt;— VAD GÄLLER DETTA, NILESH

![Används av referenser för fragmentet](assets/fragment-used-by-published.png){width="600" zoomable="yes"}

Klicka på länken för att öppna motsvarande e-post- eller e-postmall där fragmentet används.

## Ta bort fragment {#delete-fragments}

Eftersom ett fragment som för närvarande används av en e-post- eller e-postmall inte kan tas bort bör du kontrollera _som används av_-referenserna innan du påbörjar en fragmentborttagning. En borttagning kan inte ångras, så kontrollera innan du startar en borttagningsåtgärd.

Du kan ta bort ett fragment på något av följande sätt:

* Klicka på **[!UICONTROL Delete]** från fragmentinformationen till höger.
* Klicka på ellipsen bredvid fragmentet på listsidan _[!UICONTROL Fragments]_och välj **[!UICONTROL Delete]**.

Åtgärden öppnar en bekräftelsedialogruta. Du kan avbryta processen genom att klicka på **[!UICONTROL Cancel]** eller klicka på **[!UICONTROL Delete]** för att bekräfta borttagningen.

![Dialogrutan Ta bort fragment](assets/fragment-delete-dialog.png){width="400"}

## Redigera fragment {#edit-fragments}

Ändringar i ett fragment beror på dess aktuella status:

* När ett fragment har statusen _Utkast_ kan du redigera alla dess detaljer och det visuella innehållet.
* När ett fragment har statusen _Publicerad_ kan du redigera fragmentbeskrivningen, men inte namnet. Du kan inte redigera det visuella innehållet.
* När ett fragment har statusen _Publicerat med utkast_ begränsas redigeringen till beskrivningen. Du kan också redigera det visuella innehållet för utkastversionen.

>[!BEGINTABS]

>[!TAB Utkast]

1. Klicka på fragmentnamnet på listsidan _[!UICONTROL Fragments]_för att öppna det.

   En förhandsgranskning av det visuella innehållet visas, med fragmentinformationen till höger.

1. Gör önskade redigeringar.

   ![Information om rament med utkaststatus](assets/fragment-draft-details.png){width="600" zoomable="yes"}

1. Om du vill ändra innehållet i den visuella designern klickar du på **[!UICONTROL Edit fragment]**.

   Använd de visuella designverktygen efter behov:

   * [Lägga till struktur och innehåll](#add-structure-and-content)
   * [Lägg till Assets](#add-assets)
   * [Navigera mellan lager, inställningar och format](#navigate-the-layers-settings-and-styles)
   * [Anpassa innehåll](#personalize-content)
   * [Redigera länkad URL-spårning](#edit-linked-url-tracking)

   Klicka på **[!UICONTROL Save]** eller **[!UICONTROL Save & close]** för att återgå till fragmentinformationen.

1. När fragmentet uppfyller dina villkor och du vill göra det tillgängligt för användning i en e-postmall eller e-postmall klickar du på **[!UICONTROL Publish]**.

>[!TAB Publicerad]

1. Klicka på fragmentnamnet på listsidan _[!UICONTROL Fragments]_för att öppna det.

   En förhandsgranskning av det visuella innehållet visas, med fragmentinformationen till höger.

1. Ändra beskrivningen om det behövs.

   För ett publicerat fragment går det inte att ändra all annan information.

1. Om du vill uppdatera innehållet klickar du på **[!UICONTROL Create draft version]** längst upp till höger.

   Klicka på **[!UICONTROL OK]** i dialogrutan för att öppna utkastet i den visuella designern. Du kan ändra `image source` KG - LÄNK HÄR om det behövs.

   ![Skapa dialogruta för utkastversion](assets/fragments-create-draft-version.png){width="300"}

   Använd de visuella designverktygen efter behov:

   * [Lägga till struktur och innehåll](#add-structure-and-content)
   * [Lägg till Assets](#add-assets)
   * [Navigera mellan lager, inställningar och format](#navigate-the-layers-settings-and-styles)
   * [Anpassa innehåll](#personalize-content)
   * [Redigera länkad URL-spårning](#edit-linked-url-tracking)

   Klicka på **[!UICONTROL Save]** eller **[!UICONTROL Save & close]** för att återgå till fragmentinformationen.

1. När utkastet uppfyller dina villkor och du vill göra ändringarna tillgängliga för användning i en e-postmall eller e-postmall klickar du på **[!UICONTROL Publish]**.

   När du publicerar utkastet ersätts den aktuella publicerade versionen och innehållet uppdateras i e-postmallarna och i e-postmallarna där det redan används.

>[!TAB Publicerat med utkast]

Det finns två sätt att öppna utkastet för redigering från listsidan _[!UICONTROL Fragments]_:

* Klicka på ikonen _Mer_ (**..**) bredvid fragmentnamnet och välj **[!UICONTROL Open draft version]**.

  ![Öppna utkastversion](assets/fragments-create-draft-version.png){width="300"}

* Klicka på fragmentnamnet för att öppna det. Klicka sedan på **[!UICONTROL Open draft version]** överst till höger.

  En förhandsgranskning av det visuella innehållet för utkastversionen visas, med fragmentinformationen till höger.

Så här uppdaterar du innehållet:

1. Klicka på **[!UICONTROL Edit fragment]** överst till höger. Använd de visuella designverktygen efter behov:

   * [Lägga till struktur och innehåll](#add-structure-and-content)
   * [Lägg till Assets](#add-assets)
   * [Navigera mellan lager, inställningar och format](#navigate-the-layers-settings-and-styles)
   * [Anpassa innehåll](#personalize-content)
   * [Redigera länkad URL-spårning](#edit-linked-url-tracking)

   Klicka på **[!UICONTROL Save]** eller **[!UICONTROL Save & close]** för att återgå till fragmentinformationen.

1. När utkastet uppfyller dina villkor och du vill göra ändringarna tillgängliga för användning i en e-postmall eller e-postmall klickar du på **[!UICONTROL Publish]**.

   När du publicerar utkastet ersätts den aktuella publicerade versionen och innehållet uppdateras i e-postmallarna och i e-postmallarna där det redan används.

>[!ENDTABS]

## Duplicera fragment {#duplicate-fragments}

Du kan duplicera ett fragment på något av följande sätt:

* Klicka på ikonen _Mer_ (**..**) bredvid fragmentnamnet på listsidan _[!UICONTROL Fragments]_och välj **[!UICONTROL Duplicate]**.
* Klicka på **[!UICONTROL ... More]** längst upp till höger på sidan med fragmentinformation och välj **[!UICONTROL Duplicate]**.

![Duplicera fragmentet](assets/fragment-details-duplicate.png){width="600" zoomable="yes"}

Ange ett unikt namn och en valfri beskrivning i dialogrutan. Klicka på **[!UICONTROL Duplicate]** för att slutföra åtgärden.

![Ange ett namn och en beskrivning för det duplicerade fragmentet](assets/fragment-duplicate-dialog.png){width="400"}

Det duplicerade fragmentet visas sedan i listan _Fragment_.

## Spara ett nytt fragment från e-post eller mallinnehåll {#save-a-new-fragment-from-email-or-template-content}

När du skapar/redigerar en e-post- eller e-postmall i den visuella innehållredigeraren kan du välja att spara hela eller delar av innehållet som ett fragment så att det är tillgängligt för återanvändning.

1. Om du vill spara innehåll som ett fragment klickar du på **[!UICONTROL More]** och väljer **[!UICONTROL Save as Fragment]**.

1. Markera de olika element som ska inkluderas i fragmentet.

   Markera flera strukturer genom att hålla ned Skift eller Ctrl.

   Du kan bara markera strukturer som ligger intill varandra och gränssnittet tillåter inte att du markerar element som inte ligger intill varandra.

1. Markera innehållet och klicka på **[!UICONTROL Create]** överst till höger.

1. Ange ett namn och en valfri beskrivning för fragmentet i dialogrutan. Klicka sedan på **[!UICONTROL Create]**.

   Fragmentet visas sedan på listsidan _Fragment_ och kan även användas i e-postmeddelanden och e-postmallar.

## Lägga till visuella fragment i e-post- eller mallinnehåll {#add-visual-fragments-to-your-email-or-template-content}

Fragment är utformade för återanvändning och du kan lägga till upp till 30 i en e-postmall eller e-postmall. Fragment kan bara kapslas upp till en nivå.

>[!BEGINTABS]

>[!TAB Lägg till fragment i ett e-postmeddelande]

1. Navigera till **[!UICONTROL Account Journeys]** och öppna en befintlig resa eller skapa en ny. &lt;— ENDAST OM DE FINNS I E-POST- ELLER E-POSTMALLEN

—STOPPAD REDIGERING HÄR—

1. Skapa en [_[!UICONTROL Send Email]_-nod ](./email-authoring.md#add-an-email-action-in-an-account-journey).

1. Skapa eller redigera [e-postinnehåll för noden](./email-authoring.md#create-the-email-content).

1. Dra och släpp ett objekt från menyn **[!UICONTROL Components]** för att ange en _struktur_ för fragmentet.

1. Klicka på ikonen _Fragment_ om du vill öppna en lista med publicerade fragment.

   Du kan:
   * Sortera listan.
   * Bläddra, sök och filtrera listan.
   * Växla mellan kort (miniatyrbild) och listvyer.
   * Uppdatera listan så att den återspeglar något av de nyligen skapade fragmenten.

SCREENSHOT

1. Dra och släpp något av fragmenten till platshållaren för strukturkomponenten.

   Redigeraren återger fragmentet i avsnittet/elementet i e-poststrukturen.

Fragmentets innehåll uppdateras dynamiskt i strukturen för att återge hur innehållet visas i e-postmeddelandet.

>[!TIP]
>
>Om du vill att fragmentet ska uppta hela den vågräta layouten i e-postmeddelandet lägger du till en [!UICONTROL 1:1 column]-struktur och drar och släpper fragmentet i den.

När e-postmeddelandet har sparats visas det på fragmentinformationssidan när fliken _[!UICONTROL Used By]_har valts. Fragment som läggs till i ett e-postmeddelande kan inte redigeras i e-postmeddelandet eller mallen - det publicerade källfragmentet definierar innehållet.

>[!TAB Lägg till fragment i en e-postmall]

1. Klicka på **[!UICONTROL Content Management]** > **[!UICONTROL Templates]** i den vänstra navigeringen.

1. Skapa en ny mall eller öppna en befintlig e-postmall och klicka på **[!UICONTROL Edit Email Template]**.

1. Dra och släpp ett objekt från menyn **[!UICONTROL Components]** för att ange en _struktur_ för fragmentet.

1. Om du vill öppna fragmentlistan klickar du på ikonen _Fragment_ .

   Du kan:
   * Sortera listan.
   * Bläddra, sök och filtrera listan.
   * Växla mellan kort (miniatyrbild) och listvyer.
   * Uppdatera listan så att den återspeglar något av de nyligen skapade fragmenten.

SCREENSHOT

1. Dra och släpp något av fragmenten till platshållaren för strukturkomponenten.

   Redigeraren återger fragmentet i avsnittet/elementet i e-postmallstrukturen.

1. Dra och släpp något av fragmenten till platshållaren för strukturkomponenten.

   Redigeraren återger fragmentet i avsnittet/elementet i e-postmallstrukturen.

>[!TIP]
>
>Om du vill att fragmentet ska uppta hela den vågräta layouten i e-postmallen lägger du till en _[!UICONTROL 1:1 column]_-struktur och drar och släpper fragmentet i den.

När e-postmallen har sparats visas den på fragmentinformationssidan när fliken _[!UICONTROL Used By]_har valts. Fragment som läggs till i en e-postmall kan inte redigeras i mallen - det publicerade källfragmentet definierar innehållet.

>[!ENDTABS]

## Fragmentåtgärder vid e-post- och mallutveckling

När ett fragment läggs till i en e-post- eller e-postmall kan fragmentinnehållet inte redigeras i e-postmeddelandet eller mallen. Du kan dock använda följande åtgärder:

* **[!UICONTROL Delete]** - Den här åtgärden tar bort fragmentet från det aktuella e-postmallinnehållet eller e-postmallinnehållet (fragmentkällan påverkas inte).
* **[!UICONTROL Refresh]** - Den här åtgärden uppdaterar innehållet i fragmentet i den aktuella e-post- eller e-postmallen. Det är praktiskt att uppdatera när du vill spegla de senaste ändringarna i fragmentet efter att ha lagt till e-post- eller e-postmallen.
* **[!UICONTROL Duplicate]** - Den här åtgärden duplicerar fragmentet inom samma e-post- eller e-postmall i redigeraren, med samma dimensioner och lägger till precis nedanför det.
* **[!UICONTROL Open Fragment]** - Den här åtgärden öppnar en ny webbläsarflik med fragmentredigeringssidan och information.
* **[!UICONTROL Break inheritance]** - Den här åtgärden bryter arvet av fragmentet (och dess ändringar) från källan. Använd den här åtgärden om du vill göra fragmentinnehållet tillgängligt som oberoende och redigerbart innehåll i e-post- eller e-postmallen. Den här åtgärden tar också bort e-post- eller e-postmallen från referensen _Används av_ för det ursprungliga fragmentet.

När du markerar fragmentet på redigeringssidan är de här åtgärderna tillgängliga från kontextverktygsfältet och egenskapspanelen till höger.

![Tillämpa åtgärder på det markerade fragmentet](assets/fragment-actions-email-authoring.png){width="600" zoomable="yes"}
