---
title: Løse problemer med installationen af DKIM
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: ''
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom: 1389
ms.assetid: ''
ms.openlocfilehash: 4d6dadbcbf71fe6e9ea56d6a82a7d8ababdd38ef
ms.sourcegitcommit: 4b7e478ce700c0b781efec3857ac4dce5bdf00c6
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 06/07/2019
ms.locfileid: "34764955"
---
# <a name="fix-dkim-setup-issues"></a>Løse problemer med installationen af DKIM

Hvis du oplever problemer med at aktivere DKIM for dit brugerdefinerede domæne, kan du bruge følgende trin:

- De fleste problemer med installationen af DKIM er relateret til forkert DNS-poster. Kontroller, at DKIM CNAME-posten (**ikke** en TXT-post) er formateret korrekt. Yderligere oplysninger finder du i dette [emne](https://docs.microsoft.com/office365/SecurityCompliance/use-dkim-to-validate-outbound-email#what-you-need-to-do-to-manually-set-up-dkim-in-office-365).

- Når du opretter eller opdaterer din DKIM DNS-poster på DNS-værtstjeneste for dit domæne (typisk din domæneregistrator), venter på DNS-poster til at sprede.

- Hvis du ikke kan oprette DKIM DNS poster i admin center, kan du erstatte \<CustomDomain\> med dit brugerdefinerede domæne (for eksempel contoso.com) og køre denne kommando i [Exchange Online PowerShell](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell): `New-DkimSigningConfig -DomainName <CustomDomain> -Enabled $true`.
