---
title: Sådan tilføjer eller fjerner du en stedfortræder i Outlook til Windows
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
ms.openlocfilehash: fcbd6082c104f0e1bca022a23cbbeb6e3363a6c5
ms.sourcegitcommit: c069f1b53567ad14711c423740f120439a312a60
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 12/04/2020
ms.locfileid: "49573339"
---
# <a name="how-to-add-or-remove-a-delegate-in-outlook-for-windows"></a>Sådan tilføjer eller fjerner du en stedfortræder i Outlook til Windows

Sådan tilføjer du en stedfortræder i Outlook til Windows: 

1. Klik på fanen **filer** efterfulgt af **kontoindstillinger**, og vælg derefter **stedfortræderadgang**.
2. Klik på **Tilføj**. Hvis **Tilføj** ikke vises, findes der muligvis ikke en aktiv forbindelse mellem Outlook og Exchange. Statuslinjen i Outlook viser Forbindelsesstatus.
3. Skriv navnet på den person, du vil angive som stedfortræder, eller Søg, og vælg navnet på listen over søgeresultater.

    > [!NOTE]
    > Stedfortræderen skal være en person på din organisations globale Exchange-adresseliste (GAL).
4. Klik på **Tilføj** efterfulgt af **OK**.
5. I dialogboksen **stedfortrædertilladelser** skal du acceptere standardindstillingerne for tilladelser eller vælge brugerdefinerede adgangsniveauer for Exchange-mapper.

    - Hvis en stedfortræder skal have tilladelse til kun at fungere med mødeindkaldelser og svar, er standardindstillingerne for tilladelse som **stedfortræder modtager kopier af møderelaterede meddelelser, der er sendt til mig** , der er tilstrækkelige. Du kan lade **indbakkens** tilladelsesindstilling være **none**. Mødeindkaldelser og svar sendes direkte til stedfortræderens indbakke.

    > [!NOTE]
    > Som standard er stedfortræderen tildelt **redaktør (kan læse, oprette og ændre elementer)** til din **kalender** mappe. Når stedfortræderen svarer på et møde på dine vegne, føjes det automatisk til din **kalender** mappe.

5. Hvis du vil sende en meddelelse for at underrette stedfortræderen om de ændrede tilladelser, skal du markere afkrydsningsfeltet **Send automatisk en meddelelse til stedfortrædere med en sammenfatning af disse tilladelser** .
6. Hvis du vil, kan du markere afkrydsningsfeltet **stedfortræderen kan se mine private elementer** .

    > [!IMPORTANT]
    > Denne indstilling påvirker alle Exchange-mapper. Dette omfatter alle mail-, kontakt-, kalender-, opgaver, noter og Journal-mapper. Det er ikke muligt at give adgang til private elementer i bestemte mapper.

7. Vælg **OK**.

    > [!NOTE]
    >
    > - Meddelelser, der sendes med tilladelsen Send på vegne af, omfatter både stedfortræderens og dine navne ud for **fra**. Når en meddelelse sendes med Send som-tilladelser, vises kun dit navn.
    > - Når du har tilføjet en person som stedfortræder, kan vedkommende tilføje din Exchange-postkasse til sin Outlook-profil. Hvis du vil have mere at vide, skal du se [administrere en anden persons mail og kalender](https://support.microsoft.com/office/manage-another-person-s-mail-and-calendar-items-afb79d6b-2967-43b9-a944-a6b953190af5).

Sådan fjerner du en stedfortræder i Outlook til Windows:

1. Klik på fanen **filer** .
2. Klik på **kontoindstillinger** efterfulgt af **stedfortræderadgang**.
3. Vælg navnet på den stedfortræder, du vil ændre tilladelser for, og klik derefter på **Fjern** efterfulgt af **OK**.
