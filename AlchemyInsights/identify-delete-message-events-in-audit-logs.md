---
title: Identificer slette meddelelseshændelser i overvågningslogfiler
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
ms.openlocfilehash: 641c0216491186aeb423a13854c6b39ee005e5df
ms.sourcegitcommit: bc7d6f4f3c9f7060d073f5130e1ec856e248d020
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 06/02/2020
ms.locfileid: "44508982"
---
# <a name="audit-logs-for-deleted-email-messages"></a>Overvåge logfiler for slettede mails

Fra januar 2019 slår Microsoft som standard loggerføring af postkasseovervågning til. Hvis du vil gennemse slette meddelelseshændelser for en bestemt bruger, skal du manuelt aktivere slettehandlingerne til overvågning. Hvis logføring af postkasseovervågning allerede er aktiveret for din organisation eller for den specifikke bruger, skal du følge nedenstående trin.

1. Log på [Microsoft 365 Security & Compliance Center](https://protection.office.com/)

2. Klik på **Søg og undersøg,** og vælg **Søg i overvågningsloggen**.

3. Vælg datointervallet i felterne **Startdato** og **Slutdato.** Angiv brugernavn til den bruger, du vil undersøge (den bruger, der har slettet elementerne). I feltet **Aktiviteter** skal du vælge **Slettede meddelelser fra mappen Slettet post** og **Flyttede meddelelser til mappen Slettet post**.

4. Klik på **Søg**.

Vælg en overvågningspost i resultaterne. Klik på **Flere oplysninger**i pop op-vinduet med oplysninger . Yderligere oplysninger om det slettede element (f.eks. emnelinjen og placeringen af elementet, da det blev slettet) vises i feltet **AffectedItems.** Egenskaben **ClientInfoString** viser, om sletningen fandt sted i Outlook, Outlook på internettet (tidligere kaldet Outlook Web App) eller en anden enhed.

Du kan finde flere oplysninger [under Bestemme, hvem der konfigurerer videresendelse af mail til en postkasse](https://docs.microsoft.com/microsoft-365/compliance/auditing-troubleshooting-scenarios#determine-if-a-user-deleted-email-items).

**Bemærk:** Du kan ikke hente slettede elementer ved hjælp af overvågningslogfunktionen. Hvis du vil hente slettede meddelelser i Outlook på internettet, skal du se [Gendanne slettede elementer i Outlook Web App](https://support.office.com/article/C3D8FC15-EEEF-4F1C-81DF-E27964B7EDD4).
