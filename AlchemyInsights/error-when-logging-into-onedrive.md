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
ms.openlocfilehash: 23c57356c8bd94c1cbafb538c9318208429754115a7c4e88abc93d293b5ea6e1
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 08/05/2021
ms.locfileid: "53946573"
---
# <a name="0x8004de40-error-when-launching-onedrive"></a>0x8004de40, når du starter OneDrive

Hvis du modtager en fejlmeddelelse, **0x8004de40,** når du logger på OneDrive, skal du genstarte computeren, mens du har forbindelse til dit arbejds- eller skoledomæne. Hvis du får vist denne fejl efter genstart, kan du prøve dette, mens du har forbindelse til dit arbejds- eller skoledomæne:

1. Klik på Start, og **skriv cmd** eller **kommandoprompt** i søgefeltet, højreklik på appen kommandoprompt, og **vælg Kør som administrator.** Hvis du bliver bedt om at angive en administratoradgangskode eller en bekræftelse, skal du skrive adgangskoden eller klikke på **Tillad.**  

2. I vinduet Kommandoprompt skal du **skrive dsregcmd /leave**  og vente på, at kommandoen fuldføres. Skriv derefter **dsregcmd /join,** og vent på, at kommandoen fuldføres.
3. Genstart computeren.
