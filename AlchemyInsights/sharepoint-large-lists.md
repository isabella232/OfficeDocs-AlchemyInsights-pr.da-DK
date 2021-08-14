---
title: SharePoint store lister
ms.author: toresing
author: tomresing
manager: scotv
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "407"
- "530001"
ms.assetid: ee07bf74-7aeb-4c47-8f5d-f496d6c09d79
ms.openlocfilehash: c67632e323f2068faba06779b94ba4fd8e9f319e18cefb7977bd3038ca770210
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 08/05/2021
ms.locfileid: "53941562"
---
# <a name="work-with-large-lists-and-libraries-in-sharepoint"></a>Arbejd med store lister og biblioteker i SharePoint

SharePoint lister og biblioteker kan indeholde op til 30 millioner elementer, men når de har mere end 5.000 elementer, vises der muligvis en fejl i Grænseværdi for listevisning, når du forsøger at arbejde med dem. Denne grænseværdi er der for at opretholde tjenestens ydeevne. Den kan ikke ændres. Sådan undgår du at nå denne grænseværdi:

**Brug moderne**

Visninger, der viser mange elementer fungerer bedst i den moderne oplevelse. [Brug den moderne oplevelse](https://support.office.com/article/66dac24b-4177-4775-bf50-3d267318caa9) for at undgå fejl, som du kan se i den klassiske oplevelse.

**Tilføj indekser**

Når du filtrerer eller sorterer efter en kolonne, der ikke har et indeks, får du muligvis vist en fejlmeddelelse. [Tilføj et indeks](https://support.office.com/article/f3f00554-b7dc-44d1-a2ed-d477eac463b0) manuelt **fra liste Indstillinger** i menuen Indstillinger og derefter **Indekserede kolonner**.

**Rediger listevisningen**

Hvis der opstår en fejl, når du arbejder med en stor liste, [skal du redigere listevisningen.](https://support.office.com/article/15916903-e79a-423f-b4e2-02d37e1ff372)

Følgende fire ændringer fjerner grænseværdien for listevisning. Foretag alle fire ændringer for at fjerne alle fejl. Hvis du stadig får fejl, skal du markere [Administrer store lister og biblioteker.](https://support.office.com/article/B8588DAE-9387-48C2-9248-C24122F07C59)

1. Vælg **Ingen** fra begge **Sortér først efter kolonnen,** **og sortér derefter efter kolonnen**.
2. Vælg **Ingen** fra begge **Grupper først efter kolonnen,** og **grupperer derefter efter kolonnen**.
3. Vælg **Ingen** for alle kolonner i **sektionen Totaler.**
4. Fravælg alle andre kolonner end én visning fra **sektionen** Kolonner.

