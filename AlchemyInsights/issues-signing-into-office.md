---
title: Problemer, der logger på Office apps
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000571"
- "2574"
ms.openlocfilehash: 3622a3408b25b43090e9414ae5ffcfc2760264ee
ms.sourcegitcommit: 699ac3b0d66e0640f8e933eba3c2a4ba1cfcf3c7
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 07/30/2019
ms.locfileid: "35938174"
---
# <a name="issues-signing-in-to-office-apps"></a>Problemer, der logger på Office apps

For at løse problemer-logon med Office apps, kan du prøve følgende:

- Fjerne alle konti i arbejde, bortset fra den berørte konto ved hjælp af Windows-indstillinger > **Access arbejdet eller i skolen**.
- [Fjern Office legitimationsoplysninger](https://docs.microsoft.com/office/troubleshoot/error-messages/another-account-already-signed-in#step-3-clear-cached-credentials-on-the-computer) ved hjælp af styring af legitimationsoplysninger i Windows.<br/>
    **Bemærk:** Stier i registreringsdatabasen for Office 2016 er ændret til 16,0. (Ex: \Software\Microsoft\Office\16.0\Common\Identity\)
- Åbn et Office-program, skal du vælge **filen** > **konto** > **Log af**. Log på ved hjælp af en brugerkonto med en gyldig licens. Du kan finde detaljerede oplysninger [konti i Office](https://support.office.com/article/accounts-in-office-628ea040-f265-49de-b986-be09c3ebf8a9).
- Du [kan ikke logge på en Office-2016 for Mac app](https://docs.microsoft.com/office365/troubleshoot/authentication/sign-in-to-office-2016-for-mac-fail)til Mac.
- Hvis der opstår fejl under oprettelse af forbindelse til Office 365 ved hjælp af Office-2013, skal du aktivere moderne godkendelse for Office-klienten.

Du kan finde flere oplysninger under:
- [Du kan ikke logge på Office 365, Azure eller Intune](https://docs.microsoft.com/office365/troubleshoot/authentication/sign-in-to-office-365-azure-intune)
- [Forbindelsesproblemer i logon efter opdatering til Office 2016 bygge 16.0.7967 på Windows-10](https://docs.microsoft.com/office365/troubleshoot/administration/connection-issue-when-sign-in-office-2016)
- ["Undskyld, en anden konto fra organisationen allerede er logget på på denne computer" i Office](https://docs.microsoft.com/office/troubleshoot/error-messages/another-account-already-signed-in)
- [Fejlfinding af logonproblemer med moderne Office-godkendelse, når du bruge ADFS](https://docs.microsoft.com/office365/troubleshoot/authentication/sign-in-issue-with-modern-auth)