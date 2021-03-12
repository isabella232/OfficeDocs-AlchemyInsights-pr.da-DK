---
title: Adgangskodepolitikker
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 03/11/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004595"
- "9277"
ms.openlocfilehash: 826e266d08aa68c0d4213d8058a0244f404fe965
ms.sourcegitcommit: 186281d0b87d67f041c127d4334faa937da9a48a
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 03/11/2021
ms.locfileid: "50743954"
---
# <a name="password-policies"></a><span data-ttu-id="123db-102">Adgangskodepolitikker</span><span class="sxs-lookup"><span data-stu-id="123db-102">Password policies</span></span>

<span data-ttu-id="123db-103">**Jeg har problemer med adgangskodepolitikken for en bruger**</span><span class="sxs-lookup"><span data-stu-id="123db-103">**I'm having problems with the password policy for a user**</span></span>

- <span data-ttu-id="123db-104">Adgangskodepolitikken for en bruger afhænger af, om brugeren kun er skybaseret eller lokal.</span><span class="sxs-lookup"><span data-stu-id="123db-104">The password policy for a user depends on whether the user is cloud only or on-premises.</span></span>
- <span data-ttu-id="123db-105">Kun skybrugere skal vælge en adgangskode, der opfylder kravene i denne artikel: Adgangskodepolitikker, [der kun gælder for skybrugerkonti](https://docs.microsoft.com/azure/active-directory/authentication/concept-sspr-policy?WT.mc_id=Portal-Microsoft_Azure_Support#password-policies-that-only-apply-to-cloud-user-accounts)</span><span class="sxs-lookup"><span data-stu-id="123db-105">Cloud only users must choose a password that meets the requirements in this article: [Password policies that only apply to cloud user accounts](https://docs.microsoft.com/azure/active-directory/authentication/concept-sspr-policy?WT.mc_id=Portal-Microsoft_Azure_Support#password-policies-that-only-apply-to-cloud-user-accounts)</span></span>
- <span data-ttu-id="123db-106">Lokale brugere skal vælge en adgangskode, der opfylder de lokale krav.</span><span class="sxs-lookup"><span data-stu-id="123db-106">On-premises users must choose a password that meets the on-premises requirements.</span></span> <span data-ttu-id="123db-107">Hvis en lokal bruger ikke kan angive sin adgangskode, skal du kontrollere dine lokale krav.</span><span class="sxs-lookup"><span data-stu-id="123db-107">If an on-premises user is unable to set their password, check your on-premises requirements.</span></span>

<span data-ttu-id="123db-108">**Jeg ved ikke, hvordan jeg angiver eller kontrollerer udløbspolitikker for adgangskoder**</span><span class="sxs-lookup"><span data-stu-id="123db-108">**I don't know how to set or check password expiration policies**</span></span>

- <span data-ttu-id="123db-109">Du kan angive og kontrollere udløbspolitikken for skybrugere i din lejer ved hjælp af PowerShell.</span><span class="sxs-lookup"><span data-stu-id="123db-109">You can set and check the expiration policy for cloud users in your tenant by using PowerShell.</span></span> <span data-ttu-id="123db-110">Følg vejledningen i denne artikel: Angiv [eller kontrollér adgangskodepolitikker ved hjælp af PowerShell](https://docs.microsoft.com/azure/active-directory/authentication/concept-sspr-policy?WT.mc_id=Portal-Microsoft_Azure_Support#set-or-check-the-password-policies-by-using-powershell)</span><span class="sxs-lookup"><span data-stu-id="123db-110">Follow the instructions in this article: [Set or check the password policies by using PowerShell](https://docs.microsoft.com/azure/active-directory/authentication/concept-sspr-policy?WT.mc_id=Portal-Microsoft_Azure_Support#set-or-check-the-password-policies-by-using-powershell)</span></span>
- <span data-ttu-id="123db-111">Udløbspolitikken for adgangskoder for lokale brugere er angivet i dit lokale AD.</span><span class="sxs-lookup"><span data-stu-id="123db-111">The password expiration policy for on-premises users is set in your on-premises AD.</span></span>

<span data-ttu-id="123db-112">**Andre nyttige links:**</span><span class="sxs-lookup"><span data-stu-id="123db-112">**Other Helpful links:**</span></span>
- [<span data-ttu-id="123db-113">Introduktion til nulstilling af adgangskode</span><span class="sxs-lookup"><span data-stu-id="123db-113">Getting Started with Password Reset</span></span>](https://docs.microsoft.com/azure/active-directory/authentication/concept-sspr-policy?WT.mc_id=Portal-Microsoft_Azure_Support#set-or-check-the-password-policies-by-using-powershell)
- [<span data-ttu-id="123db-114">Fejlfinding af administrator-startet nulstilling af adgangskode</span><span class="sxs-lookup"><span data-stu-id="123db-114">Troubleshoot Administrator-initiated Password Reset</span></span>](https://docs.microsoft.com/azure/active-directory/active-directory-passwords-troubleshoot?WT.mc_id=Portal-Microsoft_Azure_Support#troubleshoot-the-password-reset-portal)
