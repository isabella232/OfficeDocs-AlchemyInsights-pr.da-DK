---
title: 1065 ændrede funktionsmåde af EOP udgående IP-adresse rangesMC146155
ms.author: chrisda
author: chrisda
manager: serdars
ms.date: 9/28/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.assetid: bd41784e-8002-428d-bc19-25671cfd34e8
ms.openlocfilehash: ec87141ffaa2fa3484620a9b52851e3e92f20b6b
ms.sourcegitcommit: d6ea5e9458a2b8ceaab3ac4bd483e1130b9a398a
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 01/15/2019
ms.locfileid: "28282716"
---
# <a name="deprecation-of-eop-outbound-ip-address-ranges"></a><span data-ttu-id="30fa9-102">Ændrede funktionsmåde for EOP udgående IP-adresseområder</span><span class="sxs-lookup"><span data-stu-id="30fa9-102">Deprecation of EOP outbound IP address ranges</span></span>

<span data-ttu-id="30fa9-p101">Vi har registreret et potentielt problem med din organisation, der (Hvis ikke rettet af 26. oktober 2018) kan afbryde strømmen af e-mails til din lokale eller eksterne destinationer. Som tidligere meddelt, for at forenkle administration af IP-adressen område konsoliderer vi de Exchange Online beskyttelse (EOP) IP-adresseområder, der bruges til at sende og modtage e-mail uden for Office 365. Vores analyse viser, at en eller flere af de eksterne e-mail-kilder eller destinationer, som du har konfigureret i mail flow forbindelser ikke acceptere forbindelser fra den IP-adresse intervaller vises [her](https://docs.microsoft.com/office365/SecurityCompliance/eop/exchange-online-protection-ip-addresses).</span><span class="sxs-lookup"><span data-stu-id="30fa9-p101">We've detected a potential issue with your organization that (if not corrected by October 26th, 2018) might break mail flow to your on-premises or external destinations. As previously communicated, to simplify IP address range management, we're consolidating the Exchange Online Protection (EOP) IP address ranges that are used to send and receive email outside of Office 365. Our analysis indicates that one or more of the external email sources or destinations that you've configured in mail flow connectors aren't accepting connections from the IP address ranges shown [here](https://docs.microsoft.com/office365/SecurityCompliance/eop/exchange-online-protection-ip-addresses).</span></span>
  
<span data-ttu-id="30fa9-106">Tage stilling til inden oktober 26 for at sikre, at disse kilder til og destinationer accepterer forbindelser til og fra alle [udgivet EOP IP-adresser](https://docs.microsoft.com/office365/SecurityCompliance/eop/exchange-online-protection-ip-addresses).</span><span class="sxs-lookup"><span data-stu-id="30fa9-106">Act before October 26th to ensure these sources and destinations will accept connections to and from all [published EOP IP addresses](https://docs.microsoft.com/office365/SecurityCompliance/eop/exchange-online-protection-ip-addresses).</span></span>
  
<span data-ttu-id="30fa9-107">Yderligere oplysninger om denne ændring, finder du bogfører Message Center, [MC146155](https://portal.office.com/AdminPortal/home?switchtomodern=true#/MessageCenter?id=MC146155), [MC148620](https://portal.office.com/AdminPortal/home?switchtomodern=true#/MessageCenter?id=MC148620)eller [MC149274](https://portal.office.com/AdminPortal/home?switchtomodern=true#/MessageCenter?id=MC149274).</span><span class="sxs-lookup"><span data-stu-id="30fa9-107">For more information about this change, please see Message Center posts [MC146155](https://portal.office.com/AdminPortal/home?switchtomodern=true#/MessageCenter?id=MC146155), [MC148620](https://portal.office.com/AdminPortal/home?switchtomodern=true#/MessageCenter?id=MC148620), or [MC149274](https://portal.office.com/AdminPortal/home?switchtomodern=true#/MessageCenter?id=MC149274).</span></span>
  
 <span data-ttu-id="30fa9-p102">**Bemærk**: Hvis du tidligere har brugt IP- eller URL-adresse til udgivelse via HTML-, XML- og RSS-slutpunkt opdateringer, du også bør skifte til de nye webtjenester til automatisering af disse typer opdateringer. Yderligere oplysninger finder du i [Office 365 slutpunkt kategorier og Office 365 IP-adresse og URL-adresse til webtjeneste](https://techcommunity.microsoft.com/t5/Office-365-Blog/Announcing-Office-365-endpoint-categories-and-Office-365-IP/ba-p/177638).</span><span class="sxs-lookup"><span data-stu-id="30fa9-p102">**Note**: If you previously used IP or URL publishing via HTML, XML, and RSS for endpoint updates, you also should migrate to the new web services for automating these types of updates. For more information, see [Office 365 endpoint categories and Office 365 IP Address and URL web service](https://techcommunity.microsoft.com/t5/Office-365-Blog/Announcing-Office-365-endpoint-categories-and-Office-365-IP/ba-p/177638).</span></span>
  

