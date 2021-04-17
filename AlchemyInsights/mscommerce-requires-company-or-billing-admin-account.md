---
title: Opret forbindelse til MSCommerce-modulet
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
- "9001212"
- "3529"
ms.openlocfilehash: 8e6819f6d6ff37baab4bdd49cb5a87c32490f841
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 04/15/2021
ms.locfileid: "51829730"
---
# <a name="mscommerce-requires-a-company-or-billing-administrator-account"></a>MSCommerce kræver en firma- eller faktureringsadministratorkonto

Modulet MSCommerce kræver en konto med firma- eller faktureringsadministratorrettigheder. Hvis du modtager følgende fejlmeddelelse, skal du genoprette forbindelsen til en anden konto.

*ErrorMessage – Fjernserveren returnerede en fejl: (403) Forbudt. ErrorDetails – At C:\Program Files\WindowsPowerShell\Modules\MSCommerce\1.2\MSCommerce.psm1:216 char:5*<br>
*+&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;HandleError -ErrorContext $_ -CustomErrorMessage "Failed to retri ...*<br>
\+&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~<br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;*+ CategoryInfo: NotSpecified: (:) [Write-Error], WriteErrorException*<br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;*+ fullyQualifiedErrorId: Microsoft.PowerShell.Commands.WriteErrorException,HandleError*

Hvis din konto ikke har rettigheder som firma- eller faktureringsadministrator, skal du kontakte din it-administrator.
