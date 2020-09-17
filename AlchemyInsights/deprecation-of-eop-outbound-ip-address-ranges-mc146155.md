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
# <a name="deprecation-of-eop-outbound-ip-address-ranges"></a>Frarådes for EOP udgående IP-adresseområder

Vi har registreret et potentielt problem med din organisation, som (hvis det ikke er rettet i oktober 26th, 2018), kan bryde mail flow til dit lokale eller eksterne destinationer. Som tidligere blevet kommunikeret for at forenkle administration af IP-adresser, konsoliderer vi IP-adresseområder for Exchange Online Protection (EOP), der bruges til at sende og modtage mails uden for Microsoft 365. Vores analyse angiver, at en eller flere af de eksterne mail kilder eller destinationer, du har konfigureret i mail flow forbindelser, ikke accepterer forbindelser fra de IP-adresseområder, der er vist [her](https://docs.microsoft.com/office365/SecurityCompliance/eop/exchange-online-protection-ip-addresses).

Act før oktober 26th for at sikre, at disse kilder og destinationer accepterer forbindelser til og fra alle [publicerede EOP-IP-adresser](https://docs.microsoft.com/office365/SecurityCompliance/eop/exchange-online-protection-ip-addresses).

Hvis du vil have mere at vide om denne ændring, skal du se meddelelses Center indlæg [MC146155](https://portal.office.com/AdminPortal/home?switchtomodern=true#/MessageCenter?id=MC146155), [MC148620](https://portal.office.com/AdminPortal/home?switchtomodern=true#/MessageCenter?id=MC148620)eller [MC149274](https://portal.office.com/AdminPortal/home?switchtomodern=true#/MessageCenter?id=MC149274).

**Bemærk**! hvis du tidligere har brugt IP-eller URL-udgivelse via HTML, XML og RSS til Endpoint-opdateringer, skal du også overføre til de nye webtjenester for at automatisere disse typer opdateringer. Du kan finde flere oplysninger i [Microsoft 365-slutpunkts kategorier og microsoft 365 IP address and URL-adresse til webtjeneste](https://techcommunity.microsoft.com/t5/Office-365-Blog/Announcing-Office-365-endpoint-categories-and-Office-365-IP/ba-p/177638).
