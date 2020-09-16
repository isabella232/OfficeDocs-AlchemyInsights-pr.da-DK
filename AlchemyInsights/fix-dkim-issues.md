---
title: Ret DKIM-konfigurationsproblemer
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
ms.openlocfilehash: 35e8023d26fe26211e27521ceb8751d2d7fc7a21
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 09/14/2020
ms.locfileid: "47744944"
---
# <a name="fix-dkim-setup-issues"></a>Ret DKIM-konfigurationsproblemer

Hvis du oplever problemer med at aktivere DKIM til dit brugerdefinerede domæne, skal du følge disse trin:

- De fleste DKIM-konfigurationsproblemer er relateret til forkerte DNS-poster. Kontrollér, at posten DKIM CNAME (**ikke** en TXT-post) er formateret korrekt. Du kan finde flere oplysninger i dette [emne](https://docs.microsoft.com/microsoft-365/security/office-365-security/use-dkim-to-validate-outbound-email#steps-you-need-to-do-to-manually-set-up-dkim).

- Når du har oprettet eller opdateret dine DKIM DNS-poster hos DNS-værtstjenesten for dit domæne (typisk en domæneregistrator), skal du vente på, at DNS-posterne skal overføres.

- Hvis du ikke kan oprette DKIM DNS-poster i administration, kan du erstatte \<CustomDomain\> med dit brugerdefinerede domæne (f. eks contoso.com) og køre denne kommando i [Exchange Online PowerShell](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell): `New-DkimSigningConfig -DomainName <CustomDomain> -Enabled $true` .
