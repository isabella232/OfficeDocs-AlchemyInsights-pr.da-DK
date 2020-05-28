---
title: Går Teams-klient ned?
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9002323"
- "4512"
ms.openlocfilehash: ac1cc05adfa33626ff34d30dca6c77f1bb96477a
ms.sourcegitcommit: c46b8df485edbd13e8bb4d1b2ba1c2821ddc9da0
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 05/23/2020
ms.locfileid: "44354046"
---
# <a name="teams-client-crashing"></a><span data-ttu-id="070db-102">Går Teams-klient ned?</span><span class="sxs-lookup"><span data-stu-id="070db-102">Teams client crashing?</span></span>

<span data-ttu-id="070db-103">Hvis din Teams-klient går ned, kan du prøve følgende:</span><span class="sxs-lookup"><span data-stu-id="070db-103">If your Teams client is crashing, try the following:</span></span>

- <span data-ttu-id="070db-104">Hvis du bruger Teams-skrivebordsapp, [skal du sørge for, at appen er helt opdateret](https://support.office.com/article/Update-Microsoft-Teams-535a8e4b-45f0-4f6c-8b3d-91bca7a51db1).</span><span class="sxs-lookup"><span data-stu-id="070db-104">If you are using the Teams desktop app, [make sure the app is fully updated](https://support.office.com/article/Update-Microsoft-Teams-535a8e4b-45f0-4f6c-8b3d-91bca7a51db1).</span></span>

- <span data-ttu-id="070db-105">Sørg for, at alle [Microsoft 365-url'er og adresseområder](https://docs.microsoft.com/microsoftteams/connectivity-issues) er tilgængelige.</span><span class="sxs-lookup"><span data-stu-id="070db-105">Make sure all the [Microsoft 365 URLs and address ranges](https://docs.microsoft.com/microsoftteams/connectivity-issues) are accessible.</span></span>

- <span data-ttu-id="070db-106">Log på med din lejeradministratorkonto, og tjek [dashboardet for tjenestetilstand](https://docs.microsoft.com/office365/enterprise/view-service-health) for at kontrollere, at der ikke er nogen nedbrud eller forringelse af tjenesten.</span><span class="sxs-lookup"><span data-stu-id="070db-106">Log in with your tenant admin account and check your [Service Health Dashboard](https://docs.microsoft.com/office365/enterprise/view-service-health) to verify that no outage or service degradation exists.</span></span>

- <span data-ttu-id="070db-107">Fjerne og geninstallere programmet Teams (link)</span><span class="sxs-lookup"><span data-stu-id="070db-107">Uninstall and reinstall the Teams Application (link)</span></span>
    - <span data-ttu-id="070db-108">Gå til mappen %appdata%\Microsoft\teams\ på computeren, og slet alle filer i den pågældende mappe.</span><span class="sxs-lookup"><span data-stu-id="070db-108">Browse to the %appdata%\Microsoft\teams\ folder on your computer and delete all files in that directory.</span></span>
    - <span data-ttu-id="070db-109">[Download og installer Teams-appen](https://www.microsoft.com/microsoft-365/microsoft-teams/group-chat-software#office-DesktopAppDownload-ofoushy), og installer, hvis det er muligt, Teams som administrator (højreklik på installationsprogrammet Teams, og vælg "Kør som administrator", hvis det er muligt).</span><span class="sxs-lookup"><span data-stu-id="070db-109">[Download and install the Teams App](https://www.microsoft.com/microsoft-365/microsoft-teams/group-chat-software#office-DesktopAppDownload-ofoushy), and if possible, install Teams as an administrator (right click the Teams installer and select "Run as administrator" if available).</span></span>

<span data-ttu-id="070db-110">Hvis din Teams-klient stadig går ned, kan du så genskabe problemet?</span><span class="sxs-lookup"><span data-stu-id="070db-110">If your Teams client is still crashing, can you reproduce the issue?</span></span> <span data-ttu-id="070db-111">Hvis ja:</span><span class="sxs-lookup"><span data-stu-id="070db-111">If so:</span></span>

1. <span data-ttu-id="070db-112">Brug Trinoptageren til at hente dine trin.</span><span class="sxs-lookup"><span data-stu-id="070db-112">Use the Steps Recorder to capture your steps.</span></span>
    - <span data-ttu-id="070db-113">Luk ALLE unødvendige eller fortrolige ansøgninger.</span><span class="sxs-lookup"><span data-stu-id="070db-113">Close ALL unnecessary or confidential applications.</span></span>
    - <span data-ttu-id="070db-114">Start Trinoptageren, og gengiv problemet, mens du er logget på med den berørte brugerkonto.</span><span class="sxs-lookup"><span data-stu-id="070db-114">Launch the Steps Recorder and reproduce the issue while logged in with the affected user account.</span></span>
    - <span data-ttu-id="070db-115">[Saml de holdlogfiler, der registrerer de registrerede reprotrin](https://docs.microsoft.com/microsoftteams/log-files).</span><span class="sxs-lookup"><span data-stu-id="070db-115">[Collect the teams logs that capture the recorded repro steps](https://docs.microsoft.com/microsoftteams/log-files).</span></span> <span data-ttu-id="070db-116">**Bemærk:** Sørg for at registrere logonadressen for den påvirkede bruger.</span><span class="sxs-lookup"><span data-stu-id="070db-116">**Note**: Make sure you capture the sign-in address of the impacted user.</span></span>
    - <span data-ttu-id="070db-117">Indsaml oplysningerne om dump og/eller fejlbucket (Windows).</span><span class="sxs-lookup"><span data-stu-id="070db-117">Collect the dump and/or Fault bucket info (Windows).</span></span> <span data-ttu-id="070db-118">Start Windows Powershell på den maskine, hvor nedbruddet sker, og kør følgende kommandoer:</span><span class="sxs-lookup"><span data-stu-id="070db-118">Launch Windows Powershell on the machine where the crash is occurring and run the following commands:</span></span>

        `
        PS C:\Users\user01> cd $env:temp
        PS C:\Users\user01\AppData\Local\Temp> Get-EventLog -LogName Application -Message "*Teams.exe*" -InstanceId 1001 | Select-Object -First 10 | Format-List > FaultBuckets.txt
        PS C:\Users\user01\AppData\Local\Temp> notepad .\FaultBuckets.txt
        `
    
2. <span data-ttu-id="070db-119">Vedhæft filen til supportsagen.</span><span class="sxs-lookup"><span data-stu-id="070db-119">Attach the file to your support case.</span></span>
