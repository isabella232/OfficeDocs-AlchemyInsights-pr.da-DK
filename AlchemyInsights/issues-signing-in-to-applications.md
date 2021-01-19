---
title: Problemer med at logge på programmer
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 01/16/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "7788"
- "9004355"
ms.openlocfilehash: 2d073367dc1c3e8e117c0b68e205297a65024872
ms.sourcegitcommit: 6d02eb533fd74199af6b20f714b3720991da2c4a
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 01/18/2021
ms.locfileid: "49900875"
---
# <a name="issues-signing-in-to-applications"></a>Problemer med at logge på programmer

Hvis du vil registrere årsagen eller diagnose problemer, der er relateret til brugerlogon, skal du udføre følgende trin:

1. Start den [diagnosticering, du har logget på](https://ms.portal.azure.com/#blade/Microsoft_AAD_IAM/ActiveDirectoryMenuBlade/diagnose/symptomId/ms_aad_dxp_signin_caDiagnoseAndSolveSummarySymptom).
2. Find den hændelse, der skal analyseres, ved at angive de oplysninger, du har om brugeren, programmet, klokkeslættet for logon, anmodnings-id eller korrelations-id.
3. Gennemgå de diagnostiske resultater, der viser oplysninger om, hvad der er sket, og hvilke handlinger du kan udføre for at foretage ændringer, hvis der er behov for ændringer.

Følgende er nogle almindelige problemer, du kan opleve, når du logger på programmer:

1. Du eller brugeren **har fuldført et Azure ad-logon, men får vist en uventet prompt** – Se artiklerne [om uventet samtykke, når du logger på et program og en](https://docs.microsoft.com/azure/active-directory/manage-apps/application-sign-in-unexpected-user-consent-prompt) [uventet fejl, når du udfører et samtykke til et program](https://docs.microsoft.com/azure/active-directory/manage-apps/application-sign-in-unexpected-user-consent-error).
2. Du eller en bruger **har logget på et program direkte, men du kan ikke logge på det fra en deeplink på den brugerdefinerede Portal eller i adgangs panelet**: Se [fejlfinding af problemer med at logge på et program fra Azure ad mine apps](https://docs.microsoft.com/azure/active-directory/manage-apps/application-sign-in-other-problem-access-panel).
3. Du eller en bruger **har fuldført et Azure ad-logon, men programmet viser en fejlmeddelelse og giver ikke brugeren mulighed for at afslutte tilmeldingsprocessen**: problemet er, at appen ikke har accepteret det svar, som Azure ad udstedte. Følg [disse trin](https://docs.microsoft.com/azure/active-directory/application-sign-in-problem-application-error) for at foretage fejlfinding.
4. Du eller en bruger **kan ikke logge på et ikke-galleri-program, der er konfigureret til adgangskode enkeltlogon**: Følg vejledningen i [disse trin](https://docs.microsoft.com/azure/active-directory/manage-apps/troubleshoot-password-based-sso) for at foretage fejlfinding.
5. Du eller en bruger **kan ikke logge på et Azure ad Gallery-program, der er konfigureret til adgangskode enkeltlogon**: Følg [disse trin](https://docs.microsoft.com/azure/active-directory/manage-apps/troubleshoot-password-based-sso) for at foretage fejlfinding.
6. Du eller en bruger **kan ikke logge på et Microsoft-program**: Følg [disse trin](https://docs.microsoft.com/azure/active-directory/manage-apps/application-sign-in-problem-first-party-microsoft) for at foretage fejlfinding.
7. Du eller en bruger **kan ikke logge på et ikke-galleri-program, der er konfigureret til Single Sign-on til organisationsnetværket**: Følg [disse trin](https://docs.microsoft.com/azure/active-directory/application-sign-in-problem-federated-sso-non-gallery) for at foretage fejlfinding.
8. Du eller en bruger **kan ikke logge på et Azure ad Gallery-program, der er konfigureret til Single Sign-on til organisationsnetværket**: Følg [disse trin](https://docs.microsoft.com/azure/active-directory/manage-apps/application-sign-in-problem-federated-sso-gallery) for at foretage fejlfinding.
9. Du eller en bruger **kan ikke logge på et specialudviklet program**: Følg [disse trin](https://docs.microsoft.com/azure/active-directory/manage-apps/application-sign-in-problem-federated-sso-gallery) for at foretage fejlfinding.
10. Du eller en bruger **kan ikke logge på et lokalt program ved hjælp af Azure ad Application proxy**: Følg [disse trin](https://docs.microsoft.com/azure/active-directory/manage-apps/application-sign-in-problem-on-premises-application-proxy) for at foretage fejlfinding.

