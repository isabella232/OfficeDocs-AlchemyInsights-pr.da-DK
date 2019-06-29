---
title: Fejlkode 0x15
ms.author: pebaum
author: pebaum
ms.date: 10/31/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "919"
- "2000022"
ms.assetid: 0d566afe-b21f-4f1b-8ca9-4b4d3b0f5435
description: Hvis du modtager en fejl under aktivering af Office-2013 på Remote Desktop Services (RDS) installationer, kan du overveje at aktivere ADAL ved at redigere registreringsdatabasen.
ms.openlocfilehash: e2249d8ebbd2313c64dda5656a3243fa76d97a9a
ms.sourcegitcommit: 5fb7a4b28859690020efdea630d03e70cc0e6334
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 06/28/2019
ms.locfileid: "35388239"
---
<span data-ttu-id="d8fe2-103">Hvis du modtager en fejl under aktivering af Office-2013 på Remote Desktop Services (RDS) installationer, kan du overveje at aktivere ADAL ved at redigere registreringsdatabasen.</span><span class="sxs-lookup"><span data-stu-id="d8fe2-103">If you're receiving an error while activating Office 2013 on Remote Desktop Services (RDS) deployments, consider enabling ADAL by editing the registry.</span></span>
  
|<span data-ttu-id="d8fe2-104">**Nøgle i registreringsdatabasen**</span><span class="sxs-lookup"><span data-stu-id="d8fe2-104">**Registry key**</span></span>|<span data-ttu-id="d8fe2-105">**Type**</span><span class="sxs-lookup"><span data-stu-id="d8fe2-105">**Type**</span></span>|<span data-ttu-id="d8fe2-106">**Værdi**</span><span class="sxs-lookup"><span data-stu-id="d8fe2-106">**Value**</span></span>|
|:-----|:-----|:-----|
|<span data-ttu-id="d8fe2-107">HKEY_CURRENT_USER\Software\Microsoft\Office\15.0\Common\Identity\EnableADAL</span><span class="sxs-lookup"><span data-stu-id="d8fe2-107">HKEY_CURRENT_USER\Software\Microsoft\Office\15.0\Common\Identity\EnableADAL</span></span>  <br/> |<span data-ttu-id="d8fe2-108">REG_DWORD</span><span class="sxs-lookup"><span data-stu-id="d8fe2-108">REG_DWORD</span></span>  <br/> |<span data-ttu-id="d8fe2-109">1</span><span class="sxs-lookup"><span data-stu-id="d8fe2-109">1</span></span>  <br/> |

<span data-ttu-id="d8fe2-110">Yderligere oplysninger finder du under [Aktivere moderne godkendelse for 2013 til Office på Windows-enheder](https://docs.microsoft.com/office365/admin/security-and-compliance/enable-modern-authentication).</span><span class="sxs-lookup"><span data-stu-id="d8fe2-110">For more information, see [Enable Modern Authentication for Office 2013 on Windows devices](https://docs.microsoft.com/office365/admin/security-and-compliance/enable-modern-authentication).</span></span>
  
> [!NOTE]
>  <span data-ttu-id="d8fe2-111">ADAL er aktiveret som standard i Office 365 ProPlus og Office 2016.</span><span class="sxs-lookup"><span data-stu-id="d8fe2-111">ADAL is enabled by default in Office 365 ProPlus and Office 2016.</span></span> <span data-ttu-id="d8fe2-112">> remote Desktop Services (RDS) blev tidligere kaldt Terminal Services.</span><span class="sxs-lookup"><span data-stu-id="d8fe2-112">>  Remote Desktop Services (RDS) was previously named Terminal Services.</span></span>
  