---
title: Sådan tilføjes eller fjernes en stedfortræder i Outlook for Windows
ms.author: v-jmathew
author: v-jmathew
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3800004"
- "7334"
ms.openlocfilehash: 8db800d5c23b4cc2057f94abaf357082914143d3
ms.sourcegitcommit: ab75f66355116e995b3cb5505465b31989339e28
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 08/13/2021
ms.locfileid: "58329019"
---
# <a name="how-to-add-or-remove-a-delegate-in-outlook-for-windows"></a>Sådan tilføjes eller fjernes en stedfortræder i Outlook for Windows

Sådan føjer du en stedfortræder Outlook for Windows: 

1. Klik på fanen **Filer** efterfulgt af Firma **Indstillinger**, og vælg derefter **Stedfortræderadgang**.
2. Klik på **Tilføj.** Hvis **Tilføj** ikke vises, findes der muligvis ikke en aktiv forbindelse mellem Outlook og Exchange. Statuslinjen Outlook statuslinjen viser forbindelsesstatussen.
3. Skriv navnet på den person, du vil udpege som stedfortræder, eller søg og vælg navnet på listen over søgeresultater.

    **Bemærk!** Stedfortræderen skal være en person i din organisations Exchange globale adresseliste (GAL).
4. Klik på **Tilføj** efterfulgt af **OK.**
5. I dialogboksen **Stedfortrædertilladelser skal** du acceptere standardtilladelsesindstillingerne eller vælge brugerdefinerede adgangsniveauer for Exchange mapper.

    - Hvis en stedfortræder har brug for tilladelse til kun at arbejde med mødeindkaldelser og svar, er indstillingerne for standardtilladelser som f.eks. Stedfortræderen modtager kopier af møderelaterede meddelelser, **der** er sendt til mig, tilstrækkelige. Du kan lade **tilladelsesindstillingen** Indbakke være på **Ingen**. Mødeindkaldelser og svar går direkte til stedfortræderens indbakke.

    **Bemærk!** Som standard får stedfortræderen **Redaktør (kan læse, oprette og redigere elementer)-tilladelse** til **mappen** Kalender. Når stedfortræderen svarer på et møde på dine vegne, føjes det automatisk til **mappen** Kalender.

5. Hvis du vil sende en meddelelse til stedfortræderen om de ændrede tilladelser, skal du markere afkrydsningsfeltet Send automatisk en meddelelse til stedfortrædere med en kortfatning **af** disse tilladelser.
6. Hvis du vil, kan du markere **afkrydsningsfeltet Stedfortræderen kan se mine private** elementer.

    **Vigtigt!** Denne indstilling påvirker alle Exchange mapper. Dette omfatter alle mapperne Mail, Kontakter, Kalender, Opgaver, Noter og Journal. Det er ikke muligt at give adgang til private elementer i kun angivne mapper.

7. Vælg **OK.**

    **Bemærk!**
    - Meddelelser, der sendes med Send på vegne af-tilladelser, omfatter både stedfortræderens og dit navn ud for **Fra**. Når en meddelelse sendes med Send som-tilladelser, er det kun dit navn, der vises.
    - Når du tilføjer en person som stedfortræder, kan de føje din Exchange postkasse til deres Outlook profil. Du kan finde en vejledning [i Administrere en anden persons mail og kalender.](https://support.microsoft.com/office/manage-another-person-s-mail-and-calendar-items-afb79d6b-2967-43b9-a944-a6b953190af5)

Sådan fjerner du en stedfortræder Outlook for Windows:

1. Klik på **fanen** Filer.
2. Klik på **Konto Indstillinger** efterfulgt af **Stedfortræderadgang**.
3. Vælg navnet på den stedfortræder, du vil ændre tilladelser for, og klik derefter på **Fjern** efterfulgt af **OK.**
