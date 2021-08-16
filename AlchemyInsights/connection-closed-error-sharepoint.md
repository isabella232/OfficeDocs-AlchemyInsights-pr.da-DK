---
title: Den underliggende forbindelse blev lukket fejl i SharePoint
ms.author: pebaum
author: pebaum
manager: dansimp
ms.date: 04/01/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "10802"
- "9006390"
ms.openlocfilehash: 101c0ba90d2bec6b1684fd63645ba2f8f89783ad5bfdf0efe739d31dfd951f66
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 08/05/2021
ms.locfileid: "54044406"
---
# <a name="the-underlying-connection-was-closed-error-in-sharepoint"></a>Fejlen "Den underliggende forbindelse blev lukket" i SharePoint

Hvis du modtager fejlen "Den underliggende forbindelse blev lukket" i SharePoint kan det være relateret til udrådningen af TLS 1.0/1.1. Du kan finde flere oplysninger i følgende artikler:

- [Forberedelse til TLS 1.2 i Office 365 og Office 365 GCC](/microsoft-365/compliance/prepare-tls-1.2-in-office-365)

- [Godkendelsesfejl opstår, hvis klienten ikke har understøttelse af TLS 1.2](https://review.docs.microsoft.com/sharepoint/troubleshoot/administration/authentication-errors-tls12-support)

- [Opdater for at aktivere TLS 1.1 og TLS 1.2 som standard sikre protokoller i WinHTTP Windows](https://support.microsoft.com/topic/update-to-enable-tls-1-1-and-tls-1-2-as-default-secure-protocols-in-winhttp-in-windows-c4bd73d2-31d7-761e-0178-11268bb10392)

Hvis brugerne er på Windows 7, skal du kontrollere, at de markerer [TLS Cipher Suites i Windows 7.](/windows/win32/secauthn/tls-cipher-suites-in-windows-7)