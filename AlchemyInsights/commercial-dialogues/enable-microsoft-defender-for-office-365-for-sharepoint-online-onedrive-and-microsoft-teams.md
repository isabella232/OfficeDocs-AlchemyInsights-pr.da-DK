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
ms.openlocfilehash: 61372075ac8ccf04606a8003b4ec29f89fc048e5
ms.sourcegitcommit: ab75f66355116e995b3cb5505465b31989339e28
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 08/13/2021
ms.locfileid: "58332373"
---
# <a name="enable-safe-attachments-for-sharepoint-online-onedrive-and-microsoft-teams"></a>Aktivér Pengeskab vedhæftede filer SharePoint Online, OneDrive og Microsoft Teams

1. Ved hjælp af din globale administrator eller dine sikkerhedsadministratorlegitimationsoplysninger skal du åbne Microsoft 365 Defender-portalen på og derefter gå til Politikker & regler for trusselspolitikker <https://security.microsoft.com>  \>  \> **Pengeskab Vedhæftede**  filer i sektionen Politikker

   For at gå direkte til siden **Pengeskab vedhæftede filer** skal du bruge <https://security.microsoft.com/safeattachmentv2> .

2. På siden **Pengeskab vedhæftede filer** skal du klikke på **Globale indstillinger**.
3. I pop op-dialogboksen, der vises, skal du vælge **Slå Microsoft Defender til for Office 365 for SharePoint, OneDrive og Microsoft Teams** og derefter vælge **Gem**.

    **Tip:** Gør følgende for at forbedre beskyttelsen af Pengeskab vedhæftede filer til SharePoint, OneDrive og Microsoft Teams:
    - For at forhindre brugere i at downloade skadelige filer, skal du bruge værdien `$true` for *parameteren DisallowInfectedFileDownload* på **[Set-SPOTenant-cmdlet'en](https://docs.microsoft.com/powershell/module/sharepoint-online/Set-SPOTenant)** i SharePoint Online PowerShell. Du kan få mere at vide [under Brug SharePoint Online PowerShell til at forhindre brugere i at downloade skadelige filer](https://docs.microsoft.com/microsoft-365/security/office-365-security/turn-on-mdo-for-spo-odb-and-teams#step-2-recommended-use-sharepoint-online-powershell-to-prevent-users-from-downloading-malicious-files).
    - [Opret en beskedpolitik for registrerede filer](https://docs.microsoft.com/microsoft-365/security/office-365-security/turn-on-mdo-for-spo-odb-and-teams#step-3-recommended-use-the-microsoft-365-defender-portal-to-create-an-alert-policy-for-detected-files)

Du kan finde flere [oplysninger Pengeskab Vedhæftede filer til Office 365 for SharePoint, OneDrive og Microsoft Teams.](https://go.microsoft.com/fwlink/?linkid=2092041)
