---
title: Rettelse af Office Apps Din konto er i en meddelelse om dårlig tilstand
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
ms.openlocfilehash: ac760b417ad98b9d5bb6be4b92e60074ab93ceb3
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 04/22/2020
ms.locfileid: "43708681"
---
# <a name="fixing-the-office-apps-your-account-is-in-a-bad-state-error"></a>Rettelse af Office-apps "Din konto er i en dårlig tilstand"

Du kan løse denne fejl ved at prøve følgende indstillinger på den berørte computer:

- Åbn en Office-app, og vælg > **Filkontologon** > **af alle konti**. **File** Log på igen ved hjælp af en brugerkonto med en gyldig licens. Hvis du vil have mere at vide, skal du se [Konti i Office](https://support.office.com/article/accounts-in-office-628ea040-f265-49de-b986-be09c3ebf8a9).
- [Ryd Office-legitimationsoplysninger](https://docs.microsoft.com/office/troubleshoot/error-messages/another-account-already-signed-in#step-3-clear-cached-credentials-on-the-computer) ved hjælp af Windows Credential Manager.<br>
  **Bemærk:** Registreringsdatabasestierne til Office 2016 er ændret til 16.0. \Software\Microsoft\Office\16.0\Common\Identity\
- Hvis fejlen opstår under oprettelse af forbindelse til Office 365 ved hjælp af Office 2013, [skal du aktivere moderne godkendelse](https://docs.microsoft.com/office365/admin/security-and-compliance/enable-modern-authentication) for Office-klienten.

Du kan finde flere oplysninger [under Sådan foretager du fejlfinding af apps, der ikke er browserapps, der ikke kan logge på Microsoft 365, Azure eller Intune](https://support.office.com/article/how-to-troubleshoot-non-browser-apps-that-can-t-sign-in-to-office-365-azure-or-intune-3ba1b268-66f6-462c-b0e5-070f5c2603c1).

