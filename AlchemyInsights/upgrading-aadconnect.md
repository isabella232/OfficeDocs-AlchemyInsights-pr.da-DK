---
title: 932 Opgradering af AADConnect
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "932"
- "1300025"
ms.assetid: 8f43f36c-9722-43a4-b0de-c5341c06dac5
ms.openlocfilehash: fcc5fddb5cfd15407d0533449035317d187931ed
ms.sourcegitcommit: 631cbb5f03e5371f0995e976536d24e9d13746c3
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 04/22/2020
ms.locfileid: "43766487"
---
# <a name="upgrade-azure-ad-connect"></a>Opgrader Azure AD Connect

Automatisk opgradering er som standard aktiveret for Azure AD Connect, hvilket er med til at sikre, at du kører den nyeste version. Hvis du vil kontrollere de automatiske opgraderingsindstillinger, skal du bruge cmdlet'en **Get-ADSyncAutoUpgrade** i Azure AD PowerShell. Cmdlet'en returnerer en af følgende værdier:

- **Aktiveret**: Automatisk opgradering er aktiveret.

- **Deaktiveret**: Automatisk opgradering er deaktiveret.

- **Suspenderet**: Systemet er ikke længere berettiget til at modtage automatiske opgraderinger. Du kan ikke konfigurere denne værdi. det er indstillet af systemet.

Yderligere oplysninger finder du i [Automatic upgrade](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-feature-automatic-upgrade).

Hvis du vil hente den nyeste [https://www.microsoft.com/download/details.aspx?id=47594](https://www.microsoft.com/download/details.aspx?id=47594)version af Azure AD Connect, skal du gå til .
