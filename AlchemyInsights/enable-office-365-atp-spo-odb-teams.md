---
title: Aktivere Office 365 DTT for SharePoint, OneDrive og Microsoft-Team
ms.author: deniseb
author: denisebmsft
manager: laurawi
ms.date: 04/01/2019
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Admin_O365
ms.custom: 3100021
ms.openlocfilehash: ae2f574663ae3233a056589c2d5a578171f3b2f4
ms.sourcegitcommit: 9d78905c512192ffc4675468abd2efc5f2e4baf4
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 04/23/2019
ms.locfileid: "32403027"
---
# <a name="enable-office-365-advanced-threat-protection-for-sharepoint-online-onedrive-and-microsoft-teams"></a>Aktivere Office 365 avancerede Threat Protection til SharePoint Online, OneDrive og Microsoft-Team

1. Gå til https://protection.office.com og logge på.
2. Vælg **trussel management** > **politik** > **Sikre vedhæftede filer**.
3. Vælg **Slå DTT for SharePoint, OneDrive, og Microsoft-Team**, og klik derefter på **Gem**.
4. (Anbefales) Som en global administrator eller en SharePoint Online-administratoren, køre [Set-SPOTenant](https://docs.microsoft.com/powershell/module/sharepoint-online/Set-SPOTenant?view=sharepoint-ps) -cmdlet med parameteren **DisallowInfectedFileDownload** er indstillet til *Sand*.
5. (Anbefales) [Konfigurer påmindelser](https://docs.microsoft.com/office365/securitycompliance/turn-on-atp-for-spo-odb-and-teams#set-up-alerts-for-detected-files) for fundne filer.

> [!NOTE]
> ATP vil nDu kan kun scanning hver enkelt fil i SharePoint Online, OneDrive eller Microsoft Teams. Filer scannes asynkront, gennem en proces, der bruger Deling og gæster aktivitet hændelser, sammen med intelligent heuristik og trussel signaler til at identificere skadelige filer. Se [https://docs.microsoft.com/office365/securitycompliance/atp-for-spo-odb-and-teams](https://docs.microsoft.com/office365/securitycompliance/atp-for-spo-odb-and-teams).