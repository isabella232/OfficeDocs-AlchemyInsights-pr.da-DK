---
title: Ret 0x8004de40-fejl i OneDrive
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: ''
ms.openlocfilehash: 5da4271f242597b195ef61d553fd4a2ffb313025
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 04/22/2020
ms.locfileid: "43716022"
---
# <a name="fix-0x8004de40-error-in-onedrive"></a>Ret 0x8004de40-fejl i OneDrive

Hvis du får vist en 0x8004de40-fejl med OneDrive:

- Genstart den berørte computer, mens den er tilsluttet Acitve Directory-domænet.
- Hvis en genstart ikke løser problemet, skal du fjerne forbindelsen til din enhed og slutte sig til din enhed fra Azure AD. 

**Bemærk:** Du skal være på virksomhedens netværk, mens du udfører disse trin. Udfør ikke disse trin, når du ikke kan oprette forbindelse til virksomhedens infrastruktur (f.eks. under rejsen). 

- Åbn en kommandoprompt med en forhøjet kommando. 
- Hvis du vil åbne en kommandoprompt med administrator, skal du klikke på - **Start**, højreklikke på **Kommandoprompt**og derefter klikke på **Kør som administrator**.
- Skriv *dsregcmd /leave,* og tryk på **Enter**.
- Skriv *dsregcmd /join,* når den er fuldført, og tryk på **Enter**.
- Når kommandoprompten er fuldført, skal du lukke den.
- Genstart computeren, og log på OneDrive.