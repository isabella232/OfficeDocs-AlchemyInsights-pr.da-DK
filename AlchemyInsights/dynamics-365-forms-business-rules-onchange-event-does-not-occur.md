---
title: Dynamics 365 Forms Forretningsregler – Forretningsregel køres ikke for en formular
ms.author: pebaum
author: pebaum
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1926"
- "6200018"
ms.openlocfilehash: 8425918950e1ef6c44f2866e6fa8987fe165536ae21e08ea6a1da880f761d512
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 08/05/2021
ms.locfileid: "53947293"
---
# <a name="onchange-event-does-not-occur-if-the-field-is-changed-programmatically"></a>Hændelsen VedÆndring forekommer ikke, hvis feltet ændres via programmering

Hændelsen *VedÆndring* udføres ikke, hvis feltet ændres via programmering ved hjælp af *attributten.* [setValue-metode.](https://docs.microsoft.com/dynamics365/customer-engagement/developer/clientapi/reference/attributes/setvalue) Hvis du vil have hændelseshandlerne for hændelsen *VedÆndring* til at køre, efter du har angivet værdien, skal du bruge *attributten formContext.data.entity* [fireOnchange](https://docs.microsoft.com/dynamics365/customer-engagement/developer/clientapi/reference/attributes/fireonchange) i din kode.

[https://docs.microsoft.com/dynamics365/customer-engagement/developer/clientapi/reference/events/attribute-onchange](https://docs.microsoft.com/dynamics365/customer-engagement/developer/clientapi/reference/events/attribute-onchange)
