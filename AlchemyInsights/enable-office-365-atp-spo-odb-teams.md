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
ms.openlocfilehash: fdfdc97a198898051a3388672d01994d96dd5e97
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 04/22/2020
ms.locfileid: "43703420"
---
# <a name="enable-office-365-advanced-threat-protection-for-sharepoint-online-onedrive-and-microsoft-teams"></a>Aktivere Avanceret trusselsbeskyttelse i Office 365 til SharePoint Online, OneDrive og Microsoft Teams

1. Gå https://protection.office.com til og log på.
2. Vælg**Politik** >  **for trusselshåndtering** > **.**
3. Vælg **Slå ATP til for SharePoint, OneDrive og Microsoft Teams**, og klik derefter på **Gem**.
4. (Anbefalet) Som global administrator eller SharePoint Online-administrator skal du køre cmdlet'en [Set-SPOTenant](https://docs.microsoft.com/powershell/module/sharepoint-online/Set-SPOTenant?view=sharepoint-ps) med parameteren **DisallowInfectedFileDownload** angivet til *true*.
5. (Anbefalet) [Konfigurer beskeder](https://docs.microsoft.com/office365/securitycompliance/turn-on-atp-for-spo-odb-and-teams#set-up-alerts-for-detected-files) for fundne filer.

> [!NOTE]
> ATP scanner hver enkelt fil i SharePoint Online, OneDrive eller Microsoft Teams. Filer scannes asynkront, gennem en proces, der bruger deling og gæst aktivitet begivenheder, sammen med smart heuristik og trussel signaler til at identificere ondsindede filer. Se [https://docs.microsoft.com/office365/securitycompliance/atp-for-spo-odb-and-teams](https://docs.microsoft.com/office365/securitycompliance/atp-for-spo-odb-and-teams).