---
unique-page-id: 7512524
description: Best Practices for Smart Lists - Marketo Docs - produktdokumentation
title: Bästa praxis för smarta listor
exl-id: 466de198-1012-4ac3-906c-d41943fe5bc0
source-git-commit: 72e1d29347bd5b77107da1e9c30169cb6490c432
workflow-type: tm+mt
source-wordcount: '521'
ht-degree: 0%

---

# Bästa praxis för smarta listor {#best-practices-for-smart-lists}

Smarta listor är det mest kraftfulla frågeverktyget i marknadsföringsuniversum. De hittar de personer du söker med magisk hastighet och enkelhet.

För att göra dem enkla att arbeta med och optimera prestanda har vi skapat en lista med bra metoder. Mycket nöje!

>[!NOTE]
>
>**Alla kunder är olika.** Ju större databas, desto mer bearbetning sker. Ju fler aktiviteter du har lagrat, desto längre tid tar det att söka igenom dem.
>
>Om du är långsam kan du prova med tipsen nedan. Om problemet kvarstår kontaktar du [Marketo Support](https://nation.marketo.com/t5/Support/ct-p/Support).

1. **Begränsa historik -** Historikfilter (alias Aktivitetsfilter) är bland de mest resurskrävande och tidskrävande åtgärderna. Om du måste använda dem kan du försöka begränsa datumintervallet till så kort som möjligt, vilket minskar den sökbara datauppsättningen.
1. **Begränsa kapslade smarta listor -** När du skapar en ny smart lista bör du begränsa mängden &quot;Medlem i smart lista&quot;-filter som används. Detta kallas att kapsla smarta listor och varje smart lista som refereras ökar bearbetningstiden. Referera i stället till statiska listor eller använd [segmentering](/help/marketo/product-docs/personalization/segmentation-and-snippets/segmentation/create-a-segmentation.md).
1. **Använd positiva över negativa operatorer** Även om&quot;inte&quot;-filter är tillgängliga måste de söka igenom hela datauppsättningen i din instans, vilket kan vara extremt tidskrävande. Positiva&quot;is&quot;-filter kan utnyttja effektivare sökalgoritmer.
1. **Undvik &quot;contains&quot; -** Om du bara har partiella data kommer &quot;börjar med&quot;-kvalificerare att ge mycket snabbare resultat än &quot;innehåller&quot;. &quot;Is&quot; går ännu snabbare. Undvik att använda&quot;contains&quot; med flera värden. kan de båda samtidigt göra en kampanj ännu långsammare.
1. **Använd slumpmässigt prov -** Random Sample är ett specialfilter. Använd den fristående för att placera ut dina medarbetare i färdiga listor. Använd sedan&quot;Member of List&quot; för att göra den smarta listan supersnabb. Slumpmässigt prov **NOT** arbeta med kapslade smarta listor. Filtret Slumpmässigt exempel fungerar inte om det är den smarta listan som refereras till för filtret&quot;Medlem i smart lista&quot;.
1. **Var livskraftig med inaktivitetsfilter -** Filter som&quot;Inte ifyllt formulär&quot; kan vara mycket användbara, men kräver mycket mer processorkraft.
1. **Var livfull med att klistra in i flera olika värden -** Flerval är utformat för att klistra in i dussintals eller eventuellt hundratals värden. Men om man lägger in för många så kommer det att sakta ner.
1. **Var livfull när du lägger till begränsningar -** Detta är de små detaljerna i en regel och relaterade värden. Ju fler begränsningar du lägger till, desto långsammare bearbetningstid.
1. **Förenkla era kampanjer -** Över 100 oberoende regler (vi har sett det!) kommer naturligtvis att ta lite tid att behandla. Gör det enkelt så märker du hastighetsökningarna - och det blir lättare för dig att förstå.
1. **Inkludera @-symbolen före domännamnet när du använder e-postadressfiltret** **-** Det gör att det krävs en snabbare fråga. Exempel: I stället för att använda _e-postmeddelandet innehåller &quot;somedomain.com&quot;_, använda _e-postmeddelandet innehåller @somedomain.com_.&#39; Om du använder flera e-postadresser med &quot;contains&quot; måste ALLA börja med &quot;@&quot;.

>[!TIP]
>
>Marketo kan användas på många sätt och vissa tekniker är bättre för dig och ditt företag. Överväg [Marketo professionella tjänster](https://pages2.marketo.com/72-hour-survival-guide.html) för att göra er investering ännu bättre.
