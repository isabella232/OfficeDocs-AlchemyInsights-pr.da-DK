---
title: Drevforsendelse i Microsoft 365 Importtjeneste
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 06/01/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "11514"
- "9003046"
ms.openlocfilehash: 85d6e723e56b01fd9914165d8c9740f3b055947d
ms.sourcegitcommit: 1226e9a9601dc8fc8ec427235f3c2dd88ff84ced
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 06/02/2021
ms.locfileid: "52731440"
---
# <a name="drive-shipping-in-the-microsoft-365-import-service"></a>Drevforsendelse i Microsoft 365 Importtjeneste

Brug drevforsendelse ved at kopiere PST'er til en harddisk og derefter sende harddisken til Microsoft.

Sådan startes jobbet:

1. Vælg Importér Microsoft 365 i Center **for** overholdelse af regler og standarder under **Styring af oplysninger.**

1. Vælg **Vælg importjobtype**, og vælg derefter **Næste**.

1. Hvis du vil se trinnene for denne importindstilling, skal **du vælge Send harddiske til en af vores fysiske placeringer.**

Her er nogle ting, du skal huske:

- Du skal have tildelt rollen Postkasse Import Eksport i en Exchange Online for at importere PST-filer Microsoft 365 postkasser.
Ydeevnen kan påvirkes for PST'er, der er større end 20 GB.

- Kun 2,5"-solid state-drev (SSD'er) eller 2,5" eller 3,5" SATA II/III-interne harddiske understøttes.
Harddisk, der indeholder PST-filer, skal være krypteret BitLocker.

- Import af PST-filer til postkasser Microsoft 365 drevforsendelse koster 2 USD pr. GB data.

Du kan finde flere oplysninger om brug af drevforsendelsesmetode til import af PST'er i Brug drevforsendelse til at importere [din organisations PST-filer.](/microsoft-365/compliance/use-drive-shipping-to-import-pst-files-to-office-365)