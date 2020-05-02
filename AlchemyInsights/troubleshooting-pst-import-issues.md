---
title: Fejlfinding af problemer med PST-import
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "1800027"
- "1225"
ms.openlocfilehash: 58fdd509fae5e87bf5ae72db5d8926c4367cdd64
ms.sourcegitcommit: 87aa36e3ff4835efb120a320c5169bfa77199ec4
ms.translationtype: HT
ms.contentlocale: da-DK
ms.lasthandoff: 05/01/2020
ms.locfileid: "43991153"
---
# <a name="troubleshooting-pst-import-issues"></a><span data-ttu-id="94654-102">Fejlfinding af problemer med PST-import</span><span class="sxs-lookup"><span data-stu-id="94654-102">Troubleshooting PST import issues</span></span>

- <span data-ttu-id="94654-103">Hvis du importerer i selve Outlook-klienten, skal du se [Løs problemer med at importere en Outlook .pst-fil](https://support.office.com/article/Fix-problems-importing-an-Outlook-pst-file-2d2e50dc-5c36-4ab2-ab50-f1be733b3d6e).</span><span class="sxs-lookup"><span data-stu-id="94654-103">If you are importing within the Outlook client itself, please see [Fix problems importing an Outlook .pst file](https://support.office.com/article/Fix-problems-importing-an-Outlook-pst-file-2d2e50dc-5c36-4ab2-ab50-f1be733b3d6e).</span></span>

- <span data-ttu-id="94654-104">Hvis du bruger importtjenesten, og den er gået i stå, skal du være opmærksom på, at hver PST-fil, du overfører til Azure-lagerplaceringen, ikke må være større end 20 GB.</span><span class="sxs-lookup"><span data-stu-id="94654-104">If you are using Import Service and it is stuck, please note that each PST file that you upload to the Azure Storage location should be no larger than 20 GB.</span></span> <span data-ttu-id="94654-105">PST-filer, der er større end 20 GB, kan påvirke ydeevnen af PST-importen.</span><span class="sxs-lookup"><span data-stu-id="94654-105">PST files larger than 20 GB may impact the performance of the PST import process.</span></span>

- <span data-ttu-id="94654-106">Hvis du vil bekræfte statussen på et bestemt importjob, kan du bruge [Get-MailboxImportRequest -batchname](https://docs.microsoft.com/powershell/module/exchange/mailboxes/get-mailboximportrequest).</span><span class="sxs-lookup"><span data-stu-id="94654-106">If you want to verify the status of a specific Import job, you can use [Get-MailboxImportRequest -batchname](https://docs.microsoft.com/powershell/module/exchange/mailboxes/get-mailboximportrequest).</span></span>

- <span data-ttu-id="94654-107">Hvis du vil have detaljerede oplysninger om importtjenesten, skal du se [Oversigt over import af din organisations PST-filer](https://docs.microsoft.com/microsoft-365/compliance/importing-pst-files-to-office-365?view=o365-worldwide).</span><span class="sxs-lookup"><span data-stu-id="94654-107">For full details on the import service, please see [Overview of importing your organization's PST files](https://docs.microsoft.com/microsoft-365/compliance/importing-pst-files-to-office-365?view=o365-worldwide).</span></span>
