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
ms.openlocfilehash: 4653fdef7e9226f05809d56e9a445cd1da35b0578c088bea72252a281d4527d2
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: HT
ms.contentlocale: da-DK
ms.lasthandoff: 08/05/2021
ms.locfileid: "54030752"
---
# <a name="do-site-discovery"></a>Do site discovery

Hvis din organisation stadig bruger ældre webprogrammer og planer til at bruge Internet Explorer-tilstand (hvilket de fleste kunder gør), skal du udføre en vis yderligere opdagelse af webstedet.

**Du har allerede installeret en ældre version af Microsoft Edge**

Hvis du allerede har konfigureret din Enterprise-webstedsliste til at fungere i den ældre version af Microsoft Edge, er din webstedsregistrering næsten færdig. Den eneste, du måske skal gøre, er at tilføje neutrale websteder.

Neutrale websteder er typisk websteder, der leverer enkelt logon (SSO). Hvis du går til et neutralt websted Microsoft Edge, så vil du forblive i Microsoft Edge for at godkende. Hvis du går til et neutralt websted i Internet Explorer-tilstand, vil du forblive i Internet Explorer-tilstand for at godkende.

Identificer eventuelle SSO-websteder eller andre neutrale websteder, som du bruger, og føj dem til din Enterprise-webstedsliste.

**Internet Explorer er din standardbrowser**

Hvis du kun bruger Internet Explorer nu, ved du muligvis ikke, hvilke websteder der har opgraderet til moderne webstandarder, og hvilke der stadig kræver Internet Explorer. Du skal finde og føje disse websteder til virksomhedswebstedslisten, så du kun kan bruge Internet Explorer-tilstand til disse websteder.

> [!NOTE]
> [Enterprise Site Discovery finder](https://docs.microsoft.com/internet-explorer/ie11-deploy-guide/collect-data-using-enterprise-site-discovery) websteder, der muligvis skal bruge Internet Explorer-tilstand. Det kan indsamle data på computere, der Windows Internet Explorer 8 via Internet Explorer 11 på Windows 10, Windows 8.1 eller Windows 7.

**Analysér dataene**

Når du har indsamlet webstedsdata, anbefaler vi følgende firetrinsproces for at analysere dataene:
1. Sortér dataene efter domæne og derefter efter URL-adresse.
2. Definer grænsen for en app, der skal konfigureres i Internet Explorer-tilstand. Du vil medtage alle de websteder og webkontrolelementer, der definerer appen, men du ønsker ikke at medtage ekstra websteder og kontrolelementer. Nogle websteder kan være så enkle, som *https://contoso.com/app1* mens andre kan kræve, at du definerer flere websteder og sider.
3. Test appen for at bekræfte, at den ikke fungerer indbygget. Mange websteder tilbyder moderne indhold, når de registrerer en moderne browser og tilbyder kun ældre indhold, når de registrerer Internet Explorer.
4. Føj appen til din Enterprise-webstedsliste, hvis der ikke kan udføres test.

> [!NOTE]
> Som bedste fremgangsmåde skal du gruppere alle de websteder, der udgør en app. Når du opgraderer en app, er det på denne måde nemmere at fjerne hele webstedet fra Internet Explorer-tilstand og begynde at bruge en moderne browser til den pågældende app.

Når du er færdig med at finde websteder, og du har analyseret dataene, er du klar til at begynde at kigge på din kanalstrategi.

