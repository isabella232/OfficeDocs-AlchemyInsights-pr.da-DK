---
title: Log automatisk på Microsoft Edge
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 12/03/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9003848"
- "6898"
- "8333"
- "9004625"
ms.openlocfilehash: 6021991c125f5cb2a33ce8db8fe7717b528bf49b
ms.sourcegitcommit: 6bfe9cd9d0b18481e0cac6f1f5bc86ed7df31037
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 03/27/2021
ms.locfileid: "51398723"
---
# <a name="sign-in-to-microsoft-edge-automatically"></a><span data-ttu-id="d6174-102">Log automatisk på Microsoft Edge</span><span class="sxs-lookup"><span data-stu-id="d6174-102">Sign in to Microsoft Edge automatically</span></span>

<span data-ttu-id="d6174-103">Microsoft Edge bruger OS-standardkontoen til automatisk at logge en bruger på i overensstemmelse med, hvordan brugerens enhed er konfigureret.</span><span class="sxs-lookup"><span data-stu-id="d6174-103">Microsoft Edge uses the OS default account to automatically sign in a user according to how the user's device is configured.</span></span> 

<span data-ttu-id="d6174-104">Scenarierne for hver type enhedskonfiguration og den afhængige brugers logonproces er beskrevet nedenfor:</span><span class="sxs-lookup"><span data-stu-id="d6174-104">The scenarios of each type of device configuration and its dependent user sign-in process are described below:</span></span>

- <span data-ttu-id="d6174-105">**Enheden er hybrid/AAD-J: Denne** indstilling er tilgængelig i Windows 10, Windows på ned niveau og tilsvarende serverversioner.</span><span class="sxs-lookup"><span data-stu-id="d6174-105">**The device is hybrid/AAD-J**: This option is available on Windows 10, down-level Windows, and corresponding server versions.</span></span> <span data-ttu-id="d6174-106">Brugere logges automatisk på med deres Azure Active Directory-konti (AD).</span><span class="sxs-lookup"><span data-stu-id="d6174-106">Users are automatically signed in with their Azure Active Directory (AD)accounts.</span></span>
- <span data-ttu-id="d6174-107">**Enheden er domæne-forbundet:** Denne indstilling er tilgængelig i Windows 10, Windows på ned niveau og tilsvarende serverversioner.</span><span class="sxs-lookup"><span data-stu-id="d6174-107">**The device is domain-joined**: This option is available on Windows 10, down-level Windows, and corresponding server versions.</span></span> <span data-ttu-id="d6174-108">Som standard er brugere med domænekonti ikke logget på automatisk. hvis du vil aktivere automatisk logon for dem, skal du bruge **politikken ConfigureOnPremisesAccountAutoSignIn.**</span><span class="sxs-lookup"><span data-stu-id="d6174-108">By default, users with domain accounts are not signed in automatically; to enable automatic sign-in for them, use the **ConfigureOnPremisesAccountAutoSignIn** policy.</span></span> <span data-ttu-id="d6174-109">Hvis du vil aktivere automatisk logon for brugere med Azure AD-konti, kan du overveje at deltage hybridt på deres enheder.</span><span class="sxs-lookup"><span data-stu-id="d6174-109">To enable automatic sign-in for users with Azure AD accounts, consider hybrid-joining their devices.</span></span>
- <span data-ttu-id="d6174-110">**Os-standardkontoen** er en Microsoft-konto: Denne indstilling er tilgængelig på Windows 10 RS3 (version 1709, build 10.0.16299) og nyere versioner.</span><span class="sxs-lookup"><span data-stu-id="d6174-110">**The OS's default account is a Microsoft account**: This option is available on Windows 10 RS3 (version 1709, build 10.0.16299) and later versions.</span></span> <span data-ttu-id="d6174-111">Scenariet er usandsynligt på virksomhedsenheder.</span><span class="sxs-lookup"><span data-stu-id="d6174-111">The scenario is unlikely to occur on enterprise devices.</span></span> <span data-ttu-id="d6174-112">Men hvis OS-standardkontoen er en Microsoft-konto, logger Microsoft Edge automatisk brugeren på med Microsoft-kontoen.</span><span class="sxs-lookup"><span data-stu-id="d6174-112">However, if the OS default account is a Microsoft account, then Microsoft Edge will automatically sign in the user with the Microsoft account.</span></span>
 
 
