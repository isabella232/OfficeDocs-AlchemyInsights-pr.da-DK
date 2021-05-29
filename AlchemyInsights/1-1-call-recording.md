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
ms.openlocfilehash: 8cdadf34a059856338d7f40528446b70373465e4
ms.sourcegitcommit: d2108b13acc44e26b65f9a2739cbce9bf98959a5
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 05/28/2021
ms.locfileid: "52702084"
---
# <a name="11-call-recording"></a><span data-ttu-id="c67ba-102">1:1 opkaldsoptagelse</span><span class="sxs-lookup"><span data-stu-id="c67ba-102">1:1 call recording</span></span>

<span data-ttu-id="c67ba-103">Hvis knappen **Start optagelse** er nedtonet i et 1:1-opkald, skal du ændre politikindstillingerne for den påvirkede bruger.</span><span class="sxs-lookup"><span data-stu-id="c67ba-103">If the **Start Recording** button is grayed out in a 1:1 call, you need to change the policy settings for the impacted user.</span></span> <span data-ttu-id="c67ba-104">Hvis du vil kontrollere politikindstillingen, skal du køre Diagnosticering for den påvirkede bruger ved at skrive **Diag: Teams 1:1 opkaldsoptagelse** ovenfor.</span><span class="sxs-lookup"><span data-stu-id="c67ba-104">To check the policy setting, run the Diagnostic for the impacted user by typing **Diag: Teams 1:1 Call Recording** above.</span></span>     

<span data-ttu-id="c67ba-105">Fra og med den 31. maj 2021 begynder vi at håndhæve en ny Teams-opkaldspolitik *AllowCloudRecordingForCalls*.</span><span class="sxs-lookup"><span data-stu-id="c67ba-105">Beginning May 31, 2021, we'll start enforcing a new Teams Calling Policy *AllowCloudRecordingForCalls*.</span></span> <span data-ttu-id="c67ba-106">Før denne ændring styres 1:1-opkaldsoptagelse af *politikken AllowCloudRecording* Teams Meeting Policy.</span><span class="sxs-lookup"><span data-stu-id="c67ba-106">Prior to this change, 1:1 call recording is controlled by the *AllowCloudRecording* Teams Meeting Policy.</span></span> <span data-ttu-id="c67ba-107">Denne ændring er dokumenteret i indlægget i Meddelelsescenter: [(Opdateret) 1:1 Introduktion til](https://portal.microsoft.com/Adminportal/Home?ref=MessageCenter/:/messages/MC238796)optagelsespolitik for opkald.</span><span class="sxs-lookup"><span data-stu-id="c67ba-107">This change is documented in the Message Center post: [(Updated) 1:1 Call recording policy introduction](https://portal.microsoft.com/Adminportal/Home?ref=MessageCenter/:/messages/MC238796).</span></span>  

<span data-ttu-id="c67ba-108">*AllowCloudRecordingForCalls*   opkaldspolitik er indstillet til **$False** som standard.</span><span class="sxs-lookup"><span data-stu-id="c67ba-108">*AllowCloudRecordingForCalls* calling policy option is set to **$False** by default.</span></span> <span data-ttu-id="c67ba-109">Hvis du foretrækker at blokere alle brugere fra at optage 1:1-opkald, behøver du ikke at foretage dig noget.</span><span class="sxs-lookup"><span data-stu-id="c67ba-109">If you prefer to block all users from recording 1:1 calls, you don't need to take any action.</span></span>  

<span data-ttu-id="c67ba-110">For at aktivere opkaldsoptagelse for alle brugere i 1:1-opkald [skal Teams PowerShell](/microsoftteams/teams-powershell-install) til at køre følgende cmdlet:</span><span class="sxs-lookup"><span data-stu-id="c67ba-110">To enable call recording for all users in 1:1 calls use [Teams PowerShell](/microsoftteams/teams-powershell-install) to run the following cmdlet:</span></span> 

<span data-ttu-id="c67ba-111">**Set-CsTeamsCallingPolicy -Identity Global -AllowCloudRecordingForCalls $True**</span><span class="sxs-lookup"><span data-stu-id="c67ba-111">**Set-CsTeamsCallingPolicy -Identity Global -AllowCloudRecordingForCalls $True**</span></span> 

<span data-ttu-id="c67ba-112">Alternativt kan du oprette en ny politik og indstille **AllowCloudRecordingForCalls** **til at $true** og tildele denne politik til dine brugere.</span><span class="sxs-lookup"><span data-stu-id="c67ba-112">Alternatively, you can create a new policy and set **-AllowCloudRecordingForCalls** to **$true** and assign that policy to your users.</span></span> 

<span data-ttu-id="c67ba-113">Du kan få mere at vide [under 1:1 Politikkontrolelementer for opkaldsoptagelse er (næsten!) Her](https://techcommunity.microsoft.com/t5/microsoft-teams-support/1-1-call-recording-policy-controls-are-almost-here/ba-p/2217668).</span><span class="sxs-lookup"><span data-stu-id="c67ba-113">For more information, see [1:1 Call Recording Policy Controls Are (Almost!) Here](https://techcommunity.microsoft.com/t5/microsoft-teams-support/1-1-call-recording-policy-controls-are-almost-here/ba-p/2217668).</span></span>
