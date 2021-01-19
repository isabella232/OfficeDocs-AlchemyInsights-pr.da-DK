---
title: Domænecontroller
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 01/17/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "7909"
- "9003233"
ms.openlocfilehash: d4cbe80c3e8f0ce32fcbe89e852f24efd6f50575
ms.sourcegitcommit: 6d02eb533fd74199af6b20f714b3720991da2c4a
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 01/18/2021
ms.locfileid: "49900870"
---
# <a name="domain-controller"></a>Domænecontroller

**Det er ikke muligt at aktivere AAD-DS, eller installationen mislykkedes**

Hvis du vil løse problemet med Azure AD-domæne tjenesten (AAD-DS), der ikke er aktiveret eller ikke kan installeres, skal du udføre følgende trin:

1. Hvis du bruger et allerede eksisterende virtuelt netværk, skal du kontrollere din NSG for regler, der blokerer de porte, der kræves for at synkronisere på en AAD-DOMÆNEadministrator i portalen https://aka.ms/aadds-networking .
2. Kontrollér, om din fejlmeddelelse er besvaret i denne fejlfindingsvejledning, der er tilgængelig i  https://aka.ms/aadds-troubleshoot-enable .
3. Prøv at installere Azure AD-domæne tjenester i et nyt virtuelt netværk.
4. Følg vejledningen Introduktion til, hvordan du installerer AAD-DS, som er tilgængelig via et [selvstudium til oprettelse af Azure ad-domæne tjenester](https://docs.microsoft.com/azure/active-directory-domain-services/tutorial-create-instance).
5. Hvis du har problemer med at installere Azure AD-domæne tjenester, skal du se [fejlfinding i forbindelse med Azure ad-domæne tjenester](https://docs.microsoft.com/azure/active-directory-domain-services/troubleshoot) for at løse almindelige fejl, så du kan få tingene til at fungere igen. 

**AAD-DS kan ikke deaktiveres**

AAD-DS kan ikke afbrydes midlertidigt. Hvis du vil stoppe med at bruge dit administrerede domæne, skal det slettes.

Hvis du støder på problemer, skal du se [fejlfinding af Azure Active Directory-domæne tjenester](https://docs.microsoft.com/azure/active-directory-domain-services/troubleshoot)for at løse almindelige fejlmeddelelser og tilknyttede fejlfindingstrin, der kan hjælpe dig med at få tingene til at køre igen.
