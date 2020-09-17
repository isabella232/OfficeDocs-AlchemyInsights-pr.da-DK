---
title: 932-opgradering AADConnect
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "932"
- "1300025"
ms.assetid: 8f43f36c-9722-43a4-b0de-c5341c06dac5
ms.openlocfilehash: 5c8ec5d9282c53c655e28f5d38fe36fc3ab005b8
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 09/15/2020
ms.locfileid: "47806033"
---
# <a name="upgrade-azure-ad-connect"></a><span data-ttu-id="1e528-102">Opgrader Azure AD Connect</span><span class="sxs-lookup"><span data-stu-id="1e528-102">Upgrade Azure AD Connect</span></span>

<span data-ttu-id="1e528-103">Automatisk opgradering er som standard aktiveret for Azure AD Connect, hvilket er med til at sikre, at du kører den nyeste version.</span><span class="sxs-lookup"><span data-stu-id="1e528-103">By default, automatic upgrade is enabled for Azure AD Connect, which helps to ensure you're running the latest version.</span></span> <span data-ttu-id="1e528-104">Hvis du vil kontrollere indstillingerne for automatisk opgradering, skal du bruge **Get-ADSyncAutoUpgrade** -cmdlet'en i Azure ad PowerShell.</span><span class="sxs-lookup"><span data-stu-id="1e528-104">To verify the automatic upgrade settings, use the **Get-ADSyncAutoUpgrade** cmdlet in Azure AD PowerShell.</span></span> <span data-ttu-id="1e528-105">Cmdlet returnerer en af følgende værdier:</span><span class="sxs-lookup"><span data-stu-id="1e528-105">The cmdlet will return one of following values:</span></span>

- <span data-ttu-id="1e528-106">**Aktiveret**: automatisk opgradering er aktiveret.</span><span class="sxs-lookup"><span data-stu-id="1e528-106">**Enabled**: Automatic upgrade is enabled.</span></span>

- <span data-ttu-id="1e528-107">**Deaktiveret**: automatisk opgradering er deaktiveret.</span><span class="sxs-lookup"><span data-stu-id="1e528-107">**Disabled**: Automatic upgrade is disabled.</span></span>

- <span data-ttu-id="1e528-108">**Suspenderet**: systemet er ikke længere berettiget til at modtage automatiske opgraderinger.</span><span class="sxs-lookup"><span data-stu-id="1e528-108">**Suspended**: The system is no longer eligible to receive automatic upgrades.</span></span> <span data-ttu-id="1e528-109">Du kan ikke konfigurere denne værdi. den er indstillet af systemet.</span><span class="sxs-lookup"><span data-stu-id="1e528-109">You can't configure this value; it's set by the system.</span></span>

<span data-ttu-id="1e528-110">Hvis du vil have mere at vide, skal du se [automatisk opgradering](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-feature-automatic-upgrade).</span><span class="sxs-lookup"><span data-stu-id="1e528-110">For more information, see [Automatic upgrade](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-feature-automatic-upgrade).</span></span>

<span data-ttu-id="1e528-111">Hvis du vil hente den nyeste version af Azure AD Connect, skal du gå til [https://www.microsoft.com/download/details.aspx?id=47594](https://www.microsoft.com/download/details.aspx?id=47594) .</span><span class="sxs-lookup"><span data-stu-id="1e528-111">To download the latest version of Azure AD Connect, go to [https://www.microsoft.com/download/details.aspx?id=47594](https://www.microsoft.com/download/details.aspx?id=47594).</span></span>
