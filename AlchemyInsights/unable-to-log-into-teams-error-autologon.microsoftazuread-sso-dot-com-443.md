---
title: Der kan ikke logges på teams på grund af fejl autologon.microsoftazuread-sso.com:443
ms.author: pebaum
author: pebaum
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.assetid: 686e8f18-b871-4dd2-864f-8562947ab583
ms.collection: Adm_O365
ms.custom:
- "9001686"
- "3750"
ms.openlocfilehash: 649124db135805d8101b43dbead63860d36853ed
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 09/15/2020
ms.locfileid: "47799954"
---
# <a name="unable-to-log-into-teams-due-to-error-autologonmicrosoftazuread-sso-dot-com443"></a>Det er ikke muligt at logge på teams på grund af fejl i automatisk logon. microsoftazuread-SSO-dk-com: 443

Hvis problemfrit SSO er aktiveret som O365-godkendelse, skal URL-adressen "autologon.microsoftazuread-sso.com" muligvis føjes til intranet websteder.  Hvis det tidligere er blevet føjet til websteder, der er tillid til, og problem løse SSO er i brug, bør det fjernes fra websteder, du har tillid til.

Gennemse [checklisten Problemløser for SSO](https://docs.microsoft.com/azure/active-directory/hybrid/tshoot-connect-sso#troubleshooting-checklist).

Følg disse trin for at tilføje en URL-adresse på listen over intranet websteder:

1. Åbn Internet Explorer ved at klikke på knappen **Start** . I søgefeltet skal du skrive Internet Explorer og derefter klikke på **Internet Explorer**på listen over resultater.
2. Klik på **værktøjer**, og klik derefter på **Internet indstillinger**.
3. Klik på fanen **sikkerhed** .
4. Klik nu på **lokale intranet websteder** , og klik derefter på knappen **websteder** og derefter knappen **Avanceret** .
5. Indtast webstedets URL-adresse, og klik på **Tilføj**.
6. Klik på **Luk**, når du er færdig.

Du kan finde flere oplysninger i [dokumentationen til installation af problemfrit SSO til O365](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-sso-quick-start) (omfatter politikbaseret proces, hvor du kan tilføje en URL-adresse til intranet websteder i trin 3).
