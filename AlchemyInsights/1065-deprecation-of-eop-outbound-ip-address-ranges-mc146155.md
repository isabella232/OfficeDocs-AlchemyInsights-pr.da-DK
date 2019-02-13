---
title: 1065 ændrede funktionsmåde af EOP udgående IP-adresse rangesMC146155
ms.author: chrisda
author: chrisda
manager: serdars
ms.date: 9/28/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: bd41784e-8002-428d-bc19-25671cfd34e8
ms.openlocfilehash: 2b4b2e2341f45e2d37713d72a2e0d34fa1a9a7cc
ms.sourcegitcommit: dd43cc0a9470f98b8ef2a3787c823801d674c666
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 02/12/2019
ms.locfileid: "29934878"
---
# <a name="deprecation-of-eop-outbound-ip-address-ranges"></a>Ændrede funktionsmåde for EOP udgående IP-adresseområder

Vi har registreret et potentielt problem med din organisation, der (Hvis ikke rettet af 26. oktober 2018) kan afbryde strømmen af e-mails til din lokale eller eksterne destinationer. Som tidligere meddelt, for at forenkle administration af IP-adressen område konsoliderer vi de Exchange Online beskyttelse (EOP) IP-adresseområder, der bruges til at sende og modtage e-mail uden for Office 365. Vores analyse viser, at en eller flere af de eksterne e-mail-kilder eller destinationer, som du har konfigureret i mail flow forbindelser ikke acceptere forbindelser fra den IP-adresse intervaller vises [her](https://docs.microsoft.com/office365/SecurityCompliance/eop/exchange-online-protection-ip-addresses).
  
Tage stilling til inden oktober 26 for at sikre, at disse kilder til og destinationer accepterer forbindelser til og fra alle [udgivet EOP IP-adresser](https://docs.microsoft.com/office365/SecurityCompliance/eop/exchange-online-protection-ip-addresses).
  
Yderligere oplysninger om denne ændring, finder du bogfører Message Center, [MC146155](https://portal.office.com/AdminPortal/home?switchtomodern=true#/MessageCenter?id=MC146155), [MC148620](https://portal.office.com/AdminPortal/home?switchtomodern=true#/MessageCenter?id=MC148620)eller [MC149274](https://portal.office.com/AdminPortal/home?switchtomodern=true#/MessageCenter?id=MC149274).
  
 **Bemærk**: Hvis du tidligere har brugt IP- eller URL-adresse til udgivelse via HTML-, XML- og RSS-slutpunkt opdateringer, du også bør skifte til de nye webtjenester til automatisering af disse typer opdateringer. Yderligere oplysninger finder du i [Office 365 slutpunkt kategorier og Office 365 IP-adresse og URL-adresse til webtjeneste](https://techcommunity.microsoft.com/t5/Office-365-Blog/Announcing-Office-365-endpoint-categories-and-Office-365-IP/ba-p/177638).
  

