---
title: 932-opgradering AADConnect
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
ms.openlocfilehash: 5c8ec5d9282c53c655e28f5d38fe36fc3ab005b8
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 09/15/2020
ms.locfileid: "47806033"
---
# <a name="upgrade-azure-ad-connect"></a>Opgrader Azure AD Connect

Automatisk opgradering er som standard aktiveret for Azure AD Connect, hvilket er med til at sikre, at du kører den nyeste version. Hvis du vil kontrollere indstillingerne for automatisk opgradering, skal du bruge **Get-ADSyncAutoUpgrade** -cmdlet'en i Azure ad PowerShell. Cmdlet returnerer en af følgende værdier:

- **Aktiveret**: automatisk opgradering er aktiveret.

- **Deaktiveret**: automatisk opgradering er deaktiveret.

- **Suspenderet**: systemet er ikke længere berettiget til at modtage automatiske opgraderinger. Du kan ikke konfigurere denne værdi. den er indstillet af systemet.

Hvis du vil have mere at vide, skal du se [automatisk opgradering](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-feature-automatic-upgrade).

Hvis du vil hente den nyeste version af Azure AD Connect, skal du gå til [https://www.microsoft.com/download/details.aspx?id=47594](https://www.microsoft.com/download/details.aspx?id=47594) .
