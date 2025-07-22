---
unique-page-id: 14352407
description: Översikt över leveranskanalen - Marketo Docs - produktdokumentation
title: Översikt över leveranskanalen
exl-id: 432bad1e-4eaf-4be8-b856-be364c44816e
feature: Marketo Sales Connect
source-git-commit: 0d37fbdb7d08901458c1744dc68893e155176327
workflow-type: tm+mt
source-wordcount: '552'
ht-degree: 0%

---

# Översikt över leveranskanalen {#delivery-channel-overview}

Marketo [!DNL Sales Connect] ger dig flera alternativ för att leverera e-postmeddelanden. I den här artikeln beskrivs de leveranskanaler du kan utnyttja, hur du väljer ut dem och när du ska välja ut en av dem.

## Rekommenderas: Gmail eller [!DNL Exchange] via e-postanslutning {#recommended-gmail-or-exchange-via-email-connection}

[!DNL Sales Connect] möjliggör en smidig konfiguration och förbättrad leverans via vår e-postanslutningstjänst. Med [!UICONTROL Email Connection] kan varje användare ansluta till sitt [Gmail](/help/marketo/product-docs/marketo-sales-connect/email-plugins/gmail/email-connection-for-gmail-users.md)- eller [Exchange](/help/marketo/product-docs/marketo-sales-connect/email-plugins/msc-for-outlook/email-connection-for-outlook-users.md)-konto till [!DNL Sales Connect] och använda det som leveranskanal för alla [!DNL Sales Connect]-e-postmeddelanden.

Att använda Gmail eller [!DNL Exchange] ger vissa tydliga fördelar jämfört med andra alternativ för leveranskanaler:

* Detta är en beprövad leveranskanal med välrenommerat rykte som hjälper till att hålla leveranssäkerheten hög.
* Autentiseringsmetoder som SPF och DKIM har redan konfigurerats och hanteras av IT-teamet, så det finns ingen ytterligare konfiguration.
* Att skicka e-postmeddelanden inom ett givet e-postnätverk (dvs. att skicka ett e-postmeddelande som en [!DNL Exchange]-användare till ett företag som tar emot e-post via [!DNL Exchange]) kan öka leveransmöjligheterna ytterligare.

Det är viktigt att notera att dessa leveranskanaler har sina egna sändningsgränser som upprätthålls av Microsoft och Google. För att bekämpa detta använder vi en begränsningsmekanism som hjälper användarna att hålla sig inom dessa gränser. Läs mer om [begränsning av e-post här](/help/marketo/product-docs/marketo-sales-connect/email/email-delivery/email-connection-throttling.md).

>[!NOTE]
>
>Som standard kommer O365-pluginen alltid att använda din Exchange-leveranskanal och Gmail-pluginen kommer alltid att använda din Gmail-leveranskanal för att leverera e-postmeddelanden från plugin-programmen.

**Studsspårning**: MSC kan identifiera studsar för [!DNL Exchange Online] - eller Gmail-användare genom att identifiera studsmeddelandet som skickas till avsändarens inkorg. Dessa studsmeddelanden kommer att samlas i mallanalyser, kampanjanalyser och Live Feed-meddelanden för användarna. Studsspårning stöds inte för [!DNL Exchange] On-Prem-kunder.

## Anpassad leveranskanal via SMTP {#custom-delivery-channel-via-smtp}

[!DNL Sales Connect] erbjuder ytterligare ett alternativ för att ansluta en SMTP-server från tredje part som ska användas som leveranskanal för ditt säljteam.

Att använda en SMTP-leverantör från en annan leverantör är ett bra alternativ för säljteam där e-postvolymen är den främsta prioriteten. SMTP-providers som [!DNL Sendgrid] och [!DNL Sparkpost] är optimerade för att hantera behoven av massutskick av e-post och kan skalas för att uppfylla behoven hos dem som vill distribuera stora mängder e-post.

Dessutom erbjuder tredjepartsleverantörer av SMTP en mängd funktioner som hjälper ditt team att leverera (till exempel e-postrapporter och dedikerade IP-adresser), vilket gör detta till ett bra alternativ för dem som vill ha mer detaljerade kontroller och synlighet kring sin e-postkanal för försäljning.

## MSC-servrar (äldre) {#msc-servers-legacy}

MSC-servrar är bara tillgängliga för vissa äldre ToutApp-kunder. Dessa kunder kommer att se vilka MSC-servrar som är tillgängliga i deras e-postinställningar. Alla icke-äldre kunder ser inte MSC som ett alternativ och bör ansluta sitt Gmail- eller [!DNL Outlook]-konto till [!DNL Sales Connect] för att låsa upp en leveranskanal.

MSC-servrar saknar stöd för autentiseringsmetoderna DKIM och SPF, vilket kan sänka leveransgraden. På grund av detta rekommenderar vi att alla kunder ansluter till Gmail eller [!DNL Outlook] för att få bästa möjliga leverans.

## Marketo-servrar {#marketo-servers}

Marketo e-postservrar kan inte integreras med [!DNL Sales Connect]. Marketo-servrar är optimerade för massleverans så att de kan anpassas efter marknadsförarnas behov. Gmail och [!DNL Exchange] har dock högre framgångsgrad för 1:1-säljkommunikation, vilket är anledningen till att vi rekommenderar att du använder de här servrarna för din säljkommunikation.

>[!MORELIKETHIS]
>
>* [E-postanslutning för Gmail-användare](/help/marketo/product-docs/marketo-sales-connect/email-plugins/gmail/email-connection-for-gmail-users.md)
>* [E-postanslutning för [!DNL Outlook] användare](/help/marketo/product-docs/marketo-sales-connect/email-plugins/msc-for-outlook/email-connection-for-outlook-users.md)
>* [Konfigurera en anpassad leveranskanal](/help/marketo/product-docs/marketo-sales-connect/email/email-delivery/setting-up-a-custom-delivery-channel.md)
>* [Begränsning för e-postanslutning](/help/marketo/product-docs/marketo-sales-connect/email/email-delivery/email-connection-throttling.md)
