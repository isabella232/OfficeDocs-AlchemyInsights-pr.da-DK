---
title: Teams-tilføjelsesprogram til Mac
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 08/10/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "6173"
- "9003233"
ms.openlocfilehash: 74bd424f71a59b80a91b960b815363668bee7036
ms.sourcegitcommit: 1361b2b37fd0201502a1a3547084961de284a3fc
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 08/11/2020
ms.locfileid: "46629463"
---
# <a name="teams-add-in-for-mac"></a>Teams-tilføjelsesprogram til Mac

Hvis du vil foretage fejlfinding af et manglende teams-tilføjelsesprogram til Mac-operativsystem, skal du følge disse trin:

**Trin 1:** Hvis du har hybrid Exchange i det lokale miljø (2016 CU3 eller senere påkrævet), skal du bruge Test-HMA.ps1s værktøjet til at bekræfte, at hybrid moderne godkendelse er konfigureret korrekt. Hvis du vil have mere at vide, skal du se [validere hybrid installation af moderne godkendelse til Outlook til iOS og Android](https://aka.ms/AA980zq).  

**Bemærk!** Brug UPN-adresseformatet (f. eks. [username@contoso.com](mailto:username@contoso.com)), ikke DOMAIN\USERNAME. Gør dette selv for brugere med Exchange Online-postkasser.

**Trin 2:** Få brugeren til at gå til **værktøjer**-  >  **konti**... i Outlook til Mac og finde og vælge kontoen. Bekræft, at det Brugernavn, der er angivet, er i UPN-formatet (f. eks. [username@contoso.com](mailto:username@contoso.com)).

**Trin 3:** Bekræft, at brugeren er licenseret af Microsoft teams-brugere. Brugeren skal bruge Office 365 til Mac-abonnement, produktversion 16,24 eller nyere.