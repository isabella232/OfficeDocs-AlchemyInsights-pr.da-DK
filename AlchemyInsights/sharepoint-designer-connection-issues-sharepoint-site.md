---
title: Problemer med SharePoint Designer-forbindelse
ms.author: pebaum
author: pebaum
manager: pamgreen
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: f2b1b6b4-10c9-4e83-b9cb-529a0b8a3c55
ms.openlocfilehash: 01ccc6bc28148f397fb6cd2b7a0eaaeb5b51973f
ms.sourcegitcommit: bc7d6f4f3c9f7060d073f5130e1ec856e248d020
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 06/02/2020
ms.locfileid: "44511538"
---
# <a name="sharepoint-designer-connection-issues"></a>Problemer med SharePoint Designer-forbindelse 

Hvis SharePoint Designer oplever forbindelsesproblemer til SharePoint-websteder, skal du prøve følgende almindelige løsninger.

Trin 1: Kontroller, at SharePoint Designer 2013 er opdateret med [SharePoint Designer Service Pack 1](https://support.microsoft.com/help/2817441/description-of-microsoft-sharepoint-designer-2013-service-pack-1-sp1) og [den 2.](https://support.microsoft.com/help/3114721/august-2-2016-update-for-sharepoint-designer-2013-kb3114721)



Trin 2: Ryd de lokale cachefiler:

1. Luk SharePoint Designer 2013.

2. Fjern alle filer, der findes i hver af følgende mapper, på den lokale computer.

    - %APPDATA%\Microsoft\WebServerudvidelser\Cache
    - %APPDATA%\Microsoft\SharePoint Designer\ProxyAssemblyCache
    - %USERPROFILE%\AppData\Lokal\Microsoft\WebsiteCache

3. Åbn SharePoint Designer 2013, og angiv kontoen igen for at se, om den virker.

Trin 3: [Aktiver moderne godkendelse til Office 2013 på Windows-enheder](https://docs.microsoft.com/microsoft-365/admin/security-and-compliance/enable-modern-authentication).

Trin 4: Administratorer skal **tillade brugerdefineret script** i Indstillingerne for SharePoint Administration for at tillade SharePoint Designer-forbindelsen. Se [Tillad eller forhindre brugerdefineret script](https://docs.microsoft.com/sharepoint/allow-or-prevent-custom-script) for at få flere oplysninger.


