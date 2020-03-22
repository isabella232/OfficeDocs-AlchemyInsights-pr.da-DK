---
title: Der kan ikke få adgang til offentlige mapper
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
ms.openlocfilehash: a579b89b68bfb8432adfe64b155803eda2c3b086
ms.sourcegitcommit: a3b42ee05224846327d353b48a8c67dab724f6eb
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 03/21/2020
ms.locfileid: "42891743"
---
# <a name="outlook-cannot-connect-to-public-folders"></a><span data-ttu-id="a69b5-102">Outlook kan ikke oprette forbindelse til offentlige mapper</span><span class="sxs-lookup"><span data-stu-id="a69b5-102">Outlook cannot connect to public folders</span></span>

<span data-ttu-id="a69b5-103">Hvis adgang til offentlige mapper ikke fungerer for nogle brugere, kan du prøve følgende:</span><span class="sxs-lookup"><span data-stu-id="a69b5-103">If public folder access isn't working for some users, try the following:</span></span>

<span data-ttu-id="a69b5-104">Opret forbindelse til EXO PowerShell, og konfigurer parameteren DefaultPublicFolderMailbox på problembrugerkontoen, så den svarer til parameteren på en fungerende brugerkonto.</span><span class="sxs-lookup"><span data-stu-id="a69b5-104">Connect to EXO PowerShell and configure the DefaultPublicFolderMailbox parameter on the problem user account to match the parameter on a working user account.</span></span>

<span data-ttu-id="a69b5-105">Eksempel:</span><span class="sxs-lookup"><span data-stu-id="a69b5-105">Example:</span></span>

<span data-ttu-id="a69b5-106">Arbejdsbruger til hent postkasse | ft DefaultPublicFolderMailbox,EffektivPublicFolderMailbox</span><span class="sxs-lookup"><span data-stu-id="a69b5-106">Get-Mailbox WorkingUser | ft DefaultPublicFolderMailbox,EffectivePublicFolderMailbox</span></span>

<span data-ttu-id="a69b5-107">Set-Mailbox ProblemBruger -DefaultPublicFolderMailbox-værdi \<fra tidligere kommando></span><span class="sxs-lookup"><span data-stu-id="a69b5-107">Set-Mailbox ProblemUser -DefaultPublicFolderMailbox \<value from previous command></span></span>

<span data-ttu-id="a69b5-108">Vent mindst en time, før ændringen træder i kraft.</span><span class="sxs-lookup"><span data-stu-id="a69b5-108">Wait at least one hour for the change to take effect.</span></span>

<span data-ttu-id="a69b5-109">Hvis problemet stadig er, skal du følge [denne fremgangsmåde](https://aka.ms/pfcte) for at foretage fejlfinding af problemer med adgang til offentlige mapper ved hjælp af Outlook.</span><span class="sxs-lookup"><span data-stu-id="a69b5-109">If the issue remains, please follow [this procedure](https://aka.ms/pfcte) to troubleshoot public folder access issues using Outlook.</span></span>