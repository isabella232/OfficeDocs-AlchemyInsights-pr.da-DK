---
title: Fejlfinding af problemer med registrering af Android-enheder i Microsoft Intune
ms.author: pebaum
author: pebaum
manager: mnirkhe
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
ms.openlocfilehash: b5cb2e8a76e8e7d91bd9cd8789ae1623a7f96579
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 09/14/2020
ms.locfileid: "47689948"
---
# <a name="troubleshoot-issues-with-enrolling-android-devices-in-microsoft-intune"></a>Fejlfinding af problemer med registrering af Android-enheder i Microsoft Intune

Gennemse de ressourcer, der er anført nedenfor, for at løse problemet nu.
  
Nogle almindelige problemer og løsnings trin:
  
 **Enheden har ikke en krypteret fejl i firmaportalen:** Nyere versioner af Android, især fra og med v 7.0, kræver en start adgangskode for at sikre, at enheden er fuldt krypteret. Almindelige løsninger er at aktivere en startpinkode eller en fuldt krypteret enhed. Gennemse [dette dokument](https://docs.microsoft.com/intune-user-help/your-device-appears-encrypted-but-cp-says-otherwise-android) for at få flere oplysninger.
  
 Det **lykkedes ikke at tjekke enheder ind med tjenesten Intune eller Vis som "usund" i Intune-administrationskonsollen:** Nogle Samsung 4,4-og 5,5-enheder kan muligvis ikke tjekkes ind i tjenesten. Der er 3 mulige løsninger på dette problem:
  
1. Åbn appen Intune-Firmaportalen manuelt, der starter automatisk en enhedssynkronisering.

2. Opdater enheden til Android 6,0 eller nyere.

3. Deaktiver Samsung Smart Manager fra at administrere Intune-Firmaportalen. Gennemse [dette dokument](https://docs.microsoft.com/intune-classic/troubleshoot/troubleshoot-device-enrollment-in-intune#devices-fail-to-check-in-with-the-intune-service-and-display-as-unhealthy-in-the-intune-admin-console) for at få flere oplysninger om disse problemer og løsninger.

 **Brugerlicens typen er ugyldig** , eller **brugernavnet blev ikke genkendt fejlen:** brugeren skal have tildelt en Intune-eller EMS-licens. Gennemgå disse dokumenter for at tildele en licens via: Office administration eller Azure-portalen.
  
Yderligere ressourcer, der kan hjælpe med at løse dit problem:
  
1. Brug [fejlfindings portalen til Intune](https://devicemanagement.microsoft.com/#blade/Microsoft_Intune_DeviceSettings/TroubleshootBlade) til at diagnosticere og løse almindelige tilmeldings fejl. Gennemse [dokumentet](https://docs.microsoft.com/intune/help-desk-operators) for at få flere oplysninger.

2. Gennemse [dette dokument](https://docs.microsoft.com/intune-classic/Troubleshoot/troubleshoot-device-enrollment-in-intune) for at få en liste over almindelige fejl, der forhindrer registrering og løsninger til hver enkelt.

3. [Få mere at vide om, hvordan du registrerer Android-enheder i Microsoft Intune](https://docs.microsoft.com/intune/android-enroll).
