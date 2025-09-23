---
description: Hantering av användare och licenser - Marketo Docs - produktdokumentation
title: Hantering av användare och licenser
exl-id: 1fee628b-e9f3-46ab-b993-f2d09fe5e183
feature: Interactive Webinars
source-git-commit: 09a656c3a0d0002edfa1a61b987bff4c1dff33cf
workflow-type: tm+mt
source-wordcount: '717'
ht-degree: 0%

---

# Hantering av användare och licenser {#user-and-license-management}

Lär dig hur du lägger till och tar bort användare och visar dina aktuella licenser.

## Lägg till en användare {#add-a-user}

1. Gå till området **Admin**.

   ![](assets/user-and-license-management-1.png)

1. Klicka på **Interaktiva webbinarier**.

   ![](assets/user-and-license-management-2.png)

1. Klicka på **Lägg till/ta bort användare**.

   ![](assets/user-and-license-management-3.png)

1. Klicka på listrutan Tillgängliga användare, markera de användare som du vill lägga till och klicka på **OK**.

   ![](assets/user-and-license-management-4.png)

## Ta bort en användare {#remove-a-user}

1. Gå till området **Admin**.

   ![](assets/user-and-license-management-5.png)

1. Klicka på **Interaktiva webbinarier**.

   ![](assets/user-and-license-management-6.png)

1. Klicka på **Lägg till/ta bort användare**.

   ![](assets/user-and-license-management-7.png)

1. Markera de användare som du vill ta bort och tryck på Delete-tangenten på tangentbordet. Klicka på **OK** när du är klar.

   ![](assets/user-and-license-management-8.png)

## Licensanvändning {#license-usage}

Interactive Webinars erbjuder specifika licenser för att skapa event som drivs av Adobe Connect. Varje gång en licens läggs till visas en ny ruta för licensanvändning. Marketo-administratörer kan visa (inte redigera) licenserna genom att följa stegen nedan. Kontakta Adobe Account Team (er Account Manager) för att få ytterligare licenser.

1. Gå till området **Admin**.

   ![](assets/user-and-license-management-9.png)

1. Klicka på **Interaktiva webbinarier**.

   ![](assets/user-and-license-management-10.png)

1. Bläddra ned till License Usage-kortet/korten.

   ![](assets/user-and-license-management-11.png)

<table>
  <tr>
   <td width="20%"><b>Startdatum</b></td>
   <td width="80%">Datum då licensen börjar.</td>
  </tr>
  <tr>
   <td width="20%"><b>Förfallodatum</b></td>
   <td width="80%">Datum när licensen upphör att gälla.</td>
  </tr>
  <tr>
   <td width="20%"><b>Typ</b></td>
   <td width="80%">Den typ av licens som köpts. Det finns tre typer: licens för delade händelser, licens för delade rum, ytterligare lagringslicens.</td>
  </tr>
  <tr>
   <td width="20%"><b>Händelsekapacitet</b></td>
   <td width="80%">Det högsta antalet deltagare som kan inrymmas i en händelse.</td>
  </tr>
  <tr>
   <td width="20%"><b>Totalt antal händelser</b></td>
   <td width="80%">Det totala antalet händelser som har etablerats med den här licensen.</td>
  </tr>
  <tr>
   <td width="20%"><b>Förbrukade händelser</b></td>
   <td width="80%">Alla slutförda och schemalagda händelser. <a href="#things-to-note">läs mer</a></td>
  </tr>
  <tr>
   <td width="20%"><b>Lagringskapacitet</b></td>
   <td width="80%">Mängd tillgängligt lagringsutrymme för lagring av inspelningar, kollateraler, hjältebilder, dokumentation och andra resurser.</td>
  </tr>
  </tbody>
</table>

### Saker att notera {#things-to-note}

* Varje gång en händelse skapas räknas den som&quot;förbrukad&quot; från respektive licens (om det inte är en delad rumslicens). &quot;Shared Event License&quot; ges om det finns både &quot;Shared Event License&quot; och &quot;Shared Room License&quot; med samma kapacitet. Om händelsen inte har levererats och händelseprogrammet tas bort före den schemalagda tiden fylls antalet händelser på igen. Om händelsen inte levereras och Event Program inte tas bort före den schemalagda tidpunkten fylls händelsen inte på igen.

* Typen&quot;Additional Storage License&quot; ger bara lagringsutrymme, därför kommer värdet i alla fält _förutom_ som lagringskapacitet att listas som &quot;-&quot;.

* Typen &quot;Shared Room License&quot; har obegränsat antal händelser och &quot;Additional Storage License&quot; (Tilläggslicens för lagring) erbjuder bara lagring, så fältet Total Events för dessa licenser listas helt enkelt som &quot;-&quot;.

* När en licens har tömts finns dess panel kvar på skärmen Interaktiva webbinarier i administratörsavsnittet där&quot;Totalt antal händelser&quot; och&quot;Använda händelser&quot; har samma värde. Först när licensen upphör att gälla tas den bort från skärmen.

## Användaråtkomst {#user-access}

Interaktiva webbinarier kan reglera användningen genom att ge Marketo Engage-användare tillstånd att skapa och leverera interaktiva webbinarier. En Interactive Webinar-användare (eller icke-användare) kan dock fortfarande ha läs-/redigeringsåtkomst till händelseprogram för interaktiva webbinarier som skapats av andra användare.

Marketo-användare som har fått tillstånd att använda interaktiva webbinarier och som är ägare till ett visst händelseprogram för interaktiva webbinarier kan utföra alla interaktiva webbinarifunktioner som är relaterade till det programmet. Detta inkluderar: skapa, komma åt, ändra, klona, flytta och ta bort programmet. Men när användaren inte längre är en interaktiv webbinäranvändare, kan ägaren av programmet komma åt och flytta programmet, men inte utföra några andra funktioner.

Marketo-användare som har fått tillstånd att använda interaktiva webbinarier och som _inte_ äger ett visst händelseprogram för interaktiva webbinarier kan utföra begränsade funktioner i dessa program. Marketo icke-admin-användare kan komma åt och klona programmet, men kan inte utföra några andra funktioner om de har behörighet för Interactive Webinars. Marketo Admin-användare _kan dock_ utföra alla funktioner, som att komma åt, ändra, klona, flytta och ta bort det programmet (förutsatt att de har behörighet för Interactive Webinars). När behörigheten har återkallats för användare av Marketo Admin och andra användare, kan de bara komma åt händelseprogrammet för interaktiva webbinarier och kan inte utföra några andra funktioner.

Begränsningen av de funktioner som kan användas anges med en nedtonad åtgärdsknapp och ett hovringsmeddelande. Några exempel på de nedtonade åtgärdsknapparna är&quot;Design Your Webinar&quot; eller&quot;Enter Your Webinar&quot;. För icke-åtgärdbara funktioner visas ett meddelande som markerar begränsningarna. Se exemplet nedan:

![](assets/user-and-license-management-12.png)
