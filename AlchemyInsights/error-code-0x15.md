---
title: Fejlkode 0x15
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "919"
- "2000022"
ms.assetid: 0d566afe-b21f-4f1b-8ca9-4b4d3b0f5435
description: Hvis du modtager en fejl under aktivering af Office 2013 på RDS-installationer (Remote Desktop Services), kan du overveje at aktivere ADAL ved at redigere registreringsdatabasen.
ms.openlocfilehash: 566d63cbe37d295b3546b9d7d5b14dfc8e8fe0ec
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 04/22/2020
ms.locfileid: "43703132"
---
# <a name="error-while-activation-office-2013-on-remote-desktop-services"></a><span data-ttu-id="1c74d-103">Der opstod en fejl under aktivering af Office 2013 på Fjernskrivebord-tjenester</span><span class="sxs-lookup"><span data-stu-id="1c74d-103">Error while activation Office 2013 on Remote Desktop Services</span></span>

<span data-ttu-id="1c74d-104">Hvis du modtager en fejl under aktivering af Office 2013 på RDS-installationer (Remote Desktop Services), kan du overveje at aktivere ADAL ved at redigere registreringsdatabasen.</span><span class="sxs-lookup"><span data-stu-id="1c74d-104">If you're receiving an error while activating Office 2013 on Remote Desktop Services (RDS) deployments, consider enabling ADAL by editing the registry.</span></span>
  
|<span data-ttu-id="1c74d-105">**Registreringsdatabasenøgle**</span><span class="sxs-lookup"><span data-stu-id="1c74d-105">**Registry key**</span></span>|<span data-ttu-id="1c74d-106">**Type**</span><span class="sxs-lookup"><span data-stu-id="1c74d-106">**Type**</span></span>|<span data-ttu-id="1c74d-107">**Værdi**</span><span class="sxs-lookup"><span data-stu-id="1c74d-107">**Value**</span></span>|
|:-----|:-----|:-----|
|<span data-ttu-id="1c74d-108">HKEY_CURRENT_USER\Software\Microsoft\Office\15.0\Common\Identity\EnableADAL</span><span class="sxs-lookup"><span data-stu-id="1c74d-108">HKEY_CURRENT_USER\Software\Microsoft\Office\15.0\Common\Identity\EnableADAL</span></span>  <br/> |<span data-ttu-id="1c74d-109">Reg_dword</span><span class="sxs-lookup"><span data-stu-id="1c74d-109">REG_DWORD</span></span>  <br/> |<span data-ttu-id="1c74d-110">1</span><span class="sxs-lookup"><span data-stu-id="1c74d-110">1</span></span>  <br/> |

<span data-ttu-id="1c74d-111">Yderligere oplysninger finder du [i Enable Modern Authentication for Office 2013 on Windows devices](https://docs.microsoft.com/office365/admin/security-and-compliance/enable-modern-authentication).</span><span class="sxs-lookup"><span data-stu-id="1c74d-111">For more information, see [Enable Modern Authentication for Office 2013 on Windows devices](https://docs.microsoft.com/office365/admin/security-and-compliance/enable-modern-authentication).</span></span>
  
> [!NOTE]
>  <span data-ttu-id="1c74d-112">ADAL er som standard aktiveret i Microsoft 365 Apps til virksomheder og Office 2016.</span><span class="sxs-lookup"><span data-stu-id="1c74d-112">ADAL is enabled by default in Microsoft 365 Apps for enterprise and Office 2016.</span></span> <span data-ttu-id="1c74d-113">RDS (Remote Desktop Services) hed tidligere Terminal Services.</span><span class="sxs-lookup"><span data-stu-id="1c74d-113">Remote Desktop Services (RDS) was previously named Terminal Services.</span></span>
  