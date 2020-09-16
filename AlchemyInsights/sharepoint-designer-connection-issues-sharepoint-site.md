---
title: Forbindelsesproblemer i SharePoint Designer
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
ms.openlocfilehash: 997ba3de58485d4fe6d24b926c33348378af8cd3
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 09/14/2020
ms.locfileid: "47727165"
---
# <a name="sharepoint-designer-connection-issues"></a>Forbindelsesproblemer i SharePoint Designer 

Hvis SharePoint Designer har forbindelsesproblemer til SharePoint-websteder, kan du prøve følgende almindelige løsninger.

Trin 1: Kontrollér, at SharePoint Designer 2013 er opdateret med [SharePoint Designer Service Pack 1](https://support.microsoft.com/help/2817441/description-of-microsoft-sharepoint-designer-2013-service-pack-1-sp1) og den [2. august 2016-opdatering til sharepoint designer 2013](https://support.microsoft.com/help/3114721/august-2-2016-update-for-sharepoint-designer-2013-kb3114721).



Trin 2: Ryd op i de lokale cachefiler:

1. Luk SharePoint Designer 2013.

2. På den lokale computer skal du fjerne alle filer, der findes i følgende mapper.

    - %APPDATA%\Microsoft\Web server Extensions\Cache
    - %APPDATA%\Microsoft\SharePoint Designer\ProxyAssemblyCache
    - %USERPROFILE%\AppData\Local\Microsoft\WebsiteCache

3. Åbn SharePoint Designer 2013, og Angiv kontoen igen for at se, om den fungerer.

Trin 3: [Aktivér moderne godkendelse for Office 2013 på Windows-enheder](https://docs.microsoft.com/microsoft-365/admin/security-and-compliance/enable-modern-authentication).

Trin 4: Administratorer skal tillade et **brugerdefineret script** i SharePoint-administrations Center indstillinger for at tillade SharePoint Designer-forbindelsen. Se [Tillad eller Forbyd brugerdefineret script for at](https://docs.microsoft.com/sharepoint/allow-or-prevent-custom-script) få flere oplysninger.


