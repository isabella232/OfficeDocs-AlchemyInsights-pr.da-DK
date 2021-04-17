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
ms.openlocfilehash: 5be1ac4c8a4044adbc7d37c32ba7b3cb67c6cc25
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 04/15/2021
ms.locfileid: "51831800"
---
# <a name="mc210173---sharepoint-designer-new-custom-form-feature-deprecation"></a><span data-ttu-id="1e752-102">MC210173 – udfasning af funktionen ny brugerdefineret formular i SharePoint Designer</span><span class="sxs-lookup"><span data-stu-id="1e752-102">MC210173 - SharePoint Designer new custom Form feature deprecation</span></span>

<span data-ttu-id="1e752-103">Vi har fundet et problem, der påvirker funktionen SharePoint Designer til [oprettelse af brugerdefinerede formularer](https://support.microsoft.com/en-us/office/create-a-custom-list-form-using-sharepoint-designer-917d8fdb-ee00-4441-adb3-a94612d1d105?ui=en-us&rs=en-us&ad=us#bm2) i SharePoint Online.</span><span class="sxs-lookup"><span data-stu-id="1e752-103">We’ve identified an issue affecting SharePoint Designer functionality for [creating custom Forms](https://support.microsoft.com/en-us/office/create-a-custom-list-form-using-sharepoint-designer-917d8fdb-ee00-4441-adb3-a94612d1d105?ui=en-us&rs=en-us&ad=us#bm2) within SharePoint Online.</span></span> <span data-ttu-id="1e752-104">Efter omhyggelig undersøgelse har vi fastslået, at der ikke er nogen kendt løsning på dette problem, så vi vælger at deaktivere funktionen til oprettelse af brugerdefinerede formularer, hvilket træder i kraft lørdag d. 25. april 2020 kl. 3:00 am UTC. </span><span class="sxs-lookup"><span data-stu-id="1e752-104">After careful examination, we’ve determined that there is no known fix for this issue and have elected to disable the custom Form creation feature effective as of 3:00 AM UTC on Saturday, April 25, 2020.</span></span> <span data-ttu-id="1e752-105">Denne ændring påvirker ikke muligheden for at redigere tidligere oprettede formularer eller andre eksisterende funktioner i SharePoint Online Designer.</span><span class="sxs-lookup"><span data-stu-id="1e752-105">This change does not impact the ability to edit previously created Forms or other existing features in SharePoint Online Designer.</span></span>

<span data-ttu-id="1e752-106">Efter at vi har foretaget denne ændring, har brugerne måske modtaget følgende fejl ved opretning af nye formularer: "Ændringslisten kunne ikke gemmes på serveren". </span><span class="sxs-lookup"><span data-stu-id="1e752-106">After this change was made, users may have received the error: "Could not save the list changes to the server," when creating new Forms.</span></span>

<span data-ttu-id="1e752-107">Brugere, der tidligere har udnyttet SharePoint Designer til at oprette brugerdefinerede formularer, kan i stedet bruge [PowerApps](https://docs.microsoft.com/powerapps/maker/canvas-apps/customize-list-form) til dette formål.</span><span class="sxs-lookup"><span data-stu-id="1e752-107">Users who have previously leveraged SharePoint Designer to create custom Forms are instead able to utilize [PowerApps](https://docs.microsoft.com/powerapps/maker/canvas-apps/customize-list-form) for this purpose.</span></span>

<span data-ttu-id="1e752-108">PowerApps er et nemt og effektivt værktøj, der gør det muligt for brugere, der opererer i den moderne oplevelse i SharePoint Online, at oprette og redigere brugerdefinerede formularer til SharePoint-lister og -dokumentbiblioteker direkte fra et browservindue.</span><span class="sxs-lookup"><span data-stu-id="1e752-108">PowerApps is an easy and powerful tool that allows users operating in the SharePoint Online Modern experience to create and edit custom Forms for SharePoint lists and document libraries right from a browser window.</span></span> <span data-ttu-id="1e752-109">PowerApps kræver ikke traditionel kodningsviden eller downloads af andre apps som f.eks. InfoPath.</span><span class="sxs-lookup"><span data-stu-id="1e752-109">PowerApps does not require traditional coding knowledge or any additional app downloads such as InfoPath.</span></span>

<span data-ttu-id="1e752-110">**Bemærk!**: Klassiske SharePoint Online-brugere skal midlertidigt skifte til den moderne oplevelse for at få adgang til og bruge PowerApps. Alle brugerdefinerede formularer, der er oprettet i PowerApps, er dog tilgængelige for brugere af den klassiske oplevelse i SharePoint Online.</span><span class="sxs-lookup"><span data-stu-id="1e752-110">**Note**: SharePoint Online Classic users will need to temporarily switch to the Modern experience to access and utilize PowerApps; though, all custom Forms created in PowerApps are accessible by SharePoint Online Classic experience users.</span></span>
