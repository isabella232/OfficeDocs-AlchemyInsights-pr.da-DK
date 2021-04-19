---
title: Fejlfinding af problemer med PST-import
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "1800027"
- "1225"
ms.openlocfilehash: 07609b39149c003b029f3ea5669f4044af43c25d
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 04/15/2021
ms.locfileid: "51826157"
---
# <a name="troubleshooting-pst-import-issues"></a>Fejlfinding af problemer med PST-import

- Hvis du importerer i selve Outlook-klienten, skal du se [Løs problemer med at importere en Outlook .pst-fil](https://support.office.com/article/Fix-problems-importing-an-Outlook-pst-file-2d2e50dc-5c36-4ab2-ab50-f1be733b3d6e).

- Hvis du bruger importtjenesten, og den er gået i stå, skal du være opmærksom på, at hver PST-fil, du overfører til Azure-lagerplaceringen, ikke må være større end 20 GB. PST-filer, der er større end 20 GB, kan påvirke ydeevnen af PST-importen.

- Hvis du vil bekræfte statussen på et bestemt importjob, kan du bruge [Get-MailboxImportRequest -batchname](https://docs.microsoft.com/powershell/module/exchange/mailboxes/get-mailboximportrequest).

- Hvis du vil have detaljerede oplysninger om importtjenesten, skal du se [Oversigt over import af din organisations PST-filer](https://docs.microsoft.com/microsoft-365/compliance/importing-pst-files-to-office-365?view=o365-worldwide).
