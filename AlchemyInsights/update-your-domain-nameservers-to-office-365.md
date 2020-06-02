---
title: Opdater dine domænenavneservere til at pege på Microsoft
ms.author: v-crytho
author: CrystalThomasMS
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 5d38b331-a0e8-4937-8bda-4f8f715e1976
ms.custom:
- "6"
- "14"
ms.openlocfilehash: 9dd52c60b2d15d66c1c3f2a96c9db08ea2a010c6
ms.sourcegitcommit: bc7d6f4f3c9f7060d073f5130e1ec856e248d020
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 06/02/2020
ms.locfileid: "44510278"
---
# <a name="update-your-domain-nameservers-to-point-to-microsoft"></a><span data-ttu-id="4215c-102">Opdater dine domænenavneservere til at pege på Microsoft</span><span class="sxs-lookup"><span data-stu-id="4215c-102">Update your domain nameservers to point to Microsoft</span></span>

<span data-ttu-id="4215c-103">Bemærk! Nogle gange kan der gå op til 48 timer, før ændringer af navneservere overføres.</span><span class="sxs-lookup"><span data-stu-id="4215c-103">Note: Nameserver changes can sometimes take up to 48 hours to propagate.</span></span>
  
<span data-ttu-id="4215c-104">Hvis du vil konfigurere dit domæne hos Microsoft, skal navneserverne hos registratoren opdateres.</span><span class="sxs-lookup"><span data-stu-id="4215c-104">To set up your domain with Microsoft, the nameservers at your registrar need to be updated.</span></span> <span data-ttu-id="4215c-105">Opret eller rediger dine navneserverposter hos din domæneregistrator.</span><span class="sxs-lookup"><span data-stu-id="4215c-105">Create or edit your nameserver records at your domain registrar.</span></span>
  
1. <span data-ttu-id="4215c-106">Gå til domæneregistratorens websted, og find det område, hvor du kan redigere navneserverne.</span><span class="sxs-lookup"><span data-stu-id="4215c-106">Go to your domain registrar's website and find the area where you can edit the nameservers.</span></span>

2. <span data-ttu-id="4215c-107">Opret eller rediger to navneserverposter, så de matcher med følgende værdier:</span><span class="sxs-lookup"><span data-stu-id="4215c-107">Create or edit two nameserver records to match these values:</span></span>

  - <span data-ttu-id="4215c-108">ns1.bdm.microsoftonline.com</span><span class="sxs-lookup"><span data-stu-id="4215c-108">ns1.bdm.microsoftonline.com</span></span>

  - <span data-ttu-id="4215c-109">ns2.bdm.microsoftonline.com</span><span class="sxs-lookup"><span data-stu-id="4215c-109">ns2.bdm.microsoftonline.com</span></span>

3. <span data-ttu-id="4215c-110">Gem ændringerne.</span><span class="sxs-lookup"><span data-stu-id="4215c-110">Save changes.</span></span>

<span data-ttu-id="4215c-111">Du kan også finde detaljerede instruktioner i denne artikel: [Ændre navneservere for at konfigurere Microsoft 365 med en domæneregistrator](https://docs.microsoft.com/microsoft-365/admin/get-help-with-domains/change-nameservers-at-any-domain-registrar)</span><span class="sxs-lookup"><span data-stu-id="4215c-111">You can also find detailed instructions in this article: [Change nameservers to set up Microsoft 365 with any domain registrar](https://docs.microsoft.com/microsoft-365/admin/get-help-with-domains/change-nameservers-at-any-domain-registrar)</span></span>
  