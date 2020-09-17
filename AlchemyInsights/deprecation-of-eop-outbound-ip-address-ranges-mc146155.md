---
title: 1065 fraråder EOP udgående IP-adresse rangesMC146155
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom: 1065
ms.assetid: bd41784e-8002-428d-bc19-25671cfd34e8
ms.openlocfilehash: afd725668f906339f4b7d769bb67a4d2ee5a6ac6
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 09/15/2020
ms.locfileid: "47806789"
---
# <a name="deprecation-of-eop-outbound-ip-address-ranges"></a><span data-ttu-id="83a7f-102">Frarådes for EOP udgående IP-adresseområder</span><span class="sxs-lookup"><span data-stu-id="83a7f-102">Deprecation of EOP outbound IP address ranges</span></span>

<span data-ttu-id="83a7f-103">Vi har registreret et potentielt problem med din organisation, som (hvis det ikke er rettet i oktober 26th, 2018), kan bryde mail flow til dit lokale eller eksterne destinationer.</span><span class="sxs-lookup"><span data-stu-id="83a7f-103">We've detected a potential issue with your organization that (if not corrected by October 26th, 2018) might break mail flow to your on-premises or external destinations.</span></span> <span data-ttu-id="83a7f-104">Som tidligere blevet kommunikeret for at forenkle administration af IP-adresser, konsoliderer vi IP-adresseområder for Exchange Online Protection (EOP), der bruges til at sende og modtage mails uden for Microsoft 365.</span><span class="sxs-lookup"><span data-stu-id="83a7f-104">As previously communicated, to simplify IP address range management, we're consolidating the Exchange Online Protection (EOP) IP address ranges that are used to send and receive email outside of Microsoft 365.</span></span> <span data-ttu-id="83a7f-105">Vores analyse angiver, at en eller flere af de eksterne mail kilder eller destinationer, du har konfigureret i mail flow forbindelser, ikke accepterer forbindelser fra de IP-adresseområder, der er vist [her](https://docs.microsoft.com/office365/SecurityCompliance/eop/exchange-online-protection-ip-addresses).</span><span class="sxs-lookup"><span data-stu-id="83a7f-105">Our analysis indicates that one or more of the external email sources or destinations that you've configured in mail flow connectors aren't accepting connections from the IP address ranges shown [here](https://docs.microsoft.com/office365/SecurityCompliance/eop/exchange-online-protection-ip-addresses).</span></span>

<span data-ttu-id="83a7f-106">Act før oktober 26th for at sikre, at disse kilder og destinationer accepterer forbindelser til og fra alle [publicerede EOP-IP-adresser](https://docs.microsoft.com/office365/SecurityCompliance/eop/exchange-online-protection-ip-addresses).</span><span class="sxs-lookup"><span data-stu-id="83a7f-106">Act before October 26th to ensure these sources and destinations will accept connections to and from all [published EOP IP addresses](https://docs.microsoft.com/office365/SecurityCompliance/eop/exchange-online-protection-ip-addresses).</span></span>

<span data-ttu-id="83a7f-107">Hvis du vil have mere at vide om denne ændring, skal du se meddelelses Center indlæg [MC146155](https://portal.office.com/AdminPortal/home?switchtomodern=true#/MessageCenter?id=MC146155), [MC148620](https://portal.office.com/AdminPortal/home?switchtomodern=true#/MessageCenter?id=MC148620)eller [MC149274](https://portal.office.com/AdminPortal/home?switchtomodern=true#/MessageCenter?id=MC149274).</span><span class="sxs-lookup"><span data-stu-id="83a7f-107">For more information about this change, please see Message Center posts [MC146155](https://portal.office.com/AdminPortal/home?switchtomodern=true#/MessageCenter?id=MC146155), [MC148620](https://portal.office.com/AdminPortal/home?switchtomodern=true#/MessageCenter?id=MC148620), or [MC149274](https://portal.office.com/AdminPortal/home?switchtomodern=true#/MessageCenter?id=MC149274).</span></span>

<span data-ttu-id="83a7f-108">**Bemærk**! hvis du tidligere har brugt IP-eller URL-udgivelse via HTML, XML og RSS til Endpoint-opdateringer, skal du også overføre til de nye webtjenester for at automatisere disse typer opdateringer.</span><span class="sxs-lookup"><span data-stu-id="83a7f-108">**Note**: If you previously used IP or URL publishing via HTML, XML, and RSS for endpoint updates, you also should migrate to the new web services for automating these types of updates.</span></span> <span data-ttu-id="83a7f-109">Du kan finde flere oplysninger i [Microsoft 365-slutpunkts kategorier og microsoft 365 IP address and URL-adresse til webtjeneste](https://techcommunity.microsoft.com/t5/Office-365-Blog/Announcing-Office-365-endpoint-categories-and-Office-365-IP/ba-p/177638).</span><span class="sxs-lookup"><span data-stu-id="83a7f-109">For more information, see [Microsoft 365 endpoint categories and Microsoft 365 IP Address and URL web service](https://techcommunity.microsoft.com/t5/Office-365-Blog/Announcing-Office-365-endpoint-categories-and-Office-365-IP/ba-p/177638).</span></span>
