---
title: Løse problemer med Microsoft 365-apps Din konto er i en dårlig tilstand
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
- "2558"
- "9000571"
ms.openlocfilehash: 4654b49289a455c1e6641f47fae573d2fcebc717
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 04/15/2021
ms.locfileid: "51812530"
---
# <a name="fixing-the-microsoft-365-apps-your-account-is-in-a-bad-state-error"></a>Fejl ved løsning af Microsoft 365-appsene "Din konto er i en dårlig tilstand"

Du kan løse denne fejl ved at prøve følgende indstillinger på den pågældende computer:

- Åbn en Office-app, vælg   >  **Filkonto**  >  **Log af alle konti**. Log på igen med en brugerkonto med en gyldig licens. Hvis du vil have mere at vide, skal du se [Konti i Office](https://support.office.com/article/accounts-in-office-628ea040-f265-49de-b986-be09c3ebf8a9).
- [Ryd Office-legitimationsoplysninger ved](https://docs.microsoft.com/office/troubleshoot/error-messages/another-account-already-signed-in#step-3-clear-cached-credentials-on-the-computer) hjælp af Windows Legitimationsstyring.<br>
  **Bemærk!** Stierne i registreringsdatabasen til Office 2016 er ændret til 16.0. F.eks. \Software\Microsoft\Office\16.0\Common\Identity\
- Hvis fejlen opstår, når du opretter forbindelse til Office 365 ved hjælp af Office 2013, skal du aktivere moderne [godkendelse](https://docs.microsoft.com/microsoft-365/admin/security-and-compliance/enable-modern-authentication) for Office-klienten.

Du kan finde flere oplysninger i Sådan foretager du fejlfinding af apps, der ikke er i en browser, og som ikke kan logges på [Microsoft 365, Azure eller Intune.](https://support.office.com/article/how-to-troubleshoot-non-browser-apps-that-can-t-sign-in-to-office-365-azure-or-intune-3ba1b268-66f6-462c-b0e5-070f5c2603c1)

