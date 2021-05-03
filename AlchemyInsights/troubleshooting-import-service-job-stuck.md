---
title: Fejlfinding i forbindelse med import af tjenestejob er gået i stå
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 04/27/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "7907"
- "9003046"
ms.openlocfilehash: 987383037f843d347477c0becc859c663736a676
ms.sourcegitcommit: c977687a7dd03288a9ba396cf2a48ea384d72634
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 04/27/2021
ms.locfileid: "52124917"
---
# <a name="troubleshooting-import-service-job-stuck"></a>Fejlfinding i forbindelse med import af tjenestejob er gået i stå

Hvis du oplever problemer med at importere tjenestejob, der går i stå eller mislykkes, kan du undersøge og prøve følgende:

- Gennemse størrelsen på PST-filen. Den maksimale anbefalede størrelse på en PST-fil til import er 20 GB.

- Hvis du har mistanke om ignorerede elementer på grund af beskadigelse, skal Scanpst.exe for at diagnosticere og rette fejl i PST-filer.

- Hvis du får vist fejlen "MapiExceptionShutoffQuotaExceed" under importen, skal du sikre dig, at målpostkassen har tilstrækkelig kapacitet til at importere de ønskede PST-filer.

Du kan finde flere oplysninger om fejlfinding af problemer med PST-importjob [i Fejlfinding af problemer med PST-importjob.](https://docs.microsoft.com/office365/troubleshoot/pst-import-service/issues-with-pst-import-job)

Hvis du vil have mere at vide om, hvordan du løser problemer, når du importerer PST'er til Outlook, skal du se Løs problemer med at importere en [Outlook .pst-fil (microsoft.com).](https://support.microsoft.com/topic/fix-problems-importing-an-outlook-pst-file-2d2e50dc-5c36-4ab2-ab50-f1be733b3d6e?ui=en-us&rs=en-us&ad=us)