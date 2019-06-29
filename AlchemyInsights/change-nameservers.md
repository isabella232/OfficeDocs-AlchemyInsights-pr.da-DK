---
title: Skift navneservere
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 4/20/2018
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "5"
- "14"
ms.assetid: d011531a-0951-49c0-af30-40d2e765f381
ms.openlocfilehash: 148fbee1c14a8da6ede5ec5ccae90b1a4340ce32
ms.sourcegitcommit: 5fb7a4b28859690020efdea630d03e70cc0e6334
ms.translationtype: HT
ms.contentlocale: da-DK
ms.lasthandoff: 06/28/2019
ms.locfileid: "35363071"
---
# <a name="update-your-domain-nameservers-to-office-365"></a><span data-ttu-id="6f1ba-102">Opdater dine domænenavneservere til Office 365</span><span class="sxs-lookup"><span data-stu-id="6f1ba-102">Update your domain nameservers to Office 365</span></span>

<span data-ttu-id="6f1ba-103">Bemærk! Nogle gange kan der gå op til 48 timer, før ændringer af navneservere overføres.</span><span class="sxs-lookup"><span data-stu-id="6f1ba-103">Note: Nameserver changes can sometimes take up to 48 hours to propagate.</span></span>
  
<span data-ttu-id="6f1ba-104">For at konfigurere dit domæne i Office 365 skal navneserverne hos din registrator opdateres.</span><span class="sxs-lookup"><span data-stu-id="6f1ba-104">To set up your domain in Office 365, the nameservers at your registrar need to be updated.</span></span> <span data-ttu-id="6f1ba-105">Opret eller rediger dine navneserverposter hos din domæneregistrator.</span><span class="sxs-lookup"><span data-stu-id="6f1ba-105">Create or edit your nameserver records at your domain registrar.</span></span>
  
1. <span data-ttu-id="6f1ba-106">Gå til domæneregistratorens websted, og find det område, hvor du kan redigere navneserverne.</span><span class="sxs-lookup"><span data-stu-id="6f1ba-106">Go to your domain registrar's website and find the area where you can edit the nameservers.</span></span>
  
2. <span data-ttu-id="6f1ba-107">Opret eller rediger to navneserverposter, så de matcher med følgende værdier:</span><span class="sxs-lookup"><span data-stu-id="6f1ba-107">Create or edit two nameserver records to match these values:</span></span>

  - <span data-ttu-id="6f1ba-108">ns1.bdm.microsoftonline.com</span><span class="sxs-lookup"><span data-stu-id="6f1ba-108">ns1.bdm.microsoftonline.com</span></span>

  - <span data-ttu-id="6f1ba-109">ns2.bdm.microsoftonline.com</span><span class="sxs-lookup"><span data-stu-id="6f1ba-109">ns2.bdm.microsoftonline.com</span></span>

3. <span data-ttu-id="6f1ba-110">Gem ændringerne.</span><span class="sxs-lookup"><span data-stu-id="6f1ba-110">Save changes.</span></span>

<span data-ttu-id="6f1ba-111">Du kan også finde detaljerede instruktioner i denne artikel: [Skift navneservere for at konfigurere Office 365 med en domæneregistrator](https://support.office.com/article/Change-nameservers-at-any-domain-registrar-to-set-up-Office-365-a8b487a9-2a45-4581-9dc4-5d28a47010a2.aspx)</span><span class="sxs-lookup"><span data-stu-id="6f1ba-111">You can also find detailed instructions in this article: [Change nameservers to set up Office 365 with any domain registrar](https://support.office.com/article/Change-nameservers-at-any-domain-registrar-to-set-up-Office-365-a8b487a9-2a45-4581-9dc4-5d28a47010a2.aspx)</span></span>
  