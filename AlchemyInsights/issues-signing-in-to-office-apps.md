---
title: Problemer med at logge på Microsoft 365 apps
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000571"
- "2560"
ms.openlocfilehash: 454000eafa6818f91e3c302cc69fbf252aae1107aa18904ac93a4756d4db642b
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 08/05/2021
ms.locfileid: "54028034"
---
# <a name="fixing-the-microsoft-365-apps-sorry-another-account-from-your-organization-is-already-signed-in-message"></a>Fejlmeddelelsen Microsoft 365 "Beklager, en anden konto fra din organisation er allerede logget på" i problemer

Du kan rette fejlen ved at følge disse trin:

- Fjern alle arbejdskonti, undtagen den pågældende konto, ved hjælp Windows Indstillinger > **Adgang til arbejde eller skole.**
- [Ryd Office legitimationsoplysninger ved](https://docs.microsoft.com/office/troubleshoot/error-messages/another-account-already-signed-in#step-3-clear-cached-credentials-on-the-computer) Windows Legitimationsstyring.<br/>
    **Bemærk!** Stierne i registreringsdatabasen Office 2016 ændret til 16.0. (Eksempel: \Software\Microsoft\Office\16.0\Common\Identity\)
- Åbn en Office-app, og vælg **Log**  >  **af**  >  **filkonto.** Log derefter på med en brugerkonto med en gyldig licens. Hvis du vil have mere at vide, skal du se [Konti i Office](https://support.office.com/article/accounts-in-office-628ea040-f265-49de-b986-be09c3ebf8a9).
- For Mac skal du se [Jeg kan ikke logge på en Office 2016 til Mac-app](https://docs.microsoft.com/office365/troubleshoot/authentication/sign-in-to-office-2016-for-mac-fail).

Du kan få mere at vide [under "Vi beklager,](https://docs.microsoft.com/office/troubleshoot/error-messages/another-account-already-signed-in)men en anden konto fra din organisation allerede er logget på denne computer" Office .