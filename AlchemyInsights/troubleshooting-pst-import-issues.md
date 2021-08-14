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
ms.openlocfilehash: 549af832f9c58db1cdd8fbe80b8b5bd2aba9bd937f33116806a9391cbc9a5d4c
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 08/05/2021
ms.locfileid: "53972413"
---
# <a name="troubleshooting-pst-import-issues"></a>Fejlfinding af problemer med PST-import

- Hvis du importerer i selve Outlook, skal du se Løs problemer med [at importere en Outlook .pst-fil.](https://support.office.com/article/Fix-problems-importing-an-Outlook-pst-file-2d2e50dc-5c36-4ab2-ab50-f1be733b3d6e)

- Hvis du bruger importtjenesten, og den sidder fast, skal du være opmærksom på, at hver enkelt PST-fil, du overfører til placeringen Azure Storage, ikke må være større end 20 GB. PST-filer, der er større end 20 GB, kan påvirke ydeevnen for PST-importprocessen. Du kan finde flere oplysninger om fejlfinding af fastlåsde job [under Problemer, der påvirker PST-importjob.](https://docs.microsoft.com/office365/troubleshoot/pst-import-service/issues-with-pst-import-job)

- Hvis du vil bekræfte status for et bestemt Importjob, skal du bruge [Get-MailboxImportRequest -batchname](https://docs.microsoft.com/powershell/module/exchange/mailboxes/get-mailboximportrequest).

- Se Oversigt over import af organisationens PST-filer for at få flere oplysninger [om importtjenesten.](https://docs.microsoft.com/microsoft-365/compliance/importing-pst-files-to-office-365?view=o365-worldwide)
