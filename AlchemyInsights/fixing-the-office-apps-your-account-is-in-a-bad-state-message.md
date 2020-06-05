---
title: Rettelse af Microsoft 365-apps Din konto er i en dårlig tilstand
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "2558"
- "9000571"
ms.openlocfilehash: 264307f23a349ef4ebf40f48ddbcddd3216a4927
ms.sourcegitcommit: f28dafa0f727870038f72bc904da926daf4ec07b
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 06/05/2020
ms.locfileid: "44580111"
---
# <a name="fixing-the-microsoft-365-apps-your-account-is-in-a-bad-state-error"></a>Rettelse af Microsoft 365-apps "Din konto er i en dårlig tilstand"

Du kan rette denne fejl ved at prøve følgende indstillinger på den berørte computer:

- Åbn en Office-app, og vælg **Log**af  >  **filkonto**  >  **for alle konti**. Log på igen ved hjælp af en brugerkonto med en gyldig licens. Hvis du vil have mere at vide, skal du se [Konti i Office](https://support.office.com/article/accounts-in-office-628ea040-f265-49de-b986-be09c3ebf8a9).
- [Ryd Office-legitimationsoplysninger](https://docs.microsoft.com/office/troubleshoot/error-messages/another-account-already-signed-in#step-3-clear-cached-credentials-on-the-computer) ved hjælp af Windows Legitimationsstyring.<br>
  **Bemærk:** Registreringsdatabasen stier for Office 2016 er ændret til 16.0. \Software\Microsoft\Office\16.0\Common\Identity\
- Hvis fejlen opstår under oprettelse af forbindelse til Office 365 ved hjælp af Office 2013, [skal du aktivere moderne godkendelse](https://docs.microsoft.com/microsoft-365/admin/security-and-compliance/enable-modern-authentication) for Office-klienten.

Du kan finde flere oplysninger under [Sådan foretages fejlfinding af apps, der ikke er browsere, og som ikke kan logge på Microsoft 365, Azure eller Intune](https://support.office.com/article/how-to-troubleshoot-non-browser-apps-that-can-t-sign-in-to-office-365-azure-or-intune-3ba1b268-66f6-462c-b0e5-070f5c2603c1).

