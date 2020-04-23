---
title: 1554 Winsock-fejl 10061
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1554"
- "9000079"
ms.assetid: caecfa19-86c9-4aa4-9c83-b8a974ce60b9
ms.openlocfilehash: e8f62d97efc937518ef766b45e1747e83b7f99c3
ms.sourcegitcommit: 631cbb5f03e5371f0995e976536d24e9d13746c3
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 04/22/2020
ms.locfileid: "43766163"
---
# <a name="winsock-error-10061"></a>Winsock-fejl 10061

Denne fejlkode betyder, at Microsoft ikke kunne oprette en TCP-socket (forbindelse) med destinationsværten. Den mest sandsynlige årsag til denne fejl er et problem med firewallkonfigurationen. Du kan løse problemet ved at kontrollere disse indstillinger:

- Kontroller din firewallkonfiguration med oplysningerne i [Microsoft 365 URL-adresser og IP-adresseområder](https://docs.microsoft.com/office365/enterprise/urls-and-ip-address-ranges)

- Hvis fejlen er specifik for Exchange Online Protection (EOP), skulle du tidligere have fået besked om en ændring af [Exchange Online Protection IP-adresserne](https://docs.microsoft.com/office365/SecurityCompliance/eop/exchange-online-protection-ip-addresses).

- Kontroller, at internetudbyderen ikke blokerer porten.

- Kontroller indstillingerne for smart-vært og målserver i dine forbindelser.

Bemærk, at Microsoft 365 ikke blokerer *indgående* forbindelser på denne måde.
