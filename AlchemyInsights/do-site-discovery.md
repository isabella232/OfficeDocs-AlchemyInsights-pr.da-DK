---
title: Do site discovery
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 03/08/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9143"
- "9005291"
ms.openlocfilehash: bdf94220de45d92f63e56501ea4e35389224d25c
ms.sourcegitcommit: 475a9eaa095812091991857df6cf6490a8bbe179
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 03/08/2021
ms.locfileid: "50692937"
---
# <a name="do-site-discovery"></a>Do site discovery

Hvis din organisation stadig bruger ældre webprogrammer og planer om at bruge Internet Explorer-tilstand (hvilket de fleste kunder gør), skal du gøre noget yderligere opdagelse af webstedet.

**Du har allerede installeret en ældre version af Microsoft Edge**

Hvis du allerede har konfigureret din enterprise-webstedsliste til at fungere for den ældre version af Microsoft Edge, er din webstedsregistrering næsten færdig. Den eneste, du muligvis skal gøre, er at tilføje neutrale websteder.

Neutrale websteder er typisk websteder, der leverer enkelt-logon (SSO). Hvis du går til et neutralt websted fra Microsoft Edge, vil du forblive i Microsoft Edge for at godkende. Hvis du går til et neutralt websted i Internet Explorer-tilstand, vil du forblive i Internet Explorer-tilstand for at godkende.

Identificer eventuelle SSO-websteder eller andre neutrale websteder, du bruger, og føj dem til din enterprise-webstedsliste.

**Internet Explorer er din standardbrowser**

Hvis du kun bruger Internet Explorer nu, ved du muligvis ikke, hvilke websteder der har opgraderet til moderne webstandarder, og hvilke der stadig kræver Internet Explorer. Du skal finde og føje disse websteder til listen over virksomhedswebsteder, så du kun kan bruge Internet Explorer-tilstand til disse websteder.

> [!NOTE]
> [Enterprise Site Discovery finder](https://docs.microsoft.com/internet-explorer/ie11-deploy-guide/collect-data-using-enterprise-site-discovery) websteder, der muligvis skal bruge Internet Explorer-tilstand. Det kan indsamle data på computere, der kører Windows Internet Explorer 8 via Internet Explorer 11 på Windows 10, Windows 8.1 eller Windows 7.

**Analysér dataene**

Når du har indsamlet webstedsdata, anbefaler vi følgende proces i fire trin for at analysere dataene:
1. Sortér dataene efter domæne og derefter efter URL-adresse.
2. Definer grænserne for en app, der skal konfigureres i Internet Explorer-tilstand. Du vil medtage alle de websteder og webkontrolelementer, der definerer appen, men du vil ikke inkludere ekstra websteder og kontrolelementer. Nogle websteder kan være så enkle, som *https://contoso.com/app1* mens andre muligvis kræver, at du definerer flere websteder og sider.
3. Test appen for at bekræfte, at den ikke fungerer oprindeligt. Mange websteder tilbyder moderne indhold, når de registrerer en moderne browser og tilbyder kun ældre indhold, når de registrerer Internet Explorer.
4. Føj appen til din enterprise-webstedsliste, hvis det mislykkes at teste.

> [!NOTE]
> Som bedste fremgangsmåde skal du gruppere alle de websteder, der udgør en app. På denne måde er det nemmere, når du opgraderer en app, at fjerne hele webstedet fra Internet Explorer-tilstand og begynde at bruge en moderne browser til den pågældende app.

Når du er færdig med webstedsregistreringen, og du har analyseret dataene, er du klar til at begynde at kigge på din kanalstrategi.

