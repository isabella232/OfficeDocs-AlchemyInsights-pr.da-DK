---
title: Tip til DLP-politik fungerer ikke
ms.author: deniseb
author: denisebmsft
manager: laurawims
ms.date: 11/7/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: c03d30be-474a-4a34-b3c0-240eb2a2c466
ms.custom:
- "1428"
- "3200001"
ms.openlocfilehash: 51b4472fa721443192eb542cac45965df67634df
ms.sourcegitcommit: b0d5b68366028abcf08610672d5bc9d3b25ac433
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 03/24/2020
ms.locfileid: "42932580"
---
# <a name="dlp-policy-tip-issues"></a>Problemer med DLP-politiktip

**Vigtigt**: Mange SharePoint Online- og OneDrive-kunder kører forretningskritiske programmer mod den tjeneste, der kører i baggrunden. Disse omfatter indholdsmigrering, Forebyggelse af datatab (DLP) og sikkerhedskopieringsløsninger. I disse hidtil usete tider tager vi skridt til at sikre, at SharePoint Online- og OneDrive-tjenester forbliver meget tilgængelige og pålidelige for dine brugere, der er afhængige af tjenesten mere end nogensinde før i scenarier for fjernarbejde.

Til støtte for dette mål har vi implementeret strammere begrænsningsgrænser for baggrundsapps (migrering, DLP og backupløsninger) i dagtimerne på hverdage. Du bør forvente, at disse apps vil opnå meget begrænset gennemløb i disse tider. I løbet af aftenen og i weekenden for regionen vil tjenesten dog være klar til at behandle en betydeligt større mængde anmodninger fra baggrundsapps.

**Tip til DLP-politik**

Når brugerne bruger **DLP-politikker**, kan de få besked om en politikovertrædelse med **politiktip**. Administratorer kan konfigurere politiktip, der skal vises, mens de tester deres DLP-politik, eller når politikken er i fuld håndhævelsestilstand.
  
Hvis du vil konfigurere politiktip om din DLP-politik i Center for Sikkerhed og Overholdelse i fuld håndhævelsestilstand, skal du gøre følgende:
  
- Sørg for, at politiktip er **aktiveret** på DLP-reglen ved hjælp af trinnene [her](https://docs.microsoft.com/office365/securitycompliance/use-notifications-and-policy-tips).

- Sørg **for,** at dit indhold svarer til det, **der kræves** for at udløse den regel, der er beskrevet i denne artikel [her](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for).

- Politiktip vises i både OWA og Outlook. Men når du bruger **Outlook 2013 eller nyere**, vises politiktip kun under visse betingelser. Disse betingelser er angivet her: [Understøttede betingelser for Outlook 2013 eller nyere til visning af politiktip](https://docs.microsoft.com/office365/securitycompliance/use-notifications-and-policy-tips#outlook-2013-and-later-supports-showing-policy-tips-for-only-some-conditions)

Yderligere oplysninger om Tip til DLP-politik finder du i: [Vis politiktip til DLP-politikker](https://docs.microsoft.com/office365/securitycompliance/use-notifications-and-policy-tips)
  