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
ms.openlocfilehash: 51532f42e7cbd39ebad3f0160465218c6e1454a2
ms.sourcegitcommit: a256e8680379c006287ae30996763051c4d9ff85
ms.translationtype: HT
ms.contentlocale: da-DK
ms.lasthandoff: 09/04/2019
ms.locfileid: "36736643"
---
# <a name="update-your-domain-nameservers-to-office-365"></a><span data-ttu-id="6ef49-102">Opdater dine domænenavneservere til Office 365</span><span class="sxs-lookup"><span data-stu-id="6ef49-102">Update your domain nameservers to Office 365</span></span>

<span data-ttu-id="6ef49-103">Bemærk! Nogle gange kan der gå op til 48 timer, før ændringer af navneservere overføres.</span><span class="sxs-lookup"><span data-stu-id="6ef49-103">Note: Nameserver changes can sometimes take up to 48 hours to propagate.</span></span>
  
<span data-ttu-id="6ef49-104">For at konfigurere dit domæne i Office 365 skal navneserverne hos din registrator opdateres.</span><span class="sxs-lookup"><span data-stu-id="6ef49-104">To set up your domain in Office 365, the nameservers at your registrar need to be updated.</span></span> <span data-ttu-id="6ef49-105">Opret eller rediger dine navneserverposter hos din domæneregistrator.</span><span class="sxs-lookup"><span data-stu-id="6ef49-105">Create or edit your nameserver records at your domain registrar.</span></span>
  
1. <span data-ttu-id="6ef49-106">Gå til domæneregistratorens websted, og find det område, hvor du kan redigere navneserverne.</span><span class="sxs-lookup"><span data-stu-id="6ef49-106">Go to your domain registrar's website and find the area where you can edit the nameservers.</span></span>
  
2. <span data-ttu-id="6ef49-107">Opret eller rediger to navneserverposter, så de matcher med følgende værdier:</span><span class="sxs-lookup"><span data-stu-id="6ef49-107">Create or edit two nameserver records to match these values:</span></span>

  - <span data-ttu-id="6ef49-108">ns1.bdm.microsoftonline.com</span><span class="sxs-lookup"><span data-stu-id="6ef49-108">ns1.bdm.microsoftonline.com</span></span>

  - <span data-ttu-id="6ef49-109">ns2.bdm.microsoftonline.com</span><span class="sxs-lookup"><span data-stu-id="6ef49-109">ns2.bdm.microsoftonline.com</span></span>

3. <span data-ttu-id="6ef49-110">Gem ændringerne.</span><span class="sxs-lookup"><span data-stu-id="6ef49-110">Save changes.</span></span>

<span data-ttu-id="6ef49-111">Du kan også finde detaljerede instruktioner i denne artikel: [Skift navneservere for at konfigurere Office 365 med en domæneregistrator](https://docs.microsoft.com//office365/admin/get-help-with-domains/change-nameservers-at-any-domain-registrar)</span><span class="sxs-lookup"><span data-stu-id="6ef49-111">You can also find detailed instructions in this article: [Change nameservers to set up Office 365 with any domain registrar](https://docs.microsoft.com//office365/admin/get-help-with-domains/change-nameservers-at-any-domain-registrar)</span></span>
  