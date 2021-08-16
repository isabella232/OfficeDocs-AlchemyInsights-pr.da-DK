---
title: MC210173 – udfasning af funktionen ny brugerdefineret formular i SharePoint Designer
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9002886"
- "5508"
- "9000127"
- "5507"
ms.openlocfilehash: f72d6ce6931b39d5d4a4835cee0ed2952407b13187213cca5bd483acb1e192bf
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 08/05/2021
ms.locfileid: "54077648"
---
# <a name="mc210173---sharepoint-designer-new-custom-form-feature-deprecation"></a>MC210173 – udfasning af funktionen ny brugerdefineret formular i SharePoint Designer

Vi har fundet et problem, der påvirker funktionen SharePoint Designer til [oprettelse af brugerdefinerede formularer](https://support.microsoft.com/en-us/office/create-a-custom-list-form-using-sharepoint-designer-917d8fdb-ee00-4441-adb3-a94612d1d105?ui=en-us&rs=en-us&ad=us#bm2) i SharePoint Online. Efter omhyggelig undersøgelse har vi fastslået, at der ikke er nogen kendt løsning på dette problem, så vi vælger at deaktivere funktionen til oprettelse af brugerdefinerede formularer, hvilket træder i kraft lørdag d. 25. april 2020 kl. 3:00 am UTC.  Denne ændring påvirker ikke muligheden for at redigere tidligere oprettede formularer eller andre eksisterende funktioner i SharePoint Online Designer.

Efter at vi har foretaget denne ændring, har brugerne måske modtaget følgende fejl ved opretning af nye formularer: "Ændringslisten kunne ikke gemmes på serveren". 

Brugere, der tidligere har udnyttet SharePoint Designer til at oprette brugerdefinerede formularer, kan i stedet bruge [PowerApps](https://docs.microsoft.com/powerapps/maker/canvas-apps/customize-list-form) til dette formål.

PowerApps er et nemt og effektivt værktøj, der gør det muligt for brugere, der opererer i den moderne oplevelse i SharePoint Online, at oprette og redigere brugerdefinerede formularer til SharePoint-lister og -dokumentbiblioteker direkte fra et browservindue. PowerApps kræver ikke traditionel kodningsviden eller downloads af andre apps som f.eks. InfoPath.

**Bemærk!**: Klassiske SharePoint Online-brugere skal midlertidigt skifte til den moderne oplevelse for at få adgang til og bruge PowerApps. Alle brugerdefinerede formularer, der er oprettet i PowerApps, er dog tilgængelige for brugere af den klassiske oplevelse i SharePoint Online.
