---
title: Fejlfinding af problemer med tilmelding af Android-enheder i Microsoft Intune
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: d0269461-20a8-4c9e-83b2-8fcf608dc0a5
ms.custom:
- "787"
- "6200002"
ms.openlocfilehash: bd6d278ebf6cca7fb6e4ac1049deae600b516707
ms.sourcegitcommit: 631cbb5f03e5371f0995e976536d24e9d13746c3
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 04/22/2020
ms.locfileid: "43759614"
---
# <a name="troubleshoot-issues-with-enrolling-android-devices-in-microsoft-intune"></a>Fejlfinding af problemer med tilmelding af Android-enheder i Microsoft Intune

Gennemgå de ressourcer, der er angivet nedenfor, for at løse problemet nu.
  
Nogle almindelige problemer og løsningstrin:
  
 **Enheden er ikke krypteret i firmaportalen:** Nyere versioner af Android, især startende med v7.0, kræver en startadgangskode for at sikre, at din enhed er fuldt krypteret. Almindelige løsninger er at aktivere en startpin eller kryptere enheden helt. Gennemse [dette dokument](https://docs.microsoft.com/intune-user-help/your-device-appears-encrypted-but-cp-says-otherwise-android) for at få flere oplysninger.
  
 **Enheder undlader at tjekke ind med Intune service eller vise som "Usundt" i Intune admin konsol:** Nogle Samsung 4.4- og 5.5-enheder tjekker muligvis ikke ind i tjenesten. Der er 3 mulige løsninger på dette problem:
  
1. Åbn intune-firmaportalappen manuelt, som automatisk starter en enhedssynkronisering.

2. Opdater enheden til Android 6.0 eller nyere.

3. Deaktiver Samsung Smart Manager fra at administrere Intune Company Portal. Læs [dette dokument](https://docs.microsoft.com/intune-classic/troubleshoot/troubleshoot-device-enrollment-in-intune#devices-fail-to-check-in-with-the-intune-service-and-display-as-unhealthy-in-the-intune-admin-console) for at få yderligere oplysninger om disse spørgsmål og løsninger.

 **Brugerlicenstype Ugyldig** eller **Fejl i brugernavnet ikke genkendt:** Brugeren skal tildeles en Intune- eller EMS-licens. Gennemse disse dokumenter for at tildele en licens via: Office Administration eller Azure-portalen.
  
Yderligere ressourcer, der kan hjælpe dig med at løse problemet:
  
1. Brug [Intune Troubleshooting Portal](https://devicemanagement.microsoft.com/#blade/Microsoft_Intune_DeviceSettings/TroubleshootBlade) til at diagnosticere og løse almindelige tilmeldingsfejl. Gennemse [dette dokument](https://docs.microsoft.com/intune/help-desk-operators) for at få flere oplysninger.

2. Gennemse [dette dokument](https://docs.microsoft.com/intune-classic/Troubleshoot/troubleshoot-device-enrollment-in-intune) for at få en liste over almindelige fejl, der forhindrer tilmelding og løsninger til hver enkelt.

3. [Få mere at vide om, hvordan du tilmelder Android-enheder i Microsoft Intune](https://docs.microsoft.com/intune/android-enroll).
