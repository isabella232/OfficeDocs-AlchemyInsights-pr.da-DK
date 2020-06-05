---
title: Problemer med at logge på Microsoft 365-apps
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
- "2560"
ms.openlocfilehash: e4f2fea5c2f368ae240614ee1f7bc729338dd75d
ms.sourcegitcommit: f28dafa0f727870038f72bc904da926daf4ec07b
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 06/05/2020
ms.locfileid: "44579931"
---
# <a name="fixing-the-microsoft-365-apps-sorry-another-account-from-your-organization-is-already-signed-in-message"></a>Rettelse af Microsoft 365-apps "Beklager, en anden konto fra din organisation er allerede logget på"

Du kan rette fejlen ved at følge disse trin:

- Fjern alle arbejdskonti undtagen den berørte konto ved hjælp af Windows-indstillinger > **Access-arbejde eller -skole**.
- [Ryd Office-legitimationsoplysninger](https://docs.microsoft.com/office/troubleshoot/error-messages/another-account-already-signed-in#step-3-clear-cached-credentials-on-the-computer) ved hjælp af Windows Legitimationsstyring.<br/>
    **Bemærk:** Registreringsdatabasen stier for Office 2016 er ændret til 16.0. (Eks.: \Software\Microsoft\Office\16.0\Common\Identity\)
- Åbn en Office-app, og vælg **Log**af  >  **filkonto.**  >  **Sign Out** Log derefter på med en brugerkonto med en gyldig licens. Hvis du vil have mere at vide, skal du se [Konti i Office](https://support.office.com/article/accounts-in-office-628ea040-f265-49de-b986-be09c3ebf8a9).
- For Mac skal du se [Jeg kan ikke logge på en Office 2016 til Mac-app](https://docs.microsoft.com/office365/troubleshoot/authentication/sign-in-to-office-2016-for-mac-fail).

Du kan finde flere oplysninger under ["Beklager, at en anden konto fra din organisation allerede er logget på denne computer" i Office](https://docs.microsoft.com/office/troubleshoot/error-messages/another-account-already-signed-in).