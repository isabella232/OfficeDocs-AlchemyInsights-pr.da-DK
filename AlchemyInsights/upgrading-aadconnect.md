---
title: 932 Opgradering af AADConnect
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "932"
- "1300025"
ms.assetid: 8f43f36c-9722-43a4-b0de-c5341c06dac5
ms.openlocfilehash: 9582f1f56e6730e35520b5d79bc245cd74bea0bf4db39b379a7cd133bafc16ee
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 08/05/2021
ms.locfileid: "54104806"
---
# <a name="upgrade-azure-ad-connect"></a>Opgrader Azure AD-Forbind

Automatisk opgradering er som standard aktiveret for Azure AD Forbind, hvilket er med til at sikre, at du kører den nyeste version. For at bekræfte indstillingerne for automatisk opgradering skal du **bruge Get-ADSyncAutoUpgrade-cmdlet'en** i Azure AD PowerShell. Cmdlet'en returnerer en af følgende værdier:

- **Aktiveret:** Automatisk opgradering er aktiveret.

- **Deaktiveret:** Automatisk opgradering er deaktiveret.

- **Suspenderet:** Systemet er ikke længere berettiget til at modtage automatiske opgraderinger. Du kan ikke konfigurere denne værdi. det er indstillet af systemet.

Du kan finde flere oplysninger [under Automatisk opgradering.](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-feature-automatic-upgrade)

Hvis du vil downloade den nyeste version af Azure AD Forbind, skal du gå til [https://www.microsoft.com/download/details.aspx?id=47594](https://www.microsoft.com/download/details.aspx?id=47594) .
