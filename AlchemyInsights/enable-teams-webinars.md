---
title: Aktivere Teams webinarer
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
- "11513"
- "9006672"
ms.openlocfilehash: 5a732e6746e9fd23e54a0b2ffeabb59623012a0e
ms.sourcegitcommit: 9de78b30602f917d58705057cdcce31fec349969
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 06/04/2021
ms.locfileid: "52793581"
---
# <a name="enable-teams-webinars"></a><span data-ttu-id="ab877-102">Aktivere Teams webinarer</span><span class="sxs-lookup"><span data-stu-id="ab877-102">Enable Teams Webinars</span></span>

<span data-ttu-id="ab877-103">Webinarer er aktiveret som standard.</span><span class="sxs-lookup"><span data-stu-id="ab877-103">Webinars are enabled by default.</span></span> <span data-ttu-id="ab877-104">Du kan styre, hvem der kan planlægge og tilmelde dig Teams webinarer ved hjælp Teams PowerShell-kommandoer.</span><span class="sxs-lookup"><span data-stu-id="ab877-104">You can manage who can schedule and register for Teams Webinars by using Teams PowerShell commands.</span></span>

- <span data-ttu-id="ab877-105">Alle brugere, der kan oprette et møde, kan også oprette et webinarmøde.</span><span class="sxs-lookup"><span data-stu-id="ab877-105">All users who can create a meeting can also create a webinar meeting.</span></span> <span data-ttu-id="ab877-106">Hvis du vil administrere, hvem der kan planlægge Teams webinarer, skal du *bruge AllowMeetingRegistration*.</span><span class="sxs-lookup"><span data-stu-id="ab877-106">If you want to manage who can schedule Teams Webinars, use *AllowMeetingRegistration*.</span></span> 
- <span data-ttu-id="ab877-107">*WhoCanRegister er som standard* aktiveret og indstillet til **Alle**.</span><span class="sxs-lookup"><span data-stu-id="ab877-107">By default, *WhoCanRegister* is enabled and set to **Everyone**.</span></span> <span data-ttu-id="ab877-108">Hvis du vil deaktivere møderegistrering, skal du *angive AllowMeetingRegistration* til **False**.</span><span class="sxs-lookup"><span data-stu-id="ab877-108">If you want to turn off meeting registration, set *AllowMeetingRegistration* to **False**.</span></span>

<span data-ttu-id="ab877-109">Hvis du vil ændre disse indstillinger, skal du [installere Teams PowerShell.](/microsoftteams/teams-powershell-install)</span><span class="sxs-lookup"><span data-stu-id="ab877-109">To change these settings, you must install [Teams PowerShell](/microsoftteams/teams-powershell-install).</span></span> <span data-ttu-id="ab877-110">Desuden håndhæves mødepolitikker i Teams webinarer.</span><span class="sxs-lookup"><span data-stu-id="ab877-110">Also, Meeting Policies are enforced on Teams Webinars.</span></span> <span data-ttu-id="ab877-111">Hvis anonym deltagelse f.eks. er slået fra i mødeindstillinger, kan anonyme brugere ikke deltage i webinarer.</span><span class="sxs-lookup"><span data-stu-id="ab877-111">For example, if anonymous join is turned off in meeting settings, anonymous users can't join webinars.</span></span>

<span data-ttu-id="ab877-112">Hvis du vil have mere at vide om, hvem der kan tilmelde sig webinarer, skal [du se Konfigurer, hvem der kan tilmelde sig webinarer.](/microsoftteams/set-up-webinars?source=docs#configure-who-can-register-for-webinars)</span><span class="sxs-lookup"><span data-stu-id="ab877-112">To learn more about configuring who can register for webinars, see [Configure who can register for webinars](/microsoftteams/set-up-webinars?source=docs#configure-who-can-register-for-webinars).</span></span> <span data-ttu-id="ab877-113">Hvis du vil have mere at vide om indstillinger for Microsoft-lister, skal [du se Kontrolindstillinger for Microsoft-lister](/sharepoint/control-lists).</span><span class="sxs-lookup"><span data-stu-id="ab877-113">For more information about settings for Microsoft Lists, see [Control settings for Microsoft Lists](/sharepoint/control-lists).</span></span>