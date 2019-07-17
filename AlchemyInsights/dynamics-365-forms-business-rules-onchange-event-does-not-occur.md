---
title: Dynamics 365 danner forretningsregler - forretningsregel udløser ikke i en formular
ms.author: pebaum
author: pebaum
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1926"
- "6200018"
ms.openlocfilehash: 4ade8d2f68b465298e2d6efff3eef4f04f25c3bf
ms.sourcegitcommit: a413a0e27ef4ab8c484fa9fccff8bbef381c8b96
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 07/16/2019
ms.locfileid: "35747293"
---
# <a name="onchange-event-does-not-occur-if-the-field-is-changed-programmatically"></a>OnChange-hændelsen opstår ikke, hvis feltet ændres via programmering

*OnChange* -hændelsen opstår ikke, hvis feltet ændres via programmering ved hjælp af den *attribut.* [AngivVærdi](https://docs.microsoft.com/en-us/dynamics365/customer-engagement/developer/clientapi/reference/attributes/setvalue) metode. Hvis du vil hændelseshandlere for hændelsen *OnChange* til at køre, når du angiver den værdi, du skal bruge den *attribut for formContext.data.entity.* [fireOnchange](https://docs.microsoft.com/en-us/dynamics365/customer-engagement/developer/clientapi/reference/attributes/fireonchange) metode i din kode.

[https://docs.microsoft.com/dynamics365/customer-engagement/developer/clientapi/reference/events/attribute-onchange](https://docs.microsoft.com/en-us/dynamics365/customer-engagement/developer/clientapi/reference/events/attribute-onchange)
