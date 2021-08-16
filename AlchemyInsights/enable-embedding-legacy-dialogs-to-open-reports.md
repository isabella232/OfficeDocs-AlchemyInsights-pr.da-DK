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
ms.openlocfilehash: e1ad34e8a5cefe168b86727ac3ca208d90f8d4478696cef58a7d0b04475fba56
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 08/05/2021
ms.locfileid: "54003383"
---
# <a name="enable-embedding-legacy-dialogs-to-open-reports"></a>Aktivere integrering af ældre dialogbokse for at åbne rapporter

**Symptom**

Brugerne kan ikke åbne rapporter. "Noget er gået galt. Kontrollér de tekniske detaljer for at få flere oplysninger."

**Årsag**

Rapporter indlæses ikke i UCI med fejlen "Formularbeskrivelse er null eller ikke defineret." Rapporter i UCI kræver stadig ældre dialogbokse, så kundens system skal have *aktiveret tilladlegacydialogsembedding.*

**Løsning**

1. Gå til **Indstillinger >Administration > Indstillinger > Generelt.**

2. Angiv "Aktivér integrering af visse ældre dialogbokse i Unified Interface-browserklienten" til **Ja**.
