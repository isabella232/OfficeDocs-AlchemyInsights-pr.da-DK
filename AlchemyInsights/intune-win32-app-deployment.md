---
title: Installation af Win32-app til Win32
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/28/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "6446"
- "6700004"
ms.openlocfilehash: 5ccbf37bd3f06da2f8c3955d87e449ea58caab1c
ms.sourcegitcommit: 9fd002ce49ad9a7e58c3eb997a8063e2e1feab55
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 10/06/2020
ms.locfileid: "48461759"
---
# <a name="intune-win32-app-deployment"></a>Installation af Win32-app til Win32

Microsoft Intune tillader Win32-programmer, herunder, men ikke begrænset til MSI og. EXE skal installeres på Windows 10-enheder. Den anvendte installationsmekanisme kræver, at Intune Management Extension er tilgængelig på destinationsenheden. IME installeres automatisk som et resultat af målretning af et PowerShell-script eller en Win32-Programinstallation til en bruger/enhed.

Der er også en række forudsætninger, der skal opfyldes, for at du kan installere Win32-apps, der omfatter:

- Understøttede platforme: Windows 10 version 1607 eller nyere (Enterprise, Pro og Education versions).
- Understøttet arkitektur: x86 og x64.
- Enhedshåndtering: AAD-tilmeldt og automatisk tilmeldt (herunder hybridt domæne, der er joinforbundet og Gruppepolitik automatisk tilmeldt).
- Programpakke format:. **intunewin**  -fil, der er udarbejdet af [Microsoft Win32-indholds forberedelsesværktøjet](https://docs.microsoft.com/mem/intune/apps/apps-win32-prepare).
- Begrænsede
    - Maksimal størrelse: 8 GB.
    - Ikke-understøttet arkitektur: arme.

Gennemse dokumentet "[Tilføj, Tildel og Overvåg en Win32-app i Microsoft Intune](https://docs.microsoft.com/mem/intune/apps/apps-win32-add)" for oplysninger, der er relateret til disse trin.

Oplysninger om fejlfinding i forbindelse med installation af programmer på Windows, herunder Win32-apps, kan gennemses i følgende dokumenter

- [Fejlfinding af problemer med App-installation](https://docs.microsoft.com/mem/intune/apps/troubleshoot-app-install)  
- [Fejlfinding af Win32-apps](https://docs.microsoft.com/mem/intune/apps/apps-win32-troubleshoot)