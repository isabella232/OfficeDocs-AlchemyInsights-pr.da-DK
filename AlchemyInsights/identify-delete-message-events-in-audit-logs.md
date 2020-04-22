---
title: Identificer slettemeddelelseshændelser i overvågningslogfiler
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1370"
- "3100005"
ms.assetid: ''
ms.openlocfilehash: 797a4b1146862faf91d2b9e8d74feade90f71650
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 04/22/2020
ms.locfileid: "43716490"
---
# <a name="audit-logs-for-deleted-email-messages"></a>Overvåge logfiler for slettede mails

Fra og med januar 2019 slår Microsoft som standard til for logføring af postkasseovervågning. Ellers skal du manuelt aktivere slettehandlingerne til overvågning for at gennemse slette meddelelseshændelser for en bestemt bruger. Hvis logføring af postkasseovervågning allerede er aktiveret for din organisation eller for den specifikke bruger, skal du følge nedenstående trin.

1. Log på [Microsoft 365 Security & Compliance Center](https://protection.office.com/)

2. Klik **på Søg og undersøgelse,** og vælg **Overvågningslogsøgning**.

3. Vælg datointervallet i felterne **Startdato** **og Slutdato.** Angiv brugernavn et brugernavn for den bruger, du vil undersøge (den bruger, der har slettet elementerne). Vælg **Slettede meddelelser fra mappen Slettet post i feltet** **Aktiviteter** og **flyttede meddelelser til mappen Slettet post**.

4. Klik på **Søg**.

Vælg en overvågningspost i resultaterne. Klik på Flere oplysninger i pop **op-vinduet med**detaljer . Yderligere oplysninger om det slettede element (f.eks. emnelinjen og varens placering, da den blev slettet) vises i feltet **AffectedItems.** Egenskaben **ClientInfoString** viser, om sletningen fandt sted i Outlook, Outlook på internettet (tidligere kendt som Outlook Web App) eller en anden enhed.

Du kan finde flere oplysninger [under Bestemme, hvem der konfigurerer videresendelse af mail for en postkasse](https://docs.microsoft.com/office365/securitycompliance/auditing-troubleshooting-scenarios#determining-if-a-user-deleted-email-items).

**Bemærk:** Du kan ikke hente slettede elementer ved hjælp af overvågningslogfunktionen. Hvis du vil hente slettede meddelelser i Outlook på internettet, skal du se [Gendanne slettede elementer i Outlook Web App](https://support.office.com/article/C3D8FC15-EEEF-4F1C-81DF-E27964B7EDD4).
