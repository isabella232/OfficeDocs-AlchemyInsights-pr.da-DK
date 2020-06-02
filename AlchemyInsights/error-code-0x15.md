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
description: Hvis du modtager en fejl under aktivering af RDS-installationer (Office 2013 on Remote Desktop Services), kan du overveje at aktivere ADAL ved at redigere registreringsdatabasen.
ms.openlocfilehash: 468d13e59602cf173ed2e17af44c66babfc28703
ms.sourcegitcommit: bc7d6f4f3c9f7060d073f5130e1ec856e248d020
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 06/02/2020
ms.locfileid: "44506840"
---
# <a name="error-while-activation-office-2013-on-remote-desktop-services"></a>Fejl under aktivering af Office 2013 på Fjernskrivebord-tjenester

Hvis du modtager en fejl under aktivering af RDS-installationer (Office 2013 on Remote Desktop Services), kan du overveje at aktivere ADAL ved at redigere registreringsdatabasen.
  
|**Registreringsdatabasenøgle**|**Type**|**Værdi**|
|:-----|:-----|:-----|
|HKEY_CURRENT_USER\Software\Microsoft\Office\15.0\Common\Identity\EnableADAL  <br/> |Reg_dword  <br/> |1  <br/> |

Du kan finde flere oplysninger under [Aktivere moderne godkendelse til Office 2013 på Windows-enheder](https://docs.microsoft.com/microsoft-365/admin/security-and-compliance/enable-modern-authentication).
  
> [!NOTE]
>  ADAL er som standard aktiveret i Microsoft 365 Apps til virksomheder og Office 2016. RDS (Remote Desktop Services) hed tidligere Terminal Services.
  