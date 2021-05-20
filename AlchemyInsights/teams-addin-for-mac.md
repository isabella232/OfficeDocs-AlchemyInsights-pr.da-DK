---
title: Teams-tilføjelsesprogrammet til Mac
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 08/10/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "6173"
- "6166"
- "9003233"
- "9002573"
ms.openlocfilehash: 45df4381688335f10f6699d8b5ff1aaafd6f7257
ms.sourcegitcommit: 730efbac8eec016b2b4f83f1b0e01e077f28c444
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 05/20/2021
ms.locfileid: "52582064"
---
# <a name="teams-add-in-for-mac"></a>Teams-tilføjelsesprogrammet til Mac

Hvis du vil foretage fejlfinding Teams til tilføjelsesprogrammet til Mac-operativsystemets brugere, skal du følge disse trin:

**Trin 1:** Hvis du har en Exchange lokal (2016 CU3 eller nyere påkrævet), skal du bruge værktøjet Test-HMA.ps1 til at bekræfte, at hybrid moderne godkendelse er konfigureret korrekt. Du kan få mere at vide [under Validering af konfiguration af hybrid moderne godkendelse Outlook til iOS og Android.](https://aka.ms/TestHMAEAS)  

**Bemærk!** Brug UPN-adresseformatet (f.eks. [username@contoso.com](mailto:username@contoso.com)), ikke domæne\brugernavn. Gør dette selv for brugere med Exchange Online postkasser.

**Trin 2:** Få brugeren til at gå **til**  >  **Værktøjskonti**... i Outlook til Mac, og find og vælg kontoen. Bekræft, at det angivne brugernavn er i UPN-format (f.eks. [username@contoso.com](mailto:username@contoso.com)).

**Trin 3:** Bekræft, at brugeren er en Microsoft Teams bruger. Brugeren skal bruge abonnementet Office 365 til Mac, produktversion 16.24 eller nyere.