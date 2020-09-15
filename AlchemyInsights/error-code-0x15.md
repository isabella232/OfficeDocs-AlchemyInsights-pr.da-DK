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
# <a name="error-while-activation-office-2013-on-remote-desktop-services"></a>Fejl under aktivering af Office 2013 på Fjernskrivebord-tjenester

Hvis du får en fejl, når du aktiverer Office 2013 på installation af Fjernskrivebord-tjenester (RDS), kan du overveje at aktivere ADAL ved at redigere registreringsdatabasen.
  
|**Registreringsdatabasenøgle**|**Indtaste**|**Talværdi**|
|:-----|:-----|:-----|
|HKEY_CURRENT_USER \Software\Microsoft\Office\15.0\Common\Identity\EnableADAL  <br/> |REG_DWORD  <br/> |ét  <br/> |

Hvis du vil have mere at vide, skal du se [aktivere moderne godkendelse for Office 2013 på Windows-enheder](https://docs.microsoft.com/microsoft-365/admin/security-and-compliance/enable-modern-authentication).
  
> [!NOTE]
>  ADAL er som standard aktiveret i Microsoft 365-apps til Enterprise og Office 2016. Fjernskrivebord-tjenester (RDS) har tidligere kaldt Terminal Services.
  