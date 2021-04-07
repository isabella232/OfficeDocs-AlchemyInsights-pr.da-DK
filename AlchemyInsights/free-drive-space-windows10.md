---
title: Frigøre plads på drevet i Windows 10
ms.author: pebaum
author: pebaum
manager: dansimp
ms.date: 03/16/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9771"
- "9774"
- "9005390"
- "9005403"
ms.openlocfilehash: 2313636307bfddce2810c2d4c4ce9e3b407a7bdf
ms.sourcegitcommit: 7b2e5078dd65f11af6650e692a7ea48e91f544e0
ms.translationtype: HT
ms.contentlocale: da-DK
ms.lasthandoff: 04/02/2021
ms.locfileid: "51505350"
---
# <a name="free-up-drive-space-in-windows-10"></a>Frigøre plads på drevet i Windows 10

Her er to muligheder for at frigøre plads på harddisken i Windows:

- Frigøre plads på drevet i Windows 10.
- Frigør plads til Windows 10-opdateringer med ekstern lagerenhed.

Hvis du stadig har lav diskplads efter brug af diskoprydning, er det muligt, at din Temp-mappe hurtigt udfylder programfiler (.appx), der bruges af Microsoft Store. Du kan løse dette problem ved at nulstille Store, rydde Store-cachen og derefter køre fejlfindingsværktøjet Windows Update. Sørg for, at Microsoft Store er lukket, før du fortsætter med disse trin.

**Trin 1: Nulstil Microsoft Store**

**Bemærk** Dette sletter appdataene på enheden permanent, herunder dine præferencer og logon-oplysninger.

1. Vælg **Start** > **Indstillinger** > **Apps** > **Apps og funktioner**.

1. Find og vælg Microsoft Store på listen over apps.

1. Vælg **Avancerede indstillinger**.

1. Rul ned, og vælg **Nulstil**, og **Bekræft nulstil**.

**Trin 2: Ryd Microsoft Store-cachen**

1. Tryk på Windows-logotasten + R for at åbne dialogboksen Kør.

1. Skriv wsreset.exe, og vælg **OK**.

1. Der åbnes et tomt kommandoprompt-vindue. Efter ca. 10 sekunder lukkes vinduet, og Store åbnes automatisk.

**Trin 3: Nulstil Windows Update**

1. Vælg **Start** > **Indstillinger** > **Opdatering og sikkerhed for** > **fejlfinding**.

1. Rul ned, og vælg **Windows Update** på listen, og vælg **Kør fejlfinding**.

1. Genstart computeren, og kontrollér, om du stadig oplever problemet.

