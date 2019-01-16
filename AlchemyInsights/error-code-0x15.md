---
title: Fejlkode 0x15
ms.author: pebaum
author: pebaum
ms.date: 10/31/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.assetid: 0d566afe-b21f-4f1b-8ca9-4b4d3b0f5435
description: Hvis du modtager en fejl under aktivering af Office-2013 på Remote Desktop Services (RDS) installationer, kan du overveje at aktivere ADAL ved at redigere registreringsdatabasen.
ms.openlocfilehash: 89f9270169e13fd7706f7826c624ef8ae4d47b3f
ms.sourcegitcommit: d6ea5e9458a2b8ceaab3ac4bd483e1130b9a398a
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 01/15/2019
ms.locfileid: "28282875"
---
<span data-ttu-id="d9d4c-103">Hvis du modtager en fejl under aktivering af Office-2013 på Remote Desktop Services (RDS) installationer, kan du overveje at aktivere ADAL ved at redigere registreringsdatabasen.</span><span class="sxs-lookup"><span data-stu-id="d9d4c-103">If you're receiving an error while activating Office 2013 on Remote Desktop Services (RDS) deployments, consider enabling ADAL by editing the registry.</span></span> 
  
|<span data-ttu-id="d9d4c-104">**Nøgle i registreringsdatabasen**</span><span class="sxs-lookup"><span data-stu-id="d9d4c-104">**Registry key**</span></span>|<span data-ttu-id="d9d4c-105">**Type**</span><span class="sxs-lookup"><span data-stu-id="d9d4c-105">**Type**</span></span>|<span data-ttu-id="d9d4c-106">**Værdi**</span><span class="sxs-lookup"><span data-stu-id="d9d4c-106">**Value**</span></span>|
|:-----|:-----|:-----|
|<span data-ttu-id="d9d4c-107">HKEY_CURRENT_USER\Software\Microsoft\Office\15.0\Common\Identity\EnableADAL</span><span class="sxs-lookup"><span data-stu-id="d9d4c-107">HKEY_CURRENT_USER\Software\Microsoft\Office\15.0\Common\Identity\EnableADAL</span></span>  <br/> |<span data-ttu-id="d9d4c-108">REG_DWORD</span><span class="sxs-lookup"><span data-stu-id="d9d4c-108">REG_DWORD</span></span>  <br/> |<span data-ttu-id="d9d4c-109">1</span><span class="sxs-lookup"><span data-stu-id="d9d4c-109">1</span></span>  <br/> |
   
<span data-ttu-id="d9d4c-110">Yderligere oplysninger finder du under [Aktivere moderne godkendelse for 2013 til Office på Windows-enheder](https://docs.microsoft.com/office365/admin/security-and-compliance/enable-modern-authentication).</span><span class="sxs-lookup"><span data-stu-id="d9d4c-110">For more information, see [Enable Modern Authentication for Office 2013 on Windows devices](https://docs.microsoft.com/office365/admin/security-and-compliance/enable-modern-authentication).</span></span>
  
> [!NOTE]
>  <span data-ttu-id="d9d4c-p101">ADAL er aktiveret som standard i Office 365 ProPlus og Office 2016. > Fjernskrivebord-tjenester (RDS) blev tidligere kaldt Terminal Services.</span><span class="sxs-lookup"><span data-stu-id="d9d4c-p101">ADAL is enabled by default in Office 365 ProPlus and Office 2016. >  Remote Desktop Services (RDS) was previously named Terminal Services.</span></span> 
  

