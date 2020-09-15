---
title: DLP virker ikke som forventet
ms.author: deniseb
author: denisebmsft
manager: laurawi
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1241"
- "3200001"
ms.assetid: f6fcf5ad-55a1-4f25-af27-1f7c1ce06409
ms.openlocfilehash: 0ed893420b5813d5d18639c2c226c12f0306a13f
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 09/14/2020
ms.locfileid: "47679687"
---
# <a name="dlp-not-working-as-expected"></a>DLP virker ikke som forventet

**Vigtigt**: I disse hidtil usete tider bestræber vi os på at sikre, at SharePoint Online- og OneDrive-tjenesterne fastholder sin høje tilgængelighed. Hvis du ønsker flere oplysninger, skal du besøge [Midlertidige funktionsjusteringer i SharePoint Online](https://aka.ms/ODSPAdjustments).

 **Konfigurere DLP**

Har du problemer med forebyggelse af datatab **(DLP)** i Office 365 fungerer ikke som forventet? Hvis det er tilfældet, skal du sørge for, at din **DLP-politik** er konfigureret korrekt, og at dine data indeholder, hvad **DLP-politikken** leder efter, når den evalueres.
  
DLP-politikker gør det muligt at identificere og beskytte følsomme oplysninger i organisationen. Hvis du vil konfigurere DLP-politikker, skal du bruge oplysningerne [her](https://docs.microsoft.com/office365/securitycompliance/prevent-data-loss#set-up-dlp).
  
 **Hvilke DLP-politikker leder efter**
  
Når du bruger de **indbyggede følsomme oplysningstyper** i sikkerheds-og overholdelses centre, søger DLP-politikker efter bestemte mønstre og elementer, når du registrerer disse følsomme typer.
  
- **Indbyggede typer af følsomme oplysninger**

    Hvis du vil have mere at vide om de indbyggede følsomme typer, og hvordan en DLP-politik ser ud, når du registrerer den følsomme type, skal du se: [hvad de følsomme oplysningstyper ser ud](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions).

- **Brugerdefinerede følsomme oplysningstyper**

    Hvis du forsøger at oprette brugerdefinerede typer af følsomme oplysninger, kan du bruge følgende artikel for at få mere at vide om, hvordan du opretter en brugerdefineret følsom type: [Opret en brugerdefineret følsom oplysningstype](https://docs.microsoft.com/microsoft-365/compliance/create-a-custom-sensitive-information-type).

**Test en DLP-politik**

Hvis du vil teste dine data med en indbygget eller brugerdefineret følsom oplysningstype, skal du bruge indstillingen **testtype** under **klassifikationer**  >  **følsomme oplysningstyper**. Hvis du vil have mere at vide, skal du se [test brugerdefinerede følsomme oplysningstyper](https://docs.microsoft.com/microsoft-365/compliance/create-a-custom-sensitive-information-type#create-custom-sensitive-information-types-in-the-security--compliance-center).

 **Årsrapport**
  
- Få følsomme data indsigt i DLP- [rapporter.](https://docs.microsoft.com/microsoft-365/compliance/data-loss-prevention-policies#dlp-reports)

- Se specifikke oplysninger om begivenheden med en [hændelses rapport](https://docs.microsoft.com/microsoft-365/compliance/data-loss-prevention-policies#incident-reports).
