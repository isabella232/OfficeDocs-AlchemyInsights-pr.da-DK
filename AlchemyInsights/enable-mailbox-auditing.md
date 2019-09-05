---
title: Aktivér overvågning af postkasse
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 4/5/2018
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: 19997b0a-394f-4943-8908-c601696a332c
ms.openlocfilehash: 73517f46935a67a4a8a3e4770090ac897fe67979
ms.sourcegitcommit: a256e8680379c006287ae30996763051c4d9ff85
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 09/04/2019
ms.locfileid: "36736247"
---
# <a name="enable-mailbox-auditing"></a><span data-ttu-id="3afe7-102">Aktivér overvågning af postkasse</span><span class="sxs-lookup"><span data-stu-id="3afe7-102">Enable mailbox auditing</span></span>

<span data-ttu-id="3afe7-103">Hvis du vil aktivere postkasseovervågning for enten en enkelt bruger eller en hel organisation, skal følgende cmdletter køres fra Remote Power shell:</span><span class="sxs-lookup"><span data-stu-id="3afe7-103">To enable Mailbox Auditing for either a single user or an entire organization the following cmdlets must be run from Remote Power Shell:</span></span>
  
 <span data-ttu-id="3afe7-104">**Enkelt bruger**</span><span class="sxs-lookup"><span data-stu-id="3afe7-104">**Single User**</span></span>
  
<span data-ttu-id="3afe7-105">Set-postkasse-identitet "Jane Dow"-AuditEnabled $true</span><span class="sxs-lookup"><span data-stu-id="3afe7-105">Set-Mailbox -Identity "Jane Dow" -AuditEnabled $true</span></span>
  
 <span data-ttu-id="3afe7-106">**Organisation**</span><span class="sxs-lookup"><span data-stu-id="3afe7-106">**Organization**</span></span>
  
<span data-ttu-id="3afe7-107">Hent-postkasse-ResultSize ubegrænset-filter {RecipientTypeDetails-EQ "User Mailbox"} | Set-Mailbox-AuditEnabled $true</span><span class="sxs-lookup"><span data-stu-id="3afe7-107">Get-Mailbox -ResultSize Unlimited -Filter {RecipientTypeDetails -eq "UserMailbox"} | Set-Mailbox -AuditEnabled $true</span></span>
  
[<span data-ttu-id="3afe7-108">Lær mere</span><span class="sxs-lookup"><span data-stu-id="3afe7-108">Learn more</span></span>](https://docs.microsoft.com/office365/securitycompliance/enable-mailbox-auditing)
  

