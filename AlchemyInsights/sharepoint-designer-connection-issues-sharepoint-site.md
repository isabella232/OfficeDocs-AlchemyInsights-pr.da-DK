---
title: SharePoint Online tilladelsesniveauer
ms.author: kirks
author: Techwriter40
manager: pamgreen
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: f2b1b6b4-10c9-4e83-b9cb-529a0b8a3c55
ms.openlocfilehash: 356fef8e02f2c1fd9d209c68194685bb0acaa367
ms.sourcegitcommit: 4b7e478ce700c0b781efec3857ac4dce5bdf00c6
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 06/07/2019
ms.locfileid: "34760687"
---
# <a name="sharepoint-designer-connection-issues"></a>SharePoint Designer forbindelsesproblemer 

Hvis SharePoint Designer problemer med forbindelsen til SharePoint-websteder, skal du forsøge følgende fælles løsninger.

Trin 1: Kontroller, at SharePoint Designer er opdateret.

- [SharePoint Designer 2013](https://www.microsoft.com/download/details.aspx?id=35491)

- [SharePoint Designer Service Pack 1 (SP1)](https://support.microsoft.com/help/2817441/description-of-microsoft-sharepoint-designer-2013-service-pack-1-sp1)

- [Opdatering til SharePoint Designer 2013 (KB3114721)](https://support.microsoft.com/help/3114721/august-2-2016-update-for-sharepoint-designer-2013-kb3114721)

Trin 2: Fjern de lokale cache-filer

- Lukke SharePoint Designer 2013.

- Gå til følgende mapper til at fjerne cachelagrede filer på den lokale computer.

- Klik på Start, Kør og slette alle filer, der er fundet under hver af de nedenstående placeringer.

%APPDATA%\Microsoft\Web server Extensions\Cache %APPDATA%\Microsoft\SharePoint Designer\ProxyAssemblyCache %USERPROFILE%\AppData\Local\Microsoft\WebsiteCache

Åbn SharePoint Designer 2013 og angive kontoen igen for at se, hvis det virker.

Trin 3: [Aktivér moderne godkendelse for 2013 til Office på Windows-enheder](https://docs.microsoft.com/office365/admin/security-and-compliance/enable-modern-authentication?redirectSourcePath=/article/Enable-Modern-Authentication-for-Office-2013-on-Windows-devices-7dc1c01a-090f-4971-9677-f1b192d6c910&view=o365-worldwide)

Trin 4: Administratorer skal tillade brugerdefineret Script til at tillade forbindelse til SharePoint Designer.

Se flere detaljerede oplysninger, eksempler og overvejelser i forbindelse med [Tillad eller forhindre brugerdefineret script](https://docs.microsoft.com/sharepoint/allow-or-prevent-custom-script).


