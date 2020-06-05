---
title: Rettede Microsoft 365-apps Kunne ikke finde tilknyttede office-licenser
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3421"
- "9001426"
ms.openlocfilehash: 65ffae1a784f841cb08a5df52b02671a4526d9d4
ms.sourcegitcommit: f28dafa0f727870038f72bc904da926daf4ec07b
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 06/05/2020
ms.locfileid: "44580435"
---
# <a name="fixing-the-microsoft-365-apps-couldnt-find-office-licenses-associated-message"></a>Rettelse af Microsoft 365-apps "Kunne ikke finde tilknyttede kontorlicenser"

Hvis du modtager denne meddelelse, kan du prøve følgende:

1. Kontroller din firewall, dit antivirusprogram og dine proxyindstillinger for at bekræfte, at de ikke blokerer for internetadgang til Microsoft 365-apps. Se [Microsoft 365 URL-adresser og IP-adresseområder](https://docs.microsoft.com/office365/enterprise/urls-and-ip-address-ranges).
2. Fjern og [tildel Office-licensen](https://docs.microsoft.com/microsoft-365/admin/manage/assign-licenses-to-users) til den berørte bruger igen. 
3. Åbn en Office-app, og [log](https://support.office.com/article/5a20dc11-47e9-4b6f-945d-478cb6d92071) af eksisterende brugerkonti.
4. Gå til Windows-indstillinger **Accounts**>  >  **konti, & konti,** og fjern alle arbejdskonti undtagen den berørte konto.
5. Gå til Windows-indstillinger > **Konti**  >  **Access-arbejde eller -skole**, og afbryd forbindelsen til alle arbejdskonti undtagen den berørte konto.
6. Nulstil office-aktiveringstilstanden. [Få mere at vide om, hvordan](https://docs.microsoft.com/office365/troubleshoot/activation/reset-office-365-proplus-activation-state).
7. [Log på](https://support.office.com/article/628ea040-f265-49de-b986-be09c3ebf8a9) med den berørte brugerkonto.

Du kan finde flere fejlfindingsløsninger [under Produkt- og aktiveringsfejl uden licens i Office](https://support.office.com/Article/0d23d3c0-c19c-4b2f-9845-5344fedc4380).