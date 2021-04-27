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
ms.openlocfilehash: 5065b9895954371e4298c98e8aadb67ba8f140fd
ms.sourcegitcommit: c977687a7dd03288a9ba396cf2a48ea384d72634
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 04/27/2021
ms.locfileid: "52059809"
---
# <a name="troubleshooting-pst-import-issues"></a><span data-ttu-id="3d49a-102">Fejlfinding af problemer med PST-import</span><span class="sxs-lookup"><span data-stu-id="3d49a-102">Troubleshooting PST import issues</span></span>

- <span data-ttu-id="3d49a-103">Hvis du importerer i selve Outlook-klienten, skal du se [Løs problemer med at importere en Outlook .pst-fil.](https://support.office.com/article/Fix-problems-importing-an-Outlook-pst-file-2d2e50dc-5c36-4ab2-ab50-f1be733b3d6e)</span><span class="sxs-lookup"><span data-stu-id="3d49a-103">If you are importing within the Outlook client itself, see [Fix problems importing an Outlook .pst file](https://support.office.com/article/Fix-problems-importing-an-Outlook-pst-file-2d2e50dc-5c36-4ab2-ab50-f1be733b3d6e).</span></span>

- <span data-ttu-id="3d49a-104">Hvis du bruger importtjenesten, og den sidder fast, skal du bemærke, at hver ENKELT PST-fil, du overfører til Azure Storage-placeringen, ikke må være større end 20 GB.</span><span class="sxs-lookup"><span data-stu-id="3d49a-104">If you are using Import Service and it's stuck, note that each PST file that you upload to the Azure Storage location should be no larger than 20GB.</span></span> <span data-ttu-id="3d49a-105">PST-filer, der er større end 20 GB, kan påvirke ydeevnen for PST-importprocessen.</span><span class="sxs-lookup"><span data-stu-id="3d49a-105">PST files larger than 20GB may impact the performance of the PST import process.</span></span> <span data-ttu-id="3d49a-106">Du kan finde flere oplysninger om fejlfinding af fastlåsde job [under Problemer, der påvirker PST-importjob.](https://docs.microsoft.com/office365/troubleshoot/pst-import-service/issues-with-pst-import-job)</span><span class="sxs-lookup"><span data-stu-id="3d49a-106">For more information troubleshooting stuck jobs, see [Issues that affect PST import jobs](https://docs.microsoft.com/office365/troubleshoot/pst-import-service/issues-with-pst-import-job).</span></span>

- <span data-ttu-id="3d49a-107">Hvis du vil bekræfte status for et bestemt Importjob, skal du bruge [Get-MailboxImportRequest -batchname](https://docs.microsoft.com/powershell/module/exchange/mailboxes/get-mailboximportrequest).</span><span class="sxs-lookup"><span data-stu-id="3d49a-107">If you want to verify the status of a specific Import job, use [Get-MailboxImportRequest -batchname](https://docs.microsoft.com/powershell/module/exchange/mailboxes/get-mailboximportrequest).</span></span>

- <span data-ttu-id="3d49a-108">Se Oversigt over import af organisationens PST-filer for at få flere oplysninger [om importtjenesten.](https://docs.microsoft.com/microsoft-365/compliance/importing-pst-files-to-office-365?view=o365-worldwide)</span><span class="sxs-lookup"><span data-stu-id="3d49a-108">For full details on the import service, see [Overview of importing your organization's PST files](https://docs.microsoft.com/microsoft-365/compliance/importing-pst-files-to-office-365?view=o365-worldwide).</span></span>
