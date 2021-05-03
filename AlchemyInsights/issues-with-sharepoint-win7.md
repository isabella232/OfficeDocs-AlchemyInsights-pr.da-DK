---
title: Problemer med SharePoint på Windows 7 computere
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9006484"
- "11070"
ms.openlocfilehash: 787f0e713cc95b590bc494868d5098a25131ac56
ms.sourcegitcommit: d33ab8c73d8af51da782094fb8f8abf7626f4df3
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 04/28/2021
ms.locfileid: "52124923"
---
# <a name="issues-with-sharepoint-on-windows-7-machines"></a>Problemer med SharePoint på Windows 7 computere

Hvis du modtager fejl på Windows 7-computere, mens du arbejder på SharePoint eller OneDrive, kan de være relateret til udrådningen af TLS 1.0/1.1. Du kan finde flere oplysninger under:

- [Forberedelse til TLS 1.2 i Office 365 og Office 365 GCC](https://docs.microsoft.com/microsoft-365/compliance/prepare-tls-1.2-in-office-365)

- Windows 7 SP1/Windows 8 skal have TLS1.2 aktiveret. Få mere at vide under [Godkendelsesfejl opstår, når klienten ikke har understøttelse af TLS 1.2](https://review.docs.microsoft.com/sharepoint/troubleshoot/administration/authentication-errors-tls12-support)

- Installér KB3140245, og opret registreringsdatabaseværdien. Få mere at vide under Opdater for at aktivere [TLS 1.1 og TLS 1.2](https://support.microsoft.com/topic/update-to-enable-tls-1-1-and-tls-1-2-as-default-secure-protocols-in-winhttp-in-windows-c4bd73d2-31d7-761e-0178-11268bb10392) som standard sikre protokoller i WinHTTP Windows

- Windows 7 SP1/Windows 8-klienter skal sikre, at de nyeste TLS-krypteringspakker er installeret. Du kan finde flere oplysninger [under Microsoft-sikkerhedsmeddelelse 3042058.](https://docs.microsoft.com/security-updates/SecurityAdvisories/2015/3042058) 


