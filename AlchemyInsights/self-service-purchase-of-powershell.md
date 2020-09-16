---
title: Selvbetjenings opkøb af PowerShell
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9001212"
- "3516"
ms.openlocfilehash: e6cc504ebef19cbe78f576d9b207fe2d951d0ef5
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 09/14/2020
ms.locfileid: "47739964"
---
# <a name="self-service-purchase-of-powershell"></a><span data-ttu-id="26603-102">Selvbetjenings opkøb af PowerShell</span><span class="sxs-lookup"><span data-stu-id="26603-102">Self-service purchase of PowerShell</span></span>

<span data-ttu-id="26603-103">Hvis du vil bruge MSCommerce PowerShell-modulet, skal du installere det på en Windows 10-enhed med TLS 1,2 (kræver lokale administratortilladelser).</span><span class="sxs-lookup"><span data-stu-id="26603-103">To use the MSCommerce PowerShell module, you need to install it on a Windows 10 device with TLS 1.2 (local administrator permissions required).</span></span>  <span data-ttu-id="26603-104">Importér og Opret forbindelse til MSCommerce-modulet.</span><span class="sxs-lookup"><span data-stu-id="26603-104">Import and connect to the MSCommerce module.</span></span>  <span data-ttu-id="26603-105">Når du bliver bedt om at logge på, skal du bruge globale eller Faktureringsadministratorens legitimationsoplysninger.</span><span class="sxs-lookup"><span data-stu-id="26603-105">When prompted to log in, you will need to use Global or Billing Admin role credentials.</span></span>  

<span data-ttu-id="26603-106">Hvis du ikke har TLS 1,2, modtager du muligvis følgende fejlmeddelelse, når du forsøger at hente eller opdatere politikken:</span><span class="sxs-lookup"><span data-stu-id="26603-106">If you don't have TLS 1.2, you may receive the following error when attempting to get or update the policy:</span></span>

<span data-ttu-id="26603-107">*ErrorMessage – den underliggende forbindelse blev lukket: der opstod en uventet fejl ved afsendelse*.</span><span class="sxs-lookup"><span data-stu-id="26603-107">*ErrorMessage -The underlying connection was closed: An unexpected error occurred on a send*.</span></span>



