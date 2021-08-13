---
title: Tilbagetrækning af adgang til tjenester
ms.author: pebaum
author: pebaum
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "9000356"
- "2009"
ms.assetid: ''
ms.openlocfilehash: 32da879de230dc0ed99563ad881ab5b2479b8453933a127961a26d619e108ab9
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 08/05/2021
ms.locfileid: "53938689"
---
# <a name="access-services-retirement"></a>Tilbagetrækning af adgang til tjenester

Som vi oprindeligt annoncerede i MC97576 i marts 2017 og fortsat kommunikerede i løbet af det sidste år, Access-tjenester nu udgå. Den næste fase i denne proces bliver fjernelse af Access-webdatabaser, der bruger SharePoint lister som deres underliggende datalager.

**Hvordan påvirker det mig?**

Fra og med juni 2019 stopper vi oprettelsen af nye Access-databaser i SharePoint Online og lukker tjenesten og eventuelle resterende apps inden april 2020.

**Hvad skal jeg gøre for at forberede denne ændring?**

Vi opfordrer dig til at oprette en overgangsplan til din organisations Access-webdatabaser. Administratorer kan bruge [Access SharePoint appscanneren](https://github.com/SharePoint/PnP-Tools/tree/master/Solutions/SharePoint.AccessApp.Scanner) til at få en oversigt over de Access-apps, som webstederne bruger.

Der er flere måder at overføre Access-webdatabasedata på:

- Importere til en lokal Access-database (. ACCDB) eller i en Excel fil.
- Vi anbefaler også at Microsoft PowerApps som en alternativ platform til at oprette virksomhedsløsninger uden brug af kode til web- og mobilenheder.