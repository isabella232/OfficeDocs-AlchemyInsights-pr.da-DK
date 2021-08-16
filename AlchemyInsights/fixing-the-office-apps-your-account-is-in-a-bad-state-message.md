---
title: Løse problemer Microsoft 365 apps Din konto er i en dårlig tilstand
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
ms.openlocfilehash: 68c4dfcc0500761f8ce5090fddb9f2ad58af77bc411c9e714b14c383fef177de
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 08/05/2021
ms.locfileid: "54068230"
---
# <a name="fixing-the-microsoft-365-apps-your-account-is-in-a-bad-state-error"></a>Du kan Microsoft 365 problemer med appsene "Din konto er i en dårlig tilstand"

Du kan løse denne fejl ved at prøve følgende indstillinger på den pågældende computer:

- Åbn en Office-app, vælg  >  **Filkonto**  >  **Log af alle konti**. Log på igen med en brugerkonto med en gyldig licens. Hvis du vil have mere at vide, skal du se [Konti i Office](https://support.office.com/article/accounts-in-office-628ea040-f265-49de-b986-be09c3ebf8a9).
- [Ryd Office legitimationsoplysninger ved](https://docs.microsoft.com/office/troubleshoot/error-messages/another-account-already-signed-in#step-3-clear-cached-credentials-on-the-computer) Windows Legitimationsstyring.<br>
  **Bemærk!** Stierne i registreringsdatabasen Office 2016 ændret til 16.0. F.eks. \Software\Microsoft\Office\16.0\Common\Identity\
- Hvis fejlen opstår, når du opretter forbindelse til en Office 365 bruger [](https://docs.microsoft.com/microsoft-365/admin/security-and-compliance/enable-modern-authentication) Office 2013, skal du aktivere moderne godkendelse for Office klient.

Du kan finde flere oplysninger i Sådan foretager du fejlfinding af apps, der ikke er i en browser, og som ikke kan logges på [Microsoft 365, Azure eller Intune.](https://support.office.com/article/how-to-troubleshoot-non-browser-apps-that-can-t-sign-in-to-office-365-azure-or-intune-3ba1b268-66f6-462c-b0e5-070f5c2603c1)

