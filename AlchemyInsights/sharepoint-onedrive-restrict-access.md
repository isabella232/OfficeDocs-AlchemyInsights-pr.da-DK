---
title: Begrænse adgangen i SharePoint eller OneDrive
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: af1b936b-0475-497b-a6d3-e671aef7b717
ms.openlocfilehash: 39aa8cd6e649eca4a1e196eeb589a825364d0977
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 04/22/2020
ms.locfileid: "43692759"
---
# <a name="restrict-access-in-sharepoint-or-onedrive"></a>Begrænse adgangen i SharePoint eller OneDrive

Der er mange måder at begrænse adgangen til SharePoint Online/OneDrive-tjenester på. Disse forskellige adgangsbegrænsningsmetoder er beskrevet nedenfor. 

**Begrænsning af tilladelse**

I SharePoint Online og OneDrive for Business begrænser vi adgangen til emner som websteder, filer og mapper ved kun at give adgang til de grupper/personer, der skal have adgang.

- [Tilpasse tilladelser for en SharePoint-liste eller et SharePoint-bibliotek](https://support.office.com/article/Customize-permissions-for-a-SharePoint-list-or-library-02d770f3-59eb-4910-a608-5f84cc297782)

- [Tilpasse sharepoint-webstedstilladelser](https://docs.microsoft.com/sharepoint/customize-sharepoint-site-permissions)

- [Ændre tilladelserne for en undermappe](https://support.office.com/article/Change-the-permissions-on-a-subfolder-5427BD7C-F20A-4F75-8CF2-5359DD45A1A6)

- [Styre adgangen fra ikke-administrerede enheder](https://docs.microsoft.com/sharepoint/control-access-from-unmanaged-devices)

Som SharePoint- eller global administrator kan du blokere eller begrænse adgangen til SharePoint- og OneDrive-indhold fra ikke-administrerede enheder (dem, der ikke er hybride AD-medlemmer eller overholder i Intune).

**Begrænsning af netværksplacering**

Som it-administrator kan du styre adgangen til SharePoint- og OneDrive-ressourcer baseret på definerede netværksplaceringer, som du har tillid til. Dette kaldes også lokationsbaseret politik. Du kan finde flere oplysninger under [Styre adgangen til SharePoint Online- og OneDrive-data baseret på netværksplacering](https://docs.microsoft.com/sharepoint/control-access-based-on-network-location)

**Begrænsning af webstedslås** 

I SharePoint Online har du mulighed for at låse en gruppe af websteder, så ingen har adgang. Dette angives via PowerShell og [SharePoint Online Management Shell](https://docs.microsoft.com/powershell/sharepoint/sharepoint-online/connect-sharepoint-online?view=sharepoint-ps) ved hjælp af egenskaben [Set-SPOSite](https://docs.microsoft.com/powershell/module/sharepoint-online/set-sposite?view=sharepoint-ps) -LockState.

**Begrænse brugeres mulighed for at oprette websteder eller underordnede websteder**

Som SharePoint-administrator eller global administrator kan du lade dine brugere oprette og administrere deres egne SharePoint-websteder, bestemme, hvilken type websteder de kan oprette, og angive placeringen af webstederne. Du kan finde flere oplysninger under [Administrere oprettelse af websteder i SharePoint Online](https://docs.microsoft.com/sharepoint/manage-site-creation)

