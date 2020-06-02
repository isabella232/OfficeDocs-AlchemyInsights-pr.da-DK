---
title: Identificer IP-adresse og klient i overvågningslogfiler
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
ms.openlocfilehash: 80b652eb65612093252dee226a19ec74bc035faa
ms.sourcegitcommit: bc7d6f4f3c9f7060d073f5130e1ec856e248d020
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 06/02/2020
ms.locfileid: "44508910"
---
# <a name="identify-ip-address-and-client-in-audit-logs"></a>Identificer IP-adresse og klient i overvågningslogfiler

Den IP-adresse, der svarer til en aktivitet af en Microsoft 365-bruger eller -administrator, vises i overvågningsloggene. Klientoplysningerne logføres også. Her er de skridt til at identificere sådanne oplysninger

1. Log på [Microsoft 365 Security & Compliance Center](https://protection.office.com/).

2. Gå til søgesiden for søgesøgning i søgeloggen søge i søgeloggen **for søgeloggen søge**i søgeloggen for  >  **søgesøgning.**

   Hvis du er interesseret i en bestemt aktivitet, skal du vælge den på listen **Aktiviteter.** Hvis ikke, returneres alle aktiviteter for den valgte bruger (standardindstilling).

   **Bemærk:** Visse aktiviteter er muligvis ikke tilgængelige i menuen **Aktiviteter.** Disse overvågningselementer returneres dog, hvis **Vis resultater for alle aktiviteter** er valgt (standardindstilling).

3. Angiv brugernavnet i feltet **Brugere,** vælg det relevante datointerval for aktiviteten, og klik derefter på **Søg**.

I resultaterne kan du se IP-adressen for den pågældende aktivitet i resultatruden. Vælg overvågningsposten for at få vist detaljerede oplysninger i pop op-vinduet **Detaljer** (f.eks. klient, bruger, der udførte handlingen osv.).

Du kan finde flere oplysninger [under Finde IP-adressen på den computer, der bruges til at få adgang til en kompromitteret konto](https://docs.microsoft.com/microsoft-365/compliance/auditing-troubleshooting-scenarios#find-the-ip-address-of-the-computer-used-to-access-a-compromised-account).
