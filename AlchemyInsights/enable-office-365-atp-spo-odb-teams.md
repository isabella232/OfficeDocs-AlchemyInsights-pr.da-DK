---
title: Aktivér Office 365 ATP for SharePoint, OneDrive og Microsoft Teams
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
ms.openlocfilehash: 4a29fdf1b61dd51b85793a1346bea193c67f70d32344470cb5449cf767da4a24
ms.sourcegitcommit: 920051182781bd97ce4d4d6fbd268cb37b84d239
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 08/11/2021
ms.locfileid: "57896597"
---
# <a name="enable-microsoft-defender-for-office-365-for-sharepoint-online-onedrive-and-microsoft-teams"></a>Aktivér Microsoft Defender Office 365 til SharePoint Online, OneDrive og Microsoft Teams

1. Gå til https://protection.office.com , og log på.
2. Vælg **Politik for**  >  **trusselsadministration**  >  **Pengeskab vedhæftede filer**.
3. Vælg **Slå Defender til for Office 365 for SharePoint, OneDrive og Microsoft Teams**, og klik derefter på **Gem**.
4. (Anbefalet) Som global administrator eller SharePoint Online-administrator skal du køre [Set-SPOTenant-cmdlet'en](https://docs.microsoft.com/powershell/module/sharepoint-online/Set-SPOTenant?view=sharepoint-ps) med parameteren **DisallowInfectedFileDownload** angivet til *sand*.
5. (Anbefalet) [Konfigurer beskeder for](https://docs.microsoft.com/microsoft-365/security/office-365-security/turn-on-atp-for-spo-odb-and-teams#set-up-alerts-for-detected-files) registrerede filer.

> [!NOTE]
> Microsoft Defender for Office 365 scanner ikke hver enkelt fil i SharePoint Online, OneDrive eller Microsoft Teams. Filer scannes asynkront gennem en proces, der bruger delings- og gæsteaktivitetshændelser sammen med smarte heuristiske og trusselssignaler til at identificere skadelige filer. Se [Microsoft Defender for Office 365 for SharePoint, OneDrive og Microsoft Teams](https://docs.microsoft.com/microsoft-365/security/office-365-security/atp-for-spo-odb-and-teams).