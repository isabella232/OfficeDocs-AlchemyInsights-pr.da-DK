---
title: 1554 Winsock-fejl 10061
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1554"
- "9000079"
ms.assetid: caecfa19-86c9-4aa4-9c83-b8a974ce60b9
ms.openlocfilehash: 7991f83a0b4791eaa7eb3246f7e61f781e4c7430931fbf920d7fd9e44c018d13
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 08/05/2021
ms.locfileid: "54083224"
---
# <a name="winsock-error-10061"></a>Winsock-fejl 10061

Denne fejlkode betyder, at Microsoft ikke kunne oprette en TCP-socket (forbindelse) med destinationsværten. Den mest sandsynlige årsag til denne fejl er et problem med konfigurationen af din firewall. Du kan løse problemet ved at kontrollere disse indstillinger:

- Bekræft din firewallkonfiguration med oplysningerne i [Microsoft 365 URL-adresser og IP-adresseintervaller](https://docs.microsoft.com/office365/enterprise/urls-and-ip-address-ranges)

- Hvis fejlen er specifik for Exchange Online Protection (EOP), skulle du tidligere have fået besked om en ændring af [Exchange Online Protection IP-adresserne.](https://docs.microsoft.com/office365/SecurityCompliance/eop/exchange-online-protection-ip-addresses)

- Kontrollér, at din internetudbyder ikke blokerer porten.

- Bekræft indstillingerne for den intelligente vært og målserver i dine forbindelser.

Bemærk, Microsoft 365 ikke blokerer for *indgående* forbindelser på denne måde.
