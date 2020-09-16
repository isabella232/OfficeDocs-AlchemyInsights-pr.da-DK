---
title: Skift navneservere
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "5"
- "14"
ms.openlocfilehash: 07a0dd19a768dd2b97923f0ced566b69ca2d6ba7
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 09/14/2020
ms.locfileid: "47714682"
---
# <a name="update-your-domain-nameservers-to-point-to-microsoft"></a><span data-ttu-id="045cc-102">Opdater dine domænenavneservere til at pege på Microsoft</span><span class="sxs-lookup"><span data-stu-id="045cc-102">Update your domain nameservers to point to Microsoft</span></span>

<span data-ttu-id="045cc-103">Bemærk! Nogle gange kan der gå op til 48 timer, før ændringer af navneservere overføres.</span><span class="sxs-lookup"><span data-stu-id="045cc-103">Note: Nameserver changes can sometimes take up to 48 hours to propagate.</span></span>
  
<span data-ttu-id="045cc-104">For at konfigurere dit domæne i Microsoft 365 skal navneserverne hos din registrator opdateres.</span><span class="sxs-lookup"><span data-stu-id="045cc-104">To set up your domain in Microsoft 365, the nameservers at your registrar need to be updated.</span></span> <span data-ttu-id="045cc-105">Opret eller rediger dine navneserverposter hos din domæneregistrator.</span><span class="sxs-lookup"><span data-stu-id="045cc-105">Create or edit your nameserver records at your domain registrar.</span></span>
  
1. <span data-ttu-id="045cc-106">Gå til domæneregistratorens websted, og find det område, hvor du kan redigere navneserverne.</span><span class="sxs-lookup"><span data-stu-id="045cc-106">Go to your domain registrar's website and find the area where you can edit the nameservers.</span></span>
  
2. <span data-ttu-id="045cc-107">Opret eller rediger to navneserverposter, så de matcher med følgende værdier:</span><span class="sxs-lookup"><span data-stu-id="045cc-107">Create or edit two nameserver records to match these values:</span></span>

  - <span data-ttu-id="045cc-108">ns1.bdm.microsoftonline.com</span><span class="sxs-lookup"><span data-stu-id="045cc-108">ns1.bdm.microsoftonline.com</span></span>

  - <span data-ttu-id="045cc-109">ns2.bdm.microsoftonline.com</span><span class="sxs-lookup"><span data-stu-id="045cc-109">ns2.bdm.microsoftonline.com</span></span>

3. <span data-ttu-id="045cc-110">Gem ændringerne.</span><span class="sxs-lookup"><span data-stu-id="045cc-110">Save changes.</span></span>

<span data-ttu-id="045cc-111">Du kan også finde detaljerede instruktioner i denne artikel: [Skift navneservere for at med en hvilken som helst domæneregistrator](https://docs.microsoft.com/microsoft-365/admin/get-help-with-domains/change-nameservers-at-any-domain-registrar)</span><span class="sxs-lookup"><span data-stu-id="045cc-111">You can also find detailed instructions in this article: [Change nameservers with any domain registrar](https://docs.microsoft.com/microsoft-365/admin/get-help-with-domains/change-nameservers-at-any-domain-registrar)</span></span>
  