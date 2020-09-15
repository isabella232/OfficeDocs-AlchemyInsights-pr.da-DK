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
ms.openlocfilehash: 4f8007bd8ccb4666260c75fdca15dd0b14eb4e96
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 09/14/2020
ms.locfileid: "47698856"
---
# <a name="winsock-error-10061"></a>Winsock-fejl 10061

Denne fejlkode betyder, at Microsoft ikke kan oprette en TCP-sokkel (forbindelse) med destinationsværten. Den mest sandsynlige årsag til fejlen er et problem med konfigurationen af din firewall. Hvis du vil rette problemet, skal du kontrollere disse indstillinger:

- Kontrollér din firewall-konfiguration med oplysningerne i [Microsoft 365 URL-adresser og IP-adresseområder](https://docs.microsoft.com/office365/enterprise/urls-and-ip-address-ranges)

- Hvis fejlen er specifik for Exchange Online Protection (EOP), skal du tidligere have fået besked om en ændring af [IP-adresserne for Exchange Online Protection](https://docs.microsoft.com/office365/SecurityCompliance/eop/exchange-online-protection-ip-addresses).

- Kontrollér, at din internetudbyder ikke blokerer porten.

- Kontrollér indstillingerne for smart Host og destinationsserveren i dine forbindelser.

Bemærk, at Microsoft 365 ikke blokerer *indgående* forbindelser på denne måde.
