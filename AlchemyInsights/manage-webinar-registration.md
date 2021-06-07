---
title: Administrere registrering af webinarer
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 06/02/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "11512"
- "9006672"
ms.openlocfilehash: c5b0721d286b07d7e0f84199885b6f527a2b42a2
ms.sourcegitcommit: f7a9e97d04b7b6cbb633b32094d40f1874bf0fce
ms.translationtype: HT
ms.contentlocale: da-DK
ms.lasthandoff: 06/06/2021
ms.locfileid: "52793706"
---
# <a name="manage-webinar-registration"></a><span data-ttu-id="1c607-102">Administrere registrering af webinarer</span><span class="sxs-lookup"><span data-stu-id="1c607-102">Manage webinar registration</span></span>

<span data-ttu-id="1c607-103">Du styrer, hvem der kan tilmelde dig Teams webinarer ved hjælp Teams Powershell-kommandoer.</span><span class="sxs-lookup"><span data-stu-id="1c607-103">You manage who can register for Teams Webinars by using Teams Powershell commands.</span></span> <span data-ttu-id="1c607-104">Hvis du vil Teams Powershell, skal [du se Teams PowerShell.](/microsoftteams/teams-powershell-install)</span><span class="sxs-lookup"><span data-stu-id="1c607-104">To install Teams Powershell, see [Teams PowerShell](/microsoftteams/teams-powershell-install).</span></span> 

<span data-ttu-id="1c607-105">*WhoCanRegister er som standard* aktiveret og indstillet til **EveryoneInCompany.**</span><span class="sxs-lookup"><span data-stu-id="1c607-105">By default, *WhoCanRegister* is enabled and set to **EveryoneInCompany**.</span></span> <span data-ttu-id="1c607-106">Hvis du vil tillade, at alle, herunder anonyme brugere, kan tilmelde sig, skal du angive mødepolitikken **til Alle** ved hjælp af kommandoen Powershell:</span><span class="sxs-lookup"><span data-stu-id="1c607-106">To allow anyone, including anonymous users, to register, you must set the Meeting Policy to **Everyone** by using the Powershell command:</span></span>

`Set-CsTeamsMeetingPolicy -WhoCanRegister Everyone`

<span data-ttu-id="1c607-107">**Bemærk!** Hvis anonym deltagelse er slået fra i mødeindstillinger, kan anonyme brugere ikke deltage i webinarer.</span><span class="sxs-lookup"><span data-stu-id="1c607-107">**Note**: If anonymous join is turned off in meeting settings, anonymous users can't join webinars.</span></span> <span data-ttu-id="1c607-108">Du kan få mere at vide og aktivere denne indstilling [under Administrer mødeindstillinger i Microsoft Teams](/microsoftteams/meeting-settings-in-teams).</span><span class="sxs-lookup"><span data-stu-id="1c607-108">To learn more and enable this setting, see [Manage meeting settings in Microsoft Teams](/microsoftteams/meeting-settings-in-teams).</span></span>

<span data-ttu-id="1c607-109">Hvis du vil deaktivere møderegistrering, skal du *angive AllowMeetingRegistration* til **False**.</span><span class="sxs-lookup"><span data-stu-id="1c607-109">If you want to turn off meeting registration, set *AllowMeetingRegistration* to **False**.</span></span>

<span data-ttu-id="1c607-110">Hvis du vil have mere at vide om, hvem der kan tilmelde sig webinarer, skal [du se Konfigurer, hvem der kan tilmelde sig webinarer.](/microsoftteams/set-up-webinars?source=docs#configure-who-can-register-for-webinars)</span><span class="sxs-lookup"><span data-stu-id="1c607-110">To learn more about configuring who can register for webinars, see [Configure who can register for webinars](/microsoftteams/set-up-webinars?source=docs#configure-who-can-register-for-webinars).</span></span> <span data-ttu-id="1c607-111">Hvis du vil have mere at vide om indstillinger for Microsoft-lister, skal [du se Kontrolindstillinger for Microsoft-lister](/sharepoint/control-lists).</span><span class="sxs-lookup"><span data-stu-id="1c607-111">For more information about settings for Microsoft Lists, see [Control settings for Microsoft Lists](/sharepoint/control-lists).</span></span>
