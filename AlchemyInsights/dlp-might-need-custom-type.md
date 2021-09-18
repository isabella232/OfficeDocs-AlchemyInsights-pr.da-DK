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
ms.openlocfilehash: c0996e0cc923c13b7de3752ac6534026e8627c51
ms.sourcegitcommit: dcd1c76ced1a0cec27f4cf8d383593760c198424
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 09/18/2021
ms.locfileid: "59446685"
---
# <a name="dlp-might-need-a-custom-type"></a>DLP skal muligvis bruge en brugerdefineret type

**Vigtigt**: I disse hidtil usete tider bestræber vi os på at sikre, at SharePoint Online- og OneDrive-tjenesterne fastholder sin høje tilgængelighed. Hvis du ønsker flere oplysninger, skal du besøge [Midlertidige funktionsjusteringer i SharePoint Online](https://aka.ms/ODSPAdjustments).

**DLP kan kræve en brugerdefineret oplysningstype**

Med en politik til forebyggelse af datatab (DLP) kan du identificere og beskytte følsomme data i organisationen. I nogle situationer kan det være nødvendigt at oprette din egen brugerdefinerede type af følsomme oplysninger for at beskytte din organisations data. Få mere at vide under [Få mere at vide om typer af følsomme oplysninger](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-learn-about) og [enhedsdefinitioner for typer af følsomme oplysninger.](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions)

Du kan finde flere oplysninger om, hvordan du opretter brugerdefinerede typer af følsomme oplysninger og politikker, under: 

**Tilpasse en indbygget følsom oplysningstype**

Hvis en indbygget følsom oplysningstype opfylder dine behov med blot nogle få finjusteringer, skal du se Tilpasse [en indbygget type af følsomme oplysninger.](https://docs.microsoft.com/microsoft-365/compliance/customize-a-built-in-sensitive-information-type) Du kan f.eks. tilføje eller fjerne nøgleord eller tilføje eller fjerne supplerende beviser som f.eks. en dato eller adresse.

**Oprette en brugerdefineret type af følsomme oplysninger**

Men hvis du har brug for at identificere og beskytte en anden type af følsomme oplysninger helt, kan du oprette en brugerdefineret type af følsomme oplysninger Microsoft 365 Overholdelsescenter. Få mere at vide under [Introduktion til brugerdefinerede typer af følsomme oplysninger.](https://docs.microsoft.com/microsoft-365/compliance/customize-a-built-in-sensitive-information-type)

**Opret en brugerdefineret type af følsomme oplysninger i Security & Compliance Center PowerShell**

Hvis brugergrænsefladen ikke indeholder alle de nødvendige indstillinger, kan du oprette en brugerdefineret type af følsomme oplysninger i Security & Compliance Center PowerShell. Ved at starte med en XML-fil kan du bruge alle tilgængelige indstillinger. Få mere at vide under [Opret en brugerdefineret type af følsomme oplysninger ved hjælp af PowerShell.](https://docs.microsoft.com/microsoft-365/compliance/create-a-custom-sensitive-information-type-in-scc-powershell)

Hvis du vil teste din politik i testtilstand først, skal du se Implementer politik i [testtilstand](https://docs.microsoft.com/microsoft-365/compliance/dlp-learn-about-dlp#implement-policy-in-test-mode) og [Opret, test og finjuster en DLP-politik.](https://docs.microsoft.com/microsoft-365/compliance/create-test-tune-dlp-policy) 