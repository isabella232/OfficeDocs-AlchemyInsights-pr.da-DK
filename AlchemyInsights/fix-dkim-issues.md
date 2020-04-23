---
title: Løs problemer med Konfiguration af DKIM
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
ms.openlocfilehash: d725eb0d46dcbf1b5b6d77ca9f59fcafa5298bf1
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 04/22/2020
ms.locfileid: "43717556"
---
# <a name="fix-dkim-setup-issues"></a>Løs problemer med Konfiguration af DKIM

Hvis du oplever problemer med at aktivere DKIM for dit brugerdefinerede domæne, skal du følge følgende fremgangsmåde:

- De fleste DKIM-installationsproblemer er relateret til forkerte DNS-poster. Kontroller, at DKIM CNAME-posten **(ikke** en TXT-post) er formateret korrekt. Yderligere oplysninger finder du i dette [emne](https://docs.microsoft.com/office365/SecurityCompliance/use-dkim-to-validate-outbound-email#what-you-need-to-do-to-manually-set-up-dkim-in-office-365).

- Når du har oprettet eller opdateret dine DKIM DNS-poster på DNS-hostingtjenesten for dit domæne (typisk din domæneregistrator), skal du vente på, at DNS-posterne overføres.

- Hvis du ikke kan oprette DKIM DNS-posterne i \<Administration, kan du erstatte CustomDomain\> med dit brugerdefinerede domæne `New-DkimSigningConfig -DomainName <CustomDomain> -Enabled $true`(f.eks. contoso.com) og køre denne kommando i Exchange Online [PowerShell](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell): .
