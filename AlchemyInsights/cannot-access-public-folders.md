---
title: Kan ikke få adgang til offentlige mapper
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3500007"
- "3462"
ms.openlocfilehash: a9305b175e1ca0b992c014a73705447d67e037bc
ms.sourcegitcommit: cbbd46fa9a32873c5446d9fd5a532cea0300b795
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 12/10/2019
ms.locfileid: "39959489"
---
# <a name="outlook-cannot-connect-to-public-folders"></a><span data-ttu-id="85c3a-102">Outlook kan ikke oprette forbindelse til offentlige mapper</span><span class="sxs-lookup"><span data-stu-id="85c3a-102">Outlook cannot connect to public folders</span></span>

<span data-ttu-id="85c3a-103">Hvis adgang til offentlige mapper ikke fungerer for få brugere, kan du prøve følgende:</span><span class="sxs-lookup"><span data-stu-id="85c3a-103">If public folder access isn't working for few users, try the following:</span></span>

<span data-ttu-id="85c3a-104">Opret forbindelse til EXO PowerShell, og Konfigurer DefaultPublicFolderMailbox på den problematiske brugerkonto, så den svarer til en på en fungerende brugerkonto.</span><span class="sxs-lookup"><span data-stu-id="85c3a-104">Connect to EXO PowerShell, and configure the DefaultPublicFolderMailbox on the problem user account to match one on a working user account.</span></span>

<span data-ttu-id="85c3a-105">Eksempel:</span><span class="sxs-lookup"><span data-stu-id="85c3a-105">Example:</span></span>

<span data-ttu-id="85c3a-106">Hent-postkasse WorkingUser | ft DefaultPublicFolderMailbox, Effekvepublicfoldermailbox</span><span class="sxs-lookup"><span data-stu-id="85c3a-106">Get-Mailbox WorkingUser | ft DefaultPublicFolderMailbox,EffectivePublicFolderMailbox</span></span>

<span data-ttu-id="85c3a-107">Set-postkasse Problembruger-DefaultPublicFolderMailbox \<Value fra forrige kommando></span><span class="sxs-lookup"><span data-stu-id="85c3a-107">Set-Mailbox ProblemUser -DefaultPublicFolderMailbox \<value from previous command></span></span>

<span data-ttu-id="85c3a-108">Vent mindst en time, indtil ændringen træder i kraft.</span><span class="sxs-lookup"><span data-stu-id="85c3a-108">Wait at least one hour for the change to take effect.</span></span>