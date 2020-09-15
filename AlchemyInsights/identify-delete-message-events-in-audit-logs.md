---
title: Identificer hændelser for sletning af meddelelser i overvågningslogge
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
ms.openlocfilehash: bc78076706aee15a3133c4b1a89064591f790b58
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 09/14/2020
ms.locfileid: "47696507"
---
# <a name="audit-logs-for-deleted-email-messages"></a>Overvågningslogge for slettede mails

Fra og med januar 2019 er Microsoft ved at aktivere logføring af postkasse overvågning som standard. Ellers skal du aktivere slette handlingerne til overvågning manuelt for at gennemse hændelser for sletning af meddelelser for en bestemt bruger. Hvis logføring af postkasse overvågning allerede er aktiveret for din organisation eller for den specifikke bruger, skal du følge trinnene nedenfor.

1. Logge på [Microsoft 365 Security & Compliance Center](https://protection.office.com/)

2. Klik på **Søg og foretag undersøgelsen** , og vælg **Søg i overvågningsloggen**.

3. Vælg datointervallet i felterne **Start dato** og **Slutdato** . Angiv Brugernavn til den bruger, du vil undersøge (den bruger, der har slettet elementerne). I feltet **aktiviteter** skal du vælge **slettede meddelelser fra mappen Slettet post** og **flyttede meddelelser til mappen Slettet post**.

4. Klik på **Søg**.

I resultaterne skal du vælge en revisionspost. Klik på **flere oplysninger**i pop op-vinduet detaljer. Du kan få vist flere oplysninger om det slettede element (f. eks, emnelinjen og placeringen af elementet, når det er blevet slettet) i feltet **AffectedItems** . Egenskaben **ClientInfoString** vises, hvis der opstod en sletning i Outlook, Outlook på internettet (tidligere kendt som Outlook Web App) eller en anden enhed.

Hvis du vil have mere at vide, skal du se [bestemme, hvem der skal konfigurere videresendelse af mail for en postkasse](https://docs.microsoft.com/microsoft-365/compliance/auditing-troubleshooting-scenarios#determine-if-a-user-deleted-email-items)

**Bemærk**! du kan ikke hente slettede elementer ved hjælp af funktionen Overvåg log. Hvis du vil hente slettede meddelelser i Outlook på internettet, skal du se [Gendan slettede elementer i Outlook Web App](https://support.office.com/article/C3D8FC15-EEEF-4F1C-81DF-E27964B7EDD4).
