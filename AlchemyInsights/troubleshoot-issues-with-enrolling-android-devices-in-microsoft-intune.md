---
title: Fejlfinding af problemer med registrering af Android-enheder i Microsoft Intune
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: d0269461-20a8-4c9e-83b2-8fcf608dc0a5
ms.custom:
- "787"
- "6200002"
ms.openlocfilehash: 0ae926e6b31493e7359981c621fd27e8f53d49a17bdf107173b087fe6cc688fa
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 08/05/2021
ms.locfileid: "54008072"
---
# <a name="troubleshoot-issues-with-enrolling-android-devices-in-microsoft-intune"></a>Fejlfinding af problemer med registrering af Android-enheder i Microsoft Intune

Gennemse ressourcerne nedenfor for at løse problemet nu.
  
Nogle almindelige problemer og løsningstrin:
  
 **Fejl i forbindelse med enheden ikke krypteret Firmaportal:** Nyere versioner af Android, især fra og med v7.0, kræver en start-adgangskode for at sikre, at enheden er fuldt krypteret. Almindelige løsninger er at aktivere en startpinkode eller kryptere enheden fuldt ud. Gennemgå [dette dokument for at](https://docs.microsoft.com/intune-user-help/your-device-appears-encrypted-but-cp-says-otherwise-android) få flere oplysninger.
  
 **Enheder kan ikke tjekke ind med Intune-tjenesten eller vises som "Usunde" i Intune-administrationskonsollen:** Nogle Samsung 4.4- og 5.5-enheder kan ikke tjekke ind i tjenesten. Der er tre mulige løsninger på dette problem:
  
1. Åbn appen manuelt Intune-firmaportal, som automatisk starter en enhedssynkronisering.

2. Opdater enheden til Android 6.0 eller nyere.

3. Deaktiver Samsung Smart Manager fra at administrere Intune-firmaportal. Gennemgå [dette dokument](https://docs.microsoft.com/troubleshoot/mem/intune/troubleshoot-device-enrollment-in-intune#devices-fail-to-check-in-with-the-intune-service-and-display-as-unhealthy-in-the-intune-admin-console) for at få flere oplysninger om disse problemer og løsninger.

 **Fejlen Brugerlicenstype** Ugyldig **eller Brugernavn genkendes ikke:** Brugeren skal have tildelt en Intune- eller EMS-licens. Gennemse disse dokumenter for at tildele en licens via: Office Administration eller Azure-portal.
  
Yderligere ressourcer, der kan hjælpe med at løse problemet:
  
1. Brug [Intune-fejlfindingsportalen](https://devicemanagement.microsoft.com/#blade/Microsoft_Intune_DeviceSettings/TroubleshootBlade) til at diagnosticere og løse almindelige registreringsfejl. Gennemgå [dette dokument for](https://docs.microsoft.com/intune/help-desk-operators) at få flere oplysninger.

2. Gennemgå [dette dokument](https://docs.microsoft.com/troubleshoot/mem/intune/troubleshoot-device-enrollment-in-intune) for at få en liste over almindelige fejl, der forhindrer registrering og løsninger på hver enkelt.

3. [Få mere at vide om, hvordan du tilmelder Android-enheder Microsoft Intune](https://docs.microsoft.com/intune/android-enroll).
