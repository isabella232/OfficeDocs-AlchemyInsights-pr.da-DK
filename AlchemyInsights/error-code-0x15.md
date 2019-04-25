---
title: Fejlkode 0x15
ms.author: pebaum
author: pebaum
ms.date: 10/31/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 0d566afe-b21f-4f1b-8ca9-4b4d3b0f5435
description: Hvis du modtager en fejl under aktivering af Office-2013 på Remote Desktop Services (RDS) installationer, kan du overveje at aktivere ADAL ved at redigere registreringsdatabasen.
ms.openlocfilehash: 6d4076ecb5c6ee3c3cf4c4610ad4aa29ab477d8a
ms.sourcegitcommit: 9d78905c512192ffc4675468abd2efc5f2e4baf4
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 04/23/2019
ms.locfileid: "32402733"
---
<span data-ttu-id="4e17e-103">Hvis du modtager en fejl under aktivering af Office-2013 på Remote Desktop Services (RDS) installationer, kan du overveje at aktivere ADAL ved at redigere registreringsdatabasen.</span><span class="sxs-lookup"><span data-stu-id="4e17e-103">If you're receiving an error while activating Office 2013 on Remote Desktop Services (RDS) deployments, consider enabling ADAL by editing the registry.</span></span> 
  
|<span data-ttu-id="4e17e-104">**Nøgle i registreringsdatabasen**</span><span class="sxs-lookup"><span data-stu-id="4e17e-104">**Registry key**</span></span>|<span data-ttu-id="4e17e-105">**Type**</span><span class="sxs-lookup"><span data-stu-id="4e17e-105">**Type**</span></span>|<span data-ttu-id="4e17e-106">**Værdi**</span><span class="sxs-lookup"><span data-stu-id="4e17e-106">**Value**</span></span>|
|:-----|:-----|:-----|
|<span data-ttu-id="4e17e-107">HKEY_CURRENT_USER\Software\Microsoft\Office\15.0\Common\Identity\EnableADAL</span><span class="sxs-lookup"><span data-stu-id="4e17e-107">HKEY_CURRENT_USER\Software\Microsoft\Office\15.0\Common\Identity\EnableADAL</span></span>  <br/> |<span data-ttu-id="4e17e-108">REG_DWORD</span><span class="sxs-lookup"><span data-stu-id="4e17e-108">REG_DWORD</span></span>  <br/> |<span data-ttu-id="4e17e-109">1</span><span class="sxs-lookup"><span data-stu-id="4e17e-109">1</span></span>  <br/> |
   
<span data-ttu-id="4e17e-110">Yderligere oplysninger finder du under [Aktivere moderne godkendelse for 2013 til Office på Windows-enheder](https://docs.microsoft.com/office365/admin/security-and-compliance/enable-modern-authentication).</span><span class="sxs-lookup"><span data-stu-id="4e17e-110">For more information, see [Enable Modern Authentication for Office 2013 on Windows devices](https://docs.microsoft.com/office365/admin/security-and-compliance/enable-modern-authentication).</span></span>
  
> [!NOTE]
>  <span data-ttu-id="4e17e-111">ADAL er aktiveret som standard i Office 365 ProPlus og Office 2016.</span><span class="sxs-lookup"><span data-stu-id="4e17e-111">ADAL is enabled by default in Office 365 ProPlus and Office 2016.</span></span> <span data-ttu-id="4e17e-112">> remote Desktop Services (RDS) blev tidligere kaldt Terminal Services.</span><span class="sxs-lookup"><span data-stu-id="4e17e-112">>  Remote Desktop Services (RDS) was previously named Terminal Services.</span></span> 
  

