---
title: 1065 Fraråding af EOP-udgående IP-adresseintervallerMC146155
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
ms.openlocfilehash: 214abc57a99c70a02a7d159441713e007f6ad980f67e373780d4ca297f69f764
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 08/05/2021
ms.locfileid: "54031256"
---
# <a name="deprecation-of-eop-outbound-ip-address-ranges"></a>Udrådning af EOP-udgående IP-adresseintervaller

Vi har registreret et potentielt problem med din organisation, som (hvis dette ikke er rettet d. 26. oktober 2018) kan bryde mailflow til dine lokale eller eksterne destinationer. For at forenkle administration af IP-adresseområde konsoliderer vi som tidligere de EXCHANGE ONLINE PROTECTION-adresseintervaller (EOP), der bruges til at sende og modtage mails uden for Microsoft 365. Vores analyse indikerer, at en eller flere af de eksterne mailkilder eller destinationer, som du har konfigureret i mailflowforbindelser, ikke accepterer forbindelser fra de IP-adresseområder, der er vist [her.](https://docs.microsoft.com/office365/SecurityCompliance/eop/exchange-online-protection-ip-addresses)

Der skal handles inden d. 26. oktober for at sikre, at disse kilder og destinationer accepterer forbindelser til og fra alle [publicerede EOP IP-adresser.](https://docs.microsoft.com/office365/SecurityCompliance/eop/exchange-online-protection-ip-addresses)

Du kan finde flere oplysninger om denne ændring i Indlæg i Meddelelsescenter [MC146155,](https://portal.office.com/AdminPortal/home?switchtomodern=true#/MessageCenter?id=MC146155) [MC148620](https://portal.office.com/AdminPortal/home?switchtomodern=true#/MessageCenter?id=MC148620)eller [MC149274.](https://portal.office.com/AdminPortal/home?switchtomodern=true#/MessageCenter?id=MC149274)

**Bemærk!** Hvis du tidligere har brugt IP- eller URL-publicering via HTML, XML og RSS til slutpunktsopdateringer, skal du også overføre til de nye webtjenester for at automatisere disse typer opdateringer. Du kan finde flere oplysninger [Microsoft 365 endpointkategorier og Microsoft 365 IP-adresse og URL-webtjeneste.](https://techcommunity.microsoft.com/t5/Office-365-Blog/Announcing-Office-365-endpoint-categories-and-Office-365-IP/ba-p/177638)
