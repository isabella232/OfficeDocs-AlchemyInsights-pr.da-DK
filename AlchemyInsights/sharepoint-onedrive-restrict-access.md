---
title: Begrænse adgangen i SharePoint eller OneDrive
ms.author: pebaum
author: pebaum
ms.date: 8/7/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: af1b936b-0475-497b-a6d3-e671aef7b717
ms.openlocfilehash: 242388af3ae8887616fc123f24502a8e5ac8dfbe
ms.sourcegitcommit: 0f0186044a3597e42ad14c32ca58e7224344dcfa
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 12/15/2019
ms.locfileid: "40053759"
---
# <a name="restrict-access-in-sharepoint-or-onedrive"></a>Begrænse adgangen i SharePoint eller OneDrive

Der er mange måder at begrænse adgangen til SharePoint Online/OneDrive-tjenester på. Disse forskellige adgangsbegrænsnings metoder er skitseret nedenfor. 

**Begrænsning af tilladelse**

I SharePoint Online og OneDrive for Business begrænser vi adgangen til elementer som websteder, filer og mapper ved kun at give adgang til de grupper/personer, der skal have adgang.

- [Tilpasse tilladelser for en SharePoint-liste eller et bibliotek](https://support.office.com/article/Customize-permissions-for-a-SharePoint-list-or-library-02d770f3-59eb-4910-a608-5f84cc297782)

- [Tilpas tilladelser til SharePoint-websted](https://docs.microsoft.com/sharepoint/customize-sharepoint-site-permissions)

- [Ændre tilladelserne for en undermappe](https://support.office.com/article/Change-the-permissions-on-a-subfolder-5427BD7C-F20A-4F75-8CF2-5359DD45A1A6)

- [Styre adgang fra ikke-administrerede enheder](https://docs.microsoft.com/sharepoint/control-access-from-unmanaged-devices)

Som SharePoint-eller Global administrator i Office 365 kan du blokere eller begrænse adgangen til SharePoint-og OneDrive-indhold fra ikke-administrerede enheder (dem, der ikke er hybrid annoncer, som er joinforbundne eller kompatible i Intune).

**Begrænsning af netværksplacering**

Som IT-administrator kan du styre adgangen til SharePoint-og OneDrive-ressourcer baseret på definerede netværksplaceringer, som du har tillid til. Dette kaldes også lokationsbaseret politik. Du kan finde flere oplysninger under [kontrollere adgang til SharePoint Online-og OneDrive-data baseret på netværksplacering](https://docs.microsoft.com/sharepoint/control-access-based-on-network-location)

**Begrænsning af websteds låsning** 

I SharePoint Online har du mulighed for at låse en gruppe af websteder op, så ingen har adgang. Dette angives via PowerShell og [SharePoint Online Management Shell](https://docs.microsoft.com/powershell/sharepoint/sharepoint-online/connect-sharepoint-online?view=sharepoint-ps) ved hjælp af egenskaben [set-sposite](https://docs.microsoft.com/powershell/module/sharepoint-online/set-sposite?view=sharepoint-ps) -lockstate.

**Begrænse brugere i at oprette websteder eller underordnede websteder**

Som SharePoint-administrator eller global Office 365-administrator kan du lade dine brugere oprette og administrere deres egne SharePoint-websteder, bestemme, hvilke typer websteder de kan oprette, og angive placeringen af webstederne. Du kan finde flere oplysninger under [administrere oprettelse af websteder i SharePoint Online](https://docs.microsoft.com/sharepoint/manage-site-creation)

