---
title: Aktivere Office 365 ATP til SharePoint, OneDrive og Microsoft Teams
ms.author: deniseb
author: denisebmsft
manager: laurawi
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Admin_O365
ms.custom: 3100021
ms.openlocfilehash: 564a7f1f6a37e64dbd7d679878ebadbbe35f3fa0
ms.sourcegitcommit: bc7d6f4f3c9f7060d073f5130e1ec856e248d020
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 06/02/2020
ms.locfileid: "44506912"
---
# <a name="enable-office-365-advanced-threat-protection-for-sharepoint-online-onedrive-and-microsoft-teams"></a>Aktivere avanceret beskyttelse mod office 365 til SharePoint Online, OneDrive og Microsoft Teams

1. Gå til https://protection.office.com og log på.
2. Vælg **Advarsler**  >  **Policy**  >  **om beskyttelsesstÃ evner til**politik for politik .
3. Vælg **Slå ATP til for SharePoint, OneDrive og Microsoft Teams**, og klik derefter på **Gem**.
4. (Anbefales) Kør [cmdlet'en Set-SPOTenant](https://docs.microsoft.com/powershell/module/sharepoint-online/Set-SPOTenant?view=sharepoint-ps) med parameteren **DisallowInfectedFileDownload** , der er angivet til *true,* som global administrator eller SharePoint Online-administrator.
5. (Anbefales) [Konfigurer beskeder](https://docs.microsoft.com/microsoft-365/security/office-365-security/turn-on-atp-for-spo-odb-and-teams#set-up-alerts-for-detected-files) for fundne filer.

> [!NOTE]
> ATP scanner nto-scanning af hver enkelt fil i SharePoint Online, OneDrive eller Microsoft Teams. Filer scannes asynkront gennem en proces, der bruger delings- og gæsteaktivitetshændelser sammen med smarte heuristik og trusselssignaler til at identificere skadelige filer. Se [ATP for SharePoint, OneDrive og Microsoft Teams](https://docs.microsoft.com/microsoft-365/security/office-365-security/atp-for-spo-odb-and-teams).