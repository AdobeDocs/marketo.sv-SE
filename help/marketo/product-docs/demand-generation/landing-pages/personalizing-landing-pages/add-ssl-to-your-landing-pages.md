---
unique-page-id: 2359828
description: Lägg till SSL på era landningssidor - Marketo Docs - produktdokumentation
title: Lägg till SSL på era landningssidor
exl-id: 8271d9fe-0575-430c-97c7-407e4b78cf1d
feature: Landing Pages
source-git-commit: de2f73f932fd38211dba96d8697ef4bb4fd0f0da
workflow-type: tm+mt
source-wordcount: '793'
ht-degree: 0%

---

# Lägg till SSL på era landningssidor {#add-ssl-to-your-landing-pages}

Med SSL-kryptering (Secure Socket Layer) kan du göra alla dina landningssidor för en Marketo Engage-instans säkra.

När du fyller i ett webbformulär eller besöker en landningssida som Marketo Engage är värd för, skickas informationen som standard via ett osäkert protokoll (HTTP). Enligt företagets policy kanske du vill skydda den information som skickas till Marketo via HTTPS. När du till exempel besöker `http://info.mydomain.com/` blir det nu `https://info.mydomain.com/`.

Marketo Engage spårar &quot;Besökt webbsida&quot; och &quot;Klicka på länk på webbsida&quot; som standard över osäkra HTTP-protokoll. Om du vill att dina spårningslänkar ska vara skyddade med deras egna certifikat måste du ha Marketo som en separat icke-delad server för att kunna aktivera den. För att skydda alla aspekter av en kontakts interaktion med dig måste du vanligtvis skydda både landningssidor och spårningslänkar.

>[!IMPORTANT]
>
>Innan du lägger till en SSL måste du kontrollera ditt avtal för det totala antalet domäner som du har behörighet att lägga till. Annars kan du ådra dig en avgift. Om du inte hittar informationen kan du kontakta Adobe Account Team (din kontoansvarige) för mer information.

## Aktivera SSL-certifiering {#enable-ssl-certification}

Lägg automatiskt till SSL för alla domänalias som du skapar som en del av reglerna för landningssidan.

1. Gå till området **Admin**.

   ![](assets/add-ssl-to-your-landing-pages-1.png)

1. Välj **Landningssidor** i trädet. Klicka på listrutan **Nytt** på fliken **Regler** och välj **Nytt domänalias**.

   ![](assets/add-ssl-to-your-landing-pages-2.png)

1. Ange ditt _domänalias_ och _standardsida_. Markera kryssrutan **Skapa SSL-certifikat**. Klicka på **Skapa** när du är klar.

   ![](assets/add-ssl-to-your-landing-pages-3.png)

Detta lägger automatiskt till ett SSL-certifikat för den här domänen.

## Aktivera SSL för din standarddomän {#enable-ssl-default-domain}

Följ stegen nedan för att aktivera SSL för din standarddomän.

1. I avsnittet **Admin** väljer du **Startsidor**. Klicka på den orangefärgade knappen **Redigera** bredvid _Inställningar_.

   ![](assets/add-ssl-to-your-landing-pages-4.png){width="800" zoomable="yes"}

   >[!NOTE]
   >
   >Om du vill kan du även ändra domännamnet här (en giltig domän krävs).

1. Markera kryssrutan Generera SSL-certifikat och klicka på Spara.

   ![](assets/add-ssl-to-your-landing-pages-5.png)

>[!NOTE]
>
>Det kan ta upp till tre minuter innan SSL är i tillståndet READY. Uppdatera sidan för att ändringarna ska visas.

## Redigera SSL:er till befintliga domänalias

Följ de här stegen för att aktivera SSL för dina befintliga domänalias.

1. Expandera _[!UICONTROL Admin]_&#x200B;i den vänstra navigeringen i området **[!UICONTROL Integration]**&#x200B;och välj **[!UICONTROL Landing Pages]**.

1. På sidan väljer du fliken **[!UICONTROL Rules]** överst.

1. Markera den domänaliasrad som du vill redigera och klicka på **[!UICONTROL Add SSL]** överst.

   ![Admin area - Integration > Landing Pages - Rules tab - select domain alias](./assets/admin-landing-pages-rules-add-ssl.png){width="800" zoomable="yes"}

1. Klicka på **[!UICONTROL Confirm]** i dialogrutan.

   ![Lägg till SSL - Bekräfta](./assets/generate-ssl-cert-confirm.png){width="400"}

>[!NOTE]
>
>Det kan ta upp till tre minuter innan SSL är i tillståndet READY. Uppdatera sidan för att ändringarna ska visas.

## Felmeddelanden {#error-messages}

Här nedan hittar du felmeddelanden som du kan få tillsammans med deras definitioner.

<table><thead>
  <tr>
    <th>Fel</th>
    <th>Information</th>
  </tr></thead>
<tbody>
<tr>
    <td><i>Domänen finns redan.</i></td>
    <td>Det finns redan en domän med samma namn.</td>
  </tr>
  <tr>
    <td><i>Domänen är inte mappad till standarddomänen.</i></td>
    <td>Den anpassade domänen är inte korrekt mappad till standarddomänen. Kontrollera inställningarna för domänmappning och se till att DNS-konfigurationen pekar på rätt standarddomän.</td>
  </tr>
  <tr>
    <td><i>Det gick inte att utfärda SSL-certifikat på grund av CAA-poster som inte stöds. Begär att din IT-avdelning uppdaterar dina CAA-poster.</i></td>
    <td>CAA-posterna är inte uppdaterade. För dem som använder Marketo Engage hanterade SSL-certifikat måste CAA-posterna uppdateras till certifikat som rekommenderas av vår leverantör. Kontakta din IT-avdelning för att uppdatera CAA-posterna. Mer information finns på <a href="https://nation.marketo.com/t5/product-blogs/changes-to-marketo-engage-secured-domains-platform/ba-p/329305#M2246">den här sidan</a>.</td>
  </tr>
  <tr>
    <td><i>SSL-certifikatet har redan utfärdats.</i></td>
    <td>Det finns redan ett SSL-certifikat för den här anpassade domänen. Ingen ytterligare åtgärd krävs såvida inte certifikatet har upphört att gälla eller behöver utfärdas på nytt.</td>
  </tr>
  <tr>
    <td><i>Det gick inte att hitta standarddomänen. Kontakta supporten om du behöver hjälp.</i></td>
    <td>Det uppstod ett problem när standarddomänen skulle hittas. Kontakta supporten så att de kan undersöka saken.</td>
  </tr>
  <tr>
    <td><i>Ett oväntat fel uppstod när en domän skapades. Kontakta supporten om du behöver hjälp.</i></td>
    <td>Ett oväntat fel har inträffat. Hämta loggar och felinformation och eskalera problemet till <a href="https://nation.marketo.com/t5/support/ct-p/Support" target="_blank">Marketo Support</a>.</td>
  </tr>
</tbody></table>

## Saker att notera {#things-to-note}

* **DNS-mappning för domän till Marketo Engage**: Innan du lägger till domäner i användargränssnittet måste du [mappa CNAME:er till en domän som tillhandahålls av Marketo](https://experienceleague.adobe.com/sv/docs/marketo/using/getting-started/initial-setup/setup-steps#customize-your-landing-page-urls-with-a-cname){target="_blank"}.

* **Anpassade SSL:er**: Om du behöver en anpassad SSL:er skickar du en [supportanmälan](https://nation.marketo.com/t5/support/ct-p/Support){target="_blank"}. Använd inte kryssrutan för självbetjäning när du skapar SSL.

* **Befintliga SSL:er**: När du lägger till en domän söker systemet efter befintliga SSL:er, som kan ha skapats manuellt tidigare. Om du råkar ut för den här valideringen skapar du din domän utan att välja SSL-skapande, så ansluter vi dem åt dig. [Kontakta support](https://nation.marketo.com/t5/support/ct-p/Support){target="_blank"} om du vill ha mer information/alternativ.

* **Borttagning av domäner**: SSL-certifikatet tas inte bort när domänen **tas bort automatiskt.** Skyddsplanen förhindrar användarfel som gör att en webbplats saknar SSL-certifikat. [Kontakta support](https://nation.marketo.com/t5/support/ct-p/Support){target="_blank"} om du vill ta bort SSL-certifikaten.
