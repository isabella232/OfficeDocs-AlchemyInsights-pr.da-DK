---
title: Løs problemer med DKIM-konfiguration
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom: 1389
ms.assetid: ''
ms.openlocfilehash: 5a613321ed79e657350ec4d19b1f07ac0a091b227a8268c793a10edd9990d41f
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 08/05/2021
ms.locfileid: "53945925"
---
# <a name="fix-dkim-setup-issues"></a>Løs problemer med DKIM-konfiguration

Hvis du oplever problemer med at aktivere DKIM for dit brugerdefinerede domæne, skal du følge disse trin:

- De fleste problemer med DKIM-konfigurationen er relateret til forkerte DNS-poster. Bekræft, at DKIM CNAME-posten **(ikke** en TXT-post) er formateret korrekt. Du kan finde flere oplysninger i dette [emne](https://docs.microsoft.com/microsoft-365/security/office-365-security/use-dkim-to-validate-outbound-email#steps-you-need-to-do-to-manually-set-up-dkim).

- Når du har oprettet eller opdateret dine DKIM DNS-poster hos DNS-hostingtjenesten for dit domæne (typisk din domæneregistrator), skal du vente på, at DNS-posterne overføres.

- Hvis du ikke kan oprette DKIM DNS-posterne i Administration, kan du erstatte med dit eget domæne (f.eks contoso.com) og køre denne kommando \<CustomDomain\> [i Exchange Online PowerShell:](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell) `New-DkimSigningConfig -DomainName <CustomDomain> -Enabled $true`
