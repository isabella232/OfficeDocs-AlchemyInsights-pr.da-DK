---
title: Fjern baggrundstjenesten til Microsoft Søg i Bing
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 03/12/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9214"
- "9005302"
ms.openlocfilehash: 6447137fca9b2d48508f4e240a438c7f851c103c
ms.sourcegitcommit: 3fb39a080cc8680d960b8468ac9355389a3e2df4
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 03/12/2021
ms.locfileid: "50816124"
---
# <a name="remove-the-background-service-for-microsoft-search-in-bing"></a>Fjern baggrundstjenesten til Microsoft Søg i Bing

Hvis du vil fjerne baggrundstjenesten til Microsoft Søg i Bing, kan du prøve følgende afhjælpninger:

1. Hvis du vil vende tilbage til de oprindelige søgemaskineindstillinger, skal du gøre følgende:

    a. Slå **Brug Bing som din [](https://docs.microsoft.com/deployoffice/microsoft-search-bing#change-whether-bing-is-the-default-search-engine-for-google-chrome) standardsøgemaskine fra.**

    b. [Gå til Microsoft 365 Administration, og](https://docs.microsoft.com/deployoffice/microsoft-search-bing#configure-the-setting-in-the-microsoft-365-admin-center-to-allow-the-extension-to-be-installed) ryd den indstilling, der påvirker alle brugere i organisationen.

2. Hvis du vil fjerne baggrundstjenesten fra en enkelt enhed, skal du gøre følgende:

    a. Vælg **Kontrolpanel > programmer > programmer og funktioner.**

    b. Højreklik på **Microsoft Søg i Bing** under listen over installerede programmer, og klik derefter på **Fjern.**

3. Hvis du vil fjerne baggrundstjenesten fra flere enheder i organisationen, skal du logge på som administrator og køre følgende kommando i et script: 

`"%ProgramFiles(x86)%\Microsoft\DefaultPackMSI\MainBootStrap.exe" uninstallAll`
