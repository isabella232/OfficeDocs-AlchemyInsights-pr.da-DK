---
title: SharePoint Problemer med designerforbindelsen
ms.author: pebaum
author: pebaum
manager: pamgreen
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: f2b1b6b4-10c9-4e83-b9cb-529a0b8a3c55
ms.openlocfilehash: d55f7c1902bb623900fa74bdae70695b6e04ad84ce7b6ea314db614283ec436d
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 08/05/2021
ms.locfileid: "53942019"
---
# <a name="sharepoint-designer-connection-issues"></a>SharePoint Problemer med designerforbindelsen 

Hvis SharePoint Designer oplever problemer med forbindelsen til SharePoint, kan du prøve følgende løsningsforslag.

Trin 1: Kontrollér, at SharePoint Designer 2013 er opdateret med [SharePoint Designer Service Pack 1](https://support.microsoft.com/help/2817441/description-of-microsoft-sharepoint-designer-2013-service-pack-1-sp1) og opdateringen for 2. august [2016 til SharePoint Designer 2013.](https://support.microsoft.com/help/3114721/august-2-2016-update-for-sharepoint-designer-2013-kb3114721)



Trin 2: Ryd de lokale cachefiler:

1. Luk SharePoint Designer 2013.

2. Fjern alle de filer, der findes i hver af følgende mapper, på den lokale computer.

    - %APPDATA%\Microsoft\Web Server Extensions\Cache
    - %APPDATA%\Microsoft\SharePoint Designer\ProxyAssemblyCache
    - %USERPROFILE%\AppData\Local\Microsoft\WebsiteCache

3. Åbn SharePoint Designer 2013, og angiv kontoen igen for at se, om det virker.

Trin 3: [Aktivér moderne godkendelse Office 2013 på Windows enheder.](https://docs.microsoft.com/microsoft-365/admin/security-and-compliance/enable-modern-authentication)

Trin 4: Administratorer skal tillade **brugerdefineret script** i SharePoint Administration for at tillade forbindelsen SharePoint Designer. Se [Tillad eller forbyd brugerdefineret script](https://docs.microsoft.com/sharepoint/allow-or-prevent-custom-script) for at få flere oplysninger.


