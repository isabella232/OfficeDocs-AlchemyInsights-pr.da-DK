---
title: Ejeren kan ikke oprette en undermappe ved hjælp af Outlook
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "5884"
- "3500007"
ms.openlocfilehash: 9590f780cffeaf644733752c763e04d748b1b39e
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 09/14/2020
ms.locfileid: "47665712"
---
# <a name="owner-cannot-create-sub-folder-using-outlook"></a><span data-ttu-id="eed33-102">Ejeren kan ikke oprette en undermappe ved hjælp af Outlook</span><span class="sxs-lookup"><span data-stu-id="eed33-102">Owner cannot create sub-folder using Outlook</span></span>

<span data-ttu-id="eed33-103">**Der er et vedvarende problem med ejere af offentlige mapper, som opretter undermapper ved hjælp af Outlook. Problemet kan snart rettes.**</span><span class="sxs-lookup"><span data-stu-id="eed33-103">**There's an ongoing issue with public folder owners creating subfolders using Outlook. The issue will be fixed soon.**</span></span>

<span data-ttu-id="eed33-104">I mellemtiden kan du bruge en af følgende løsninger:</span><span class="sxs-lookup"><span data-stu-id="eed33-104">Meanwhile, use one of the following workarounds:</span></span>

1. <span data-ttu-id="eed33-105">Brug Outlook til MAC til at oprette under mappen som et problem påvirker kun Outlook til stationære Windows (alle versioner)</span><span class="sxs-lookup"><span data-stu-id="eed33-105">Use Outlook for MAC to create the subfolder as the issue impacts only Outlook for desktop windows (all versions)</span></span>
2. <span data-ttu-id="eed33-106">Få administratoren til at oprette under mappen ved hjælp af EXO shell eller EAC</span><span class="sxs-lookup"><span data-stu-id="eed33-106">Have admin create the subfolder using EXO Shell or EAC</span></span>
3. <span data-ttu-id="eed33-107">Ændre DefaultPublicFolderMailbox/EffectivePublicFolderMailbox på brugeren til en anden postkasse end indholds postkassen for mappen årsag til problemet</span><span class="sxs-lookup"><span data-stu-id="eed33-107">Change the DefaultPublicFolderMailbox/EffectivePublicFolderMailbox on the user to other mailbox than the Content Mailbox for the folder causing issue</span></span>  
    - <span data-ttu-id="eed33-108">*Set-postkasse User1 DefaultPublicFolderMailbox PubMBX3*</span><span class="sxs-lookup"><span data-stu-id="eed33-108">*Set-Mailbox User1 DefaultPublicFolderMailbox PubMBX3*</span></span>
4. <span data-ttu-id="eed33-109">Vent en time, Genstart Outlook-klient</span><span class="sxs-lookup"><span data-stu-id="eed33-109">Wait for an hour, restart outlook client</span></span>