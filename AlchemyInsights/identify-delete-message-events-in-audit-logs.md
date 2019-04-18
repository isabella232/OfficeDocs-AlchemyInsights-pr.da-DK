---
title: Identificere Slet meddelelse hændelser i overvågningslogge
ms.author: chrisda
author: chrisda
manager: serdars
ms.date: ''
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom: 1370
ms.assetid: ''
ms.openlocfilehash: 93f8a192af6e689e2b2d04013f35b8da2b69e607
ms.sourcegitcommit: ffe2f489b1ac3aae62aa784c959da6a41c3261eb
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 04/17/2019
ms.locfileid: "31909141"
---
# <a name="audit-logs-for-deleted-email-messages"></a>Overvågningslogge for slettede e-mails

Starter i januar 2019, Microsoft er at aktivere postkassen Overvåg logføring som standard. Ellers for at få vist Slet meddelelse hændelser for en bestemt bruger, skal du aktivere manuelt slettehandlingerne for overvågning. Hvis overvågning af postkasse logføring er allerede aktiveret for organisationen, eller for en bestemt bruger, skal du følge nedenstående trin.

1. Log på [Office 365 & overholdelse Sikkerhedscenter](https://protection.office.com/)

2. Klik på **Søg og undersøgelse** , og vælg **Revision Log søgning**.

3. Vælg datointervallet i felterne **startdato** og **slutdato** . Angiv brugernavnet for den bruger, du vil undersøge (den bruger, der har slettet elementerne). I feltet **aktiviteter** , skal du vælge **slettede meddelelser fra mappen Slettet post** og **Moved meddelelser til mappen Slettet post**.

4. Klik på **Søg**.

Vælg en revisionspost i resultaterne. Oplysninger om mærke, klik på **Flere oplysninger**. Yderligere oplysninger om elementet slettet (for eksempel, emnelinjen og placeringen af varen, da den blev slettet) vises i feltet **AffectedItems** . Egenskaben **ClientInfoString** vises, hvis sletningen opstod i Outlook, Outlook på internettet (tidligere kendt som Outlook Web App), eller en anden enhed.

Yderligere oplysninger finder du [fastlægge, der har konfigureret e-mail videresendes til en postkasse](https://docs.microsoft.com/office365/securitycompliance/auditing-troubleshooting-scenarios#determining-if-a-user-deleted-email-items).

**Bemærk**: Du kan ikke hente slettede emner ved hjælp af funktionen overvågning log. Hvis du vil hente slettede meddelelser i Outlook på internettet, se [gendanne slettede elementer i Outlook Web App](https://support.office.com/article/C3D8FC15-EEEF-4F1C-81DF-E27964B7EDD4).
