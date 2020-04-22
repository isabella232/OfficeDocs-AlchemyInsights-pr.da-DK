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
# <a name="error-while-activation-office-2013-on-remote-desktop-services"></a>Der opstod en fejl under aktivering af Office 2013 på Fjernskrivebord-tjenester

Hvis du modtager en fejl under aktivering af Office 2013 på RDS-installationer (Remote Desktop Services), kan du overveje at aktivere ADAL ved at redigere registreringsdatabasen.
  
|**Registreringsdatabasenøgle**|**Type**|**Værdi**|
|:-----|:-----|:-----|
|HKEY_CURRENT_USER\Software\Microsoft\Office\15.0\Common\Identity\EnableADAL  <br/> |Reg_dword  <br/> |1  <br/> |

Yderligere oplysninger finder du [i Enable Modern Authentication for Office 2013 on Windows devices](https://docs.microsoft.com/office365/admin/security-and-compliance/enable-modern-authentication).
  
> [!NOTE]
>  ADAL er som standard aktiveret i Microsoft 365 Apps til virksomheder og Office 2016. RDS (Remote Desktop Services) hed tidligere Terminal Services.
  