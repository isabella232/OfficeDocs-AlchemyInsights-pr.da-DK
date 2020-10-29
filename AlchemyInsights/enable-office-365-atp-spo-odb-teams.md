---
title: Aktivér Office 365 DTT til SharePoint, OneDrive og Microsoft teams
ms.author: deniseb
author: denisebmsft
manager: laurawi
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Admin_O365
ms.custom: 3100021
ms.openlocfilehash: bef43656097c6f27677172899df1ada7900a9b64
ms.sourcegitcommit: 4caf5e6c2fee2903ccaf92cfc9006eb580faa7ba
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 10/29/2020
ms.locfileid: "48801041"
---
# <a name="enable-microsoft-defender-for-office-365-for-sharepoint-online-onedrive-and-microsoft-teams"></a>Aktivér Microsoft Defender til Office 365 til SharePoint Online, OneDrive og Microsoft teams

1. Gå til https://protection.office.com og log på.
2. Vælg politik for **trussels administrations**  >  **politik**  >  **sikre vedhæftede filer** .
3. Vælg **Aktivér DTT for SharePoint, OneDrive og Microsoft teams** , og klik derefter på **Gem** .
4. Anbefales Som global administrator eller SharePoint Online-administrator skal du køre cmdlet'en [set-SPOTenant](https://docs.microsoft.com/powershell/module/sharepoint-online/Set-SPOTenant?view=sharepoint-ps) , hvor parameteren **DisallowInfectedFileDownload** er angivet til *sand* .
5. Anbefales [Konfigurere beskeder](https://docs.microsoft.com/microsoft-365/security/office-365-security/turn-on-atp-for-spo-odb-and-teams#set-up-alerts-for-detected-files) for registrerede filer.

> [!NOTE]
> DTT vil stræbe i at scanne hver enkelt fil i SharePoint Online, OneDrive eller Microsoft teams. Filer scannes asynkront via en proces, der bruger aktiviteter til deling og gæst, samt smarte heuristik-og trussels signaler til at identificere ondsindede filer. Se [DTT til SharePoint, OneDrive og Microsoft teams](https://docs.microsoft.com/microsoft-365/security/office-365-security/atp-for-spo-odb-and-teams).