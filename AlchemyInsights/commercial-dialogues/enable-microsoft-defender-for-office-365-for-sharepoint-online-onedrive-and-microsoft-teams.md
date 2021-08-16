---
title: Aktivér Microsoft Defender Office 365 til SharePoint Online, OneDrive og Microsoft Teams
ms.author: v-jmathew
author: v-jmathew
manager: dansimp
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000760"
- "7391"
ms.openlocfilehash: db79c1d79ddb9bc92f0601ac156e5e41a8ab83cd603556f191d5491cdd5ae2a3
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 08/05/2021
ms.locfileid: "54058860"
---
# <a name="enable-microsoft-defender-for-office-365-for-sharepoint-online-onedrive-and-microsoft-teams"></a>Aktivér Microsoft Defender Office 365 til SharePoint Online, OneDrive og Microsoft Teams

1. Ved hjælp af din globale administrator eller sikkerhedsadministrators legitimationsoplysninger skal du logge [på Office 365 Security and Compliance Center.](https://protection.office.com/)
2. Vælg **Trusselsadministration** i venstre rude, og vælg derefter **Politik for**  >  [vedhæftede Pengeskab.](https://protection.office.com/safeattachment)
3. Vælg **Slå Microsoft Defender til for Office 365 for SharePoint, OneDrive og Microsoft Teams**, og vælg derefter **Gem**.
    > [!TIP]
    >
    > - Som global administrator eller SharePoint Online-administrator skal du køre følgende PowerShell-cmdlet med parameteren **DisallowInfectedFileDownload** angivet til *sand:* [Set-SPOTenant](https://go.microsoft.com/fwlink/?linkid=2092301)
    > - [Konfigurere beskeder for registrerede filer](https://go.microsoft.com/fwlink/?linkid=2092110)

Du kan finde flere [oplysninger i Microsoft Defender til Office 365 for SharePoint, OneDrive og Microsoft Teams.](https://go.microsoft.com/fwlink/?linkid=2092041)
