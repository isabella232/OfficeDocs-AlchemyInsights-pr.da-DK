---
title: Adgangsbegrænsning i SharePoint- eller OneDrive
ms.author: kirks
author: Techwriter40
ms.date: 8/7/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: af1b936b-0475-497b-a6d3-e671aef7b717
ms.openlocfilehash: 3227f10270148c0e515b687c48058affa4d2be70
ms.sourcegitcommit: 4b7e478ce700c0b781efec3857ac4dce5bdf00c6
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 06/07/2019
ms.locfileid: "34759075"
---
# <a name="restrict-access-in-sharepoint-or-onedrive"></a>Adgangsbegrænsning i SharePoint- eller OneDrive

Der er mange måder at begrænse adgangen til tjenester til SharePoint Online/OneDrive. Disse forskellige adgangsmetoder for begrænsning er beskrevet herunder. 

Begrænsning af tilladelse

I SharePoint Online og OneDrive til virksomheder kan begrænse vi adgangen til elementer som steder, filer og mapper ved kun at give adgang til de grupper/personer, der skal have adgang.

[Tilpasse tilladelser for en SharePoint-liste eller et bibliotek](https://support.office.com/article/Customize-permissions-for-a-SharePoint-list-or-library-02d770f3-59eb-4910-a608-5f84cc297782)

[Tilpasse tilladelser til SharePoint-webstedet](https://docs.microsoft.com/sharepoint/customize-sharepoint-site-permissions)

[Ændre tilladelserne for undermappen](https://support.office.com/article/Change-the-permissions-on-a-subfolder-5427BD7C-F20A-4F75-8CF2-5359DD45A1A6)

[Adgangskontrol fra ikke-administreret enheder](https://docs.microsoft.com/sharepoint/control-access-from-unmanaged-devices)

Som en SharePoint eller global administrator i Office 365, kan du blokere eller begrænse adgang til SharePoint og OneDrive indhold fra ikke-administreret enheder (de pågældende hybrid ikke AD joinforbundne eller kompatibel i Intune).

Netværk placering begrænsning

Som IT-administrator, kan du styre adgangen til SharePoint og OneDrive ressourcer, der er baseret på definerede netværksplaceringer, du har tillid til. Dette er også kendt som placering-baseret politik. Yderligere oplysninger finder du [kontrollere adgang til SharePoint Online- og OneDrive-data, der er baseret på placering på netværket](https://docs.microsoft.com/sharepoint/control-access-based-on-network-location)

Webstedsbegrænsningen Lås 

I SharePoint Online, har du mulighed for at låse en gruppe af websteder, så du ikke har adgang. Dette angives via PowerShell og [SharePoint Online Management Shell](https://docs.microsoft.com/powershell/sharepoint/sharepoint-online/connect-sharepoint-online?view=sharepoint-ps) ved hjælp af egenskaben [Sæt SPOSite](https://docs.microsoft.com/powershell/module/sharepoint-online/set-sposite?view=sharepoint-ps) - LockState.

Forhindre brugere i at oprette websteder eller underordnede websteder

Som SharePoint Administration eller global administrator af Office 365, kan du lade brugerne oprette og administrere deres egne SharePoint-websteder, skal du bestemme, hvilke websteder de kan oprette, og Angiv placeringen af websteder. Yderligere oplysninger finder du [Administrer websteder i SharePoint Online](https://docs.microsoft.com/sharepoint/manage-site-creation)

