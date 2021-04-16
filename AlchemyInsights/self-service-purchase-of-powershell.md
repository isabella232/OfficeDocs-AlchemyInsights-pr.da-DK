---
title: Selvbetjeningskøb af PowerShell
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9001212"
- "3516"
ms.openlocfilehash: 48b5b0a1be1bc03d45a531a1093f18a3f750c37d
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 04/15/2021
ms.locfileid: "51797715"
---
# <a name="self-service-purchase-of-powershell"></a><span data-ttu-id="16d29-102">Selvbetjeningskøb af PowerShell</span><span class="sxs-lookup"><span data-stu-id="16d29-102">Self-service purchase of PowerShell</span></span>

<span data-ttu-id="16d29-103">Hvis du vil bruge MSCommerce PowerShell-modulet, skal du installere det på en Windows 10-enhed med TLS 1.2 (lokale administratortilladelser påkrævet).</span><span class="sxs-lookup"><span data-stu-id="16d29-103">To use the MSCommerce PowerShell module, you need to install it on a Windows 10 device with TLS 1.2 (local administrator permissions required).</span></span>  <span data-ttu-id="16d29-104">Importér og opret forbindelse til MSCommerce-modulet.</span><span class="sxs-lookup"><span data-stu-id="16d29-104">Import and connect to the MSCommerce module.</span></span>  <span data-ttu-id="16d29-105">Når du bliver bedt om at logge på, skal du bruge legitimationsoplysningerne som global administrator eller faktureringsadministrator.</span><span class="sxs-lookup"><span data-stu-id="16d29-105">When prompted to log in, you will need to use Global or Billing Admin role credentials.</span></span>  

<span data-ttu-id="16d29-106">Hvis du ikke har TLS 1.2, modtager du muligvis følgende fejlmeddelelse, når du forsøger at få eller opdatere politikken:</span><span class="sxs-lookup"><span data-stu-id="16d29-106">If you don't have TLS 1.2, you may receive the following error when attempting to get or update the policy:</span></span>

<span data-ttu-id="16d29-107">*ErrorMessage –Den underliggende forbindelse blev lukket: Der opstod en uventet fejl i en send-.*</span><span class="sxs-lookup"><span data-stu-id="16d29-107">*ErrorMessage -The underlying connection was closed: An unexpected error occurred on a send*.</span></span>



