---
title: Ejeren kan ikke oprette undermappe ved hjælp af Outlook
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "5884"
- "3500007"
ms.openlocfilehash: 2116bb837e4378ea29d7882df1d3010b3a4e0b1c
ms.sourcegitcommit: 936330b11fec49f6174eadea6c765bdf9e6ba784
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 06/12/2020
ms.locfileid: "44748790"
---
# <a name="owner-cannot-create-sub-folder-using-outlook"></a><span data-ttu-id="a6f94-102">Ejeren kan ikke oprette undermappe ved hjælp af Outlook</span><span class="sxs-lookup"><span data-stu-id="a6f94-102">Owner cannot create sub-folder using Outlook</span></span>

<span data-ttu-id="a6f94-103">**Der er et vedvarende problem med ejere af offentlige mapper, der opretter undermapper ved hjælp af Outlook. Problemet vil blive løst snart.**</span><span class="sxs-lookup"><span data-stu-id="a6f94-103">**There's an ongoing issue with public folder owners creating subfolders using Outlook. The issue will be fixed soon.**</span></span>

<span data-ttu-id="a6f94-104">Brug i mellemtiden en af følgende løsninger:</span><span class="sxs-lookup"><span data-stu-id="a6f94-104">Meanwhile, use one of the following workarounds:</span></span>

1. <span data-ttu-id="a6f94-105">Brug Outlook til MAC til at oprette undermappen, da problemet kun påvirker Outlook til skrivebordsvinduer (alle versioner)</span><span class="sxs-lookup"><span data-stu-id="a6f94-105">Use Outlook for MAC to create the subfolder as the issue impacts only Outlook for desktop windows (all versions)</span></span>
2. <span data-ttu-id="a6f94-106">Få administratoren til at oprette undermappen ved hjælp af EXO Shell eller EAC</span><span class="sxs-lookup"><span data-stu-id="a6f94-106">Have admin create the subfolder using EXO Shell or EAC</span></span>
3. <span data-ttu-id="a6f94-107">Ændre standardpostublicFolderMailbox/EffectivePublicFolderMailbox på brugeren til en anden postkasse end indholdspostkassen for den mappe, der forårsager problemet</span><span class="sxs-lookup"><span data-stu-id="a6f94-107">Change the DefaultPublicFolderMailbox/EffectivePublicFolderMailbox on the user to other mailbox than the Content Mailbox for the folder causing issue</span></span>  
    - <span data-ttu-id="a6f94-108">*Set-Mailbox User1 DefaultPublicFolderMailbox PubMBX3*</span><span class="sxs-lookup"><span data-stu-id="a6f94-108">*Set-Mailbox User1 DefaultPublicFolderMailbox PubMBX3*</span></span>
4. <span data-ttu-id="a6f94-109">Vent i en time, genstart Outlook-klienten</span><span class="sxs-lookup"><span data-stu-id="a6f94-109">Wait for an hour, restart outlook client</span></span>