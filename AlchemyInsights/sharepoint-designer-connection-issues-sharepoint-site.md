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
ms.openlocfilehash: 1d3f6ad3128292a9dbcc46cc7da23af59a63fbb4
ms.sourcegitcommit: a285c609319ade038461e090e14a701830031825
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 07/24/2019
ms.locfileid: "35840545"
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


