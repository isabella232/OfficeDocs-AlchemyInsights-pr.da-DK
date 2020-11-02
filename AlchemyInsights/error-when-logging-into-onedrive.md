---
title: 0x8004de40-fejl ved start af OneDrive
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "6886"
- "9003837"
ms.openlocfilehash: f689fcf9432e9b356843efe73ed0f79a32735e6f
ms.sourcegitcommit: 1ac3474897abb7c4969e222f934294e05f468536
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 10/30/2020
ms.locfileid: "48823016"
---
# <a name="0x8004de40-error-when-launching-onedrive"></a>0x8004de40-fejl ved start af OneDrive

Hvis du modtager en fejl **0x8004de40** , når du logger på OneDrive, skal du genstarte computeren, mens du har forbindelse til dit arbejds-eller skole domæne. Hvis du får denne fejl, når du har genstartet, kan du prøve dette, mens du har forbindelse til dit arbejds-eller skole domæne:

1. Klik på Start, og Skriv **cmd** eller **kommandoprompt**  i søgefeltet, Højreklik på appen kommandoprompt, og vælg  **Kør som administrator** . Hvis du bliver bedt om at angive en administratoradgangskode eller en bekræftelse, skal du skrive adgangskoden eller klikke på **Tillad** .  

2. I kommando prompt vinduet skal du skrive **dsregcmd/Leave**  og vente på, at kommandoen fuldføres. Skriv derefter **dsregcmd/join** , og vent på, at kommandoen fuldføres.
3. Genstart computeren.
