---
title: Konfigurere domæne tjeneste
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 01/15/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "7931"
- "9004400"
ms.openlocfilehash: 51e0bd78240627876721cbce654188afac1ee365
ms.sourcegitcommit: a61a29dbd0382370fea0be5fa4a61c9a1a9354c7
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 01/18/2021
ms.locfileid: "49884986"
---
# <a name="unable-to-enable-aad-ds-or-deployment-is-failing"></a>Det er ikke muligt at aktivere AAD-DS, eller installationen mislykkedes

Hvis du vil løse problemet med Azure AD-domæne tjenesten (AAD-DS), der ikke er aktiveret eller ikke kan installeres, skal du udføre følgende trin:

1. Hvis du bruger et allerede eksisterende virtuelt netværk, skal du kontrollere din NSG for regler, der blokerer de porte, der kræves for at synkronisere på en AAD-DOMÆNEadministrator i portalen https://aka.ms/aadds-networking .
2. Kontrollér, om din fejlmeddelelse er besvaret i denne fejlfindingsvejledning, der er tilgængelig i  https://aka.ms/aadds-troubleshoot-enable .
3. Prøv at installere Azure AD-domæne tjenester i et nyt virtuelt netværk.
4. Følg vejledningen i Introduktion til, hvordan du installerer AAD-DS: [oprette og konfigurere Aad-domæne tjenester](https://docs.microsoft.com/azure/active-directory-domain-services/tutorial-create-instance).
5. Hvis du har problemer med at installere Azure AD-domæne tjenester, skal du se [fejlfinding i forbindelse med Azure ad-domæne tjenester](https://docs.microsoft.com/azure/active-directory-domain-services/troubleshoot) for at løse almindelige fejl, så du kan få tingene til at fungere igen. 

**AAD-DS kan ikke deaktiveres**

AAD-DS kan ikke afbrydes midlertidigt. Hvis du vil stoppe med at bruge dit administrerede domæne, skal det slettes.
Hvis du vil slette dit administrerede domæne, skal du se [Slet Aad-domæne tjeneste](https://docs.microsoft.com/azure/active-directory-domain-services/delete-aadds).



