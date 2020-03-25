---
title: DLP skal muligvis bruge en brugerdefineret type
ms.author: pebaum
author: pebaum
manager: laurawi
ms.date: ''
ms.audience: ITPro
ms.topic: article
ms.prod: office-online-server
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1647"
- "3200001"
ms.assetid: ''
ms.openlocfilehash: 890bba57bc36c034c507e6124cd6593ef4d92af8
ms.sourcegitcommit: b0d5b68366028abcf08610672d5bc9d3b25ac433
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 03/24/2020
ms.locfileid: "42932652"
---
# <a name="dlp-might-need-a-custom-type"></a>DLP skal muligvis bruge en brugerdefineret type

**Vigtigt**: Mange SharePoint Online- og OneDrive-kunder kører forretningskritiske programmer mod den tjeneste, der kører i baggrunden. Disse omfatter indholdsmigrering, Forebyggelse af datatab (DLP) og sikkerhedskopieringsløsninger. I disse hidtil usete tider tager vi skridt til at sikre, at SharePoint Online- og OneDrive-tjenester forbliver meget tilgængelige og pålidelige for dine brugere, der er afhængige af tjenesten mere end nogensinde før i scenarier for fjernarbejde.

Til støtte for dette mål har vi implementeret strammere begrænsningsgrænser for baggrundsapps (migrering, DLP og backupløsninger) i dagtimerne på hverdage. Du bør forvente, at disse apps vil opnå meget begrænset gennemløb i disse tider. I løbet af aftenen og i weekenden for regionen vil tjenesten dog være klar til at behandle en betydeligt større mængde anmodninger fra baggrundsapps.

**DLP kan kræve en brugerdefineret oplysningstype**

Med en DLP-politik (Data Loss Prevention) kan du identificere og beskytte følsomme data i organisationen. I nogle scenarier skal du muligvis oprette din egen **brugerdefinerede** følsomme oplysningstype for at beskytte organisationens data.

bruge organisationen til at identificere og beskytte medarbejder-id'er eller andre data i et format, der er specifikt for din organisation. Hvis det er tilfældet, kan du finde flere oplysninger i følgende artikler.
  
 **Tilpasse en indbygget person af følsomme oplysninger**
  
Hvis en indbygget type følsomme oplysninger opfylder dine behov med nogle få justeringer, kan du [tilpasse en indbygget type følsomme oplysninger](https://docs.microsoft.com/office365/securitycompliance/customize-a-built-in-sensitive-information-type). tilføje eller fjerne søgeord eller tilføje eller fjerne dokumentation, f.eks.
  
 **Oprette en brugerdefineret følsom oplysningstype**
  
Men hvis du har brug for helt at identificere og beskytte en anden type følsomme oplysninger, kan du [oprette en brugerdefineret følsom oplysningstype](https://docs.microsoft.com/office365/securitycompliance/create-a-custom-sensitive-information-type) i brugergrænsefladen i Sikkerheds& Compliance Center.
  
**Oprette en brugerdefineret følsom oplysningstype i Security & Compliance Center PowerShell**

Hvis brugergrænsefladen ikke indeholder alle de indstillinger, du har brug for, kan du [oprette en brugerdefineret følsom oplysningstype i Security & Compliance Center PowerShell](https://docs.microsoft.com/office365/securitycompliance/create-a-custom-sensitive-information-type-in-scc-powershell). Ved at starte med en XML-fil kan du bruge alle tilgængelige indstillinger.
