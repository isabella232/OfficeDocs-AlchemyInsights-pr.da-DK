---
title: Identificere IP-adresse og klienten i overvågningslogge
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: ''
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom: 1367
ms.assetid: ''
ms.openlocfilehash: 87e0d414fe02d5074a56cd5a77d50db1464b7faf
ms.sourcegitcommit: 4b7e478ce700c0b781efec3857ac4dce5bdf00c6
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 06/07/2019
ms.locfileid: "34752054"
---
# <a name="identify-ip-address-and-client-in-audit-logs"></a>Identificere IP-adresse og klienten i overvågningslogge

Den IP-adresse, der svarer til en aktivitet af en bruger eller administrator fremgår af overvågningslogge. Oplysningerne om klienten registreres også. Her er skridt til at identificere sådanne oplysninger

1. Log på [Office 365 & overholdelse Sikkerhedscenter](https://protection.office.com/)

2. Klik på **Søg og undersøgelse** , og vælg **Revision Log søgning**.

   Hvis du er interesseret i en bestemt aktivitet, kan du vælge den på listen **aktiviteter** . Hvis ikke, returneres alle aktiviteter for den valgte bruger (standardindstilling).

   **Bemærk**: visse aktiviteter er muligvis ikke tilgængelig i menuen **aktiviteter** . dog de overvåge varer returneres, hvis **Vis resultater for alle aktiviteter, der** er markeret (standardindstilling).

3. Angiv brugernavnet i feltet **brugere** , vælge det relevante datointerval for aktiviteten, og klik derefter på **Søg**.

I resultaterne, kan du se IP-adressen for den pågældende aktivitet i resultatruden. Vælg revisionspost for at se detaljerede oplysninger i **Detaljer** -mærke (for eksempel klienten, bruger, der foretog handlingen osv.).

Yderligere oplysninger finder du under [finde IP-adressen på den computer, der bruges til at få adgang til en kompromitteret konto](https://docs.microsoft.com/office365/securitycompliance/auditing-troubleshooting-scenarios#finding-the-ip-address-of-the-computer-used-to-access-a-compromised-account).
