---
title: Kalendertilladelser
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3800009"
- "611"
ms.openlocfilehash: 78f27014c60badc801212177dd455ef2a0de5a9e
ms.sourcegitcommit: 722e9a0ed058cb1eab2dd053be2418b60f7d4aac
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 06/23/2020
ms.locfileid: "44862059"
---
# <a name="calendar-permissions"></a><span data-ttu-id="377cb-102">Kalendertilladelser</span><span class="sxs-lookup"><span data-stu-id="377cb-102">Calendar Permissions</span></span>

<span data-ttu-id="377cb-103">Brugerne kan ændre deres egne kalendertilladelser med Outlook på internettet eller andre klienter, men som administrator skal du muligvis også undersøge det.</span><span class="sxs-lookup"><span data-stu-id="377cb-103">Users can change their own Calendar Permissions with Outlook on the Web or other clients, but as an admin you may need to investigate as well.</span></span>  
<span data-ttu-id="377cb-104">Med Exchange PowerShell-cmdlet får du tilladelse til at følge en brugers kalender:</span><span class="sxs-lookup"><span data-stu-id="377cb-104">With Exchange PowerShell cmdlet will show you the permission on a user’s calendar:</span></span>

`Get-MailboxFolderPermission <SMTPAddress>:\Calendar | FT -a`

<span data-ttu-id="377cb-105">Hvis du vil se flere oplysninger, skal du se følgende:</span><span class="sxs-lookup"><span data-stu-id="377cb-105">To see more information see the following:</span></span>

- [<span data-ttu-id="377cb-106">Hent-PostkasseFoldErPermission</span><span class="sxs-lookup"><span data-stu-id="377cb-106">Get-MailboxFolderPermission</span></span>](https://docs.microsoft.com/powershell/module/exchange/get-mailboxfolderpermission?view=exchange-ps)

- [<span data-ttu-id="377cb-107">Set-MailboxFolderPermission</span><span class="sxs-lookup"><span data-stu-id="377cb-107">Set-MailboxFolderPermission</span></span>](https://docs.microsoft.com/powershell/module/exchange/set-mailboxfolderpermission?view=exchange-ps)

- [<span data-ttu-id="377cb-108">Tilføj postkassefoldErPermission</span><span class="sxs-lookup"><span data-stu-id="377cb-108">Add-MailboxFolderPermission</span></span>](https://office.visualstudio.com/DefaultCollection/MAX/_queries/query/Add-MailboxFolderPermission)

<span data-ttu-id="377cb-109">Kalendertilladelser bruges i deling af kalendere for at få vist flere oplysninger om deling af en Outlook-kalender i disse artikler:</span><span class="sxs-lookup"><span data-stu-id="377cb-109">Calendar Permissions are used in the sharing of calendars, to see more information about sharing an Outlook calendar, see these articles:</span></span>

- [<span data-ttu-id="377cb-110">Del en Outlook-kalender med andre personer</span><span class="sxs-lookup"><span data-stu-id="377cb-110">Share an Outlook calendar with other people</span></span>](https://support.office.com/article/353ed2c1-3ec5-449d-8c73-6931a0adab88)
- [<span data-ttu-id="377cb-111">Dele din kalender i Outlook på internettet til virksomheder</span><span class="sxs-lookup"><span data-stu-id="377cb-111">Share your calendar in Outlook on the web for business</span></span>](https://support.office.com/article/7ecef8ae-139c-40d9-bae2-a23977ee58d5)

<span data-ttu-id="377cb-112">Hvis du vil foretage fejlfinding af kalendertilladelse, kan du bruge værktøjet [Support og Genoprettelsesassistent.](https://support.microsoft.com/office/e90bb691-c2a7-4697-a94f-88836856c72f)</span><span class="sxs-lookup"><span data-stu-id="377cb-112">To troubleshoot Calendar Permission you can use the [Support and Recovery Assistant](https://support.microsoft.com/office/e90bb691-c2a7-4697-a94f-88836856c72f) tool.</span></span>