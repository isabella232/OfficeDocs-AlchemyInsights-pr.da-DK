---
title: Identificer slette meddelelseshændelser i overvågningslogfiler
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
- "1370"
- "3100005"
ms.assetid: ''
ms.openlocfilehash: f5d6041fd80b4d5cae610e7d9248e45ed410a3d9
ms.sourcegitcommit: ab75f66355116e995b3cb5505465b31989339e28
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 08/13/2021
ms.locfileid: "58317588"
---
# <a name="audit-logs-for-deleted-email-messages"></a>Overvågningslogfiler for slettede mails

Fra og med januar 2019 slår Microsoft som standard logføring af postkassekontrol til. Hvis du ikke vil gennemse slette meddelelseshændelser for en bestemt bruger, skal du manuelt aktivere slettehandlingerne til overvågning. Hvis logføring af postkassekontrol allerede er aktiveret for din organisation eller for den bestemte bruger, skal du følge trinnene nedenfor.

1. Log på Microsoft 365 [Compliance Center](https://protection.office.com/)

2. Klik **på Søgning og undersøgelse,** og vælg Søgning i **overvågningslogfil**.

3. Vælg datointervallet i **felterne Startdato** **og** Slutdato. Angiv brugernavnet for den bruger, du vil undersøge (den bruger, der slettede elementerne). I feltet **Aktiviteter** skal du **vælge Slettede meddelelser fra mappen Slettet post** og Flyttede meddelelser til mappen Slettet **post.**

4. Klik **på Søg**.

Vælg en overvågningspost i resultaterne. Klik på Flere oplysninger i pop **op-menuen med oplysninger**. Yderligere oplysninger om det slettede element (f.eks. emnelinjen og placeringen af elementet, da det blev slettet) vises i feltet **AffectedItems.** Egenskaben **ClientInfoString** viser, om sletningen skete i Outlook, Outlook på internettet (tidligere kaldet Outlook Web App) eller en anden enhed.

Du kan få mere at vide [under Fastslå, hvem der har konfigureret videresendelse af mail for en postkasse](https://docs.microsoft.com/microsoft-365/compliance/auditing-troubleshooting-scenarios#determine-if-a-user-deleted-email-items).

**Bemærk!** Du kan ikke hente slettede elementer ved hjælp af funktionen overvågningslog. Hvis du vil hente slettede meddelelser Outlook på internettet, skal du [se Gendan slettede elementer Outlook Web App](https://support.office.com/article/C3D8FC15-EEEF-4F1C-81DF-E27964B7EDD4).
