---
title: Løs problemer med dkim-opsætning
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom: 1389
ms.assetid: ''
ms.openlocfilehash: 8195b0e3fada6da033b2d95b1fc6600e7fa3341e
ms.sourcegitcommit: bc7d6f4f3c9f7060d073f5130e1ec856e248d020
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 06/02/2020
ms.locfileid: "44506768"
---
# <a name="fix-dkim-setup-issues"></a>Løs problemer med dkim-opsætning

Hvis du oplever problemer med at aktivere DKIM for dit brugerdefinerede domæne, skal du følge nedenstående trin:

- De fleste DKIM-installationsproblemer er relateret til forkerte DNS-poster. Kontroller, at DKIM CNAME-posten **(ikke** en TXT-post) er formateret korrekt. Yderligere oplysninger finder du i dette [emne](https://docs.microsoft.com/microsoft-365/security/office-365-security/use-dkim-to-validate-outbound-email#steps-you-need-to-do-to-manually-set-up-dkim).

- Når du har oprettet eller opdateret dine DKIM DNS-poster på DNS-hostingtjenesten for dit domæne (typisk dit domæneregistrator), skal du vente på, at DNS-posterne overføres.

- Hvis du ikke kan oprette DKIM DNS-posterne i Administration, kan du erstatte \<CustomDomain\> med dit brugerdefinerede domæne (f.eks. contoso.com) og køre denne kommando i [Exchange Online PowerShell](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell): `New-DkimSigningConfig -DomainName <CustomDomain> -Enabled $true` .
