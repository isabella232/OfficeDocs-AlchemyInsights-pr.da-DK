---
title: 932 opgradering af AADConnect
ms.author: chrisda
author: chrisda
manager: serdars
ms.date: 6/8/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 8f43f36c-9722-43a4-b0de-c5341c06dac5
ms.openlocfilehash: 8038d5ef768d6ee228db7d038ad71d926f4047f3
ms.sourcegitcommit: dd43cc0a9470f98b8ef2a3787c823801d674c666
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 02/12/2019
ms.locfileid: "29937938"
---
# <a name="upgrade-azure-ad-connect"></a><span data-ttu-id="501c0-102">Opgradering af Azure AD forbindelse</span><span class="sxs-lookup"><span data-stu-id="501c0-102">Upgrade Azure AD Connect</span></span>

<span data-ttu-id="501c0-p101">Automatisk opgradering er som standard aktiveret for Azure AD Connect, som hjælper med at sikre, at du kører den nyeste version. For at kontrollere indstillingerne for automatiske opgradering, kan du bruge cmdlet **Get-ADSyncAutoUpgrade** i Azure AD PowerShell. Cmdlet returnerer en af følgende værdier:</span><span class="sxs-lookup"><span data-stu-id="501c0-p101">By default, automatic upgrade is enabled for Azure AD Connect, which helps to ensure you're running the latest version. To verify the automatic upgrade settings, use the **Get-ADSyncAutoUpgrade** cmdlet in Azure AD PowerShell. The cmdlet will return one of following values:</span></span> 
  
- <span data-ttu-id="501c0-106">**Aktiveret**: automatisk opgradering er aktiveret.</span><span class="sxs-lookup"><span data-stu-id="501c0-106">**Enabled**: Automatic upgrade is enabled.</span></span> 
    
- <span data-ttu-id="501c0-107">**Deaktiveret**: automatisk opgradering er deaktiveret.</span><span class="sxs-lookup"><span data-stu-id="501c0-107">**Disabled**: Automatic upgrade is disabled.</span></span> 
    
- <span data-ttu-id="501c0-p102">**Suspenderet**: systemet ikke længere er berettiget til at modtage automatiske opgraderinger. Du kan ikke konfigurere denne værdi; angives af systemet.</span><span class="sxs-lookup"><span data-stu-id="501c0-p102">**Suspended**: The system is no longer eligible to receive automatic upgrades. You can't configure this value; it's set by the system.</span></span> 
    
<span data-ttu-id="501c0-110">Yderligere oplysninger finder du under [automatisk opgradering](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-feature-automatic-upgrade).</span><span class="sxs-lookup"><span data-stu-id="501c0-110">For more information, see [Automatic upgrade](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-feature-automatic-upgrade).</span></span>
  
<span data-ttu-id="501c0-111">For at hente den nyeste version af Azure AD Connect, skal du gå til [https://www.microsoft.com/download/details.aspx?id=47594](https://www.microsoft.com/download/details.aspx?id=47594).</span><span class="sxs-lookup"><span data-stu-id="501c0-111">To download the latest version of Azure AD Connect, go to [https://www.microsoft.com/download/details.aspx?id=47594](https://www.microsoft.com/download/details.aspx?id=47594).</span></span>
  

