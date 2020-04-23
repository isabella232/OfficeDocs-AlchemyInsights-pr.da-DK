---
title: Store SharePoint-lister
ms.author: toresing
author: tomresing
manager: scotv
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "407"
- "530001"
ms.assetid: ee07bf74-7aeb-4c47-8f5d-f496d6c09d79
ms.openlocfilehash: e85686788c60d365a00970e9ffe58e97512894a3
ms.sourcegitcommit: 631cbb5f03e5371f0995e976536d24e9d13746c3
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 04/22/2020
ms.locfileid: "43767279"
---
# <a name="work-with-large-lists-and-libraries-in-sharepoint"></a>Arbejde med store lister og biblioteker i SharePoint

SharePoint-lister og -biblioteker kan indeholde op til 30 millioner elementer, men når de har mere end 5.000 elementer, får du muligvis vist en listevisningstærskelfejl, når du forsøger at arbejde med dem. Denne grænseværdi er der for at opretholde tjenestens ydeevne. Den kan ikke ændres. Sådan undgår du at ramme denne grænse:

**Brug moderne**

Visninger, der viser mange ting fungerer bedst i den moderne oplevelse. [Brug den moderne oplevelse](https://support.office.com/article/66dac24b-4177-4775-bf50-3d267318caa9) til at undgå fejl, du kan se i den klassiske oplevelse.

**Tilføje indeks**

Når du filtrerer eller sorterer efter en kolonne, der ikke har et indeks, vises der muligvis en fejlmeddelelse. [Tilføj et indeks](https://support.office.com/article/f3f00554-b7dc-44d1-a2ed-d477eac463b0) manuelt fra **Listeindstillinger** i indstillingsmenuen og derefter **indekserede kolonner**.

**Redigere listevisningen**

Hvis der opstår en fejl, når du arbejder med en stor liste, skal [du redigere listevisningen](https://support.office.com/article/15916903-e79a-423f-b4e2-02d37e1ff372).

Følgende fire ændringer fjerner listevisningstærskelfejl. Foretag alle fire ændringer for at fjerne alle fejl. Hvis du stadig får fejl, skal du markere [Administrer store lister og biblioteker](https://support.office.com/article/B8588DAE-9387-48C2-9248-C24122F07C59).

1. Vælg **Ingen** fra både **Første sortering efter kolonne** og Sorter derefter efter **kolonnen**.
2. Vælg **Ingen** fra både **første gruppe efter kolonne** og derefter **grupperefter kolonne**.
3. Vælg **Ingen** for alle kolonner i sektionen **Totaler.**
4. Fravælg alle kolonner undtagen én, der skal vises, i sektionen **Kolonner.**

