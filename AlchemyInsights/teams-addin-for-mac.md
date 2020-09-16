---
title: Teams-tilføjelsesprogram til Mac
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
- "9003233"
ms.openlocfilehash: 1e5f6d66386398ad8600f9383f9f7a1dcf0ce69f
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 09/14/2020
ms.locfileid: "47670322"
---
# <a name="teams-add-in-for-mac"></a>Teams-tilføjelsesprogram til Mac

Hvis du vil foretage fejlfinding af et manglende teams-tilføjelsesprogram til Mac-operativsystem, skal du følge disse trin:

**Trin 1:** Hvis du har hybrid Exchange i det lokale miljø (2016 CU3 eller senere påkrævet), skal du bruge Test-HMA.ps1s værktøjet til at bekræfte, at hybrid moderne godkendelse er konfigureret korrekt. Hvis du vil have mere at vide, skal du se [validere hybrid installation af moderne godkendelse til Outlook til iOS og Android](https://aka.ms/AA980zq).  

**Bemærk!** Brug UPN-adresseformatet (f. eks. [username@contoso.com](mailto:username@contoso.com)), ikke DOMAIN\USERNAME. Gør dette selv for brugere med Exchange Online-postkasser.

**Trin 2:** Få brugeren til at gå til **værktøjer**-  >  **konti**... i Outlook til Mac og finde og vælge kontoen. Bekræft, at det Brugernavn, der er angivet, er i UPN-formatet (f. eks. [username@contoso.com](mailto:username@contoso.com)).

**Trin 3:** Bekræft, at brugeren er licenseret af Microsoft teams-brugere. Brugeren skal bruge Office 365 til Mac-abonnement, produktversion 16,24 eller nyere.