---
title: Logge på Microsoft Edge automatisk
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
ms.openlocfilehash: 68a1119abd0a3f687b6448bb6e58c6485c239c0f
ms.sourcegitcommit: 94036315916fbc79dca2a692c2e9bc1139dd28f6
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 12/08/2020
ms.locfileid: "49677233"
---
# <a name="sign-in-to-microsoft-edge-automatically"></a><span data-ttu-id="05b93-102">Logge på Microsoft Edge automatisk</span><span class="sxs-lookup"><span data-stu-id="05b93-102">Sign in to Microsoft Edge automatically</span></span>

<span data-ttu-id="05b93-103">Microsoft Edge bruger OPERATIVSYSTEMETS standardkonto til automatisk at logge på en bruger, afhængigt af hvordan brugerens enhed er konfigureret.</span><span class="sxs-lookup"><span data-stu-id="05b93-103">Microsoft Edge uses the OS's default account to automatically sign in a user according to how the user's device is configured.</span></span> 

<span data-ttu-id="05b93-104">Scenarierne for hver type enhedskonfiguration og den afhængige brugerlogon er beskrevet nedenfor:</span><span class="sxs-lookup"><span data-stu-id="05b93-104">The scenarios of each type of device configuration and its dependent user sign-in process are described below:</span></span>

1. <span data-ttu-id="05b93-105">**Enheden er hybrid/Aad-J**: denne indstilling er tilgængelig på Windows 10, på et down-niveau-Windows og tilsvarende server versioner.</span><span class="sxs-lookup"><span data-stu-id="05b93-105">**The device is hybrid/AAD-J**: This option is available on Windows 10, down-level Windows, and corresponding server versions.</span></span> <span data-ttu-id="05b93-106">Brugere logges automatisk på med deres Azure Active Directory-konti (AD).</span><span class="sxs-lookup"><span data-stu-id="05b93-106">Users are automatically signed in with their Azure Active Directory (AD)accounts.</span></span>
2. <span data-ttu-id="05b93-107">**Enheden er domæne tilmeldt**: denne indstilling er tilgængelig på Windows 10, på et down-niveau-Windows og tilsvarende server versioner.</span><span class="sxs-lookup"><span data-stu-id="05b93-107">**The device is domain-joined**: This option is available on Windows 10, down-level Windows, and corresponding server versions.</span></span> <span data-ttu-id="05b93-108">Brugere med domænekonti er som standard ikke logget på automatisk. Hvis du vil aktivere automatisk logon for dem, skal du bruge **ConfigureOnPremisesAccountAutoSignIn** -politikken.</span><span class="sxs-lookup"><span data-stu-id="05b93-108">By default, users with domain accounts are not signed in automatically; to enable automatic sign-in for them, use the **ConfigureOnPremisesAccountAutoSignIn** policy.</span></span> <span data-ttu-id="05b93-109">Hvis du vil aktivere automatisk logon for brugere med Azure AD-konti, skal du overveje at oprette en hybrid forbindelse til deres enheder.</span><span class="sxs-lookup"><span data-stu-id="05b93-109">To enable automatic sign-in for users with Azure AD accounts, consider hybrid-joining their devices.</span></span>
3. <span data-ttu-id="05b93-110">**Operativsystemets standardkonto er en Microsoft-konto**: denne indstilling er tilgængelig på Windows 10 RS3 (version 1709, Build 10.0.16299) og nyere versioner.</span><span class="sxs-lookup"><span data-stu-id="05b93-110">**The OS's default account is a Microsoft account**: This option is available on Windows 10 RS3 (version 1709, build 10.0.16299) and later versions.</span></span> <span data-ttu-id="05b93-111">Scenariet vil sandsynligvis ikke forekomme på virksomhedsenheder.</span><span class="sxs-lookup"><span data-stu-id="05b93-111">The scenario is unlikely to occur on enterprise devices.</span></span> <span data-ttu-id="05b93-112">Men hvis OPERATIVSYSTEMETS standardkonto er en Microsoft-konto, logger Microsoft Edge automatisk brugeren med Microsoft-kontoen.</span><span class="sxs-lookup"><span data-stu-id="05b93-112">However, if the OS's default account is a Microsoft account, then Microsoft Edge will automatically sign in the user with the Microsoft account.</span></span>
 
 
