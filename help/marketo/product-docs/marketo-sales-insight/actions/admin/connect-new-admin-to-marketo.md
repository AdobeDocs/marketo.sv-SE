---
description: Anslut ny administratör till Marketo - Marketo Docs - produktdokumentation
title: Anslut ny administratör till Marketo
exl-id: ef405bca-a29a-40fc-9efa-eccff5f45956
feature: Sales Insight Actions
source-git-commit: 431bd258f9a68bbb9df7acf043085578d3d91b1f
workflow-type: tm+mt
source-wordcount: '495'
ht-degree: 0%

---

# Anslut ny administratör till Marketo {#connect-new-admin-to-marketo}

Om den andra administratören redan är ansluten till Marketo behöver de bara göra steg 1.

Om den andra administratören inte är ansluten till Marketo som administratör...

1. Den primära administratören måste koppla från den andra administratören från Marketo via Inställningar > Marketo > Användaråtkomst.

1. Den sekundära administratören loggar in på sitt MSC-konto, går till Inställningar > Marketo och klickar på **Anslut**.

1. Nu är den sekundära användaren ansluten till Marketo som administratör.

1. Den primära administratören kan nu logga in och koppla från sig själv från Marketo.

>[!NOTE]
>
>De andra användarna är anslutna så länge som användare B är ansluten som administratör innan användare A kopplas från.

## Uppdatera din Marketo-anslutning {#update-your-marketo-connection}

Om du bestämmer dig för att du vill ta bort den administratör som konfigurerade Marketo-integreringen läser du den här artikeln för att lära dig hur.

Integreringen av Marketo är knuten till en användare som är Sales Connect/Actions Admin. Det här är vanligtvis den administratör som först klickade på knappen &quot;Anslut&quot; på Marketo anslutningssida och upprättade anslutningen.

Om du vill ta bort den administratör som upprättade Marketo-anslutningen måste en ny anslutning först upprättas av en annan Admin-användare. Vi har listat de uppgifter nedan som måste utföras för att detta ska kunna göras.

För att förenkla instruktionerna ska vi hänvisa till den administratör som är ansluten just nu som Admin A och den administratör som du vill upprätta en ny anslutning till Marketo med som Admin B:

1. Admin A (för närvarande ansluten administratör) måste ta bort åtkomsten till integreringen med Marketo från Admin B (ny administratör).

1. Låt admin B (ny administratör) upprätta en ny anslutning till Marketo.

1. Koppla från administratör A (ursprungligen ansluten administratör).

>[!NOTE]
>
>Den ursprungliga administratören som ansvarar för Marketo-integreringen kommer att se ett&quot;Koppla från&quot;-alternativ som du kan klicka på när du navigerar till Marketo integreringssida. Andra administratörer (som inte har upprättat en anslutning) kommer inte att göra det. Dessutom kan inte administratörer som har beviljats åtkomst till Marketo-integreringen klicka på Anslut. Därför måste du följa stegen för att först ta bort åtkomsten till integreringen.

**Ta bort Marketo Access från Admin B**

Admin A (den administratör som ursprungligen var ansvarig för anslutningen) ska följa dessa steg.

1. Klicka på kugghjulsikonen i webbprogrammet och välj **Inställningar**.

1. Klicka på **Marketo**.

1. Klicka på **Användaråtkomst**.

1. Sök efter den administratör som du vill skapa den nya Marketo-anslutningen för.

1. Ta bort åtkomst.

**Skapa ny anslutning för administratör B**

Dessa steg ska följas av admin B (ny administratör)

1. Klicka på kugghjulsikonen i webbprogrammet och välj **Inställningar**.

1. Klicka på **Marketo**.

1. Klicka på **Koppla från**.

**Koppla från Marketo-integrering för admin A**

Dessa steg ska följas av admin A (ursprungligen ansluten admin).

1. Klicka på kugghjulsikonen i webbprogrammet och välj **Inställningar**.

1. Klicka på **Marketo**.

1. Klicka på **Koppla från**.

Nu när en ny administratör har upprättat en anslutning till Marketo och den ursprungliga administratören har kopplats från kan den ursprungligen anslutna administratören tas bort från Sales Connect/Actions-instansen.
