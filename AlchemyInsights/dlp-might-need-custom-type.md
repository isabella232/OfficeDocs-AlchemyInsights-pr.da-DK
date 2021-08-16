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
ms.openlocfilehash: 1b0beb89eaf8a4105659a1faa7cc723174a73940ef46bd2355bdddfee7b94adb
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 08/05/2021
ms.locfileid: "54030788"
---
# <a name="dlp-might-need-a-custom-type"></a>DLP skal muligvis bruge en brugerdefineret type

**Vigtigt**: I disse hidtil usete tider bestræber vi os på at sikre, at SharePoint Online- og OneDrive-tjenesterne fastholder sin høje tilgængelighed. Hvis du ønsker flere oplysninger, skal du besøge [Midlertidige funktionsjusteringer i SharePoint Online](https://aka.ms/ODSPAdjustments).

**DLP kan kræve en brugerdefineret oplysningstype**

Med en politik til forebyggelse af datatab (DLP) kan du identificere og beskytte følsomme data i organisationen. I nogle situationer kan det være nødvendigt at oprette din **egen** brugerdefinerede type af følsomme oplysninger for at beskytte din organisations data.

Din organisation kan f.eks. have brug for at identificere og beskytte medarbejder-id'er eller andre data i et format, som er specifikt for din organisation. Hvis det er ja, kan du finde flere oplysninger i følgende artikler.
  
 **Tilpasse en indbygget følsom oplysningstype**
  
Hvis en indbygget følsom oplysningstype opfylder dine behov med blot nogle få finjusteringer, kan du tilpasse en [indbygget følsom oplysningstype](https://docs.microsoft.com/microsoft-365/compliance/customize-a-built-in-sensitive-information-type). Du kan f.eks. tilføje eller fjerne nøgleord eller tilføje eller fjerne supplerende beviser som f.eks. en dato eller adresse.
  
 **Oprette en brugerdefineret type af følsomme oplysninger**
  
Men hvis du har brug for at identificere og [](https://docs.microsoft.com/microsoft-365/compliance/create-a-custom-sensitive-information-type) beskytte en anden type af følsomme oplysninger helt, kan du oprette en brugerdefineret type af følsomme oplysninger i brugergrænsefladen for Security & Compliance Center.
  
**Opret en brugerdefineret type af følsomme oplysninger i Security & Compliance Center PowerShell**

Hvis brugergrænsefladen ikke indeholder alle de nødvendige indstillinger, kan du oprette en brugerdefineret type af følsomme oplysninger i [Security & Compliance Center PowerShell.](https://docs.microsoft.com/microsoft-365/compliance/create-a-custom-sensitive-information-type-in-scc-powershell) Ved at starte med en XML-fil kan du bruge alle tilgængelige indstillinger.
