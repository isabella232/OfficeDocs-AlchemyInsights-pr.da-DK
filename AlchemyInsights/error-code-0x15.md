---
title: Fejlkode 0x15
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "919"
- "2000022"
ms.assetid: 0d566afe-b21f-4f1b-8ca9-4b4d3b0f5435
description: Hvis du får en fejl, når du aktiverer Office 2013 på installation af Fjernskrivebord-tjenester (RDS), kan du overveje at aktivere ADAL ved at redigere registreringsdatabasen.
ms.openlocfilehash: deb2ac4b0fb6a7b2e0045ff1b0ba95ad6e5e4a3a
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 09/14/2020
ms.locfileid: "47709181"
---
# <a name="error-while-activation-office-2013-on-remote-desktop-services"></a><span data-ttu-id="64a89-103">Fejl under aktivering af Office 2013 på Fjernskrivebord-tjenester</span><span class="sxs-lookup"><span data-stu-id="64a89-103">Error while activation Office 2013 on Remote Desktop Services</span></span>

<span data-ttu-id="64a89-104">Hvis du får en fejl, når du aktiverer Office 2013 på installation af Fjernskrivebord-tjenester (RDS), kan du overveje at aktivere ADAL ved at redigere registreringsdatabasen.</span><span class="sxs-lookup"><span data-stu-id="64a89-104">If you're receiving an error while activating Office 2013 on Remote Desktop Services (RDS) deployments, consider enabling ADAL by editing the registry.</span></span>
  
|<span data-ttu-id="64a89-105">**Registreringsdatabasenøgle**</span><span class="sxs-lookup"><span data-stu-id="64a89-105">**Registry key**</span></span>|<span data-ttu-id="64a89-106">**Indtaste**</span><span class="sxs-lookup"><span data-stu-id="64a89-106">**Type**</span></span>|<span data-ttu-id="64a89-107">**Talværdi**</span><span class="sxs-lookup"><span data-stu-id="64a89-107">**Value**</span></span>|
|:-----|:-----|:-----|
|<span data-ttu-id="64a89-108">HKEY_CURRENT_USER \Software\Microsoft\Office\15.0\Common\Identity\EnableADAL</span><span class="sxs-lookup"><span data-stu-id="64a89-108">HKEY_CURRENT_USER\Software\Microsoft\Office\15.0\Common\Identity\EnableADAL</span></span>  <br/> |<span data-ttu-id="64a89-109">REG_DWORD</span><span class="sxs-lookup"><span data-stu-id="64a89-109">REG_DWORD</span></span>  <br/> |<span data-ttu-id="64a89-110">ét</span><span class="sxs-lookup"><span data-stu-id="64a89-110">1</span></span>  <br/> |

<span data-ttu-id="64a89-111">Hvis du vil have mere at vide, skal du se [aktivere moderne godkendelse for Office 2013 på Windows-enheder](https://docs.microsoft.com/microsoft-365/admin/security-and-compliance/enable-modern-authentication).</span><span class="sxs-lookup"><span data-stu-id="64a89-111">For more information, see [Enable Modern Authentication for Office 2013 on Windows devices](https://docs.microsoft.com/microsoft-365/admin/security-and-compliance/enable-modern-authentication).</span></span>
  
> [!NOTE]
>  <span data-ttu-id="64a89-112">ADAL er som standard aktiveret i Microsoft 365-apps til Enterprise og Office 2016.</span><span class="sxs-lookup"><span data-stu-id="64a89-112">ADAL is enabled by default in Microsoft 365 Apps for enterprise and Office 2016.</span></span> <span data-ttu-id="64a89-113">Fjernskrivebord-tjenester (RDS) har tidligere kaldt Terminal Services.</span><span class="sxs-lookup"><span data-stu-id="64a89-113">Remote Desktop Services (RDS) was previously named Terminal Services.</span></span>
  