---
title: Identificer IP-adresse og klient i overvågningslogge
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
- "1367"
- "3100005"
ms.assetid: ''
ms.openlocfilehash: 295418f3c433df2ba1004f4bec4377c68e6bb155
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 09/14/2020
ms.locfileid: "47668304"
---
# <a name="identify-ip-address-and-client-in-audit-logs"></a>Identificer IP-adresse og klient i overvågningslogge

Den IP-adresse, der er knyttet til en aktivitet af en Microsoft 365-bruger eller-administrator, vises i overvågningsloggene. Klientoplysningerne logføres også. Her er de trin, du skal følge for at identificere sådanne oplysninger

1. Log på [Microsoft 365 Security & Compliance Center](https://protection.office.com/).

2. Gå til søgesiden **Søg i**  >  **overvågningslogfil** .

   Hvis du er interesseret i en bestemt aktivitet, skal du vælge den på listen **aktiviteter** . Hvis ikke, returneres alle aktiviteter for den valgte bruger (standardindstilling).

   **Bemærk**: visse aktiviteter er muligvis ikke tilgængelige i menuen **aktiviteter** . de revisions elementer returneres dog, hvis **Vis resultater for alle aktiviteter** er markeret (standardindstillingen).

3. Angiv brugernavnet i feltet **brugere** , Vælg det relevante datointerval for aktiviteten, og klik derefter på **Søg**.

I resultaterne kan du se IP-adressen for den pågældende aktivitet i ruden resultater. Markér revisions posten for at få vist detaljerede oplysninger **i pop op-vinduet (** f. eks. klient, bruger, der har udført handlingen osv.).

Du kan finde flere oplysninger i [finde IP-adressen på den computer, der bruges til at få adgang til en kompromitteret konto](https://docs.microsoft.com/microsoft-365/compliance/auditing-troubleshooting-scenarios#find-the-ip-address-of-the-computer-used-to-access-a-compromised-account).
