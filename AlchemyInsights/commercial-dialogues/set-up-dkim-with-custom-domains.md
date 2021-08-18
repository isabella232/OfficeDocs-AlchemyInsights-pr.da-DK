---
title: Konfigurer DKIM med brugerdefinerede domæner
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 02/22/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9002531"
- "7375"
ms.openlocfilehash: cb1f621dffc88464c339b55998efb5440cfd775c
ms.sourcegitcommit: ab75f66355116e995b3cb5505465b31989339e28
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 08/13/2021
ms.locfileid: "58332301"
---
# <a name="set-up-dkim-with-custom-domains"></a>Konfigurer DKIM med brugerdefinerede domæner

Du skal publicere to CNAME-poster for hvert brugerdefineret domæne i DNS. Det gør du ved at bruge følgende format:

```console
Host name:            selector1._domainkey
Points to address or value:    selector1-<domainGUID>._domainkey.<initialDomain>
TTL:                3600

Host name:            selector2._domainkey
Points to address or value:    selector2-<domainGUID>._domainkey.<initialDomain>
TTL:                3600
```
**Bemærk!** **DomainGUID** er teksten til venstre for **.mail.protection.outlook.com** i den brugerdefinerede MX-post for det brugerdefinerede domæne (f.eks. contoso-com for **domænet contoso.com).** **InitialDomain er** det domæne, du brugte, da du tilmeldte dig Office 365 (f.eks. **contoso.onmicrosoft.com**).

Du kan finde flere oplysninger om DNS-poster [under Oprette DNS-poster for din DNS-udbyder Office 365](https://docs.microsoft.com/microsoft-365/admin/get-help-with-domains/create-dns-records-at-any-dns-hosting-provider).