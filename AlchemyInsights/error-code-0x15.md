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
description: Hvis du modtager en fejl, når du aktiverer Office 2013 på RDS-installationer (Remote Desktop Services), skal du overveje at aktivere ADAL ved at redigere registreringsdatabasen.
ms.openlocfilehash: ed3770c001461c162ff5bbe24dc400a29380a03b
ms.sourcegitcommit: ab75f66355116e995b3cb5505465b31989339e28
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 08/13/2021
ms.locfileid: "58316680"
---
# <a name="error-while-activation-office-2013-on-remote-desktop-services"></a>Fejl under aktivering Office 2013 på Fjernskrivebord-tjenester

Hvis du modtager en fejl, når du aktiverer Office 2013 på RDS-installationer (Remote Desktop Services), skal du overveje at aktivere ADAL ved at redigere registreringsdatabasen.
  
|**Registreringsdatabasenøgle**|**Type**|**Værdi**|
|:-----|:-----|:-----|
|HKEY_CURRENT_USER\Software\Microsoft\Office\15.0\Common\Identity\EnableADAL  <br/> |REG_DWORD  <br/> |1  <br/> |

Du kan få mere at [vide under Aktiver moderne godkendelse Office 2013 på Windows enheder.](https://docs.microsoft.com/microsoft-365/admin/security-and-compliance/enable-modern-authentication)
  
**Bemærk!** ADAL er som standard aktiveret i Microsoft 365 Apps for enterprise og Office 2016. Rds (Remote Desktop Services) hed tidligere Terminal Services.
  