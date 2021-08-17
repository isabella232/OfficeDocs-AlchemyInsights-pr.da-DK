---
title: 401 Uautoriseret fejl i SharePoint
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 04/14/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "10935"
- "9001435"
ms.openlocfilehash: 8935f461aaf24cb100516311203ef642f5dbed931e472df944c1cd7e72a8cf4e
ms.sourcegitcommit: 920051182781bd97ce4d4d6fbd268cb37b84d239
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 08/11/2021
ms.locfileid: "57890260"
---
# <a name="401-unauthorized-error-in-sharepoint"></a>401 Uautoriseret fejl i SharePoint

Hvis du modtager fejlen "(401) Uautoriseret" i SharePoint kan det være relateret til udrådningen af TLS 1.0/1.1. For at få mere at vide, kan du se:

- [Forberedelse til TLS 1.2 i Office 365 og Office 365 GCC](https://docs.microsoft.com/microsoft-365/compliance/prepare-tls-1.2-in-office-365)

- [Godkendelsesfejl opstår, hvis klienten ikke har understøttelse af TLS 1.2](https://docs.microsoft.com/sharepoint/troubleshoot/administration/authentication-errors-tls12-support)

- [Opdater for at aktivere TLS 1.1 og TLS 1.2 som standard sikre protokoller i WinHTTP Windows](https://support.microsoft.com/topic/update-to-enable-tls-1-1-and-tls-1-2-as-default-secure-protocols-in-winhttp-in-windows-c4bd73d2-31d7-761e-0178-11268bb10392)

Hvis brugerne er på Windows 7, skal du kontrollere, at de markerer [TLS Cipher Suites i Windows 7.](https://docs.microsoft.com/windows/win32/secauthn/tls-cipher-suites-in-windows-7)