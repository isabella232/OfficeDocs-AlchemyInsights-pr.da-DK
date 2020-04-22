---
title: 1065 Udtædning af udgående IP-adresseintervallerMC146155
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom: 1065
ms.assetid: bd41784e-8002-428d-bc19-25671cfd34e8
ms.openlocfilehash: f4854c32d970d84f3a0664a9e384dc6e3cd0bfa7
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 04/22/2020
ms.locfileid: "43704591"
---
# <a name="deprecation-of-eop-outbound-ip-address-ranges"></a>Uddeførelse af udgående IP-adresseområder i EOP

Vi har opdaget et potentielt problem med din organisation, som (hvis det ikke er rettet inden den 26. oktober 2018), kan afbryde postflowet til dine lokale eller eksterne destinationer. Som tidligere meddelt konsoliderer vi de IP-adresseområder, der bruges til at sende og modtage mail uden for Microsoft 365, for at forenkle administration af IP-adresseområder. Vores analyse viser, at en eller flere af de eksterne e-mail-kilder eller destinationer, som du har konfigureret i mailflow-connectorer, ikke accepterer forbindelser fra de IP-adresseområder, der vises [her.](https://docs.microsoft.com/office365/SecurityCompliance/eop/exchange-online-protection-ip-addresses)

maj for at sikre , at disse kilder og destinationer accepterer forbindelser til og fra alle [offentliggjorte EOP IP-adresser](https://docs.microsoft.com/office365/SecurityCompliance/eop/exchange-online-protection-ip-addresses).

Yderligere oplysninger om denne ændring finder du i Message Center posts [MC146155](https://portal.office.com/AdminPortal/home?switchtomodern=true#/MessageCenter?id=MC146155), [MC148620](https://portal.office.com/AdminPortal/home?switchtomodern=true#/MessageCenter?id=MC148620)eller [MC149274](https://portal.office.com/AdminPortal/home?switchtomodern=true#/MessageCenter?id=MC149274).

**Bemærk:** Hvis du tidligere har brugt IP- eller URL-udgivelse via HTML, XML og RSS til slutpunktsopdateringer, skal du også overføre til de nye webtjenester for at automatisere disse typer opdateringer. Yderligere oplysninger finder du i [Microsoft 365-slutpunktskategorier og Microsoft 365 IP-adresse- og URL-webtjeneste](https://techcommunity.microsoft.com/t5/Office-365-Blog/Announcing-Office-365-endpoint-categories-and-Office-365-IP/ba-p/177638).
