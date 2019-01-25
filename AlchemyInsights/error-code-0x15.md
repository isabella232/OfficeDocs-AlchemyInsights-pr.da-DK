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
ms.sourcegitcommit: e2864efcfb493b6e46b662b746661a61232bdba7
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 01/24/2019
ms.locfileid: "29499376"
---
<span data-ttu-id="0702b-103">Hvis du modtager en fejl under aktivering af Office-2013 på Remote Desktop Services (RDS) installationer, kan du overveje at aktivere ADAL ved at redigere registreringsdatabasen.</span><span class="sxs-lookup"><span data-stu-id="0702b-103">If you're receiving an error while activating Office 2013 on Remote Desktop Services (RDS) deployments, consider enabling ADAL by editing the registry.</span></span> 
  
|<span data-ttu-id="0702b-104">**Nøgle i registreringsdatabasen**</span><span class="sxs-lookup"><span data-stu-id="0702b-104">**Registry key**</span></span>|<span data-ttu-id="0702b-105"> skriv </span><span class="sxs-lookup"><span data-stu-id="0702b-105">**Type**</span></span>|<span data-ttu-id="0702b-106">Værdi</span><span class="sxs-lookup"><span data-stu-id="0702b-106">**Value**</span></span>|
|:-----|:-----|:-----|
|<span data-ttu-id="0702b-107">HKEY_CURRENT_USER\Software\Microsoft\Office\15.0\Common\Identity\EnableADAL</span><span class="sxs-lookup"><span data-stu-id="0702b-107">HKEY_CURRENT_USER\Software\Microsoft\Office\15.0\Common\Identity\EnableADAL</span></span>  <br/> |<span data-ttu-id="0702b-108">REG_DWORD</span><span class="sxs-lookup"><span data-stu-id="0702b-108">REG_DWORD</span></span>  <br/> |<span data-ttu-id="0702b-109">1</span><span class="sxs-lookup"><span data-stu-id="0702b-109">1</span></span>  <br/> |
   
<span data-ttu-id="0702b-110">Yderligere oplysninger finder du under [Aktivere moderne godkendelse for 2013 til Office på Windows-enheder](https://docs.microsoft.com/office365/admin/security-and-compliance/enable-modern-authentication).</span><span class="sxs-lookup"><span data-stu-id="0702b-110">For more information, see [Enable Modern Authentication for Office 2013 on Windows devices](https://docs.microsoft.com/office365/admin/security-and-compliance/enable-modern-authentication).</span></span>
  
> [!NOTE]
>  <span data-ttu-id="0702b-p101">ADAL er aktiveret som standard i Office 365 ProPlus og Office 2016. > remote Desktop Services (RDS) blev tidligere kaldt Terminal Services.</span><span class="sxs-lookup"><span data-stu-id="0702b-p101">ADAL is enabled by default in Office 365 ProPlus and Office 2016. >  Remote Desktop Services (RDS) was previously named Terminal Services.</span></span> 
  

