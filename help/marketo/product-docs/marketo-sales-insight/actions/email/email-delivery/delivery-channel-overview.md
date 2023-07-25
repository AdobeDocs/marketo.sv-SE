---
description: Översikt över leveranskanalen - Marketo Docs - produktdokumentation
title: Översikt över leveranskanalen
exl-id: 8dd6fe3e-86ae-4361-bc0a-6488dc1df9fa
feature: Sales Insight Actions
source-git-commit: 431bd258f9a68bbb9df7acf043085578d3d91b1f
workflow-type: tm+mt
source-wordcount: '668'
ht-degree: 0%

---

# Översikt över leveranskanalen {#delivery-channel-overview}

Marketo direktförsäljning ger er flera alternativ för att leverera e-postmeddelanden. I den här artikeln beskrivs de leveranskanaler du kan utnyttja, hur du väljer ut dem och när du ska välja ut en av dem.

## Rekommenderas: Gmail eller Exchange via e-postanslutning {#recommended-gmail-or-exchange-via-email-connection}

Marketo direktförsäljning ger smidig installation och förbättrad leverans via vår e-posttjänst. Med e-postanslutningen kan alla användare ansluta till sina [Gmail](/help/marketo/product-docs/marketo-sales-connect/email-plugins/gmail/email-connection-for-gmail-users.md) eller [Exchange](/help/marketo/product-docs/marketo-sales-connect/email-plugins/msc-for-outlook/email-connection-for-outlook-users.md) konto hos Marketo direktförsäljning som ska användas som leveranskanal för alla Marketo direktförsäljning.

Att använda Gmail eller Exchange ger vissa tydliga fördelar jämfört med andra alternativ för leveranskanaler:

* Detta är en beprövad leveranskanal med välrenommerat rykte som hjälper till att hålla leveranssäkerheten hög.
* Autentiseringsmetoder som SPF och DKIM har redan konfigurerats och hanteras av IT-teamet, så det finns ingen ytterligare konfiguration.
* Att skicka e-postmeddelanden inom ett givet e-postnätverk (dvs. att skicka ett e-postmeddelande som en Exchange-användare till ett företag som tar emot e-post via Exchange) kan öka leveransmöjligheterna ytterligare.

Det är viktigt att notera att dessa leveranskanaler har sina egna sändningsgränser som upprätthålls av Microsoft och Google. För att bekämpa detta använder vi en begränsningsmekanism som hjälper användarna att hålla sig inom dessa gränser. Läs mer om [e-postbegränsning här](/help/marketo/product-docs/marketo-sales-connect/email/email-delivery/email-connection-throttling.md).

>[!NOTE]
>
>Som standard kommer O365-pluginen alltid att använda din Exchange-leveranskanal och Gmail-pluginen kommer alltid att använda din Gmail-leveranskanal för att leverera e-postmeddelanden från plugin-programmen.

**Studsspårning**: Marketo Sales kan identifiera studsningar för Exchange Online- eller Gmail-användare genom att identifiera studsmeddelandet som skickas till avsändarens inkorg. Dessa studsmeddelanden kommer att samlas i mallanalyser, kampanjanalyser och Live Feed-meddelanden för användarna. Studsspårning stöds inte för Exchange On-Prem-kunder.

## Anpassad leveranskanal via SMTP {#custom-delivery-channel-via-smtp}

Marketo Sales erbjuder ett ytterligare alternativ för att ansluta en SMTP-server från en annan leverantör som kan användas som leveranskanal för ditt säljteam.

Att använda en SMTP-leverantör från en annan leverantör är ett bra alternativ för säljteam där e-postvolymen är den främsta prioriteten. SMTP-leverantörer som Sendgrid och Sparkpost är optimerade för att tillgodose behoven hos massutskick av e-post och kan skalas för att uppfylla behoven hos dem som vill distribuera stora mängder e-post.

Dessutom erbjuder tredjepartsleverantörer av SMTP en mängd funktioner som hjälper ditt team att leverera (till exempel e-postrapporter och dedikerade IP-adresser), vilket gör detta till ett bra alternativ för dem som vill ha mer detaljerade kontroller och synlighet kring sin e-postkanal för försäljning.

## Marketo Sales Servers (Legacy) {#marketo-sales-servers-legacy}

Marketo försäljningsservrar är bara tillgängliga för vissa äldre ToutApp-kunder. Dessa kunder kommer att se Marketo försäljningsservrar tillgängliga i sina e-postinställningar. Alla icke-äldre kunder ser inte Marketo Sales som ett alternativ och bör ansluta sitt Gmail- eller Outlook-konto till Marketo Sales för att låsa upp en leveranskanal.

Marketo försäljningsservrar stöder inte DKIM- och SPF-autentiseringsmetoder, vilket kan sänka leveransgraden. Därför rekommenderar vi att alla kunder ansluter till Gmail eller Outlook för bästa slutprodukt.

## MSC-servrar (äldre) {#msc-servers-legacy}

MSC-servrar är bara tillgängliga för vissa äldre ToutApp-kunder. Dessa kunder kommer att se vilka MSC-servrar som är tillgängliga i deras e-postinställningar. Alla icke-äldre kunder ser inte MSC som ett alternativ och bör ansluta sitt Gmail- eller Outlook-konto till Sales Connect för att låsa upp en leveranskanal.

MSC-servrar saknar stöd för DKIM- och SPF-autentiseringsmetoder, vilket kan sänka leveransgraden. Därför rekommenderar vi att alla kunder ansluter till Gmail eller Outlook för bästa slutprodukt.

## Marketo-servrar {#marketo-servers}

Marketo e-postservrar kan inte integreras med Marketo direktförsäljning. Marketo-servrar är optimerade för massleverans så att de kan anpassas efter marknadsförarnas behov. Gmail och Exchange har dock högre framgångar för säljkommunikation med 1:1, vilket är anledningen till att vi rekommenderar att du använder dessa servrar för din säljkommunikation.

>[!MORELIKETHIS]
>
>* [E-postanslutning för Gmail-användare](/help/marketo/product-docs/marketo-sales-connect/email-plugins/gmail/email-connection-for-gmail-users.md)
>* [E-postanslutning för Outlook-användare](/help/marketo/product-docs/marketo-sales-connect/email-plugins/msc-for-outlook/email-connection-for-outlook-users.md)
>* [Konfigurera en anpassad leveranskanal](/help/marketo/product-docs/marketo-sales-connect/email/email-delivery/setting-up-a-custom-delivery-channel.md)
>* [Begränsning för e-postanslutning](/help/marketo/product-docs/marketo-sales-connect/email/email-delivery/email-connection-throttling.md)
