---
title: Opdater dine domænenavneservere til Office 365
ms.author: v-crytho
author: CrystalThomasMS
ms.date: 5/3/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 5d38b331-a0e8-4937-8bda-4f8f715e1976
ms.custom:
- "6"
- "14"
ms.openlocfilehash: 23d49c734148739ede0d5e5b53430a42b606c831
ms.sourcegitcommit: 037331d71f06750d972c0b6278b23bb15c4806ca
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 10/18/2019
ms.locfileid: "36742167"
---
# <a name="update-your-domain-nameservers-to-office-365"></a><span data-ttu-id="97269-102">Opdater dine domænenavneservere til Office 365</span><span class="sxs-lookup"><span data-stu-id="97269-102">Update your domain nameservers to Office 365</span></span>

<span data-ttu-id="97269-103">Bemærk! Nogle gange kan der gå op til 48 timer, før ændringer af navneservere overføres.</span><span class="sxs-lookup"><span data-stu-id="97269-103">Note: Nameserver changes can sometimes take up to 48 hours to propagate.</span></span>
  
<span data-ttu-id="97269-104">For at konfigurere dit domæne i Office 365 skal navneserverne hos din registrator opdateres.</span><span class="sxs-lookup"><span data-stu-id="97269-104">To set up your domain in Office 365, the nameservers at your registrar need to be updated.</span></span> <span data-ttu-id="97269-105">Opret eller rediger dine navneserverposter hos din domæneregistrator.</span><span class="sxs-lookup"><span data-stu-id="97269-105">Create or edit your nameserver records at your domain registrar.</span></span>
  
1. <span data-ttu-id="97269-106">Gå til domæneregistratorens websted, og find det område, hvor du kan redigere navneserverne.</span><span class="sxs-lookup"><span data-stu-id="97269-106">Go to your domain registrar's website and find the area where you can edit the nameservers.</span></span>

2. <span data-ttu-id="97269-107">Opret eller rediger to navneserverposter, så de matcher med følgende værdier:</span><span class="sxs-lookup"><span data-stu-id="97269-107">Create or edit two nameserver records to match these values:</span></span>

  - <span data-ttu-id="97269-108">ns1.bdm.microsoftonline.com</span><span class="sxs-lookup"><span data-stu-id="97269-108">ns1.bdm.microsoftonline.com</span></span>

  - <span data-ttu-id="97269-109">ns2.bdm.microsoftonline.com</span><span class="sxs-lookup"><span data-stu-id="97269-109">ns2.bdm.microsoftonline.com</span></span>

3. <span data-ttu-id="97269-110">Gem ændringerne.</span><span class="sxs-lookup"><span data-stu-id="97269-110">Save changes.</span></span>

<span data-ttu-id="97269-111">Du kan også finde detaljerede instruktioner i denne artikel: [Skift navneservere for at konfigurere Office 365 med en domæneregistrator](https://docs.microsoft.com/office365/admin/get-help-with-domains/change-nameservers-at-any-domain-registrar)</span><span class="sxs-lookup"><span data-stu-id="97269-111">You can also find detailed instructions in this article: [Change nameservers to set up Office 365 with any domain registrar](https://docs.microsoft.com/office365/admin/get-help-with-domains/change-nameservers-at-any-domain-registrar)</span></span>
  