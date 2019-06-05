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
ms.openlocfilehash: 7451cfe957545537298f57feb5b47bd6d43cddbf
ms.sourcegitcommit: 6d341637dbb14e90726a1ce1d68f077ace9bb765
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 06/04/2019
ms.locfileid: "34716886"
---
# <a name="sharepoint-designer-connection-issues"></a>SharePoint Designer forbindelsesproblemer 

<p>Hvis SharePoint Designer problemer med forbindelsen til SharePoint-websteder, skal du forsøge følgende fælles løsninger.</p> <p><strong>Trin 1:</strong> <strong>Opdateres kontrollere SharePoint Designer&nbsp; </strong></p> <ul> <li><a href="https://www.microsoft.com/en-us/download/details.aspx?id=35491">SharePoint Designer 2013</a></li> <li><a href="https://support.microsoft.com/en-us/help/2817441/description-of-microsoft-sharepoint-designer-2013-service-pack-1-sp1">SharePoint Designer Service Pack 1 (SP1)</a></li> <li><a href="https://support.microsoft.com/en-us/help/3114721/august-2-2016-update-for-sharepoint-designer-2013-kb3114721">Opdatering til SharePoint Designer 2013 (KB3114721)</a></li> </ul> <p><strong>Trin 2:</strong> <strong>Fjern markeringen i de lokale cache-filer</strong>&nbsp;</p> <ol> <li style="font-weight: 400;">Lukke SharePoint Designer 2013.&nbsp;</li> <li style="font-weight: 400;">Gå til følgende mapper til at fjerne cachelagrede filer på den lokale computer.&nbsp;</li> <li style="font-weight: 400;">Klik på <strong>Start -&gt; køre</strong> og slette alle filer, der findes under hver af de under lokationer.&nbsp;<br /><br />%APPDATA%\Microsoft\Web server Extensions\Cache<br />%APPDATA%\Microsoft\SharePoint Designer\ProxyAssemblyCache<br />%USERPROFILE%\AppData\Local\Microsoft\WebsiteCache</li> <li style="font-weight: 400;">Åbn SharePoint Designer 2013 og angive kontoen igen for at se, hvis det virker.</li> </ol> <p><strong>Trin 3:</strong> <a href="https://docs.microsoft.com/en-us/office365/admin/security-and-compliance/enable-modern-authentication?redirectSourcePath=%252fen-us%252farticle%252fEnable-Modern-Authentication-for-Office-2013-on-Windows-devices-7dc1c01a-090f-4971-9677-f1b192d6c910&amp;view=o365-worldwide"> <strong>Aktiverer moderne godkendelse for 2013 til Office på Windows-enheder</strong></a>&nbsp;</p> <p><strong>Trin 4:</strong> <strong>Administratorer skal tillade brugerdefineret Script til at tillade forbindelse til SharePoint Designer</strong>.</p> <p>Se flere detaljerede oplysninger, eksempler og overvejelser i forbindelse med <a href="https://docs.microsoft.com/en-us/sharepoint/allow-or-prevent-custom-script">Tillad eller forhindre brugerdefineret script</a>.&nbsp;</p>


