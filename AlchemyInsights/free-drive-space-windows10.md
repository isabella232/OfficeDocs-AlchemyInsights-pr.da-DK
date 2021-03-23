---
title: Frier plads på drevet i Windows 10
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
- "9005403"
ms.openlocfilehash: 3838f3db3bc5f54bcb1a2558484056f3194b76e1
ms.sourcegitcommit: c08bed4071baa3bb5879496df3ed44fb828c8367
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 03/19/2021
ms.locfileid: "51035665"
---
# <a name="free-up-drive-space-in-windows-10"></a>Frier plads på drevet i Windows 10

Her er to muligheder for at frigøre plads på drevet i Windows:

- Frier plads på drevet i Windows 10.
- Frier plads til Windows 10-opdateringer med en ekstern lagerenhed.

Hvis du stadig har for lidt diskplads efter brug af Diskoprydning, er det muligt, at din Temp-mappe hurtigt bliver fyldt med programfiler (.appx), der bruges af Microsoft Store. Du kan løse dette problem ved at nulstille Store, rydde Store-cachen og derefter køre Windows Update-fejlfindingsværktøjet. Sørg for, at Microsoft Store er lukket, før du fortsætter med disse trin.

**Trin 1: Nulstil Microsoft Store**

**Bemærk!** Dette sletter appdataene på enheden permanent, herunder dine indstillinger og logonoplysninger.

1. Vælg **Start indstillinger**  >  **for**  >  **apps** og &  >  **funktioner.**

1. Find og vælg Microsoft Store på listen over apps.

1. Vælg **Avancerede indstillinger.**

1. Rul ned, vælg **Nulstil,** og **bekræft derefter nulstilling.**

**Trin 2: Ryd Microsoft Store-cachen**

1. Tryk på Windows-tasten + R for at åbne dialogboksen Kør.

1. Skriv wsreset.exe, og vælg **OK.**

1. Der åbnes et tomt kommandopromptvindue. Efter ca. 10 sekunder lukkes vinduet, og Store åbnes automatisk.

**Trin 3: Nulstil Windows Update**

1. Vælg **Opdatering af**  >    >  **startindstillinger & Sikkerhedsfejlfinding.**  >  

1. Rul ned, **og vælg Windows Update** på listen, og vælg Kør **fejlfindingsværktøjet.**

1. Genstart computeren, og kontrollér, om du stadig oplever problemet.

