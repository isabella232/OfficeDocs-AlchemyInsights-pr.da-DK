---
title: Identificer IP-adresse og klient i overvågningslogfiler
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
ms.openlocfilehash: 57a1756787f8297a2a1ab3012b95aaa2f33e6045
ms.sourcegitcommit: ab75f66355116e995b3cb5505465b31989339e28
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 08/13/2021
ms.locfileid: "58313013"
---
# <a name="identify-ip-address-and-client-in-audit-logs"></a>Identificer IP-adresse og klient i overvågningslogfiler

Den IP-adresse, der svarer til en aktivitet Microsoft 365 en bruger eller administrator, vises i overvågningslogfilerne. Klientoplysningerne logføres også. Her er trinnene til at identificere sådanne oplysninger

1. Log på Microsoft 365 [Compliance Center.](https://protection.office.com/)

2. Gå til **søgesiden**  >  **for søgeloggen i overvågningsloggen.**

   Hvis du er interesseret i en bestemt aktivitet, skal du vælge den på **listen** Aktiviteter. Hvis ikke, returneres alle aktiviteter for den valgte bruger (standardindstilling).

   **Bemærk!** Visse aktiviteter er muligvis ikke tilgængelige i **menuen** Aktiviteter. disse overvågningselementer returneres dog, hvis **Vis resultater for alle aktiviteter** er valgt (standardindstilling).

3. Angiv brugernavnet i **feltet Brugere,** vælg det relevante datointerval for aktiviteten, og klik derefter på **Søg**.

I resultaterne kan du se IP-adressen for den pågældende aktivitet i resultatruden. Vælg overvågningsposten for at få vist detaljerede oplysninger i **pop** op-dialogboksen Detaljer (f.eks. Klient, bruger, der udførte handlingen osv.).

Du kan få mere at vide [under Finde IP-adressen på den computer, der bruges til at få adgang til en kompromitteret konto.](https://docs.microsoft.com/microsoft-365/compliance/auditing-troubleshooting-scenarios#find-the-ip-address-of-the-computer-used-to-access-a-compromised-account)
