---
title: Problemer med at logge på Office-apps
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
ms.openlocfilehash: 695d449a876c22ff441da2367ef67aaea470eb66
ms.sourcegitcommit: 631cbb5f03e5371f0995e976536d24e9d13746c3
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 04/22/2020
ms.locfileid: "43762977"
---
# <a name="issues-signing-in-to-office-apps"></a>Problemer med at logge på Office-apps

Hvis du vil løse logonproblemer med Office-apps, kan du prøve følgende:

- Fjern alle arbejdskonti, undtagen den berørte konto, ved hjælp af Windows-indstillinger > **Access-arbejde eller skole**.
- [Ryd Office-legitimationsoplysninger](https://docs.microsoft.com/office/troubleshoot/error-messages/another-account-already-signed-in#step-3-clear-cached-credentials-on-the-computer) ved hjælp af Windows Credential Manager.<br/>
    **Bemærk:** Registreringsdatabasestierne til Office 2016 er ændret til 16.0. (F.eks.: \Software\Microsoft\Office\16.0\Common\Identity\)
- Åbn en Office-app, og vælg**Log af** **filkonto** > **Account** > . Log derefter på med en brugerkonto med en gyldig licens. Hvis du vil have mere at vide, skal du se [Konti i Office](https://support.office.com/article/accounts-in-office-628ea040-f265-49de-b986-be09c3ebf8a9).
- For Mac skal du se [Jeg kan ikke logge på en Office 2016 til Mac-app](https://docs.microsoft.com/office365/troubleshoot/authentication/sign-in-to-office-2016-for-mac-fail).
- Hvis fejlene opstår under oprettelse af forbindelse til Microsoft 365 ved hjælp af Office 2013, skal du aktivere moderne godkendelse af Office-klienten.

Du kan finde flere oplysninger under:
- [Du kan ikke logge på Microsoft 365, Azure eller Intune](https://docs.microsoft.com/office365/troubleshoot/authentication/sign-in-to-office-365-azure-intune)
- [Forbindelsesproblemer i logon efter opdatering til Office 2016 build 16.0.7967 på Windows 10](https://docs.microsoft.com/office365/troubleshoot/administration/connection-issue-when-sign-in-office-2016)
- ["Beklager, en anden konto fra din organisation er allerede logget på denne computer" i Office](https://docs.microsoft.com/office/troubleshoot/error-messages/another-account-already-signed-in)
- [Fejlfinding i forbindelse med logonproblemer med moderne Office-godkendelse, når du bruger ADFS](https://docs.microsoft.com/office365/troubleshoot/authentication/sign-in-issue-with-modern-auth)