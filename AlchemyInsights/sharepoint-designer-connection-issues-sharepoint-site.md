---
title: Problemer med forbindelse til SharePoint Designer
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
ms.openlocfilehash: 9730bd66afd494385db3de605f5fe68d0f274ed3
ms.sourcegitcommit: 0f0186044a3597e42ad14c32ca58e7224344dcfa
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 12/15/2019
ms.locfileid: "40051707"
---
# <a name="sharepoint-designer-connection-issues"></a>Problemer med forbindelse til SharePoint Designer 

Hvis SharePoint Designer har forbindelsesproblemer til SharePoint-websteder, kan du prøve følgende almindeligt forekommende løsninger.

Trin 1: Kontroller, at SharePoint Designer 2013 er opdateret med [SharePoint Designer Service Pack 1](https://support.microsoft.com/help/2817441/description-of-microsoft-sharepoint-designer-2013-service-pack-1-sp1) og den [August 2, 2016 opdatering til sharepoint designer 2013](https://support.microsoft.com/help/3114721/august-2-2016-update-for-sharepoint-designer-2013-kb3114721).



Trin 2: Ryd de lokale cache filer:

1. Luk SharePoint Designer 2013.

2. Fjern alle filer, som findes i hver af følgende mapper, på den lokale computer.

    - %APPDATA%\Microsoft\Web server Extensions\Cache
    - %AppData%\microsoft\share point Designer\ProxyAssemblyCache
    - %USERPROFILE%\AppData\Local\Microsoft\WebsiteCache

3. Åbn SharePoint Designer 2013, og Angiv kontoen igen for at se, om den fungerer.

Trin 3: [Aktivér moderne godkendelse for Office 2013 på Windows-enheder](https://docs.microsoft.com/office365/admin/security-and-compliance/enable-modern-authentication?redirectSourcePath=/article/Enable-Modern-Authentication-for-Office-2013-on-Windows-devices-7dc1c01a-090f-4971-9677-f1b192d6c910&view=o365-worldwide).

Trin 4: Administratorer skal **tillade brugerdefineret script** i SharePoint Admin Center-indstillingerne for at tillade SharePoint Designer-forbindelsen. Se [tillade eller forhindre brugerdefineret script for at](https://docs.microsoft.com/sharepoint/allow-or-prevent-custom-script) få flere oplysninger.


