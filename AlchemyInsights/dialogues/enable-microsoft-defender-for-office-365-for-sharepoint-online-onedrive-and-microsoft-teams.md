---
title: Aktivér Microsoft Defender til Office 365 til SharePoint Online, OneDrive og Microsoft Teams
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
ms.openlocfilehash: 1c29afdcc52e7032fea22d698371677918665fa9
ms.sourcegitcommit: 60c504f3ac187eaf1141b3ba701d9e0633bdd968
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 03/08/2021
ms.locfileid: "50693244"
---
# <a name="enable-microsoft-defender-for-office-365-for-sharepoint-online-onedrive-and-microsoft-teams"></a>Aktivér Microsoft Defender til Office 365 til SharePoint Online, OneDrive og Microsoft Teams

1. Ved hjælp af din globale administrator- eller sikkerhedsadministratorlegitimationsoplysninger skal du logge på [Office 365 Security and Compliance Center.](https://protection.office.com/)
2. Vælg **Trusselsadministration** i venstre rude, og vælg derefter Vedhæftede   >  [filer, der er beskyttet med politik.](https://protection.office.com/safeattachment)
3. Vælg **Slå Microsoft Defender til for Office 365 til SharePoint, OneDrive og Microsoft Teams,** og vælg derefter **Gem.**
    > [!TIP]
    >
    > - Som global administrator eller SharePoint Online-administrator skal du køre følgende PowerShell-cmdlet med parameteren **DisallowInfectedFileDownload** angivet til *sand:* [Set-SPOTenant](https://go.microsoft.com/fwlink/?linkid=2092301)
    > - [Konfigurere beskeder for registrerede filer](https://go.microsoft.com/fwlink/?linkid=2092110)

Du kan finde flere oplysninger [i Microsoft Defender til Office 365 til SharePoint, OneDrive og Microsoft Teams.](https://go.microsoft.com/fwlink/?linkid=2092041)
