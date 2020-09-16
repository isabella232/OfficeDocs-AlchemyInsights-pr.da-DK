---
title: Store SharePoint-lister
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
ms.openlocfilehash: 1bc891a912c6753ea6c85d7d4b2a5d802080bd5c
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 09/14/2020
ms.locfileid: "47720127"
---
# <a name="work-with-large-lists-and-libraries-in-sharepoint"></a>Arbejde med store lister og biblioteker i SharePoint

SharePoint-lister og-biblioteker kan indeholde op til 30.000.000 elementer, men når de har mere end 5.000 elementer, får du muligvis vist en grænseværdi for listevisning, når du forsøger at arbejde med dem. Denne grænseværdi er der for at opretholde tjenestens ydeevne. Den kan ikke ændres. Sådan undgår du at bruge denne grænse:

**Brug moderne**

Visninger, der viser mange elementer, fungerer bedst i den moderne oplevelse. [Brug den moderne oplevelse](https://support.office.com/article/66dac24b-4177-4775-bf50-3d267318caa9) til at undgå fejl, du kan se i den klassiske oplevelse.

**Tilføje indeks**

Når du filtrerer eller sorterer efter en kolonne, der ikke har et indeks, får du muligvis vist en fejlmeddelelse. [Tilføje et indeks](https://support.office.com/article/f3f00554-b7dc-44d1-a2ed-d477eac463b0) manuelt fra **Listeindstillinger** i menuen Indstillinger og derefter **Indekserede kolonner**.

**Redigere listevisningen**

Hvis der opstår en fejl, når du arbejder med en stor liste, skal du [redigere listevisningen](https://support.office.com/article/15916903-e79a-423f-b4e2-02d37e1ff372).

De følgende fire ændringer fjerner fejl i liste visnings tærskelværdien. Gør alle fire ændringer for at fjerne alle fejl. Hvis du stadig får fejl, skal du kontrollere [Administrer store lister og biblioteker](https://support.office.com/article/B8588DAE-9387-48C2-9248-C24122F07C59).

1. Markér **ingen** fra både **den første sortering efter kolonnen** , og **Sortér derefter efter kolonnen**.
2. Markér **ingen** af dem **først i den første gruppe efter kolonne** , og **Gruppér efter kolonne**.
3. Vælg **ingen** for alle kolonner i sektionen **Totaler** .
4. Fjern markeringen af alle kolonnerne undtagen én, der skal vises i sektionen **kolonner** .

