---
title: Store SharePoint-lister
ms.author: toresing
author: tomresing
manager: scotv
ms.date: 2/12/2018
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "407"
- "530001"
ms.assetid: ee07bf74-7aeb-4c47-8f5d-f496d6c09d79
ms.openlocfilehash: 222ad554de0d94dcfd4e34e9a2c6aa8ab4e6f81f
ms.sourcegitcommit: d7e1b097d3866782f508527c797426dc56c6ba17
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 10/14/2019
ms.locfileid: "37488511"
---
# <a name="work-with-large-lists-and-libraries-in-sharepoint"></a>Arbejde med store lister og biblioteker i SharePoint

SharePoint-lister og-biblioteker kan indeholde op til 30.000.000 elementer, men når de har mere end 5.000 elementer, får du muligvis vist en tærskel fejl for listevisning, når du forsøger at arbejde med dem. Denne tærskel er på plads for at opretholde ydelsen af tjenesten. Det kan ikke ændres. For at undgå at ramme denne tærskel:

**Bruge moderne**

Visninger, der viser mange elementer, fungerer bedst i den moderne oplevelse. [Brug den moderne oplevelse](https://support.office.com/article/66dac24b-4177-4775-bf50-3d267318caa9) for at undgå fejl, du kan se i den klassiske oplevelse.

**Tilføje indekser**

Når du filtrerer eller sorterer efter en kolonne, der ikke har et indeks, vises der muligvis en fejlmeddelelse. [Tilføj et indeks](https://support.office.com/article/f3f00554-b7dc-44d1-a2ed-d477eac463b0) manuelt fra **Listeindstillinger** i menuen Indstillinger og derefter **Indekserede kolonner**.

**Redigere listevisningen**

Hvis der opstår en fejl, når du arbejder med en stor liste, bør du [redigere listevisningen](https://support.office.com/article/15916903-e79a-423f-b4e2-02d37e1ff372).

De følgende fire ændringer vil fjerne tærskel fejl for listevisning. Foretag alle fire ændringer for at fjerne alle fejl. Hvis du stadig får fejl, skal du kontrollere [Administrer store lister og biblioteker](https://support.office.com/article/B8588DAE-9387-48C2-9248-C24122F07C59).

1. Vælg **ingen** fra begge **første sorter efter kolonnen** , og **Sortér derefter efter kolonnen**.
2. Vælg **ingen** fra begge **første grupper efter kolonnen** , og **Gruppér derefter efter kolonnen**.
3. Vælg **ingen** for alle kolonner i afsnittet **Totaler** .
4. Fravælg alle, men én kolonne til visning fra sektionen **kolonner** .

