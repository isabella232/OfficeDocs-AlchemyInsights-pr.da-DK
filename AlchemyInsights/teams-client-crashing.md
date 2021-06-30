---
title: Teams klient går ned
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
ms.openlocfilehash: 7acb2f5f87a9cfbd67cd94efca696665fd80fc4a
ms.sourcegitcommit: 3cdfde87b7311c200431196031af92c640fd0d8d
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 06/29/2021
ms.locfileid: "53187715"
---
# <a name="teams-client-crashing"></a><span data-ttu-id="0a62b-102">Teams klient går ned</span><span class="sxs-lookup"><span data-stu-id="0a62b-102">Teams client crashing</span></span>

<span data-ttu-id="0a62b-103">Hvis din Teams-klient går ned, kan du prøve følgende:</span><span class="sxs-lookup"><span data-stu-id="0a62b-103">If your Teams client is crashing, try the following:</span></span>

- <span data-ttu-id="0a62b-104">Hvis du bruger Teams-skrivebordsapp, [skal du sørge for, at appen er helt opdateret](https://support.office.com/article/Update-Microsoft-Teams-535a8e4b-45f0-4f6c-8b3d-91bca7a51db1).</span><span class="sxs-lookup"><span data-stu-id="0a62b-104">If you are using the Teams desktop app, [make sure the app is fully updated](https://support.office.com/article/Update-Microsoft-Teams-535a8e4b-45f0-4f6c-8b3d-91bca7a51db1).</span></span>

- <span data-ttu-id="0a62b-105">Sørg for, at [alle Microsoft 365 og adresseintervaller er](/microsoftteams/connectivity-issues) tilgængelige.</span><span class="sxs-lookup"><span data-stu-id="0a62b-105">Make sure all the [Microsoft 365 URLs and address ranges](/microsoftteams/connectivity-issues) are accessible.</span></span>

- <span data-ttu-id="0a62b-106">Log på med din lejeradministratorkonto, og kontrollér dit Dashboard for [tjenestetilstand](/office365/enterprise/view-service-health) for at bekræfte, at der ikke er nogen forringelse af tjenesten eller strømsvigt.</span><span class="sxs-lookup"><span data-stu-id="0a62b-106">Log in with your tenant admin account and check your [Service Health Dashboard](/office365/enterprise/view-service-health) to verify that no outage or service degradation exists.</span></span>

- <span data-ttu-id="0a62b-107">Fjern og geninstaller Teams programmet</span><span class="sxs-lookup"><span data-stu-id="0a62b-107">Uninstall and reinstall the Teams Application</span></span>
    - <span data-ttu-id="0a62b-108">Gå til mappen %appdata%\Microsoft\Teams\ på computeren, og slet alle filer i mappen.</span><span class="sxs-lookup"><span data-stu-id="0a62b-108">Browse to the %appdata%\Microsoft\Teams\ folder on your computer and delete all files in that directory.</span></span>
    - <span data-ttu-id="0a62b-109">[Download og installér Teams-appen](https://www.microsoft.com/microsoft-teams/download-app), og hvis det er muligt, skal du installere Teams som administrator (højreklik på installationsprogrammet til Teams, og vælg Kør som **administrator,** hvis det er tilgængeligt).</span><span class="sxs-lookup"><span data-stu-id="0a62b-109">[Download and install the Teams App](https://www.microsoft.com/microsoft-teams/download-app), and if possible, install Teams as an administrator (right-click the Teams installer, and select **Run as administrator** if available).</span></span>

<span data-ttu-id="0a62b-110">Hvis klienten Teams, der stadig går ned, kan du prøve at genskabe problemet.</span><span class="sxs-lookup"><span data-stu-id="0a62b-110">If your Teams client is still crashing, try to reproduce the issue.</span></span> <span data-ttu-id="0a62b-111">Hvis du kan:</span><span class="sxs-lookup"><span data-stu-id="0a62b-111">If you can:</span></span>

1. <span data-ttu-id="0a62b-112">Brug Trinoptager til at registrere dine trin.</span><span class="sxs-lookup"><span data-stu-id="0a62b-112">Use the Steps Recorder to capture your steps.</span></span>
    - <span data-ttu-id="0a62b-113">Luk ALLE unødvendige eller fortrolige programmer.</span><span class="sxs-lookup"><span data-stu-id="0a62b-113">Close ALL unnecessary or confidential applications.</span></span>
    - <span data-ttu-id="0a62b-114">Start Trinoptager, og genskab problemet, mens du er logget på med den pågældende brugerkonto.</span><span class="sxs-lookup"><span data-stu-id="0a62b-114">Launch the Steps Recorder and reproduce the issue while logged in with the affected user account.</span></span>
    - <span data-ttu-id="0a62b-115">[Indsaml de teamlogfiler, der registrerer de registrerede genpropro trin](/microsoftteams/log-files).</span><span class="sxs-lookup"><span data-stu-id="0a62b-115">[Collect the teams logs that capture the recorded repro steps](/microsoftteams/log-files).</span></span> <span data-ttu-id="0a62b-116">**Bemærk!** Sørg for at registrere logonadressen på den pådrede bruger.</span><span class="sxs-lookup"><span data-stu-id="0a62b-116">**Note**: Make sure you capture the sign-in address of the impacted user.</span></span>
    - <span data-ttu-id="0a62b-117">Indsaml oplysninger om dump og/eller fejl bucket (Windows).</span><span class="sxs-lookup"><span data-stu-id="0a62b-117">Collect the dump and/or Fault bucket info (Windows).</span></span> <span data-ttu-id="0a62b-118">Start Windows Powershell på den computer, hvor nedbruddet sker, og kør følgende kommandoer (tryk på Enter efter hver kommando):</span><span class="sxs-lookup"><span data-stu-id="0a62b-118">Launch Windows Powershell on the machine where the crash is occurring and run the following commands (after each command, press Enter):</span></span>

    <span data-ttu-id="0a62b-119">`cd $env:temp` `Get-EventLog -LogName Application -Message "*Teams.exe*" -InstanceId 1001 | Select-Object -First 10 | Format-List > FaultBuckets.txt`</span><span class="sxs-lookup"><span data-stu-id="0a62b-119">`cd $env:temp` `Get-EventLog -LogName Application -Message "*Teams.exe*" -InstanceId 1001 | Select-Object -First 10 | Format-List > FaultBuckets.txt`</span></span>
    `notepad .\FaultBuckets.txt`
    
2. <span data-ttu-id="0a62b-120">Når tekstfilen er oprettet og vises på skærmen, skal du gemme filen og vedhæfte den til serviceanmodningen.</span><span class="sxs-lookup"><span data-stu-id="0a62b-120">After the text file is generated and appears on your screen, save the file and attach it to the service request.</span></span> 
