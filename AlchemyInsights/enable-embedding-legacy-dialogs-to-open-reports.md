---
title: Aktivere integrering af ældre dialogbokse for at åbne rapporter
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9002931"
- "5612"
ms.openlocfilehash: c8a5634d5d79cbd584284b675e5db4e448a0d157
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 04/15/2021
ms.locfileid: "51814258"
---
# <a name="enable-embedding-legacy-dialogs-to-open-reports"></a>Aktivere integrering af ældre dialogbokse for at åbne rapporter

**Symptom**

Brugerne kan ikke åbne rapporter. "Noget er gået galt. Kontrollér de tekniske detaljer for at få flere oplysninger."

**Årsag**

Rapporter indlæses ikke i UCI med fejlen "Formularbeskrivelse er null eller ikke defineret." Rapporter i UCI kræver stadig ældre dialogbokse, så kundens system skal have *aktiveret tilladlegacydialogsembedding.*

**Løsning**

1. Gå til **Indstillinger >administration > fanen Systemindstillinger > Generelt.**

2. Angiv "Aktivér integrering af visse ældre dialogbokse i Unified Interface-browserklienten" til **Ja**.
