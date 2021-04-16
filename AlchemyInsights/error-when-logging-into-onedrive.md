---
title: 0x8004de40, når du starter OneDrive
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "6886"
- "9003837"
ms.openlocfilehash: e329d7fe881a0fc9514584e06aa2d6e8ebab5b11
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 04/15/2021
ms.locfileid: "51813646"
---
# <a name="0x8004de40-error-when-launching-onedrive"></a>0x8004de40, når du starter OneDrive

Hvis du modtager en fejlmeddelelse **om 0x8004de40** når du logger på OneDrive, skal du genstarte computeren, mens du har forbindelse til dit arbejds- eller skoledomæne. Hvis du får vist denne fejl efter genstart, kan du prøve dette, mens du har forbindelse til dit arbejds- eller skoledomæne:

1. Klik på Start, og **skriv cmd** eller **kommandoprompt** i søgefeltet, højreklik på appen kommandoprompt, og **vælg Kør som administrator.** Hvis du bliver bedt om at angive en administratoradgangskode eller en bekræftelse, skal du skrive adgangskoden eller klikke på **Tillad.**  

2. I vinduet Kommandoprompt skal du **skrive dsregcmd /leave**  og vente på, at kommandoen fuldføres. Skriv derefter **dsregcmd /join,** og vent på, at kommandoen fuldføres.
3. Genstart computeren.
