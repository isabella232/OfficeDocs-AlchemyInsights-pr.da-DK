---
title: Begræns adgang i SharePoint eller OneDrive
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: af1b936b-0475-497b-a6d3-e671aef7b717
ms.openlocfilehash: fc6731d5a7747bb4fc8d6cef1b6ac0045d11917d7f97abbb21eea9613b1b1aa2
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 08/05/2021
ms.locfileid: "54093814"
---
# <a name="restrict-access-in-sharepoint-or-onedrive"></a>Begræns adgang i SharePoint eller OneDrive

Der er mange måder at begrænse adgangen til SharePoint Online/OneDrive-tjenester. Nedenfor kan du se disse forskellige metoder til adgangsbegrænsning. 

**Tilladelsesbegrænsning**

I SharePoint Online og OneDrive for Business begrænser vi adgang til elementer som f.eks. websteder, filer og mapper ved kun at give adgang til de grupper/enkeltpersoner, der skal have adgang.

- [Tilpasse tilladelser for en SharePoint liste eller et bibliotek](https://support.office.com/article/Customize-permissions-for-a-SharePoint-list-or-library-02d770f3-59eb-4910-a608-5f84cc297782)

- [Tilpasse SharePoint webstedstilladelser](https://docs.microsoft.com/sharepoint/customize-sharepoint-site-permissions)

- [Ændre tilladelserne for en undermappe](https://support.office.com/article/Change-the-permissions-on-a-subfolder-5427BD7C-F20A-4F75-8CF2-5359DD45A1A6)

- [Kontrollere adgang fra enheder, der ikke er administrerede](https://docs.microsoft.com/sharepoint/control-access-from-unmanaged-devices)

Som SharePoint eller global administrator kan du blokere eller begrænse adgangen til SharePoint- og OneDrive-indhold fra enheder, der ikke er administrerede (enheder, der ikke er hybride ad-enheder eller ikke kompatible med Intune).

**Begrænsning af netværksplacering**

Som it-administrator kan du kontrollere adgangen til SharePoint og OneDrive baseret på definerede netværksplaceringer, som du har tillid til. Dette kaldes også for placeringsbaseret politik. Du kan finde flere oplysninger i [Kontrollere adgang til SharePoint Online og OneDrive data baseret på netværksplacering](https://docs.microsoft.com/sharepoint/control-access-based-on-network-location)

**Begrænsning af webstedslås** 

Inden SharePoint Online har du mulighed for at låse en gruppe af websteder, så ingen har adgang. Dette angives via PowerShell og [SharePoint Online Management Shell](https://docs.microsoft.com/powershell/sharepoint/sharepoint-online/connect-sharepoint-online?view=sharepoint-ps) ved hjælp af [set-SPOSite](https://docs.microsoft.com/powershell/module/sharepoint-online/set-sposite?view=sharepoint-ps) -LockState-egenskaben.

**Begræns brugeres adgang til at oprette websteder eller underordnede websteder**

Som SharePoint-administrator eller global administrator kan du lade brugerne oprette og administrere deres egne SharePoint-websteder, bestemme, hvilken slags websteder de kan oprette, og angive placeringen af webstederne. Du kan finde flere oplysninger under [Administrer oprettelse af websteder i SharePoint Online](https://docs.microsoft.com/sharepoint/manage-site-creation)

