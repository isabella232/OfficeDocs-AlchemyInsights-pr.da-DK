---
title: 1:1 opkaldsoptagelse
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 12/18/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9002530"
- "7648"
ms.openlocfilehash: af09e8805409446a42a62c82aa577ad27f09a17a
ms.sourcegitcommit: 6312ee31561db36104f32282d019d069ede69174
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 03/11/2021
ms.locfileid: "50733843"
---
# <a name="11-call-recording"></a><span data-ttu-id="74435-102">1:1 opkaldsoptagelse</span><span class="sxs-lookup"><span data-stu-id="74435-102">1:1 call recording</span></span>

<span data-ttu-id="74435-103">Administratorer skal handle nu for at fortsætte med at tillade brugere at optage 1:1-opkald.</span><span class="sxs-lookup"><span data-stu-id="74435-103">Administrators need to take action now to continue allowing users to Record 1:1 calls.</span></span>
 
<span data-ttu-id="74435-104">Fra og med 12. april 2021 begynder vi at håndhæve en ny indstilling for Teams-opkaldspolitik *AllowCloudRecordingForCalls.*</span><span class="sxs-lookup"><span data-stu-id="74435-104">Beginning April 12, 2021, we will start enforcing a new Teams Calling Policy option *AllowCloudRecordingForCalls*.</span></span> 

<span data-ttu-id="74435-105">I øjeblikket styres 1:1-opkaldsoptagelsesfunktionerne af *indstillingen AllowCloudRecording* i Teams-mødepolitikker.</span><span class="sxs-lookup"><span data-stu-id="74435-105">Currently 1:1 call recording capabilities are controlled by the *AllowCloudRecording* option in Teams Meeting Policies.</span></span> <span data-ttu-id="74435-106">Hvis dine brugere har tilladelse til at optage Teams-møder, kan de også optage 1:1-opkald.</span><span class="sxs-lookup"><span data-stu-id="74435-106">If your users are allowed to record Teams Meetings they can also record 1:1 calls.</span></span>

<span data-ttu-id="74435-107">Hvis du foretrækker at blokere alle brugere fra at optage 1:1-opkald, behøver du ikke at foretage dig noget.</span><span class="sxs-lookup"><span data-stu-id="74435-107">If you prefer to block all users from recording 1:1 calls, you do not need to take any action.</span></span> <span data-ttu-id="74435-108">*Indstillingen AllowCloudRecordingForCalls-opkaldspolitik* ændres $False som standard.</span><span class="sxs-lookup"><span data-stu-id="74435-108">*AllowCloudRecordingForCalls* calling policy option will be $False by default.</span></span>

<span data-ttu-id="74435-109">Denne ændring er dokumenteret i følgende indlæg i Meddelelsescenter: [(Opdateret) 1:1](https://portal.microsoft.com/Adminportal/Home?ref=MessageCenter/:/messages/MC238796) Introduktion til politik for optagelse af opkald For at konfigurere politikindstillingen for Teams-opkaldspolitik skal du bruge [Teams PowerShell.](https://docs.microsoft.com/microsoftteams/teams-powershell-install)</span><span class="sxs-lookup"><span data-stu-id="74435-109">This change is documented in the following Message Center Post: [(Updated) 1:1 Call recording policy introduction](https://portal.microsoft.com/Adminportal/Home?ref=MessageCenter/:/messages/MC238796) To set the Teams Calling Policy Option you must use [Teams PowerShell](https://docs.microsoft.com/microsoftteams/teams-powershell-install).</span></span>

<span data-ttu-id="74435-110">**Sådan aktiverer du opkaldsoptagelse i 1:1-opkald:** Set-CsTeamsCallingPolicy -Identity Global -AllowCloudRecordingForCalls $True</span><span class="sxs-lookup"><span data-stu-id="74435-110">**To enable call recording in 1:1 calls:** Set-CsTeamsCallingPolicy -Identity Global -AllowCloudRecordingForCalls $True</span></span>

<span data-ttu-id="74435-111">**Sådan deaktiverer du opkaldsoptagelse i 1:1-opkald:** Set-CsTeamsCallingPolicy -Identity Global -AllowCloudRecordingForCalls $False</span><span class="sxs-lookup"><span data-stu-id="74435-111">**To disable call recording in 1:1 calls:** Set-CsTeamsCallingPolicy -Identity Global -AllowCloudRecordingForCalls $False</span></span>

