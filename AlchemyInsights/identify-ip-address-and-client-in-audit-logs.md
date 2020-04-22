---
title: Identificere IP-adresse og klient i overvågningslogfiler
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1367"
- "3100005"
ms.assetid: ''
ms.openlocfilehash: d1a0d412fc0c6d79e50b101ca759127522f45dcd
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 04/22/2020
ms.locfileid: "43716382"
---
# <a name="identify-ip-address-and-client-in-audit-logs"></a>Identificere IP-adresse og klient i overvågningslogfiler

Den IP-adresse, der svarer til en aktivitet fra en Microsoft 365-bruger eller -administrator, vises i overvågningsloggene. Klientoplysningerne logføres også. Her er de skridt til at identificere sådanne oplysninger

1. Log på [Microsoft 365 Security & Compliance Center](https://protection.office.com/).

2. Gå til**søgesiden for søgefilen til søgeovervågning** i **søgefilen** > til søgning i søgeområdet.

   Hvis du er interesseret i en bestemt aktivitet, skal du vælge den på listen **Aktiviteter.** Hvis ikke, returneres alle aktiviteter for den valgte bruger (standardindstilling).

   **Bemærk:** Visse aktiviteter er muligvis ikke tilgængelige i menuen **Aktiviteter.** Disse overvågningselementer returneres dog, hvis **Vis resultater for alle aktiviteter** er valgt (standardindstilling).

3. Angiv brugernavnet i feltet **Brugere,** vælg det relevante datointerval for aktiviteten, og klik derefter på **Søg**.

I resultaterne kan du se IP-adressen for den pågældende aktivitet i resultatruden. Vælg overvågningsposten for at få vist detaljerede oplysninger i pop **op-vinduet Detaljer** (f.eks.

Yderligere oplysninger finder [du i Finding the IP-adressen på den computer, der bruges til at få adgang til en kompromitteret konto](https://docs.microsoft.com/office365/securitycompliance/auditing-troubleshooting-scenarios#finding-the-ip-address-of-the-computer-used-to-access-a-compromised-account).
