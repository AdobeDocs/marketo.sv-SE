---
description: Sekretessförfrågningar - Marketo Docs - produktdokumentation
title: Sekretessförfrågningar
exl-id: ae61eabc-ad8f-4c7b-8097-838e89c1a3ec
source-git-commit: 5aa75cc35ef8d39983563ab34b075ae580f9a97b
workflow-type: tm+mt
source-wordcount: '0'
ht-degree: 0%

---

# Sekretessförfrågningar {#privacy-requests}

I det här dokumentet finns en översikt över hur du hanterar enskilda dataskyddsförfrågningar som du kan skicka till Marketo Engage via Privacy Servicens gränssnitt och Privacy Servicens API.

>[!NOTE]
>
>Begäran om sekretess som skickas via Privacy Servicens gränssnitt eller API för Marketo Engage gäller endast för följande:
>
>* Marketo Engage som har anslutit sig till Adobe Identity Management System
>
>**-or-**
>
>* Marketo Engage-användare som använder en annan Experience Cloud-produkt som redan finns i Adobe Identity Management System (t.ex. RT-CDP, B2B och B2P Editions, Audience Manager).


Du kan skicka enskilda förfrågningar om åtkomst till och radering av konsumentdata från Marketo Engage på två sätt:

* Via [Privacy Servicens användargränssnitt](https://privacyui.cloud.adobe.io/). Läs dokumentationen [här](https://experienceleague.adobe.com/docs/experience-platform/privacy/ui/user-guide.html){target=&quot;_blank&quot;}.
* Via Privacy Services-API:t. Läs dokumentationen [här](https://developer.adobe.com/experience-platform-apis/references/privacy-service/){target=&quot;_blank&quot;} och API-information [här](https://developer.adobe.com/experience-platform-apis/){target=&quot;_blank&quot;}.

The [Privacy Service](https://experienceleague.adobe.com/docs/experience-platform/privacy/home.html){target=&quot;_blank&quot;} stöder två typer av begäranden: dataåtkomst och borttagning av data.

Låt oss se hur du kan skapa förfrågningar om åtkomst och borttagning.

## Nödvändig konfiguration för att skicka begäranden för Marketo Engage {#required-setup-to-send-requests-for-marketo-engage}

Om du vill göra en begäran om åtkomst- och borttagningsdata för Marketo Engage måste du:

1. Identifiera följande:

   a. IMS-organisations-ID<br/>
b. E-postadress till den person du vill agera på

   Ett IMS-organisations-ID är en 24 tecken lång alfanumerisk sträng som läggs till med @AdobeOrg. Om ditt marknadsföringsteam eller den interna systemadministratören i Adobe inte känner till din organisations IMS-organisation kan du kontakta Adobe kundtjänst på gdprsupport@adobe.com. Du behöver IMS-organisations-ID för att kunna skicka begäranden till sekretess-API:t.

1. I Privacy Service kan du skicka in begäranden om åtkomst och borttagning till Marketo Engage och kontrollera status för befintliga begäranden.

## Obligatoriska fältvärden i JSON-begäranden i Marketo Engage {#required-field-values-in-marketo-engage-json-requests}

&quot;companyContext&quot;:

* &quot;namespace&quot;: **imsOrgID**
* &quot;value&quot;: `<Your IMS Org ID Value>`

&quot;användare&quot;:

* &quot;action&quot;: antingen **åtkomst** eller **delete**
* &quot;användar-ID&quot;:
   * &quot;namespace&quot;: **e-post**
   * &quot;type&quot;: **standard**
   * &quot;value&quot;: `<Data Subject’s Email Address>`

&quot;include&quot;:

* **marketo** (som är den Adobe-produkt som är tillämplig på ansökan)

reglering:

* **gdpr**, **ccpa**, **pdpa**, **lgpd_bra**, eller **nzpa_nzl**  (som är den sekretessregel som gäller för begäran)

## Exempel ett: Borttagningsbegäran för GDPR {#gdpr-delete-request}

JSON-begäran

```text
{
  "companyContexts": [
    {
      "namespace": "imsOrgID",
      "value": "1231659F56A68A8B7F000101@AdobeOrg"
    }
  ],
  "users": [
    {
      "action": [
        "delete"
      ],
      "userIDs": [
        {
          "namespace": "email",
          "type": "standard",
          "value": "john.doe@adobe.com"
        }
      ]
    }
  ],
  "include": [
    "marketo"
  ],
  "regulation": "gdpr",
}
```

JSON-svar

```text
{
  "requestId": "16331241037112570RX-245",
  "totalRecords": 1,
  "jobs": [
    {
      "jobId": "997b01e3-9568-402c-904b-b4e60a437875",
      "customer": {
        "user": {
          "action": [
            "delete"
          ],
          "userIDs": [
            {
              "namespace": "email",
              "value": "john.doe@adobe.com",
              "type": "standard",
              "namespaceId": 6,
              "isDeletedClientSide": false
            }
          ]
        }
      }
    }
  ]
}
```

## Exempel två: CCPA-åtkomstbegäran {#ccpa-access-request}

JSON-begäran

```text
{
  "companyContexts": [
    {
      "namespace": "imsOrgID",
      "value": "1231659F56A68A8B7F000101@AdobeOrg"
    }
  ],
  "users": [
    {
      "action": [
        "access"
      ],
      "userIDs": [
        {
          "namespace": "email",
          "type": "standard",
          "value": "john.doe@adobe.com"
        }
      ]
    }
  ],
  "include": [
    "marketo"
  ],
  "regulation": "ccpa",
}
```

JSON-svar

```text
{
  "requestId": "16329573462631890RX-207",
  "totalRecords": 1,
  "jobs": [
    {
      "jobId": "3115e42d-011b-47ab-a2b0-ed4356af4d3e",
      "customer": {
        "user": {
          "action": [
            "access"
          ],
          "userIDs": [
            {
              "namespace": "email",
              "value": "john.doe@adobe.com",
              "type": "standard",
              "namespaceId": 6,
              "isDeletedClientSide": false
            }
          ]
        }
      }
    }
  ]
}
```

>[!MORELIKETHIS]
>
>[Integritetshantering](/help/marketo/product-docs/core-marketo-concepts/miscellaneous/privacy-management.md)
