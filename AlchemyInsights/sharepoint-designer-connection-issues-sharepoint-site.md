---
title: SharePoint Designer forbindelsesproblemer
ms.author: efrene
author: efrene
manager: pamgreen
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: f2b1b6b4-10c9-4e83-b9cb-529a0b8a3c55
ms.openlocfilehash: a4aeaeaea5743c276b907c78317ff30f5610be81
ms.sourcegitcommit: 1d98db8acb9959aba3b5e308a567ade6b62da56c
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 08/22/2019
ms.locfileid: "36508417"
---
# <a name="sharepoint-designer-connection-issues"></a>SharePoint Designer forbindelsesproblemer 

Hvis SharePoint Designer problemer med forbindelsen til SharePoint-websteder, skal du prøve følgende fælles løsninger.

Trin 1: Kontroller, at SharePoint Designer 2013 opdateres med [SharePoint Designer Service Pack 1](https://support.microsoft.com/help/2817441/description-of-microsoft-sharepoint-designer-2013-service-pack-1-sp1) og den [2. August 2016 opdatering til SharePoint Designer 2013](https://support.microsoft.com/help/3114721/august-2-2016-update-for-sharepoint-designer-2013-kb3114721).



Trin 2: Fjern de lokale cache-filer:

1. Lukke SharePoint Designer 2013.

2. Fjerne alle de filer, der findes i hver af følgende mapper på den lokale computer.

    - %APPDATA%\Microsoft\Web server Extensions\Cache
    - %APPDATA%\Microsoft\SharePoint Designer\ProxyAssemblyCache
    - %USERPROFILE%\AppData\Local\Microsoft\WebsiteCache

3. Åbn SharePoint Designer 2013 og angive kontoen igen for at se, hvis det virker.

Trin 3: [Aktivér moderne godkendelse for 2013 til Office på Windows-enheder](https://docs.microsoft.com/office365/admin/security-and-compliance/enable-modern-authentication?redirectSourcePath=/article/Enable-Modern-Authentication-for-Office-2013-on-Windows-devices-7dc1c01a-090f-4971-9677-f1b192d6c910&view=o365-worldwide).

Trin 4: Administratorer skal **Tillade brugerdefineret Script** i SharePoint Admin Center-indstillingerne til at tillade forbindelse til SharePoint Designer. Se [Tillad eller forhindre brugerdefineret script](https://docs.microsoft.com/sharepoint/allow-or-prevent-custom-script) yderligere oplysninger.


