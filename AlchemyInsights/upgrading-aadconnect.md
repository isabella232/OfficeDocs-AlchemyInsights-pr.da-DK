---
title: 932 opgradering af AADConnect
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 6/8/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "932"
- "1300025"
ms.assetid: 8f43f36c-9722-43a4-b0de-c5341c06dac5
ms.openlocfilehash: ff3f74348599788edd8ce0991fe49bb6a54b55af
ms.sourcegitcommit: 1d98db8acb9959aba3b5e308a567ade6b62da56c
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 08/22/2019
ms.locfileid: "36506077"
---
# <a name="upgrade-azure-ad-connect"></a>Opgradering af Azure AD forbindelse

Automatisk opgradering er som standard aktiveret for Azure AD Connect, som hjælper med at sikre, at du kører den nyeste version. For at kontrollere indstillingerne for automatiske opgradering, kan du bruge cmdlet **Get-ADSyncAutoUpgrade** i Azure AD PowerShell. Cmdlet returnerer en af følgende værdier:

- **Aktiveret**: automatisk opgradering er aktiveret.

- **Deaktiveret**: automatisk opgradering er deaktiveret.

- **Suspenderet**: systemet ikke længere er berettiget til at modtage automatiske opgraderinger. Du kan ikke konfigurere denne værdi; angives af systemet.

Yderligere oplysninger finder du under [automatisk opgradering](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-feature-automatic-upgrade).

For at hente den nyeste version af Azure AD Connect, skal du gå til [https://www.microsoft.com/download/details.aspx?id=47594](https://www.microsoft.com/download/details.aspx?id=47594).
