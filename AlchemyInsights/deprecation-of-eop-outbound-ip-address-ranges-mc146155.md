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
ms.custom: 1065
ms.assetid: bd41784e-8002-428d-bc19-25671cfd34e8
ms.openlocfilehash: 17beb1722142d94ea05b67ce5ed1f20f8b11375c
ms.sourcegitcommit: 9d78905c512192ffc4675468abd2efc5f2e4baf4
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 04/23/2019
ms.locfileid: "32404815"
---
# <a name="deprecation-of-eop-outbound-ip-address-ranges"></a><span data-ttu-id="9c86f-102">Ændrede funktionsmåde for EOP udgående IP-adresseområder</span><span class="sxs-lookup"><span data-stu-id="9c86f-102">Deprecation of EOP outbound IP address ranges</span></span>

<span data-ttu-id="9c86f-103">Vi har registreret et potentielt problem med din organisation, der (Hvis ikke rettet af 26. oktober 2018) kan afbryde strømmen af e-mails til din lokale eller eksterne destinationer.</span><span class="sxs-lookup"><span data-stu-id="9c86f-103">We've detected a potential issue with your organization that (if not corrected by October 26th, 2018) might break mail flow to your on-premises or external destinations.</span></span> <span data-ttu-id="9c86f-104">Som tidligere meddelt, for at forenkle administration af IP-adressen område konsoliderer vi de Exchange Online beskyttelse (EOP) IP-adresseområder, der bruges til at sende og modtage e-mail uden for Office 365.</span><span class="sxs-lookup"><span data-stu-id="9c86f-104">As previously communicated, to simplify IP address range management, we're consolidating the Exchange Online Protection (EOP) IP address ranges that are used to send and receive email outside of Office 365.</span></span> <span data-ttu-id="9c86f-105">Vores analyse viser, at en eller flere af de eksterne e-mail-kilder eller destinationer, som du har konfigureret i mail flow forbindelser ikke acceptere forbindelser fra den IP-adresse intervaller vises [her](https://docs.microsoft.com/office365/SecurityCompliance/eop/exchange-online-protection-ip-addresses).</span><span class="sxs-lookup"><span data-stu-id="9c86f-105">Our analysis indicates that one or more of the external email sources or destinations that you've configured in mail flow connectors aren't accepting connections from the IP address ranges shown [here](https://docs.microsoft.com/office365/SecurityCompliance/eop/exchange-online-protection-ip-addresses).</span></span>

<span data-ttu-id="9c86f-106">Tage stilling til inden oktober 26 for at sikre, at disse kilder til og destinationer accepterer forbindelser til og fra alle [udgivet EOP IP-adresser](https://docs.microsoft.com/office365/SecurityCompliance/eop/exchange-online-protection-ip-addresses).</span><span class="sxs-lookup"><span data-stu-id="9c86f-106">Act before October 26th to ensure these sources and destinations will accept connections to and from all [published EOP IP addresses](https://docs.microsoft.com/office365/SecurityCompliance/eop/exchange-online-protection-ip-addresses).</span></span>

<span data-ttu-id="9c86f-107">Yderligere oplysninger om denne ændring, finder du bogfører Message Center, [MC146155](https://portal.office.com/AdminPortal/home?switchtomodern=true#/MessageCenter?id=MC146155), [MC148620](https://portal.office.com/AdminPortal/home?switchtomodern=true#/MessageCenter?id=MC148620)eller [MC149274](https://portal.office.com/AdminPortal/home?switchtomodern=true#/MessageCenter?id=MC149274).</span><span class="sxs-lookup"><span data-stu-id="9c86f-107">For more information about this change, please see Message Center posts [MC146155](https://portal.office.com/AdminPortal/home?switchtomodern=true#/MessageCenter?id=MC146155), [MC148620](https://portal.office.com/AdminPortal/home?switchtomodern=true#/MessageCenter?id=MC148620), or [MC149274](https://portal.office.com/AdminPortal/home?switchtomodern=true#/MessageCenter?id=MC149274).</span></span>

<span data-ttu-id="9c86f-108">**Bemærk**: Hvis du tidligere har brugt IP- eller URL-adresse til udgivelse via HTML-, XML- og RSS-slutpunkt opdateringer, du også bør skifte til de nye webtjenester til automatisering af disse typer opdateringer.</span><span class="sxs-lookup"><span data-stu-id="9c86f-108">**Note**: If you previously used IP or URL publishing via HTML, XML, and RSS for endpoint updates, you also should migrate to the new web services for automating these types of updates.</span></span> <span data-ttu-id="9c86f-109">Yderligere oplysninger finder du i [Office 365 slutpunkt kategorier og Office 365 IP-adresse og URL-adresse til webtjeneste](https://techcommunity.microsoft.com/t5/Office-365-Blog/Announcing-Office-365-endpoint-categories-and-Office-365-IP/ba-p/177638).</span><span class="sxs-lookup"><span data-stu-id="9c86f-109">For more information, see [Office 365 endpoint categories and Office 365 IP Address and URL web service](https://techcommunity.microsoft.com/t5/Office-365-Blog/Announcing-Office-365-endpoint-categories-and-Office-365-IP/ba-p/177638).</span></span>
