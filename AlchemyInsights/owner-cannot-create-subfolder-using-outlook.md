---
title: Ejeren kan ikke oprette en undermappe ved hjælp af Outlook
ms.author: pebaum
author: pebaum
manager: scotv
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
ms.openlocfilehash: b2ab7b60bc521fd28d68333bb963528f7b9e05f2
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 04/15/2021
ms.locfileid: "51836129"
---
# <a name="owner-cannot-create-sub-folder-using-outlook"></a><span data-ttu-id="43d46-102">Ejeren kan ikke oprette en undermappe ved hjælp af Outlook</span><span class="sxs-lookup"><span data-stu-id="43d46-102">Owner cannot create sub-folder using Outlook</span></span>

<span data-ttu-id="43d46-103">**Der er i øjeblikket et problem med ejere af offentlige mapper, der opretter undermapper ved hjælp af Outlook. Problemet vil snart blive rettet.**</span><span class="sxs-lookup"><span data-stu-id="43d46-103">**There's an ongoing issue with public folder owners creating subfolders using Outlook. The issue will be fixed soon.**</span></span>

<span data-ttu-id="43d46-104">I mellemtiden kan du bruge en af følgende løsninger:</span><span class="sxs-lookup"><span data-stu-id="43d46-104">Meanwhile, use one of the following workarounds:</span></span>

1. <span data-ttu-id="43d46-105">Brug Outlook til MAC til at oprette undermappen, da problemet kun påvirker Outlook til skrivebordsvinduer (alle versioner)</span><span class="sxs-lookup"><span data-stu-id="43d46-105">Use Outlook for MAC to create the subfolder as the issue impacts only Outlook for desktop windows (all versions)</span></span>
2. <span data-ttu-id="43d46-106">Få administratoren til at oprette undermappen ved hjælp af EXO Shell eller EAC</span><span class="sxs-lookup"><span data-stu-id="43d46-106">Have admin create the subfolder using EXO Shell or EAC</span></span>
3. <span data-ttu-id="43d46-107">Skift DefaultPublicFolderMailbox/EffectivePublicFolderMailbox på brugeren til en anden postkasse end indholdspostkassen for mappen, der forårsager problemer</span><span class="sxs-lookup"><span data-stu-id="43d46-107">Change the DefaultPublicFolderMailbox/EffectivePublicFolderMailbox on the user to other mailbox than the Content Mailbox for the folder causing issue</span></span>  
    - <span data-ttu-id="43d46-108">*Set-Mailbox User1 DefaultPublicFolderMailbox PubMBX3*</span><span class="sxs-lookup"><span data-stu-id="43d46-108">*Set-Mailbox User1 DefaultPublicFolderMailbox PubMBX3*</span></span>
4. <span data-ttu-id="43d46-109">Vent en time, genstart Outlook-klienten</span><span class="sxs-lookup"><span data-stu-id="43d46-109">Wait for an hour, restart outlook client</span></span>