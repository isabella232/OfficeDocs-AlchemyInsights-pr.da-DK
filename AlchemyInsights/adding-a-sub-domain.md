---
title: Tilføje et underdomæne
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
- "7"
- "13902"
ms.openlocfilehash: ea39984a54a15ae6167363eb5855943c8ab1120d
ms.sourcegitcommit: a097d1f8915a31ed8460b5b68dccc8d87e563cc0
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 09/22/2021
ms.locfileid: "59506327"
---
# <a name="adding-a-sub-domain"></a>Tilføje et underdomæne

Underdomæner kan føjes til den samme eller en anden lejer end det overordnede domæne. I begge tilfælde skal du administrere dine egne DNS-indstillinger på registratorens websted. Hvis du har ladet Microsoft administrere dine DNS-indstillinger med NS-poster, eller hvis du har købt domænet af Microsoft, kan du ikke tilføje underdomæner uden at ændre dette først.

Tilføj først det overordnede domæne, og tilføj derefter underdomænet. Hvis underdomænet er i samme lejer, kræves der ingen yderligere bekræftelse. Hvis du føjer underdomænet til en separat lejer, kræves DNS txt-posten for at bekræfte ejerskabet, før du tilføjer domænet og de ekstra DNS-poster for de tjenester, der er valgt.

- Hvis du vil tilføje et domæne eller underdomæne, skal du følge guiden [Tilføj](https://admin.microsoft.com/Adminportal#/Domains/Wizard)domæne eller tilføje domænet eller underdomænet manuelt ved at gå til **Indstilling** af  >  **domæner Tilføj**  >  **domæne.**

Hvis det er nødvendigt:

- Hvis du vil ændre, hvem der administrerer dine DNS-indstillinger for et eksisterende domæne, skal du gå til **Indstillinger**  >  [**Domains**](https://admin.microsoft.com/Adminportal/Home#/Domains), markere afkrydsningsfeltet ud for domænet og derefter vælge **Administrer DNS**. Vælg Tilføj dine egne **DNS-poster i guiden,** og fuldfør guiden.
- Hvis du vil føje underdomæner til et af Microsofts købte domæner, skal du først overføre domænet til en anden registrator og derefter foretage ændringen ovenfor for at administrere dine egne DNS-poster. Du kan finde en vejledning [under Overfør et domæne fra Microsoft til en anden vært](https://docs.microsoft.com/microsoft-365/admin/get-help-with-domains/transfer-a-domain-from-microsoft-to-another-host).
- Hvis du får en fejlmeddelelse om, at dit domæne allerede er i brug af andre medlemmer eller personer i organisationen, skal du først overtage denne ikke-administrerede konto, før du bruger domænet. Du kan finde en [vejledning under Overtage en ikke-administreret mappe som administrator i Azure Active Directory](https://docs.microsoft.com/azure/active-directory/enterprise-users/domains-admin-takeover).
