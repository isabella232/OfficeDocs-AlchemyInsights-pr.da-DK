---
title: Rettelse af Microsoft 365-apps kunne ikke finde Office-licenser knyttet meddelelse
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
- "3421"
- "9001426"
ms.openlocfilehash: bd127d6287b4438f6105a6158abdbd5b964b7e70
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 09/14/2020
ms.locfileid: "47747689"
---
# <a name="fixing-the-microsoft-365-apps-couldnt-find-office-licenses-associated-message"></a>Rettelse af Microsoft 365-apps meddelelsen "der blev ikke fundet nogen Office-licenser"

Hvis du får vist denne meddelelse, kan du prøve følgende:

1. Kontrollér din firewall, antivirussoftware og proxyindstillinger for at bekræfte, at de ikke blokerer Internet adgang til Microsoft 365-apps. Se [Microsoft 365 URL-adresser og IP-adresseområder](https://docs.microsoft.com/office365/enterprise/urls-and-ip-address-ranges).
2. Fjern og [Tildel Office-licensen](https://docs.microsoft.com/microsoft-365/admin/manage/assign-licenses-to-users) for den pågældende bruger. 
3. Åbn en Office-app, og [Log](https://support.office.com/article/5a20dc11-47e9-4b6f-945d-478cb6d92071) af fra eksisterende brugerkonti.
4. Gå til Windows-indstillinger > **konti**  >  **mail & konti**, og fjern alle arbejds konti undtagen den pågældende konto.
5. Gå til Windows-indstillinger > **konti**  >  **adgang til arbejde eller skole**, og Afbryd forbindelsen til alle arbejds konti undtagen den pågældende konto.
6. Nulstil Office-aktiveringstilstanden. [Lær hvordan](https://docs.microsoft.com/office365/troubleshoot/activation/reset-office-365-proplus-activation-state).
7. [Log på](https://support.office.com/article/628ea040-f265-49de-b986-be09c3ebf8a9) med den pågældende brugerkonto.

Du kan finde flere fejlfindings løsninger [i fejl i forbindelse med produkt og aktivering i Office](https://support.office.com/Article/0d23d3c0-c19c-4b2f-9845-5344fedc4380).