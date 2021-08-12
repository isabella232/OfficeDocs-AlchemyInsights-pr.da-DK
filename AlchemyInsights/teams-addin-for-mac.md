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
ms.openlocfilehash: c9c4eb811c93f6d11ebf606ba4bd20cddc2901d6616700ebfe6ef597dd8dc006
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 08/05/2021
ms.locfileid: "53940669"
---
# <a name="teams-add-in-for-mac"></a>Teams-tilføjelsesprogrammet til Mac

Hvis du vil foretage fejlfinding Teams til tilføjelsesprogrammet til Mac-operativsystemets brugere, skal du følge disse trin:

**Trin 1:** Hvis du har en Exchange lokal (2016 CU3 eller nyere påkrævet), skal du bruge værktøjet Test-HMA.ps1 til at bekræfte, at hybrid moderne godkendelse er konfigureret korrekt. Du kan få mere at vide [under Validering af konfiguration af hybrid moderne godkendelse Outlook til iOS og Android.](https://aka.ms/TestHMAEAS)  

**Bemærk!** Brug UPN-adresseformatet (f.eks. [username@contoso.com](mailto:username@contoso.com)), ikke domæne\brugernavn. Gør dette selv for brugere med Exchange Online postkasser.

**Trin 2:** Få brugeren til at gå **til**  >  **Værktøjskonti**... i Outlook til Mac, og find og vælg kontoen. Bekræft, at det angivne brugernavn er i UPN-format (f.eks. [username@contoso.com](mailto:username@contoso.com)).

**Trin 3:** Bekræft, at brugeren er en Microsoft Teams bruger. Brugeren skal bruge abonnementet Office 365 til Mac, produktversion 16.24 eller nyere.