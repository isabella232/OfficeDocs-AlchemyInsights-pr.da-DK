---
title: DLP skal muligvis bruge en brugerdefineret type
ms.author: pebaum
author: pebaum
manager: laurawi
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1647"
- "3200001"
ms.assetid: ''
ms.openlocfilehash: 72b16d437f97de27cbdc364f022c3e2059b31ef0
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 09/14/2020
ms.locfileid: "47712178"
---
# <a name="dlp-might-need-a-custom-type"></a>DLP skal muligvis bruge en brugerdefineret type

**Vigtigt**: I disse hidtil usete tider bestræber vi os på at sikre, at SharePoint Online- og OneDrive-tjenesterne fastholder sin høje tilgængelighed. Hvis du ønsker flere oplysninger, skal du besøge [Midlertidige funktionsjusteringer i SharePoint Online](https://aka.ms/ODSPAdjustments).

**DLP kræver muligvis en brugerdefineret oplysningstype**

Med en politik til forebyggelse af datatab (DLP) kan du identificere og beskytte følsomme data i organisationen. I visse scenarier kan det være nødvendigt at oprette din egen **brugerdefinerede** type fortrolige oplysninger for at beskytte din organisationsdata.

For eksempel skal din organisation muligvis identificere og beskytte medarbejder-id'er eller andre data i et hvilket som helst format, der er specifikt for din organisation. Hvis det er tilfældet, skal du se følgende artikler for at få flere oplysninger.
  
 **Tilpasse en indbygget type af følsomme oplysninger**
  
Hvis en indbygget følsom oplysningstype opfylder dine behov med blot nogle få tilpasninger, kan du [tilpasse en indbygget type af følsomme oplysninger](https://docs.microsoft.com/microsoft-365/compliance/customize-a-built-in-sensitive-information-type). Du kan f. eks. tilføje eller fjerne nøgleord eller tilføje eller fjerne dokumentation, som f. eks en dato eller adresse.
  
 **Oprette en brugerdefineret følsom oplysningstype**
  
Men hvis du har brug for at identificere og beskytte en anden type følsomme oplysninger, kan du [oprette en brugerdefineret følsom oplysningstype](https://docs.microsoft.com/microsoft-365/compliance/create-a-custom-sensitive-information-type) i brugergrænsefladen for sikkerheds & overholdelses Center.
  
**Oprette en brugerdefineret følsom oplysningstype i sikkerhed & overholdelses Center PowerShell**

Hvis BRUGERGRÆNSEFLADEN ikke indeholder alle de indstillinger, du har brug for, kan du [oprette en brugerdefineret følsom oplysningstype i sikkerhed & overholdelses Center-PowerShell](https://docs.microsoft.com/microsoft-365/compliance/create-a-custom-sensitive-information-type-in-scc-powershell). Når du starter med en XML-fil, kan du bruge alle tilgængelige indstillinger.
