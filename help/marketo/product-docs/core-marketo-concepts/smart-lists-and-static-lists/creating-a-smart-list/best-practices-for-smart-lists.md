---
unique-page-id: 7512524
description: Best Practices for Smart Lists - Marketo Docs - produktdokumentation
title: Bästa praxis för smarta listor
translation-type: tm+mt
source-git-commit: 47b2fee7d146c3dc558d4bbb10070683f4cdfd3d
workflow-type: tm+mt
source-wordcount: '517'
ht-degree: 0%

---


# Bästa praxis för smarta listor {#best-practices-for-smart-lists}

Smarta listor är det mest kraftfulla frågeverktyget i marknadsföringsuniversum. De hittar de personer du söker med magisk hastighet och enkelhet.

För att göra dem enkla att arbeta med och optimera prestanda har vi skapat en lista med bra metoder. Mycket nöje!

>[!NOTE]
>
>**Alla kunder är olika.** Ju större databas, desto mer bearbetning sker. Ju fler aktiviteter du har lagrat, desto längre tid tar det att söka igenom dem.
>
>Om du är långsam kan du prova med tipsen nedan. Kontakta Marketo [Support](http://support.marketo.com) om problemet kvarstår.

1. **Begränsa historik - **Historikfilter (alias) Aktivitetsfilter) är bland de mest resurskrävande och tidskrävande åtgärderna. Om du måste använda dem kan du försöka begränsa datumintervallet till så kort som möjligt, vilket minskar den sökbara datauppsättningen.
1. **Begränsa kapslade smarta listor - **När du skapar en ny smart lista bör du begränsa hur många filter för &quot;Medlem i smart lista&quot; som används. Detta kallas att kapsla smarta listor och varje smart lista som refereras ökar bearbetningstiden. Referera i stället till statiska listor eller använd [segmentering](../../../../product-docs/personalization/segmentation-and-snippets/segmentation/create-a-segmentation.md).
1. **Använd positiva operatorer framför negativa operatorer - **Även om det finns&quot;inte&quot;-filter måste de söka igenom hela datauppsättningen i instansen, vilket kan vara extremt tidskrävande. Positiva&quot;is&quot;-filter kan utnyttja effektivare sökalgoritmer.
1. **Undvik &quot;contains&quot; -** Om du bara har ofullständiga data kommer &quot;starting with&quot;-kvalificerare att ge mycket snabbare resultat än &quot;contains&quot;. &quot;Is&quot; går ännu snabbare. Undvik att använda&quot;contains&quot; med flera värden. kan de båda samtidigt göra en kampanj ännu långsammare.
1. **Använd slumpmässigt prov - **Slumpmässigt prov är ett specialfilter. Använd den fristående för att placera ut dina medarbetare i färdiga listor. Använd sedan&quot;Member of List&quot; för att göra den smarta listan supersnabb. Slumpmässigt exempel kommer **INTE** att fungera med kapslade smarta listor. Filtret Slumpmässigt exempel fungerar inte om det är den smarta listan som refereras till för filtret&quot;Medlem i smart lista&quot;.
1. **Var livfull med inaktivitetsfilter - **Filter som &quot;Inte ifyllt formulär&quot; kan vara mycket användbara, men kräver mycket mer processorkraft.
1. **Du kan arbeta med att klistra in i flera olika värden - **Flerval är utformat för att klistra in i dussintals eller eventuellt hundratals värden. Men om man lägger in för många så kommer det att sakta ner.
1. **Var kraftfull när du lägger till begränsningar - **Detta är de små detaljerna i en regel och relaterade värden. Ju fler begränsningar du lägger till, desto långsammare bearbetningstid.
1. **Förenkla era kampanjer - **100+ oberoende regler (vi har sett det!) kommer naturligtvis att ta lite tid att behandla. Gör det enkelt så märker du hastighetsökningarna - och det blir lättare för dig att förstå.
1. **Inkludera @-symbolen före domännamnet när du använder e-postadressfiltret** **-** Detta gör att en snabbare fråga används. Exempel: I stället för att använda *e-post innehåller &quot;somedomain.com*&quot; använder du *e-postadressen innehåller &#39;@somedomain.com*&#39;. Om du använder flera e-postadresser med &quot;contains&quot; måste ALLA börja med &quot;@&quot;.

>[!TIP]
>
>Marketo kan användas på många sätt och vissa tekniker är bättre för dig och ditt företag. Överväg att [Marknadsföringstjänster](http://pages2.marketo.com/72-hour-survival-guide.html) för att få din investering att se bra ut.

