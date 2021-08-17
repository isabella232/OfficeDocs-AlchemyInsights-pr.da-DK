---
title: Aktivér Pengeskab vedhæftede filer SharePoint Online, OneDrive og Microsoft Teams
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
ms.openlocfilehash: 7357f53ef7827aea9cbb0d222c338a5edf429ffd201bfbb6d7307b3d446fdae2
ms.sourcegitcommit: 920051182781bd97ce4d4d6fbd268cb37b84d239
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 08/11/2021
ms.locfileid: "57894457"
---
# <a name="enable-safe-attachments-for-sharepoint-online-onedrive-and-microsoft-teams"></a>Aktivér Pengeskab vedhæftede filer SharePoint Online, OneDrive og Microsoft Teams

1. Ved hjælp af din globale administrator eller dine sikkerhedsadministratorlegitimationsoplysninger skal du åbne Microsoft 365 Defender-portalen på og derefter gå til Politikker & regler for trusselspolitikker Pengeskab Vedhæftede filer i sektionen <https://security.microsoft.com>  \>  \>  Politikker 

   For at gå direkte til siden **Pengeskab Vedhæftede filer** skal du bruge <https://security.microsoft.com/safeattachmentv2> .

2. Klik på **Pengeskab globale indstillinger** på siden **Vedhæftede filer.**
3. I pop op-dialogboksen, der vises, skal du vælge **Slå Microsoft Defender til for Office 365 for SharePoint, OneDrive og Microsoft Teams** og derefter vælge **Gem**.

    > [!TIP]
    >
    > Gør følgende for at forbedre beskyttelsen af vedhæftede Pengeskab til SharePoint, OneDrive og Microsoft Teams:
    >
    > - For at forhindre brugere i at downloade skadelige filer, skal du bruge værdien for parameteren `$true` *DisallowInfectedFileDownload* på **[Set-SPOTenant-cmdlet'en](https://docs.microsoft.com/powershell/module/sharepoint-online/Set-SPOTenant)** i SharePoint Online PowerShell. Få mere at vide [under Brug SharePoint Online PowerShell til at forhindre brugere i at downloade skadelige filer.](https://docs.microsoft.com/microsoft-365/security/office-365-security/turn-on-mdo-for-spo-odb-and-teams#step-2-recommended-use-sharepoint-online-powershell-to-prevent-users-from-downloading-malicious-files)
    > - [Opret en beskedpolitik for registrerede filer](https://docs.microsoft.com/microsoft-365/security/office-365-security/turn-on-mdo-for-spo-odb-and-teams#step-3-recommended-use-the-microsoft-365-defender-portal-to-create-an-alert-policy-for-detected-files)

Du kan finde flere [oplysninger Pengeskab Vedhæftede filer til Office 365 for SharePoint, OneDrive og Microsoft Teams.](https://go.microsoft.com/fwlink/?linkid=2092041)
