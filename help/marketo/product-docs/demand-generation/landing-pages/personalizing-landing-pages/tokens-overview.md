---
unique-page-id: 2950799
description: Översikt över token - Marketo Docs - produktdokumentation
title: Översikt över token
exl-id: d60816ce-33fb-4e18-8acd-71d4e90f47de
source-git-commit: 4fc3cf6e6458f07df7cced9399831b8c6b50e0ad
workflow-type: tm+mt
source-wordcount: '300'
ht-degree: 0%

---

# Översikt över token {#tokens-overview}

En variabel är en variabel som kan användas i Marketo smarta kampanjflödessteg, e-post, landningssidor, kodfragment och webbkampanjer.

## Förstå standardvärden {#understanding-default-values}

När du använder en variabel vill du även ange ett standardvärde. Det här är texten som visas om en person inte har ett värde för fältet som du refererar till.

![](assets/image2014-12-2-13-3a16-3a48.png)

I det här exemplet kommer e-postmeddelandet att stå &quot;Greetings, (förnamn)&quot; eller &quot;Greetings, dagling&quot; (standardvärde).

![](assets/two.png)

>[!CAUTION]
>
>Token fungerar inte i förrubriken när Marketo e-postredigerare används. Om du vill använda en token i förrubriken måste den vara via din egen HTML i en e-postmall.

>[!NOTE]
>
>Denna lista är inte uttömmande. Token skapas också för alla anpassade fält som du har i Marketo.

## Persontoken {#person-tokens}

* `{{lead.Acquisition Date}}`
* `{{lead.Acquisition Program Name}}`
* `{{lead.Acquisition Program}}`
* `{{lead.Address}}`
* `{{lead.Anonymous IP}}`
* `{{lead.Black Listed}}`
* `{{lead.City}}`
* `{{lead.Country}}`
* `{{lead.Created At}}`
* `{{lead.Date of Birth}}`
* `{{lead.Department}}`
* `{{lead.Do Not Call}}`
* `{{lead.Do Not Call Reason}}`
* `{{lead.Email Address}}`
* `{{lead.Email Invalid}}`
* `{{lead.Email Invalid Cause}}`
* `{{lead.Fax Number}}`
* `{{lead.First Name}}`
* `{{lead.Full Name}}`
* `{{lead.Id}}`
* `{{lead.Inferred City}}`
* `{{lead.Inferred Company}}`
* `{{lead.Inferred Country}}`
* `{{lead.Inferred Metropolitan Area}}`
* `{{lead.Inferred Phone Area Code}}`
* `{{lead.Inferred Postal Code}}`
* `{{lead.Inferred State Region}}`
* `{{lead.Is Customer}}`
* `{{lead.Is Employee}}`
* `{{lead.Is Partner}}`
* `{{lead.Job Title}}`
* `{{lead.Last Name}}`
* `{{lead.Lead Source}}`
* `{{lead.Marketing Suspended}}`
* `{{lead.Middle Name}}`
* `{{lead.Mobile Phone Number}}`
* `{{lead.Original Referrer}}`
* `{{lead.Original Search Engine}}`
* `{{lead.Original Search Phrase}}`
* `{{lead.Original Source Info}}`
* `{{lead.Original Source Type}}`
* `{{lead.Person Notes}}`
* `{{lead.Phone Number}}`
* `{{lead.Registration Source Info}}`
* `{{lead.Registration Source Type}}`
* `{{lead.Salutation}}`
* `{{lead.SFDC Created Date}}`
* `{{lead.SFDC Is Deleted}}`
* `{{lead.SFDC Type}}`
* `{{lead.Unsubscribed}}`
* `{{lead.Unsubscribed Reason}}`
* `{{lead.Updated At}}`
* Anpassade personfält fungerar också om du använder deras visningsnamn, till exempel `{{lead.Custom Field Name}}`

## Företagstoken {#company-tokens}

* `{{Company.Account Owner Email Address}}`
* `{{Company.Address}}`
* `{{Company.Annual Revenue}}`
* `{{Company.City}}`
* `{{Company.Company Name}}`
* `{{Company.Company Notes}}`
* `{{Company.Country}}`
* `{{Company.Industry}}`
* `{{Company.Main Phone}}`
* `{{Company.Num Employees}}`
* `{{Company.Parent Company Name}}`
* `{{Company.Postal Code}}`
* `{{Company.SFDC Account Num}}`
* `{{Company.SFDC Created Date}}`
* `{{Company.SFDC Type}}`
* `{{Company.SIC Code}}`
* `{{Company.Site}}`
* `{{Company.State}}`
* `{{Company.Website}}`
* Anpassade företagsfält fungerar också om du använder deras visningsnamn ex. `{{Company.Custom Field Name}}`

## Kampanjtoken {#campaign-tokens}

* `{{campaign.name}}`
* `{{campaign.id}}`
* `{{campaign.description}}`

## Systemtoken {#system-tokens}

>[!NOTE]
>
>Läs mer om dessa variabler i [Ordlista för systemtoken](/help/marketo/product-docs/email-marketing/general/using-tokens/system-tokens-glossary.md).

* `{{system.date}}`
* `{{system.time}}`
* `{{system.dateTime}}`
* `{{system.forwardToFriendLink}}`
* `{{system.unsubscribeLink}}`
* `{{system.viewAsWebpageLink}}`

## Utlösartoken {#trigger-tokens}

* `{{trigger.Trigger Name}}`
* `{{trigger.Name}}`
* `{{trigger.Link}}`
* `{{trigger.Subject}}`
* `{{trigger.Category}}`
* `{{trigger.Details}}`
* `{{trigger.Web Page}}`
* `{{trigger.Client IP Address}}`
* `{{trigger.Sent By}}`
* `{{trigger.Received By}}`
* `{{trigger.Referrer}}`
* `{{trigger.Search Engine}}`
* `{{trigger.Search Query}}`

>[!NOTE]
>
>Läs mer om [variabler för intressanta ögonblick](/help/marketo/product-docs/marketo-sales-insight/msi-for-salesforce/features/tabs-in-the-msi-panel/interesting-moments/trigger-tokens-for-interesting-moments.md) baserat på utlösare som används i en smart kampanj.

## Programtoken {#program-tokens}

* `{{program.Name}}`
* `{{program.Description}}`
* `{{program.id}}`

## Mina token {#my-tokens}

Mina token definieras i ett program och börjar med `{{my.` följt av namnet som du skapade för token. Läs mer om [Mina token i ett program](/help/marketo/product-docs/core-marketo-concepts/programs/tokens/understanding-my-tokens-in-a-program.md).

## Medlemstoken {#member-token}

Medlemstoken används för att infoga unika värden från integrerade tjänstpartner. Ett vanligt användningsområde för Member Tokens är för unika URL:er för webbinarier-deltagare. Varje person har en unik URL för att komma åt webbinariet som kan infogas med en `{{member.webinar url}}` token. The `{{member.webinar url}}` -token löser automatiskt personens unika bekräftelse-URL som genereras av tjänsteleverantören.

* `{{member.webinar url}}`

>[!CAUTION]
>
>The `{{member.webinar url}}` -token fylls bara i om den smarta kampanj som skickar e-postmeddelandet är en underordnad resurs till Event Program.
