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
# <a name="enable-embedding-legacy-dialogs-to-open-reports"></a><span data-ttu-id="c7015-102">Aktivere integrering af ældre dialogbokse for at åbne rapporter</span><span class="sxs-lookup"><span data-stu-id="c7015-102">Enable embedding legacy dialogs to open reports</span></span>

<span data-ttu-id="c7015-103">**Symptom**</span><span class="sxs-lookup"><span data-stu-id="c7015-103">**Symptom**</span></span>

<span data-ttu-id="c7015-104">Brugerne kan ikke åbne rapporter.</span><span class="sxs-lookup"><span data-stu-id="c7015-104">Users are unable to open reports.</span></span> <span data-ttu-id="c7015-105">"Noget er gået galt.</span><span class="sxs-lookup"><span data-stu-id="c7015-105">"Something has gone wrong.</span></span> <span data-ttu-id="c7015-106">Kontrollér de tekniske detaljer for at få flere oplysninger."</span><span class="sxs-lookup"><span data-stu-id="c7015-106">Check technical details for more details."</span></span>

<span data-ttu-id="c7015-107">**Årsag**</span><span class="sxs-lookup"><span data-stu-id="c7015-107">**Cause**</span></span>

<span data-ttu-id="c7015-108">Rapporter indlæses ikke i UCI med fejlen "Formularbeskrivelse er null eller ikke defineret."</span><span class="sxs-lookup"><span data-stu-id="c7015-108">Reports are failing to load in UCI with the error, "Form descriptor is null or not defined."</span></span> <span data-ttu-id="c7015-109">Rapporter i UCI kræver stadig ældre dialogbokse, så kundens system skal have *aktiveret tilladlegacydialogsembedding.*</span><span class="sxs-lookup"><span data-stu-id="c7015-109">Reports in UCI still require legacy dialogs, so the customer's system needs to have *allowlegacydialogsembedding* enabled.</span></span>

<span data-ttu-id="c7015-110">**Løsning**</span><span class="sxs-lookup"><span data-stu-id="c7015-110">**Solution**</span></span>

1. <span data-ttu-id="c7015-111">Gå til **Indstillinger >administration > fanen Systemindstillinger > Generelt.**</span><span class="sxs-lookup"><span data-stu-id="c7015-111">Go to **Settings >Administration > System Settings > General tab**.</span></span>

2. <span data-ttu-id="c7015-112">Angiv "Aktivér integrering af visse ældre dialogbokse i Unified Interface-browserklienten" til **Ja**.</span><span class="sxs-lookup"><span data-stu-id="c7015-112">Set "Enable embedding of certain legacy dialogs in Unified Interface browser client" to **Yes**.</span></span>
