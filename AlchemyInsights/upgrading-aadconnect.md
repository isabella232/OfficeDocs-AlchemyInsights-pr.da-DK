---
title: 932 Opgradering af AADConnect
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "932"
- "1300025"
ms.assetid: 8f43f36c-9722-43a4-b0de-c5341c06dac5
ms.openlocfilehash: fcc5fddb5cfd15407d0533449035317d187931ed
ms.sourcegitcommit: 631cbb5f03e5371f0995e976536d24e9d13746c3
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 04/22/2020
ms.locfileid: "43766487"
---
# <a name="upgrade-azure-ad-connect"></a><span data-ttu-id="9c1c1-102">Opgrader Azure AD Connect</span><span class="sxs-lookup"><span data-stu-id="9c1c1-102">Upgrade Azure AD Connect</span></span>

<span data-ttu-id="9c1c1-103">Automatisk opgradering er som standard aktiveret for Azure AD Connect, hvilket er med til at sikre, at du kører den nyeste version.</span><span class="sxs-lookup"><span data-stu-id="9c1c1-103">By default, automatic upgrade is enabled for Azure AD Connect, which helps to ensure you're running the latest version.</span></span> <span data-ttu-id="9c1c1-104">Hvis du vil kontrollere de automatiske opgraderingsindstillinger, skal du bruge cmdlet'en **Get-ADSyncAutoUpgrade** i Azure AD PowerShell.</span><span class="sxs-lookup"><span data-stu-id="9c1c1-104">To verify the automatic upgrade settings, use the **Get-ADSyncAutoUpgrade** cmdlet in Azure AD PowerShell.</span></span> <span data-ttu-id="9c1c1-105">Cmdlet'en returnerer en af følgende værdier:</span><span class="sxs-lookup"><span data-stu-id="9c1c1-105">The cmdlet will return one of following values:</span></span>

- <span data-ttu-id="9c1c1-106">**Aktiveret**: Automatisk opgradering er aktiveret.</span><span class="sxs-lookup"><span data-stu-id="9c1c1-106">**Enabled**: Automatic upgrade is enabled.</span></span>

- <span data-ttu-id="9c1c1-107">**Deaktiveret**: Automatisk opgradering er deaktiveret.</span><span class="sxs-lookup"><span data-stu-id="9c1c1-107">**Disabled**: Automatic upgrade is disabled.</span></span>

- <span data-ttu-id="9c1c1-108">**Suspenderet**: Systemet er ikke længere berettiget til at modtage automatiske opgraderinger.</span><span class="sxs-lookup"><span data-stu-id="9c1c1-108">**Suspended**: The system is no longer eligible to receive automatic upgrades.</span></span> <span data-ttu-id="9c1c1-109">Du kan ikke konfigurere denne værdi. det er indstillet af systemet.</span><span class="sxs-lookup"><span data-stu-id="9c1c1-109">You can't configure this value; it's set by the system.</span></span>

<span data-ttu-id="9c1c1-110">Yderligere oplysninger finder du i [Automatic upgrade](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-feature-automatic-upgrade).</span><span class="sxs-lookup"><span data-stu-id="9c1c1-110">For more information, see [Automatic upgrade](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-feature-automatic-upgrade).</span></span>

<span data-ttu-id="9c1c1-111">Hvis du vil hente den nyeste [https://www.microsoft.com/download/details.aspx?id=47594](https://www.microsoft.com/download/details.aspx?id=47594)version af Azure AD Connect, skal du gå til .</span><span class="sxs-lookup"><span data-stu-id="9c1c1-111">To download the latest version of Azure AD Connect, go to [https://www.microsoft.com/download/details.aspx?id=47594](https://www.microsoft.com/download/details.aspx?id=47594).</span></span>
