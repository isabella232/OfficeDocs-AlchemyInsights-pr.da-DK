---
title: Problemer med at logge på Microsoft 365-apps
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000571"
- "2560"
ms.openlocfilehash: 7d2cfd437bb55804c3b9263428833c10d5caaa47
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 09/14/2020
ms.locfileid: "47695317"
---
# <a name="fixing-the-microsoft-365-apps-sorry-another-account-from-your-organization-is-already-signed-in-message"></a>Rettelse af Microsoft 365-apps "beklager, men en anden konto fra din organisation er allerede logget på.

Du kan rette fejlen ved at følge disse trin:

- Fjern alle arbejds konti, undtagen den pågældende konto, ved hjælp af Windows-indstillinger > **få adgang til arbejde eller skole**.
- [Ryd Office-legitimationsoplysninger](https://docs.microsoft.com/office/troubleshoot/error-messages/another-account-already-signed-in#step-3-clear-cached-credentials-on-the-computer) ved hjælp af Windows credential Manager.<br/>
    **Bemærk:** Registreringsdatabase stierne til Office 2016 er blevet ændret til 16,0. (F. eks.: \Software\Microsoft\Office\16.0\Common\Identity\)
- Åbn en Office-app, **og vælg**  >  **Account**  >  **Log af**-konto. Log derefter på ved hjælp af en brugerkonto med en gyldig licens. Hvis du vil have mere at vide, skal du se [Konti i Office](https://support.office.com/article/accounts-in-office-628ea040-f265-49de-b986-be09c3ebf8a9).
- For Mac skal du se [Jeg kan ikke logge på en Office 2016 til Mac-app](https://docs.microsoft.com/office365/troubleshoot/authentication/sign-in-to-office-2016-for-mac-fail).

Hvis du vil have mere at vide, skal du se ["Vi beklager, men en anden konto fra din organisation er allerede logget på denne computer" i Office](https://docs.microsoft.com/office/troubleshoot/error-messages/another-account-already-signed-in).