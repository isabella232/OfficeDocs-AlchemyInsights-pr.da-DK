---
title: Selvbetjeningskøb af PowerShell
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9001212"
- "3516"
ms.openlocfilehash: 5e47e08e3309b3d58908e10ee06021da00f230bb
ms.sourcegitcommit: cb9505f9eca032af3a4194c68d18c91789365690
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 02/16/2020
ms.locfileid: "42091681"
---
# <a name="self-service-purchase-of-powershell"></a><span data-ttu-id="c887e-102">Selvbetjeningskøb af PowerShell</span><span class="sxs-lookup"><span data-stu-id="c887e-102">Self-service purchase of PowerShell</span></span>

<span data-ttu-id="c887e-103">Hvis du vil bruge MSCommerce PowerShell-modulet, skal du installere det på en Windows 10-enhed med TLS 1.2 (lokale administratortilladelser påkrævet).</span><span class="sxs-lookup"><span data-stu-id="c887e-103">To use the MSCommerce PowerShell module, you need to install it on a Windows 10 device with TLS 1.2 (local administrator permissions required).</span></span>  <span data-ttu-id="c887e-104">Importér og opret forbindelse til MSCommerce-modulet.</span><span class="sxs-lookup"><span data-stu-id="c887e-104">Import and connect to the MSCommerce module.</span></span>  <span data-ttu-id="c887e-105">Når du bliver bedt om at logge på, skal du bruge rollelegitimationsoplysninger for global eller faktureringsadministrator.</span><span class="sxs-lookup"><span data-stu-id="c887e-105">When prompted to log in, you will need to use Global or Billing Admin role credentials.</span></span>  

<span data-ttu-id="c887e-106">Hvis du ikke har TLS 1.2, kan du få vist følgende fejl, når du forsøger at hente eller opdatere politikken:</span><span class="sxs-lookup"><span data-stu-id="c887e-106">If you don't have TLS 1.2, you may receive the following error when attempting to get or update the policy:</span></span>

<span data-ttu-id="c887e-107">*ErrorMessage -Den underliggende forbindelse blev lukket: Der opstod en uventet fejl under en afsendelse*.</span><span class="sxs-lookup"><span data-stu-id="c887e-107">*ErrorMessage -The underlying connection was closed: An unexpected error occurred on a send*.</span></span>



