---
title: Rettelse af Microsoft 365-apps din konto er i en fejlmeddelelse
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
- "2558"
- "9000571"
ms.openlocfilehash: ec529291ec9406eba9dc2b0f2cc7a93c77fa3456
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 09/14/2020
ms.locfileid: "47744539"
---
# <a name="fixing-the-microsoft-365-apps-your-account-is-in-a-bad-state-error"></a>Hvis du vil reparere Microsoft 365-appsene, er din konto i en fejltilstand

Hvis du vil rette fejlen, skal du prøve følgende indstillinger på den berørte computer:

- Åbne en Office-app, **File**skal du vælge  >  **Account**  >  **Log af alle konti i**logfilen. Log på igen med en brugerkonto med en gyldig licens. Hvis du vil have mere at vide, skal du se [Konti i Office](https://support.office.com/article/accounts-in-office-628ea040-f265-49de-b986-be09c3ebf8a9).
- [Ryd Office-legitimationsoplysninger](https://docs.microsoft.com/office/troubleshoot/error-messages/another-account-already-signed-in#step-3-clear-cached-credentials-on-the-computer) ved hjælp af Windows credential Manager.<br>
  **Bemærk:** Registreringsdatabase stierne til Office 2016 er blevet ændret til 16,0. For eksempel \Software\Microsoft\Office\16.0\Common\Identity\
- Hvis fejlen opstår, mens du opretter forbindelse til Office 365 med Office 2013, skal du [aktivere moderne godkendelse](https://docs.microsoft.com/microsoft-365/admin/security-and-compliance/enable-modern-authentication) for Office-klienten.

Hvis du vil have mere at vide, skal du se [Sådan foretager du fejlfinding af ikke-browser-apps, der ikke kan logge på Microsoft 365, Azure eller Intune](https://support.office.com/article/how-to-troubleshoot-non-browser-apps-that-can-t-sign-in-to-office-365-azure-or-intune-3ba1b268-66f6-462c-b0e5-070f5c2603c1).

