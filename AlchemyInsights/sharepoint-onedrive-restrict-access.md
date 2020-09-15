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
ms.openlocfilehash: e9eb1822a7770bc206992cc5fb7e54a5c972b7e2
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 09/14/2020
ms.locfileid: "47700449"
---
# <a name="restrict-access-in-sharepoint-or-onedrive"></a>Begræns adgang i SharePoint eller OneDrive

Der er mange måder at begrænse adgangen til SharePoint Online/OneDrive-tjenester på. Disse forskellige adgangs begrænsnings metoder er skitseret nedenfor. 

**Tilladelses begrænsning**

I SharePoint Online og OneDrive for Business kan vi begrænse adgangen til elementer som websteder, filer og mapper ved kun at give adgang til de grupper/enkeltpersoner, der skal have adgang.

- [Tilpasse tilladelser for en SharePoint-liste eller et bibliotek](https://support.office.com/article/Customize-permissions-for-a-SharePoint-list-or-library-02d770f3-59eb-4910-a608-5f84cc297782)

- [Tilpas tilladelser til SharePoint-websted](https://docs.microsoft.com/sharepoint/customize-sharepoint-site-permissions)

- [Ændre tilladelserne for en undermappe](https://support.office.com/article/Change-the-permissions-on-a-subfolder-5427BD7C-F20A-4F75-8CF2-5359DD45A1A6)

- [Kontrollér adgang fra ikke-administrerede enheder](https://docs.microsoft.com/sharepoint/control-access-from-unmanaged-devices)

Som SharePoint-eller Global administrator kan du blokere eller begrænse adgangen til SharePoint-og OneDrive-indhold fra ikke-administrerede enheder (dem, der ikke er hybride AD gangen eller kompatibel i Intune).

**Netværks placerings begrænsning**

Som IT-administrator kan du kontrollere adgangen til SharePoint-og OneDrive-ressourcer baseret på definerede netværksplaceringer, du har tillid til. Dette kaldes også en placerings baseret politik. Hvis du vil have mere at vide, skal du se [kontrollere adgang til SharePoint Online og OneDrive-data baseret på netværksplacering](https://docs.microsoft.com/sharepoint/control-access-based-on-network-location)

**Begrænsning af websteds låse** 

I SharePoint Online har du mulighed for at låse en gruppe af websteder, så ingen har adgang. Dette angives via PowerShell og [SharePoint Online Management Shell](https://docs.microsoft.com/powershell/sharepoint/sharepoint-online/connect-sharepoint-online?view=sharepoint-ps) ved hjælp af egenskaben [set-SPOSite](https://docs.microsoft.com/powershell/module/sharepoint-online/set-sposite?view=sharepoint-ps) -Lock.

**Begræns brugere fra at oprette websteder eller underordnede websteder**

Som SharePoint-administrator eller Global administrator kan du give brugerne mulighed for at oprette og administrere deres egne SharePoint-websteder, angive, hvilken slags websteder de kan oprette, og angive placeringen af webstederne. Hvis du vil have mere at vide, skal du se [administrere oprettelse af websteder i SharePoint Online](https://docs.microsoft.com/sharepoint/manage-site-creation)

