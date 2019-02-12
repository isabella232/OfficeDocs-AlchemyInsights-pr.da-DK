---
title: 1554 Winsock-fejl 10061
ms.author: chrisda
author: chrisda
manager: serdars
ms.date: 12/7/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: caecfa19-86c9-4aa4-9c83-b8a974ce60b9
ms.openlocfilehash: 9331a6c2b6e92a66fb97daf7dc5655ec320cba0f
ms.sourcegitcommit: dd43cc0a9470f98b8ef2a3787c823801d674c666
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 02/12/2019
ms.locfileid: "29903090"
---
# <a name="winsock-error-10061"></a><span data-ttu-id="9d5da-102">Winsock-fejl 10061</span><span class="sxs-lookup"><span data-stu-id="9d5da-102">Winsock error 10061</span></span>

<span data-ttu-id="9d5da-p101">Denne fejlkode betyder, at Office 365 ikke kunne oprette en TCP socket (connection) med destinationsværten. Den mest sandsynlige årsag til denne fejl er et problem med firewallkonfigurationen af. Du kan løse problemet ved at kontrollere disse indstillinger:</span><span class="sxs-lookup"><span data-stu-id="9d5da-p101">This error code means that Office 365 couldn't establish a TCP socket (connection) with the target host. The most likely cause of this error is a problem with your firewall configuration. To fix the problem, check these settings:</span></span>
  
- <span data-ttu-id="9d5da-106">Kontrol firewall-konfiguration med oplysninger i [Office 365 URL-adresser og IP-adresseområder](https://docs.microsoft.com/office365/enterprise/urls-and-ip-address-ranges)</span><span class="sxs-lookup"><span data-stu-id="9d5da-106">Verify your firewall configuration with the information in [Office 365 URLs and IP address ranges](https://docs.microsoft.com/office365/enterprise/urls-and-ip-address-ranges)</span></span>
    
- <span data-ttu-id="9d5da-107">Hvis fejlen er bestemt til Exchange Online beskyttelse (EOP), skal du have tidligere meddelt en ændring i [Exchange Online beskyttelse IP-adresser](https://docs.microsoft.com/office365/SecurityCompliance/eop/exchange-online-protection-ip-addresses).</span><span class="sxs-lookup"><span data-stu-id="9d5da-107">If the error is specific to Exchange Online Protection (EOP), you should have been previously notified to a change to the [Exchange Online Protection IP addresses](https://docs.microsoft.com/office365/SecurityCompliance/eop/exchange-online-protection-ip-addresses).</span></span>
    
- <span data-ttu-id="9d5da-108">Kontroller, at din internetudbyder (ISP) ikke er blokerer for porten.</span><span class="sxs-lookup"><span data-stu-id="9d5da-108">Verify that your Internet Service Provider (ISP) isn't blocking the port.</span></span>
    
- <span data-ttu-id="9d5da-109">Kontroller smart værten og målcomputerne serverindstillingerne i dine forbindelser.</span><span class="sxs-lookup"><span data-stu-id="9d5da-109">Verify the smart host and target server settings in your connectors.</span></span>
    
<span data-ttu-id="9d5da-110">Bemærk, at Office 365 ikke blokerer *indgående* forbindelser på denne måde.</span><span class="sxs-lookup"><span data-stu-id="9d5da-110">Note that Office 365 doesn't block  *incoming*  connections in this manner.</span></span> 
  

