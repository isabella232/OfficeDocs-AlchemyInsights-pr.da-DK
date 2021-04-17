---
title: Meddelelse om, at Microsoft 365-apps ikke kunne finde de tilknyttede Office-licenser
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
- "3421"
- "9001426"
ms.openlocfilehash: 1d717fce77de2f55dfc983d42b7f8d46a8c212e7
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 04/15/2021
ms.locfileid: "51816482"
---
# <a name="fixing-the-microsoft-365-apps-couldnt-find-office-licenses-associated-message"></a>Fejlmeddelelsen "Kunne ikke finde office-licenser tilknyttet" i Microsoft 365-apps

Hvis du modtager denne meddelelse, kan du prøve følgende:

1. Kontrollér din firewall, din antivirussoftware og dine proxyindstillinger for at bekræfte, at de ikke blokerer internetadgang til Microsoft 365-apps. Se [URL-adresser og IP-adresseintervaller for Microsoft 365](https://docs.microsoft.com/office365/enterprise/urls-and-ip-address-ranges).
2. Fjern og [tildel Office-licensen](https://docs.microsoft.com/microsoft-365/admin/manage/assign-licenses-to-users) for den pågældende bruger igen. 
3. Åbn en Office-app, [og log](https://support.office.com/article/5a20dc11-47e9-4b6f-945d-478cb6d92071) af eventuelle eksisterende brugerkonti.
4. Gå til Windows-indstillinger > **konti**  >  **& konti,** og fjern alle arbejdskonti undtagen den pågældende konto.
5. Gå til Windows-indstillinger **>-konti**  >  **Adgang til arbejde eller skole,** og afbryd forbindelsen til alle arbejdskonti undtagen den pågældende konto.
6. Nulstil Office-aktiveringstilstanden. [Lær hvordan.](https://docs.microsoft.com/office365/troubleshoot/activation/reset-office-365-proplus-activation-state)
7. [Log på](https://support.office.com/article/628ea040-f265-49de-b986-be09c3ebf8a9) med den pågældende brugerkonto.

Du kan finde flere fejlfindingsløsninger [under Fejl i forbindelse med produkt og aktivering uden licens i Office.](https://support.office.com/Article/0d23d3c0-c19c-4b2f-9845-5344fedc4380)