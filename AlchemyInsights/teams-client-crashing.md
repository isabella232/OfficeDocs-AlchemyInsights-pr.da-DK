---
title: Går Teams-klient ned?
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
- "9002323"
- "4512"
ms.openlocfilehash: 20f03b075787cab85ab15d5272c0416b88ebbaee
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 04/15/2021
ms.locfileid: "51826265"
---
# <a name="teams-client-crashing"></a><span data-ttu-id="1ef5b-102">Går Teams-klient ned?</span><span class="sxs-lookup"><span data-stu-id="1ef5b-102">Teams client crashing?</span></span>

<span data-ttu-id="1ef5b-103">Hvis din Teams-klient går ned, kan du prøve følgende:</span><span class="sxs-lookup"><span data-stu-id="1ef5b-103">If your Teams client is crashing, try the following:</span></span>

- <span data-ttu-id="1ef5b-104">Hvis du bruger Teams-skrivebordsapp, [skal du sørge for, at appen er helt opdateret](https://support.office.com/article/Update-Microsoft-Teams-535a8e4b-45f0-4f6c-8b3d-91bca7a51db1).</span><span class="sxs-lookup"><span data-stu-id="1ef5b-104">If you are using the Teams desktop app, [make sure the app is fully updated](https://support.office.com/article/Update-Microsoft-Teams-535a8e4b-45f0-4f6c-8b3d-91bca7a51db1).</span></span>

- <span data-ttu-id="1ef5b-105">Sørg for, at alle [URL-adresser og adresseintervaller for Microsoft 365](https://docs.microsoft.com/microsoftteams/connectivity-issues) er tilgængelige.</span><span class="sxs-lookup"><span data-stu-id="1ef5b-105">Make sure all the [Microsoft 365 URLs and address ranges](https://docs.microsoft.com/microsoftteams/connectivity-issues) are accessible.</span></span>

- <span data-ttu-id="1ef5b-106">Log på med din lejeradministratorkonto, og kontrollér dit Dashboard for [tjenestetilstand](https://docs.microsoft.com/office365/enterprise/view-service-health) for at bekræfte, at der ikke er nogen forringelse af tjenesten eller strømsvigt.</span><span class="sxs-lookup"><span data-stu-id="1ef5b-106">Log in with your tenant admin account and check your [Service Health Dashboard](https://docs.microsoft.com/office365/enterprise/view-service-health) to verify that no outage or service degradation exists.</span></span>

- <span data-ttu-id="1ef5b-107">Fjern og geninstaller Teams-programmet (link)</span><span class="sxs-lookup"><span data-stu-id="1ef5b-107">Uninstall and reinstall the Teams Application (link)</span></span>
    - <span data-ttu-id="1ef5b-108">Gå til mappen %appdata%\Microsoft\teams\ på computeren, og slet alle filer i mappen.</span><span class="sxs-lookup"><span data-stu-id="1ef5b-108">Browse to the %appdata%\Microsoft\teams\ folder on your computer and delete all files in that directory.</span></span>
    - <span data-ttu-id="1ef5b-109">[Download og installér Teams-appen](https://www.microsoft.com/microsoft-365/microsoft-teams/group-chat-software#office-DesktopAppDownload-ofoushy), og hvis det er muligt, skal du installere Teams som administrator (højreklik på Teams-installationsprogrammet, og vælg "Kør som administrator", hvis det er tilgængeligt).</span><span class="sxs-lookup"><span data-stu-id="1ef5b-109">[Download and install the Teams App](https://www.microsoft.com/microsoft-365/microsoft-teams/group-chat-software#office-DesktopAppDownload-ofoushy), and if possible, install Teams as an administrator (right click the Teams installer and select "Run as administrator" if available).</span></span>

<span data-ttu-id="1ef5b-110">Hvis din Teams-klient stadig går ned, kan du så genskabe problemet?</span><span class="sxs-lookup"><span data-stu-id="1ef5b-110">If your Teams client is still crashing, can you reproduce the issue?</span></span> <span data-ttu-id="1ef5b-111">Hvis det er sådan:</span><span class="sxs-lookup"><span data-stu-id="1ef5b-111">If so:</span></span>

1. <span data-ttu-id="1ef5b-112">Brug Trinoptager til at registrere dine trin.</span><span class="sxs-lookup"><span data-stu-id="1ef5b-112">Use the Steps Recorder to capture your steps.</span></span>
    - <span data-ttu-id="1ef5b-113">Luk ALLE unødvendige eller fortrolige programmer.</span><span class="sxs-lookup"><span data-stu-id="1ef5b-113">Close ALL unnecessary or confidential applications.</span></span>
    - <span data-ttu-id="1ef5b-114">Start Trinoptager, og genskab problemet, mens du er logget på med den pågældende brugerkonto.</span><span class="sxs-lookup"><span data-stu-id="1ef5b-114">Launch the Steps Recorder and reproduce the issue while logged in with the affected user account.</span></span>
    - <span data-ttu-id="1ef5b-115">[Indsaml de teamlogfiler, der registrerer de registrerede genpropro trin](https://docs.microsoft.com/microsoftteams/log-files).</span><span class="sxs-lookup"><span data-stu-id="1ef5b-115">[Collect the teams logs that capture the recorded repro steps](https://docs.microsoft.com/microsoftteams/log-files).</span></span> <span data-ttu-id="1ef5b-116">**Bemærk!** Sørg for at registrere logonadressen på den pådrede bruger.</span><span class="sxs-lookup"><span data-stu-id="1ef5b-116">**Note**: Make sure you capture the sign-in address of the impacted user.</span></span>
    - <span data-ttu-id="1ef5b-117">Indsaml oplysninger om dumpet og/eller Bucket (Windows).</span><span class="sxs-lookup"><span data-stu-id="1ef5b-117">Collect the dump and/or Fault bucket info (Windows).</span></span> <span data-ttu-id="1ef5b-118">Start Windows Powershell på den computer, hvor nedbruddet sker, og kør følgende kommandoer:</span><span class="sxs-lookup"><span data-stu-id="1ef5b-118">Launch Windows Powershell on the machine where the crash is occurring and run the following commands:</span></span>

        `
        PS C:\Users\user01> cd $env:temp
        PS C:\Users\user01\AppData\Local\Temp> Get-EventLog -LogName Application -Message "*Teams.exe*" -InstanceId 1001 | Select-Object -First 10 | Format-List > FaultBuckets.txt
        PS C:\Users\user01\AppData\Local\Temp> notepad .\FaultBuckets.txt
        `
    
2. <span data-ttu-id="1ef5b-119">Vedhæft filen til din supportsag.</span><span class="sxs-lookup"><span data-stu-id="1ef5b-119">Attach the file to your support case.</span></span>
